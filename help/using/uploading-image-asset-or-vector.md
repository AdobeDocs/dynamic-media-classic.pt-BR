---
title: Fazer upload de um ativo de imagem rasterizada
description: Saiba como fazer upload de um ativo de imagem rasterizada no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# Fazer upload de um ativo de imagem rasterizada {#uploading-an-image-asset-or-a-vector-asset}

Antes de carregar um ativo de imagem, primeiro solicite uma chave de segredo compartilhado. Você usa essa chave de segredo compartilhado para recuperar um token de upload. Em seguida, use o token de upload para fazer upload de ativos de imagem rasterizada.

>[!IMPORTANT]
>
>A partir de 1 de maio de 2023, os ativos UGC no Dynamic Media estarão disponíveis para uso por até 60 dias a partir da data do upload. Após 60 dias, os ativos serão removidos.

>[!NOTE]
>
>O suporte para ativos vetoriais UGC novos ou existentes no Adobe Dynamic Media Classic terminou em 30 de setembro de 2021.

## Solicitar uma chave de segredo compartilhado {#requesting-a-shared-secret-key}

Solicite uma *chave de segredo compartilhado* por [usando o Admin Console para criar um caso de suporte.](https://helpx.adobe.com/br/enterprise/using/support-for-experience-cloud.html) No caso de suporte técnico, solicite uma chave de segredo compartilhado.

Na mensagem de email, forneça o nome da empresa que você deseja usar para fazer upload de ativos de imagem. Depois de receber a chave do Adobe Dynamic Media Classic, salve-a localmente para uso futuro.

## Recuperar o token de upload {#retrieving-the-upload-token}

O *token de carregamento* garante que ninguém possa usar a mesma chave de segredo compartilhado para carregar ativos. Ele garante que o upload seja legítimo e venha de uma fonte confiável.

O token de upload é uma sequência alfanumérica que está disponível somente por um período específico. Use os URLs a seguir, substituindo sua chave de segredo compartilhado, para que você possa recuperar o token de upload.

* Imagem raster
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`Neste exemplo, a chave de segredo compartilhado é `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

Por padrão, o token de upload expira cinco minutos (300 segundos) após a recuperação. Para solicitar mais tempo, inclua `expires` na URL e o tempo necessário em segundos. Por exemplo, o seguinte URL de imagem de amostra recupera um token de upload válido por 1800 segundos:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

A resposta bem-sucedida para imagens é semelhante ao seguinte:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| op | Obrigatório | get_uploadtoken |
| shared_secret | Obrigatório | A chave de segredo compartilhado para a empresa que está fazendo o upload. |
| expira em | Opcional | Número de segundos que o token de upload é válido. O padrão é 300 segundos, se não for especificado. |

**Amostra da URL da imagem rasterizada:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**Métodos HTTP permitidos:**
`GET` e `POST`

Agora você pode fazer upload de um ativo de imagem.

Consulte [Carregar um ativo de imagem](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Fazer upload de um ativo de imagem rasterizada {#uploading-an-image-asset}

Depois de recuperar um token de upload válido por um período específico, você pode fazer upload de um ativo de imagem. Você faz upload do ativo como uma publicação multipart/form enquanto envia o restante dos valores como uma cadeia de caracteres de consulta de URL, conforme mostrado neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Os campos `upload_token` e `company_name` são obrigatórios.

Consulte [Recuperar o token de carregamento](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperar uma chave de segredo compartilhado](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Você também pode enviar outros valores opcionais como cadeias de caracteres de consulta de URL, como neste exemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

O parâmetro `file_limit` especifica o limite de tamanho de arquivo em bytes. O parâmetro `file_exts` especifica as extensões de nome de arquivo permitidas para carregamento. Ambos os valores são opcionais.

Um limite global é definido no aplicativo para o limite de tamanho do arquivo e as extensões de nome do arquivo permitidas. Se o que você enviou na solicitação for um subconjunto dos limites globais, ele será atendido. Os limites globais são os seguintes:

| Limite global | Valor |
| --- | --- |
| Tamanho do arquivo para todos os clientes | 20 MB |
| Formatos de arquivo de imagem aceitos para upload | BMP, GIF, JPG,, PNG, PSD, TIFF |

O formulário HTML a seguir permite que um usuário carregue um ativo. O formulário solicita que o usuário insira as seguintes informações:

* Um nome de empresa.
* Um token de upload.
* Um limite de tamanho de arquivo.
* Uma lista de extensões de nome de arquivo.
* Se o perfil de cores e o nome do arquivo associados ao ativo devem ser preservados.
* Usar um plano de fundo de separação. Se você ativar Plano de fundo de separação, defina o Canto, a Tolerância e o Método de preenchimento.
Consulte Plano de Fundo de Separação em [Opções de ajuste de imagem no carregamento](image-editing-options-upload.md#image-editing-options-at-upload).
* O nome do arquivo a ser carregado.

Você pode exibir o código-fonte HTML associado ao formulário acima selecionando [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

No Firefox, clique com o botão direito na janela do navegador e selecione **[!UICONTROL View Page Source]**. O código mostra a cadeia de caracteres de consulta de URL correspondente e o método POST que é executado quando o usuário seleciona **[!UICONTROL Submit]**.

Para exibir a resposta XML no Internet Explorer, vá para **[!UICONTROL View]** > **[!UICONTROL Source]**. Para exibir a resposta XML no Firefox, vá para **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Web Developer Tools]**. O Firefox é recomendado para exibir respostas XML.

Este é um exemplo de resposta de um upload bem-sucedido:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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

O ativo é como qualquer outro recurso ImageServing; você pode aplicar consultas de processamento a ele. Por exemplo, o URL a seguir solicita um ativo que é ampliado até a largura e a altura especificadas.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Envie o ativo para fazer upload como uma publicação multipart/form enquanto envia o restante dos valores como uma cadeia de caracteres de consulta de URL. Você pode usar os seguintes campos na sequência de consulta do URL para fazer upload de um ativo:

| Parâmetro de URL | Obrigatório ou Opcional | Valor |
| --- | --- | --- |
| `op` | Obrigatório | upload |
| `upload_token` | Obrigatório | Carregue um token para a chave de segredo compartilhado associada à empresa. |
| `company_name` | Obrigatório | Nome da empresa que está fazendo o upload. |
| `file_limit` | Opcional | Limite de tamanho do arquivo, em bytes, para o ativo. |
| `file_exts` | Opcional | Lista de extensões permitidas para o arquivo de ativo de imagem. |
| `preserve_colorprofile` | Opcional | Preserva qualquer perfil de cor incorporado ao converter o arquivo carregado para o formato PTIFF. Os valores possíveis são true ou false. O padrão é falso. |
| `preserve_filename` | Opcional | Preserva o nome de arquivo do ativo carregado. Os valores possíveis são true ou false. O padrão é falso. |

>[!NOTE]
>
>É necessário enviar o ativo para ser carregado como o único campo em uma solicitação POST de várias partes.

**Amostra da URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST

### Obter metadados de ativos para imagens {#getting-asset-metadata-for-images}

Você pode usar o `image_info` para recuperar metadados de um ativo carregado, conforme mostrado no exemplo a seguir:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Um exemplo de resposta bem-sucedida é semelhante ao seguinte:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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

Você pode usar os seguintes campos na cadeia de caracteres de consulta do URL para solicitar informações de um ativo:

| Parâmetro de URL | Obrigatório ou opcional | Valor |
| --- | --- | --- |
| `op` | Obrigatório | image_info |
| `shared_secret` | Obrigatório | A chave que é um segredo compartilhado para a empresa. |
| `image_name` | Obrigatório | Nome da imagem. |

**Amostra da URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Método HTTP permitido:**

GET e POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->