---
title: Obter informações de uso do disco
seo-title: Obter informações de uso do disco
description: 'null'
seo-description: Saiba como obter informações de uso do disco.
uuid: 01361693-53 d 0-4072-b 7 c 3-f 284631 d 28 cf
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6763546 d -83 c 4-42 dc -879 f -6 bbfc 8 b 56482
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Obter informações de uso do disco {#getting-disk-usage-information}

Você pode usar o `disk_info` parâmetro para recuperar informações sobre o uso do espaço em disco de uma empresa, como mostrado no exemplo a seguir:

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

Você pode usar os seguintes campos na sequência de consulta do URL para obter informações de uso do disco:

| Parâmetro de URL | Obrigatório/opcional | Valor |
|--- |--- |--- |
| op | Obrigatório | disk_ info |
| shared_ secret | Obrigatório | A chave compartilhada para a empresa |

O exemplo de código a seguir obtém informações de disco para empresas: 00:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

