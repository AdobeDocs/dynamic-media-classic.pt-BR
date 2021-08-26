---
title: Obter informações sobre o uso do disco
description: Saiba como obter informações de uso do disco no Adobe Dynamic Media Classic.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---

# Obter informações sobre o uso do disco {#getting-disk-usage-information}

Você pode usar o parâmetro `disk_info` para recuperar informações sobre o uso do espaço em disco de uma empresa, como mostrado no exemplo a seguir:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Um exemplo de resposta é semelhante ao seguinte:

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

Você pode usar os seguintes campos na string de consulta de URL para obter informações de uso do disco:

| Parâmetro de URL | Obrigatório/opcional | Valor |
| --- | --- | --- |
| op | Obrigatório | disk_info |
| shared_secret | Obrigatório | A chave secreta compartilhada para a empresa |

O código de amostra a seguir obtém informações do disco para a empresa 000Empresa:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
