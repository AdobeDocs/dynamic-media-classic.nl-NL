---
title: Een rasterafbeeldingselement uploaden
description: Leer hoe u rasterafbeeldingen kunt uploaden naar Adobe Dynamic Media Classic
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 0%

---

# Een rasterafbeeldingselement uploaden {#uploading-an-image-asset-or-a-vector-asset}

Voordat u een afbeeldingselement kunt uploaden, vraagt u eerst om een sleutel voor een gedeeld geheim. U gebruikt deze sleutel voor gedeeld geheim om een token voor uploaden op te halen. Vervolgens gebruikt u het uploadtoken om rasterafbeeldingselementen te uploaden.

>[!IMPORTANT]
>
>Vanaf 1 mei 2023 zijn UGC-middelen in Dynamic Media beschikbaar voor gebruik tot 60 dagen na de uploaddatum. Na 60 dagen worden de middelen verwijderd.

>[!NOTE]
>
>De ondersteuning voor nieuwe of bestaande UGC-vectorelementen in Adobe Dynamic Media Classic liep af op 30 september 2021.

## Een gedeelde geheime sleutel aanvragen {#requesting-a-shared-secret-key}

Verzoek om een *gedeelde geheime sleutel* door [het gebruiken van de Admin Console om een steungeval tot stand te brengen.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) In uw steungeval, verzoek om een gedeelde geheime sleutel.

Geef in het e-mailbericht de bedrijfsnaam op die u wilt gebruiken om afbeeldingselementen te uploaden. Nadat u de sleutel van Adobe Dynamic Media Classic ontvangt, bewaar het plaatselijk voor toekomstig gebruik.

## Het uploadtoken ophalen {#retrieving-the-upload-token}

De *uploadtoken* zorgt ervoor dat niemand de zelfde gedeelde geheime sleutel kan gebruiken om activa te uploaden. Het zorgt ervoor dat de upload legitiem is en uit een vertrouwde bron komt.

Het uploadtoken is een alfanumerieke tekenreeks die alleen voor een bepaalde hoeveelheid tijd beschikbaar is. Gebruik de volgende URL&#39;s, waarbij u de sleutel voor een gedeeld geheim vervangt, zodat u het token voor uploaden kunt ophalen.

* Rasterafbeelding
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`In dit voorbeeld is de sleutel voor gedeeld geheim `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

Standaard verloopt het uploadtoken vijf minuten (300 seconden) nadat u het hebt opgehaald. Als u meer tijd wilt aanvragen, neemt u `expires` in de URL en de tijd die u nodig hebt, in seconden. Met de volgende voorbeeldafbeelding haalt u bijvoorbeeld een uploadtoken op dat 1800 seconden geldig is:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

De geslaagde reactie voor afbeeldingen ziet er ongeveer als volgt uit:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Sla het token voor uploaden lokaal op voor gebruik met toekomstige aanvragen.

U kunt de volgende velden in de URL-queryreeks gebruiken om een token voor uploaden op te halen:

| URL-parameter | Vereist of optioneel | Waarde |
| --- | --- | --- |
| op | Vereist | get_uploadtoken |
| shared_geheime | Vereist | De sleutel van het gedeelde geheim voor het bedrijf dat uploadt. |
| verloopt | Optioneel | Aantal seconden dat de uploadtoken geldig is. De standaardwaarde is 300 seconden, als deze niet is opgegeven. |

**Voorbeeld van URL van rasterafbeelding:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**Toegestane HTTP-methoden:**
`GET` en `POST`

U kunt nu een afbeeldingselement uploaden.

