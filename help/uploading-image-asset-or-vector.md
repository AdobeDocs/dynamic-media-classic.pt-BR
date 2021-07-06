---
title: Upload de um ativo de imagem ou de vetor
description: Saiba como fazer upload de um ativo de imagem ou de um ativo de vetor.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1475'
ht-degree: 0%

---

# Upload de um ativo de imagem ou de vetor{#uploading-an-image-asset-or-a-vector-asset}

Antes de fazer upload de um ativo de imagem, primeiro solicite uma chave secreta compartilhada. Use essa chave secreta compartilhada para recuperar um token de upload. Em seguida, use o token de upload para carregar ativos de imagem ou ativos vetoriais.

## Solicitar uma chave secreta compartilhada {#requesting-a-shared-secret-key}

Solicite uma *chave secreta compartilhada* de [usando o Admin Console para criar um caso de suporte.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) No seu caso de suporte, solicite uma chave secreta compartilhada.

Na mensagem de email, forneça o nome da empresa que deseja usar para fazer upload de ativos de imagem. Depois de receber a chave do Dynamic Media Classic, salve-a localmente para uso futuro.

## Recuperação do token de upload {#retrieving-the-upload-token}

O *token de carregamento* garante que ninguém possa usar a mesma chave compartilhada-secreta para carregar ativos. Ele garante que o upload seja legítimo e provém de uma fonte confiável.

O token de upload é uma sequência de caracteres alfanumérica que está disponível somente para um período específico. Use os seguintes URLs, substituindo sua chave secreta compartilhada, para recuperar o token de upload.

* Imagem
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`Neste exemplo, a chave shared-secret é  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vetor
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`Neste exemplo, a chave shared-secret é  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Por padrão, o token de upload expira cinco minutos (300 segundos) após sua recuperação. Para solicitar mais tempo, inclua `expires` no URL e o tempo necessário em segundos. Por exemplo, o exemplo de URL de imagem a seguir recupera um token de upload válido por 1800 segundos:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

A resposta bem-sucedida de imagens é semelhante ao seguinte:

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

Salve o token de upload localmente para uso com solicitações futuras.

Você pode usar os seguintes campos na cadeia de caracteres do URL de consulta para recuperar um token de upload:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | get_uploadtoken |
| shared_secret | Obrigatório | A chave secreta compartilhada da empresa que está fazendo o upload. |
| expira | Opcional | Número de segundos que o token de carregamento é válido. O padrão é 300 segundos, se não especificado. |

**Exemplo de URL da imagem:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Exemplo de URL de vetor:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Métodos HTTP permitidos:**
`GET` e  `POST`

Agora é possível fazer upload de um ativo de imagem.

