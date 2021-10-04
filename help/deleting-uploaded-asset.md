---
title: Excluir um ativo carregado
description: Saiba como excluir um ativo carregado no Adobe Dynamic Media Classic.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
source-git-commit: f92109182283f3bf046604b1b6910180f858d73e
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Excluir um ativo carregado{#deleting-an-uploaded-asset}

Você pode usar o parâmetro `delete` neste formato para excluir um ativo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Este é um exemplo de resposta quando um ativo de imagem é excluído:

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

Você pode usar os seguintes campos na sequência de consulta de URL para excluir um ativo:

| Parâmetro de URL | Obrigatório/opcional | Valor |
| --- | --- | --- |
| `op` | Obrigatório | excluir |
| `shared_secret` | Obrigatório | A chave secreta compartilhada da empresa. |
| `image_name` | Obrigatório | Nome do ativo a ser excluído. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>O suporte para ativos de imagem vetorial UGC novos ou existentes no Adobe Dynamic Media Classic terminou em 30 de setembro de 2021.

**Exemplo de URL da imagem:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
