---
title: Obtendo informações de uso do disco
seo-title: Obtendo informações de uso do disco
description: nulo
seo-description: Saiba como obter informações de uso do disco.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Obtendo informações de uso do disco {#getting-disk-usage-information}

Você pode usar o `disk_info` parâmetro para recuperar informações sobre o uso do espaço em disco de uma empresa, como mostra o exemplo a seguir:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Uma amostra de resposta é semelhante ao seguinte:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Você pode usar os seguintes campos na sequência de query do URL para obter informações de uso do disco:

| Parâmetro de URL | Obrigatório/opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | disk_info |
| shared_secret | Obrigatório | A chave do segredo compartilhado para a empresa |

O código de amostra a seguir obtém informações do disco para a Empresa 000:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

