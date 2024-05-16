---
title: Een geüpload rasterafbeeldingselement verwijderen
description: Leer hoe u een geüpload element in Adobe Dynamic Media Classic verwijdert.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Een geüpload element verwijderen{#deleting-an-uploaded-asset}

U kunt de `delete` parameter in deze notatie om een element te verwijderen:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Hieronder ziet u een voorbeeld van een reactie wanneer een afbeeldingselement wordt verwijderd:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| `op` | Vereist | delete |
| `shared_secret` | Vereist | De sleutel die een gedeeld-geheim voor het bedrijf is. |
| `image_name` | Vereist | Naam van het te verwijderen element. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>Vanaf 1 mei 2023 zijn UGC-middelen in Dynamic Media beschikbaar voor gebruik tot 60 dagen na de uploaddatum. Na 60 dagen worden de middelen verwijderd.

>[!NOTE]
>
>De ondersteuning voor nieuwe of bestaande UGC-vectorafbeeldingselementen in Adobe Dynamic Media Classic is afgelopen op 30 september 2021.

**URL van voorbeeldafbeelding:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
