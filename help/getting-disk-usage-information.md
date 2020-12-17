---
title: Schijfgebruiksgegevens ophalen
seo-title: Schijfgebruiksgegevens ophalen
description: 'null'
seo-description: Leer hoe u informatie over schijfgebruik ophaalt.
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


# Informatie over schijfgebruik ophalen {#getting-disk-usage-information}

U kunt de parameter `disk_info` gebruiken om informatie over het gebruik van de schijfruimte van een bedrijf terug te winnen, zoals aangetoond in het volgende voorbeeld:

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
|--- |--- |--- |
| op | Vereist | disk_info |
| shared_geheime | Vereist | De gedeelde geheime sleutel voor het bedrijf |

De volgende steekproefcode krijgt schijfinformatie voor 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