Zie [Een afbeeldingselement uploaden](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Een rasterafbeeldingselement uploaden {#uploading-an-image-asset}

Nadat u een uploadtoken hebt opgehaald dat gedurende een bepaalde periode geldig is, kunt u een afbeeldingselement uploaden. U uploadt het element als multipart/form post terwijl het verzenden van de rest waarden als URL vraagkoord, zoals aangetoond in dit voorbeeld:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

De `upload_token` en `company_name` velden zijn vereist.

Zie [Het uploadtoken ophalen](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Zie [Een sleutel van een gedeeld geheim ophalen](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

U kunt ook andere optionele waarden verzenden als URL-querytekenreeksen, zoals in dit voorbeeld:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

De `file_limit` parameter geeft de maximale bestandsgrootte op in bytes. De `file_exts` parameter geeft de bestandsextensies aan die mogen worden geüpload. Beide waarden zijn optioneel.

Er wordt een algemene limiet ingesteld in de toepassing voor de maximale bestandsgrootte en de toegestane bestandsextensies. Als wat u in het verzoek verzendt een ondergroep van de globale grenzen is, wordt het geëerd. De globale limieten zijn als volgt:

| Globale limiet | Waarde |
| --- | --- |
| Bestandsgrootte voor alle clients | 20 MB |
| Ondersteunde bestandsindelingen voor afbeeldingen die u wilt uploaden | BMP, GIF, JPG, PNG, PSD, TIFF |

Met het volgende HTML-formulier kan een gebruiker een element uploaden. In het formulier wordt de gebruiker gevraagd de volgende gegevens in te voeren:

* Een bedrijfsnaam.
* Een token voor uploaden.
* Een maximale bestandsgrootte.
* Een lijst met bestandsextensies.
* Of het kleurprofiel en de bestandsnaam die aan het element zijn gekoppeld, behouden moeten blijven.
* Of de achtergrond uitnemen moet worden gebruikt. Als u Achtergrond uitnemen inschakelt, stelt u de Hoek, Tolerantie en Vulmethode in.
Zie Achtergrond uitnemen in [Opties voor het verfijnen van afbeeldingen tijdens het uploaden](image-editing-options-upload.md#image-editing-options-at-upload).
* De naam van het bestand dat moet worden geüpload.

U kunt de broncode van de HTML die aan het bovenstaande formulier is gekoppeld, bekijken door [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Klik in Firefox met de rechtermuisknop in het browservenster en selecteer **[!UICONTROL View Page Source]**. De code toont het overeenkomstige URL vraagkoord en de methode van de POST die in werking worden gesteld wanneer de gebruiker klikt **[!UICONTROL Submit]**.

Ga naar **[!UICONTROL View]** > **[!UICONTROL Source]**. Ga naar **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Web Developer Tools]**. Firefox wordt aanbevolen voor het weergeven van XML-reacties.

Hier volgt een voorbeeldreactie van een geslaagde upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>Het geüploade element (JPG, GIF, enzovoort) wordt geconverteerd naar de PTIFF-indeling en de reactie verstuurt een directe koppeling naar dat PTIFF-element.

Het middel is als elke andere bron ImageServing; U kunt er verwerkingsquery&#39;s op toepassen. De volgende URL vraagt bijvoorbeeld om een element dat naar de opgegeven breedte en hoogte wordt uitgerekt.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Verzend het element dat u wilt uploaden als multipart/form-post terwijl u de overige waarden verzendt als een URL-queryreeks. U kunt de volgende velden in de URL-queryreeks gebruiken om een element te uploaden:

| URL-parameter | Vereist of optioneel | Waarde |
| --- | --- | --- |
| `op` | Vereist | uploaden |
| `upload_token` | Vereist | Upload token voor de sleutel voor gedeeld geheim die aan het bedrijf is gekoppeld. |
| `company_name` | Vereist | Naam van het bedrijf dat de upload uitvoert. |
| `file_limit` | Optioneel | Bestandsgroottelimiet, in bytes, voor het element. |
| `file_exts` | Optioneel | Lijst met toegestane extensies voor het afbeeldingselementbestand. |
| `preserve_colorprofile` | Optioneel | Behoudt een ingesloten kleurprofiel terwijl het geüploade bestand wordt geconverteerd naar PTIFF-indeling. Mogelijke waarden zijn true of false. De standaardwaarde is false. |
| `preserve_filename` | Optioneel | De bestandsnaam van het geüploade element blijft behouden. Mogelijke waarden zijn true of false. De standaardwaarde is false. |

>[!NOTE]
>
>U moet het te uploaden element verzenden als het enige veld in een aanvraag voor een multipart-POST.

**Voorbeeld-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Toegestane HTTP-methode:**

POST

### Metagegevens van elementen ophalen voor afbeeldingen {#getting-asset-metadata-for-images}

U kunt `image_info` om metagegevens op te halen voor een element dat u hebt geüpload, zoals in het volgende voorbeeld wordt getoond:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Een voorbeeld van een succesvolle reactie lijkt op het volgende:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

U kunt de volgende velden in de URL-queryreeks gebruiken om informatie voor een element op te vragen:

| URL-parameter | Vereist of optioneel | Waarde |
| --- | --- | --- |
| `op` | Vereist | image_info |
| `shared_secret` | Vereist | De gedeelde geheime sleutel voor het bedrijf. |
| `image_name` | Vereist | Naam van de afbeelding. |

**Voorbeeld-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Toegestane HTTP-methode:**

GET en POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->