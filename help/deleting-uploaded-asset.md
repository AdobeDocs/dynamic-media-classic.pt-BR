---
title: Excluindo um ativo carregado
seo-title: Excluindo um ativo carregado
description: nulo
seo-description: Saiba como excluir um ativo carregado.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '99'
ht-degree: 0%

---


# Excluindo um ativo carregado{#deleting-an-uploaded-asset}

Você pode usar o parâmetro `delete` neste formato para excluir um ativo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

A seguir está um exemplo de uma resposta quando um ativo de imagem é excluído:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Você pode usar os seguintes campos na sequência de query do URL para excluir um ativo:

| Parâmetro de URL | Obrigatório/opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | delete |
| shared_secret | Obrigatório | A chave do segredo compartilhado para a empresa. |
| <ul><li>Para imagens:image_name</li><li>Para vetor:fxg_name</li></ul> | Obrigatório | Nome do ativo a ser excluído. |

**URL da imagem de amostra:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**URL de vetor de amostra:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
