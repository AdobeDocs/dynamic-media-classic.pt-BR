---
title: Fazer upload de um ativo de imagem ou de um ativo de vetor
seo-title: Fazer upload de um ativo de imagem ou de um ativo de vetor
description: 'null'
seo-description: Saiba como carregar um ativo de imagem ou um ativo de vetor.
uuid: d 0 e 4 a 754-8 a 49-4 b 0 f-b 202-e 9003 bdb 8 f 20
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: de 21 dca 9-99 fe -4183-b 647-debfe 112 fda 4
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Fazer upload de um ativo de imagem ou de um ativo de vetor{#uploading-an-image-asset-or-a-vector-asset}

Antes de fazer upload de um ativo de imagem, você solicita primeiro uma chave de segredo compartilhado. Use esta chave de segredo compartilhado para recuperar um token de upload. Em seguida, use o token de upload para carregar ativos de imagem ou ativos vetoriais.

## Solicitação de uma chave compartilhada {#requesting-a-shared-secret-key}

Solicite uma *chave ad-secreta* enviando um email para o Suporte técnico Scene 7 em s7support@adobe.com.

Na mensagem de email, forneça o nome da empresa que deseja usar para carregar ativos de imagem. Depois de receber a chave do Dynamic Media Classic, salve-a localmente para uso futuro.

## Recuperar o token de upload {#retrieving-the-upload-token}

O token *de upload* garante que ninguém pode usar a mesma chave compartilhada para carregar ativos. Isso garante que o upload seja legítimo e proveniente de uma fonte confiável.

O token de upload é uma sequência alfanumérica que está disponível somente para um período específico. Use os seguintes urls, substituindo sua chave de segredo compartilhado para recuperar o token de upload.

* Imagem
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`Neste exemplo, a chave compartilhada-segredo é `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vetor
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`Neste exemplo, a chave compartilhada-segredo é `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Por padrão, o token de upload expira cinco minutos (300 segundos) após a recuperação. Para solicitar mais tempo, inclua `expires` no URL e o tempo necessário em segundos. Por exemplo, o exemplo de URL da imagem seguinte recupera um token de upload válido por 1800 segundos:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

A resposta bem-sucedida das imagens é:

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

Você pode usar os seguintes campos na sequência de caracteres do URL de consulta para recuperar um token de upload:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | get_ uploadtoken |
| shared_ secret | Obrigatório | A chave compartilhada para a empresa que está fazendo o upload. |
| expira | Opcional | Número de segundos que o token de upload é válido. O padrão é 300 segundos, se não for especificado. |

**Exemplo de URL da imagem:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Exemplo de URL de vetor:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Métodos HTTP permitidos:** GET e POST

Agora é possível carregar um ativo de imagem.

Consulte [Upload de um ativo de imagem](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Fazer upload de um ativo de imagem {#uploading-an-image-asset}

Depois de recuperar um token de upload válido para um período específico, é possível carregar um ativo de imagem. Você carrega o ativo como uma publicação multiparte/formulário ao enviar o restante dos valores como uma sequência de consulta de URL, como mostra este exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Os campos `upload_token` e os `company_name` campos são obrigatórios.

Consulte [Recuperar o token de upload](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperar uma chave de segredo compartilhado](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Também é possível enviar outros valores opcionais como sequências de consulta de URL, como neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

O `file_limit` parâmetro especifica o limite de tamanho de arquivo em bytes. O `file_exts` parâmetro especifica as extensões de nome de arquivo permitidas para upload. Ambos os valores são opcionais.

Um limite global é definido no aplicativo para o limite de tamanho do arquivo e as extensões de nome de arquivo permitidas. Se o que você enviar na solicitação for um subconjunto dos limites globais, ele será respeitado. Os limites globais são os seguintes:

| Limite global | Valor |
|--- |--- |
| Tamanho de arquivo para todos os clientes | 20 MB |
| Formatos de arquivo de imagem suportados para upload | BMP, GIF, JPG, PNG, PSD |

O formulário HTML a seguir permite que um usuário faça upload de um ativo. O formulário solicita ao usuário que insira as seguintes informações:

* Um nome de empresa.
* Um token de upload.
* Um limite de tamanho de arquivo.
* Uma lista de extensões de nomes de arquivo.
* Se preservar ou não o perfil de cores e o nome do arquivo associados ao ativo.
* Se o plano de fundo não deve ser usado ou não. Se você ativar Plano de fundo de separação, defina o método de canto, tolerância e preenchimento. Consulte Plano de fundo de separação em [opções de edição de imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).
* O nome do arquivo a ser carregado

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment&gt; elements under &lt;adobefig&gt;.</p>

 -->

![]()

É possível exibir o código-fonte HTML associado ao formulário acima clicando no link a seguir:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

No Firefox, clique com o botão direito do mouse na janela do navegador e clique em **Exibir fonte da página**. O código mostra a sequência de consulta de URL correspondente e o método POST que são executados quando o usuário clica **em Enviar**.

Para exibir a resposta XML no Internet Explorer, clique **em Exibir** &gt; **Fonte**. Para exibir a resposta XML no Firefox, clique **em Ferramentas** &gt; **Desenvolvedor da Web** &gt; **Fonte da página**. O Firefox é recomendado para exibir respostas XML.

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
>O ativo carregado (JPG, GIF e assim por diante) é convertido para o formato PTIFF e a resposta envia um link direto para esse ativo PTIFF.

O ativo é como qualquer outro recurso imageserving; você pode aplicar consultas de processamento a ele. Por exemplo, o URL a seguir solicita um ativo que é esticado para a largura e altura especificadas.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Envie o ativo para fazer upload como uma publicação multiparte/formulário ao enviar o restante dos valores como uma sequência de consulta de URL. Você pode usar os seguintes campos na sequência de consulta do URL para fazer upload de um ativo:

| Parâmetro do URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | upload |
| upload_ token | Obrigatório | Carregar o token para a chave de segredo compartilhado associada à empresa. |
| company_ name | Obrigatório | Nome da empresa que executa o upload. |
| file_ limit | Opcional | Limite de tamanho do arquivo, em bytes, para o ativo. |
| file_ exts | Opcional | Lista de extensões permitidas para o arquivo de ativo de imagem. |
| preserve_ colorprofile | Opcional | Preserva qualquer perfil de cor incorporado ao converter o arquivo carregado no formato PTIFF. Os valores possíveis são verdadeiros ou falsos. O padrão é false. |
| preserve_ filename | Opcional | Preserva o nome de arquivo do ativo carregado. Os valores possíveis são verdadeiros ou falsos. O padrão é false. |

>[!NOTE]
>
>Você deve enviar o ativo para ser carregado como o único campo em uma solicitação POST multipart.

**URL de exemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST

### Obtenção de metadados de ativos para imagens {#getting-asset-metadata-for-images}

Você pode usar `image_info` para recuperar metadados para um ativo carregado, como mostrado no exemplo a seguir:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Um exemplo de resposta bem-sucedida é semelhante ao seguinte:

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

Você pode usar os seguintes campos na sequência de consulta do URL para solicitar informações de um ativo:

| Parâmetro do URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | image_ info |
| shared_ secret | Obrigatório | A chave compartilhada para a empresa. |
| image_ name | Obrigatório | Nome da imagem. |

**URL de exemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Método HTTP permitido:**

GET e POST

## Fazer upload de um ativo de vetor {#uploading-a-vector-asset}

Depois de recuperar um token de upload válido para um período específico, você pode carregar um ativo de vetor. Você carrega o ativo como uma publicação multiparte/formulário ao enviar o restante dos valores como uma sequência de consulta de URL, como mostra este exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

Os campos `upload_token` e os `company_name` campos são obrigatórios.

Consulte [Recuperar o token de upload](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperar uma chave de segredo compartilhado](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Também é possível enviar outros valores opcionais como sequências de consulta de URL, como neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

O `file_limit` parâmetro especifica o limite de tamanho de arquivo em bytes. O `file_exts` parâmetro especifica as extensões de nome de arquivo permitidas para upload. Ambos os valores são opcionais.

Um limite global é definido no aplicativo para o limite de tamanho do arquivo e as extensões de nome de arquivo permitidas. Se o que você enviar na solicitação for um subconjunto dos limites globais, ele será respeitado. Os limites globais são os seguintes:

| Limite global | Valor |
|--- |--- |
| Tamanho de arquivo para todos os clientes | 20 MB |
| Formatos de arquivo de vetor suportados para upload | AI, EPS, PDF (apenas quando o PDF é aberto e salvo anteriormente no Adobe Illustrator CS 6) |

O formulário HTML a seguir permite que um usuário faça upload de um ativo. O formulário solicita ao usuário que insira as seguintes informações:

* Um nome de empresa.
* Um token de upload.
* Um limite de tamanho de arquivo.
* Uma lista de extensões de nomes de arquivo.
* Se preservar ou não o perfil de cores e o nome do arquivo associados ao ativo.
* Se o plano de fundo não deve ser usado ou não. Se você ativar Plano de fundo de separação, defina o método de canto, tolerância e preenchimento. Consulte Plano de fundo de separação em [opções de edição de imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).
* O nome do arquivo a ser carregado

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment&gt; elements under &lt;adobefig&gt;.</p>

 -->

![]()

O seguinte código HTML é exibido ao clicar com o botão direito do mouse na janela do navegador e clicar **em Exibir fonte** para o formulário mostrado na ilustração. O código mostra a sequência de consulta de URL correspondente e o método POST que são executados quando o usuário clica **em Enviar**.

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

Para exibir a resposta XML no Internet Explorer, clique **em Exibir** &gt; **Fonte**. Para exibir a resposta XML no Firefox, clique **em Exibir** &gt; **Fonte da página**. O Firefox é recomendado para exibir respostas XML.

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
>O ativo carregado (AI, EPS, PDF assim por diante) é convertido para o formato FXG e a resposta envia um link direto para esse ativo FXG.

O ativo é como qualquer outro recurso Web-to-print; você pode aplicar consultas de processamento a ele. Por exemplo, o URL a seguir converte um recurso FXG em uma imagem png de 500 x 500.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Envie o ativo para fazer upload como uma publicação multiparte/formulário ao enviar o restante dos valores como uma sequência de consulta de URL. Você pode usar os seguintes campos na sequência de consulta do URL para fazer upload de um ativo:

| Parâmetro do URL | Obrigatório ou opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | upload |
| upload_ token | Obrigatório | Carregar o token para a chave de segredo compartilhado associada à empresa. |
| company_ name | Obrigatório | Nome da empresa que executa o upload. |
| file_ limit | Opcional | Limite de tamanho do arquivo, em bytes, para o ativo. |
| file_ exts | Opcional | Lista de extensões permitidas para o arquivo de ativo. |

>[!NOTE]
>
>Você deve enviar o ativo para ser carregado como o único campo em uma solicitação POST multipart.

**URL de exemplo:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST
