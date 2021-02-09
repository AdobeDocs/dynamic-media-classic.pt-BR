---
title: Fazer upload de um ativo de imagem ou de um ativo vetorial
description: Saiba como carregar um ativo de imagem ou um ativo vetorial.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '1527'
ht-degree: 0%

---


# Fazer upload de um ativo de imagem ou de um ativo vetorial{#uploading-an-image-asset-or-a-vector-asset}

Antes de poder carregar um ativo de imagem, solicite primeiro uma chave de segredo compartilhado. Use essa chave de segredo compartilhado para recuperar um token de upload. Em seguida, use o token de upload para fazer upload de ativos de imagem ou ativos de vetor.

## Solicitação de uma chave de segredo compartilhado {#requesting-a-shared-secret-key}

Solicite uma *chave de segredo compartilhado* por [usando o Admin Console para criar um caso de suporte.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Em seu caso de suporte, solicite uma chave de segredo compartilhado.

Na mensagem de email, forneça o nome da empresa que deseja usar para fazer upload de ativos de imagem. Depois de receber a chave do Dynamic Media Classic, salve-a localmente para uso futuro.

## Recuperando o token de upload {#retrieving-the-upload-token}

O *token de carregamento* garante que ninguém possa usar a mesma chave de segredo compartilhado para fazer upload de ativos. Ele garante que o upload seja legítimo e provém de uma fonte confiável.

O token de upload é uma sequência de caracteres alfanuméricos que está disponível somente por um período específico. Use os seguintes URLs, substituindo sua chave de segredo compartilhado, para recuperar o token de upload.

* Imagem
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`Neste exemplo, a chave shared-secret é  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vetor
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`Neste exemplo, a chave shared-secret é  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Por padrão, o token de upload expira cinco minutos (300 segundos) depois que você o recupera. Para solicitar mais tempo, inclua `expires` no URL e o tempo necessário em segundos. Por exemplo, o URL de exemplo a seguir recupera um token de upload válido por 1800 segundos:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

A resposta bem-sucedida para imagens é semelhante ao seguinte:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Salve o token de upload localmente para usar com solicitações futuras.

Você pode usar os seguintes campos na string do URL do query para recuperar um token de upload:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | get_uploadtoken |
| shared_secret | Obrigatório | A chave de segredo compartilhado para a empresa que está fazendo o upload. |
| expira | Opcional | Número de segundos em que o token de carregamento é válido. O padrão é 300 segundos, se não for especificado. |

**URL da imagem de amostra:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**URL de vetor de amostra:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Métodos HTTP permitidos:** GET e POST

Agora é possível carregar um ativo de imagem.

Consulte [Carregar um ativo de imagem](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Upload de um ativo de imagem {#uploading-an-image-asset}

Depois de recuperar um token de upload válido por um período específico, você pode fazer upload de um ativo de imagem. Você faz upload do ativo como uma publicação multipart/form ao enviar o restante dos valores como uma string de query de URL, como mostra este exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Os campos `upload_token` e `company_name` são obrigatórios.

Consulte [Recuperando o token de upload](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperando uma chave de segredo compartilhado](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Você também pode enviar outros valores opcionais como sequências de caracteres de query de URL, como neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

O parâmetro `file_limit` especifica o limite de tamanho de arquivo em bytes. O parâmetro `file_exts` especifica as extensões de nome de arquivo permitidas para upload. Ambos os valores são opcionais.

Um limite global é definido no aplicativo para o limite de tamanho de arquivo e as extensões de nome de arquivo permitidas. Se o que você enviar na solicitação for um subconjunto dos limites globais, ele será atendido. Os limites globais são os seguintes:

| Limite global | Valor |
|--- |--- |
| Tamanho do arquivo para todos os clientes | 20 MB |
| Formatos de arquivo de imagem suportados para upload | BMP, GIF, JPG, PNG, PSD |

O formulário HTML a seguir permite que um usuário carregue um ativo. O formulário solicita que o usuário insira as seguintes informações:

* Um nome de empresa.
* Um token de carregamento.
* Um limite de tamanho de arquivo.
* Uma lista de extensões de nome de arquivo.
* A preservação ou não do perfil de cor e do nome de arquivo associados ao ativo.
* Usar ou não o Plano de fundo de separação. Se você ativar o Plano de fundo de separação, defina o Canto, a Tolerância e o Método de preenchimento. Consulte Informações gerais em [Opções de edição de imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).
* O nome do arquivo a ser carregado

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

Você pode visualização o código-fonte HTML associado ao formulário acima clicando no link a seguir:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

No Firefox, clique com o botão direito do mouse na janela do navegador e, em seguida, clique em **Origem da página de Visualização**. O código mostra a string de query do URL correspondente e o método POST que são executados quando o usuário clica em **Submit**.

Para visualização da resposta XML no Internet Explorer, clique em **Visualização > Origem**. Para visualização da resposta XML no Firefox, clique em **Ferramentas > Desenvolvedor da Web > Fonte da página**. O Firefox é recomendado para exibir respostas XML.

A seguir está uma amostra de resposta de um upload bem-sucedido:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>O ativo carregado (JPG, GIF e assim por diante) é convertido no formato PTIFF e a resposta envia um link direto para esse ativo PTIFF.

O ativo é como qualquer outro recurso ImageServing; você pode aplicar query de processamento a ele. Por exemplo, o URL a seguir solicita um ativo que é esticado até a largura e a altura especificadas.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Envie o ativo para fazer upload como uma publicação multiparte/formulário ao enviar o restante dos valores como uma sequência de query de URL. Você pode usar os seguintes campos na sequência de query do URL para fazer upload de um ativo:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | upload |
| upload_token | Obrigatório | Carregue o token da chave de segredo compartilhado associada à empresa. |
| nome_da_empresa | Obrigatório | Nome da empresa que executa o upload. |
| file_limit | Opcional | Limite de tamanho de arquivo, em bytes, para o ativo. |
| file_exts | Opcional | Lista de extensões permitidas para o arquivo de ativo de imagem. |
| preserve_color_profile | Opcional | Preserva qualquer perfil de cor incorporado ao converter o arquivo carregado no formato PTIFF. Valores possíveis são verdadeiros ou falsos. O padrão é falso. |
| preserve_filename | Opcional | Preserva o nome de arquivo do ativo carregado. Valores possíveis são verdadeiros ou falsos. O padrão é falso. |

>[!NOTE]
>
>É necessário enviar o ativo para ser carregado como o único campo em uma solicitação de POST multiparte.

**URL de exemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST

### Obtenção de metadados de ativos para imagens {#getting-asset-metadata-for-images}

Você pode usar `image_info` para recuperar metadados de um ativo que você carregou, como mostrado no exemplo a seguir:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Um exemplo de uma resposta bem-sucedida é semelhante ao seguinte:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Você pode usar os seguintes campos na sequência de query do URL para solicitar informações para um ativo:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | image_info |
| shared_secret | Obrigatório | A chave do segredo compartilhado para a empresa. |
| image_name | Obrigatório | Nome da imagem. |

**URL de exemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Método HTTP permitido:**

GET e POST

## Carregando um ativo vetorial {#uploading-a-vector-asset}

Depois de recuperar um token de upload válido por um período específico, você pode fazer upload de um ativo de vetor. Você faz upload do ativo como uma publicação multipart/form ao enviar o restante dos valores como uma string de query de URL, como mostra este exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

Os campos `upload_token` e `company_name` são obrigatórios.

Consulte [Recuperando o token de upload](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperando uma chave de segredo compartilhado](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Você também pode enviar outros valores opcionais como sequências de caracteres de query de URL, como neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

O parâmetro `file_limit` especifica o limite de tamanho de arquivo em bytes. O parâmetro `file_exts` especifica as extensões de nome de arquivo permitidas para upload. Ambos os valores são opcionais.

Um limite global é definido no aplicativo para o limite de tamanho de arquivo e as extensões de nome de arquivo permitidas. Se o que você enviar na solicitação for um subconjunto dos limites globais, ele será atendido. Os limites globais são os seguintes:

| Limite global | Valor |
|--- |--- |
| Tamanho do arquivo para todos os clientes | 20 MB |
| Formatos de arquivo vetorial suportados para upload | AI, EPS, PDF (somente quando o PDF foi aberto e salvo anteriormente na Adobe Illustrator CS6) |

O formulário HTML a seguir permite que um usuário carregue um ativo. O formulário solicita que o usuário insira as seguintes informações:

* Um nome de empresa.
* Um token de carregamento.
* Um limite de tamanho de arquivo.
* Uma lista de extensões de nome de arquivo.
* A preservação ou não do perfil de cor e do nome de arquivo associados ao ativo.
* Usar ou não o Plano de fundo de separação. Se você ativar o Plano de fundo de separação, defina o Canto, a Tolerância e o Método de preenchimento. Consulte Informações gerais em [Opções de edição de imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).
* O nome do arquivo a ser carregado

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

O seguinte código HTML é exibido quando você clica com o botão direito do mouse na janela do navegador e, em seguida, clica em **Origem da Visualização** para o formulário mostrado na ilustração. O código mostra a string de query do URL correspondente e o método POST que são executados quando o usuário clica em **Submit**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Para visualização da resposta XML no Internet Explorer, clique em **Visualização** > **Origem**. Para visualização da resposta XML no Firefox, clique em **Visualização** > **Origem da página**. O Firefox é recomendado para exibir respostas XML.

A seguir está uma amostra de resposta de um upload bem-sucedido:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>O ativo carregado (AI, EPS, PDF etc.) é convertido para o formato FXG e a resposta envia um link direto para esse ativo FXG.

O ativo é como qualquer outro recurso Web-to-print; você pode aplicar query de processamento a ele. Por exemplo, o URL a seguir converte um recurso FXG em uma imagem 500x500 png.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Envie o ativo para fazer upload como uma publicação multiparte/formulário ao enviar o restante dos valores como uma sequência de query de URL. Você pode usar os seguintes campos na sequência de query do URL para fazer upload de um ativo:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | upload |
| upload_token | Obrigatório | Carregue o token da chave de segredo compartilhado associada à empresa. |
| nome_da_empresa | Obrigatório | Nome da empresa que executa o upload. |
| file_limit | Opcional | Limite de tamanho de arquivo, em bytes, para o ativo. |
| file_exts | Opcional | Lista de extensões permitidas para o arquivo de ativos. |

>[!NOTE]
>
>É necessário enviar o ativo para ser carregado como o único campo em uma solicitação de POST multiparte.

**URL de exemplo:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST
