---
title: Exclusão de um ativo carregado
seo-title: Exclusão de um ativo carregado
description: 'null'
seo-description: Saiba como excluir um ativo carregado.
uuid: edd 2 b 688-c 377-4 be 1-ba 16-d 2 dd 2 e 6 f 716 d
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: dd 338 c 8 c -06 c 6-44 d 5-8493-dc 2087 eeeafb
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Exclusão de um ativo carregado{#deleting-an-uploaded-asset}

É possível usar o `delete` parâmetro neste formato para excluir um ativo:

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

Você pode usar os seguintes campos na sequência de consulta do URL para excluir um ativo:

| Parâmetro de URL | Obrigatório/opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | delete |
| shared_ secret | Obrigatório | A chave compartilhada para a empresa. |
| <ul><li>Para imagens: image_ name</li><li>Para vetor: fxg_ name</li></ul> | Obrigatório | Nome do ativo a ser excluído. |

**Exemplo de URL da imagem:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Exemplo de URL de vetor:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
