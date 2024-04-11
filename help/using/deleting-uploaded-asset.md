---
title: Excluir um ativo de imagem rasterizada carregado
description: Saiba como excluir um ativo carregado no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Excluir um ativo carregado{#deleting-an-uploaded-asset}

Você pode usar o `delete` neste formato para excluir um ativo:

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

Você pode usar os seguintes campos na sequência de consulta do URL para excluir um ativo:

| Parâmetro de URL | Obrigatório/opcional | Valor |
| --- | --- | --- |
| `op` | Obrigatório | excluir |
| `shared_secret` | Obrigatório | A chave que é um segredo compartilhado para a empresa. |
| `image_name` | Obrigatório | Nome do ativo a ser excluído. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>A partir de 1 de maio de 2023, os ativos UGC no Dynamic Media estarão disponíveis para uso por até 60 dias a partir da data do upload. Após 60 dias, os ativos serão removidos.

>[!NOTE]
>
>O suporte a ativos de imagem vetorial UGC novos ou existentes no Adobe Dynamic Media Classic terminou em 30 de setembro de 2021.

**Amostra da URL da imagem:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
