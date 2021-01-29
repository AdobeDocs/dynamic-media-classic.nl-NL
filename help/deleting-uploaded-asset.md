---
title: Geüploade elementen verwijderen
description: Leer hoe u een geüpload element verwijdert.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

---


# Een geüpload element verwijderen{#deleting-an-uploaded-asset}

Met de parameter `delete` in deze notatie kunt u een element verwijderen:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Hieronder ziet u een voorbeeld van een reactie wanneer een afbeeldingselement wordt verwijderd:

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

U kunt de volgende velden in de URL-queryreeks gebruiken om een element te verwijderen:

| URL-parameter | Vereist/optioneel | Waarde |
|--- |--- |--- |
| op | Vereist | delete |
| shared_geheime | Vereist | De gedeelde geheime sleutel voor het bedrijf. |
| <ul><li>Voor afbeeldingen:image_name</li><li>Voor Vector:fxg_name</li></ul> | Vereist | Naam van het element dat moet worden verwijderd. |

**URL van voorbeeldafbeelding:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Voorbeeld-URL voor vector:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