Consulte [Fazer upload de um ativo de imagem](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Upload de um ativo de imagem {#uploading-an-image-asset}

Após recuperar um token de upload válido por um período específico, é possível fazer upload de um ativo de imagem. Você faz upload do ativo como uma publicação de várias partes/formulários ao enviar o restante dos valores como uma sequência de consulta de URL, como mostrado neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Os campos `upload_token` e `company_name` são obrigatórios.

Consulte [Recuperando o token de upload](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperando uma chave secreta compartilhada](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Você também pode enviar outros valores opcionais como cadeias de caracteres de consulta de URL, como neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

O parâmetro `file_limit` especifica o limite de tamanho do arquivo em bytes. O parâmetro `file_exts` especifica as extensões de nome de arquivo permitidas para upload. Ambos os valores são opcionais.

Um limite global é definido no aplicativo para o limite de tamanho de arquivo e as extensões de nome de arquivo permitidas. Se o que você enviou na solicitação for um subconjunto dos limites globais, ele será honrado. Os limites globais são os seguintes:

| Limite global | Valor |
|--- |--- |
| Tamanho do arquivo para todos os clientes | 20 MB |
| Formatos de arquivo de imagem compatíveis para upload | BMP, GIF, JPG, PNG, PSD |

O formulário HTML a seguir permite que um usuário carregue um ativo. O formulário solicita que o usuário insira as seguintes informações:

* Um nome de empresa.
* Um token de upload.
* Um limite de tamanho de arquivo.
* Uma lista de extensões de nome de arquivo.
* Se é necessário preservar o perfil de cor e o nome do arquivo associados ao ativo.
* Se deseja usar o Plano de Fundo do Knockout. Se você ativar o Plano de Fundo de Knockout, defina o Canto, a Tolerância e o Método de Preenchimento.
Consulte Plano de fundo de nocaute em [Opções de edição de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload).
* O nome do arquivo a ser carregado.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

Você pode exibir o código-fonte HTML associado ao formulário acima clicando em [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

No Firefox, clique com o botão direito do mouse na janela do navegador e depois clique em **[!UICONTROL View Page Source]**. O código mostra a string de consulta de URL correspondente e o método POST que são executados quando o usuário clica em **[!UICONTROL Submit]**.

Para exibir a resposta XML no Internet Explorer, clique em **[!UICONTROL View]** > **[!UICONTROL Source]**. Para exibir a resposta XML no Firefox, clique em **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Web Developer Tools]**. O Firefox é recomendado para exibir respostas XML.

Veja a seguir uma amostra de resposta de um upload bem-sucedido:

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

O ativo é como qualquer outro recurso do ImageServing; você pode aplicar consultas de processamento a ele. Por exemplo, o URL a seguir solicita um ativo que é esticado até a largura e a altura especificadas.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Envie o ativo para fazer upload como uma publicação de várias partes/formulários, enquanto envia o restante dos valores como uma sequência de consulta de URL. Você pode usar os seguintes campos na cadeia de caracteres de consulta de URL para carregar um ativo:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| `op` | Obrigatório | fazer upload |
| `upload_token` | Obrigatório | Faça upload do token da chave secreta compartilhada associada à empresa. |
| `company_name` | Obrigatório | Nome da empresa que está executando o upload. |
| `file_limit` | Opcional | Limite de tamanho do arquivo, em bytes, para o ativo. |
| `file_exts` | Opcional | Lista de extensões permitidas para o arquivo de ativo de imagem. |
| `preserve_colorprofile` | Opcional | Preserva qualquer perfil de cor incorporado durante a conversão do arquivo carregado para o formato PTIFF. Os valores possíveis são verdadeiro ou falso. O padrão é false. |
| `preserve_filename` | Opcional | Preserva o nome do arquivo do ativo carregado. Os valores possíveis são verdadeiro ou falso. O padrão é false. |

>[!NOTE]
>
>É necessário enviar o ativo para ser carregado como o único campo em uma solicitação de POST multipart.

**Exemplo de URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST

### Obter metadados de ativos para imagens {#getting-asset-metadata-for-images}

Você pode usar `image_info` para recuperar metadados para um ativo que você carregou, como mostrado no exemplo a seguir:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Um exemplo de resposta bem-sucedida é exibido de maneira semelhante ao seguinte:

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

Você pode usar os seguintes campos na sequência de consulta do URL para solicitar informações para um ativo:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| `op` | Obrigatório | image_info |
| `shared_secret` | Obrigatório | A chave secreta compartilhada da empresa. |
| `image_name` | Obrigatório | Nome da imagem. |

**Exemplo de URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Método HTTP permitido:**

GET e POST

## Upload de um ativo vetorial {#uploading-a-vector-asset}

Após recuperar um token de upload válido por um período específico, é possível fazer upload de um ativo de vetor. Você faz upload do ativo como uma publicação de várias partes/formulários ao enviar o restante dos valores como uma sequência de consulta de URL, como mostrado neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

Os campos `upload_token` e `company_name` são obrigatórios.

Consulte [Recuperando o token de upload](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperando uma chave secreta compartilhada](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Você também pode enviar outros valores opcionais como cadeias de caracteres de consulta de URL, como neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

O parâmetro `file_limit` especifica o limite de tamanho do arquivo em bytes. O parâmetro `file_exts` especifica as extensões de nome de arquivo permitidas para upload. Ambos os valores são opcionais.

Um limite global é definido no aplicativo para o limite de tamanho de arquivo e as extensões de nome de arquivo permitidas. Se o que você enviou na solicitação for um subconjunto dos limites globais, ele será honrado. Os limites globais são os seguintes:

| Limite global | Valor |
|--- |--- |
| Tamanho do arquivo para todos os clientes | 20 MB |
| Formatos de arquivo de vetor compatíveis para upload | AI, EPS, PDF (somente quando o PDF foi aberto e salvo no Adobe Illustrator CS6) |

O formulário HTML a seguir permite que um usuário carregue um ativo. O formulário solicita que o usuário insira as seguintes informações:

* Um nome de empresa.
* Um token de upload.
* Um limite de tamanho de arquivo.
* Uma lista de extensões de nome de arquivo.
* Se é necessário preservar o perfil de cor e o nome do arquivo associados ao ativo.
* Se deseja usar o Plano de Fundo do Knockout. Se você ativar o Plano de Fundo de Knockout, defina o Canto, a Tolerância e o Método de Preenchimento.
Consulte Plano de fundo de nocaute em [Opções de edição de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload).
* O nome do arquivo a ser carregado.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

O seguinte código HTML é exibido quando você clica com o botão direito do mouse na janela do navegador e, em seguida, clica em **[!UICONTROL View Source]** para o formulário mostrado no exemplo. O código mostra a string de consulta de URL correspondente e o método POST que são executados quando o usuário clica em **[!UICONTROL Submit]**.

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

Para exibir a resposta XML no Internet Explorer, clique em **[!UICONTROL View]** > **[!UICONTROL Source]**. Para exibir a resposta XML no Firefox, clique em **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. O Firefox é recomendado para exibir respostas XML.

Veja a seguir uma amostra de resposta de um upload bem-sucedido:

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

O ativo é como qualquer outro recurso Web-to-print; você aplica consultas de processamento a ele. Por exemplo, o URL a seguir converte um recurso FXG em uma imagem de 500x500 png.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Envie o ativo para fazer upload como uma publicação de várias partes/formulários, enquanto envia o restante dos valores como uma sequência de consulta de URL. Você pode usar os seguintes campos na cadeia de caracteres de consulta de URL para carregar um ativo:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| `op` | Obrigatório | fazer upload |
| `upload_token` | Obrigatório | Faça upload do token da chave secreta compartilhada associada à empresa. |
| `company_name` | Obrigatório | Nome da empresa que está executando o upload. |
| `file_limit` | Opcional | Limite de tamanho do arquivo, em bytes, para o ativo. |
| `file_exts` | Opcional | Lista de extensões permitidas para o arquivo de ativo. |

>[!NOTE]
>
>É necessário enviar o ativo para ser carregado como o único campo em uma solicitação de POST multipart.

**Exemplo de URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST
