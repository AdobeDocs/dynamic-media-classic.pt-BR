---
title: Obter informações de uso do disco
description: Saiba como obter informações de uso do disco no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '91'
ht-degree: 0%

---

# Obter informações de uso do disco {#get-disk-usage-information}

Você pode usar o `disk_info` para recuperar informações sobre o uso de espaço em disco de uma empresa, conforme mostrado no exemplo a seguir:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Uma resposta de amostra é semelhante ao seguinte:

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

Você pode usar os seguintes campos na string de consulta do URL para obter informações de uso do disco:

| Parâmetro de URL | Obrigatório/opcional | Valor |
| --- | --- | --- |
| op | Obrigatório | disk_info |
| shared_secret | Obrigatório | A chave que é um segredo compartilhado para a empresa |

O código de exemplo a seguir obtém informações do disco para 000Empresa:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
