---
title: Schijfgebruiksgegevens ophalen
description: Leer hoe u informatie over schijfgebruik ophaalt in Adobe Dynamic Media Classic.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---

# Schijfgebruiksgegevens ophalen {#getting-disk-usage-information}

U kunt de `disk_info` parameter om informatie over het gebruik van de schijfruimte van een bedrijf, zoals aangetoond in het volgende voorbeeld terug te winnen:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Een voorbeeldreactie ziet er als volgt uit:

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

U kunt de volgende velden in de URL-queryreeks gebruiken om informatie over schijfgebruik op te halen:

| URL-parameter | Vereist/optioneel | Waarde |
| --- | --- | --- |
| op | Vereist | disk_info |
| shared_geheime | Vereist | De gedeelde geheime sleutel voor het bedrijf |

De volgende steekproefcode krijgt schijfinformatie voor 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
