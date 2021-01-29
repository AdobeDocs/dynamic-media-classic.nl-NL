---
title: Een afbeeldingselement of een vectorelement uploaden
description: Leer hoe u een afbeeldingselement of een vectorelement uploadt.
uuid: d0e4a754-8a49-4b0f-b202-e9003bdb8f20
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: de21dca9-99fe-4183-b647-debfe112fda4
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1527'
ht-degree: 0%

---


# Een afbeeldingselement of een vectorelement uploaden{#uploading-an-image-asset-or-a-vector-asset}

Voordat u een afbeeldingselement kunt uploaden, vraagt u eerst om een sleutel voor een gedeeld geheim. U gebruikt deze sleutel voor gedeeld geheim om een token voor uploaden op te halen. Vervolgens gebruikt u het token voor uploaden om afbeeldingselementen of vectorelementen te uploaden.

## Verzoek om een gedeelde geheime sleutel {#requesting-a-shared-secret-key}

Vraag een *gedeelde-geheime sleutel* door [gebruikend de Admin Console om een steungeval tot stand te brengen.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) In uw steungeval, verzoek om een gedeelde geheime sleutel.

Geef in het e-mailbericht de bedrijfsnaam op die u wilt gebruiken om afbeeldingselementen te uploaden. Nadat u de sleutel van de Klassiek van Dynamic Media ontvangt, bewaar het plaatselijk voor toekomstig gebruik.

## Het uploadtoken {#retrieving-the-upload-token} ophalen

Met de *upload-token* kan niemand dezelfde sleutel voor gedeeld geheim gebruiken om elementen te uploaden. Het zorgt ervoor dat de upload legitiem is en uit een vertrouwde bron komt.

Het uploadtoken is een alfanumerieke tekenreeks die alleen voor een bepaalde hoeveelheid tijd beschikbaar is. Gebruik de volgende URL&#39;s, waarmee u de sleutel voor een gedeeld geheim vervangt, om het token voor uploaden op te halen.

* Afbeelding
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`In dit voorbeeld is de sleutel voor gedeeld geheim  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vector
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In dit voorbeeld is de sleutel voor gedeeld geheim  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Standaard verloopt het uploadtoken vijf minuten (300 seconden) nadat u het hebt opgehaald. Als u meer tijd wilt aanvragen, neemt u `expires` op in de URL en neemt u de hoeveelheid tijd op die u nodig hebt in seconden. Met de volgende voorbeeldafbeelding haalt u bijvoorbeeld een uploadtoken op dat 1800 seconden geldig is:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

De geslaagde reactie voor afbeeldingen ziet er als volgt uit:

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
|--- |--- |--- |
| op | Vereist | get_uploadtoken |
| shared_geheime | Vereist | De sleutel van het gedeelde geheim voor het bedrijf dat uploadt. |
| verloopt | Optioneel | Aantal seconden dat de uploadtoken geldig is. De standaardwaarde is 300 seconden, als deze niet is opgegeven. |

**URL van voorbeeldafbeelding:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Voorbeeld-URL voor vector:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Toegestane HTTP-methoden:** GET en POST

U kunt nu een afbeeldingselement uploaden.

Zie [Een afbeeldingselement uploaden](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Een afbeeldingselement {#uploading-an-image-asset} uploaden

Nadat u een uploadtoken hebt opgehaald dat gedurende een bepaalde periode geldig is, kunt u een afbeeldingselement uploaden. U uploadt het element als multipart/form post terwijl het verzenden van de rest waarden als URL vraagkoord, zoals aangetoond in dit voorbeeld:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

De velden `upload_token` en `company_name` zijn vereist.

Zie [De uploadtoken](uploading-image-asset-or-vector.md#retrieving_the_upload_token) ophalen.

Zie [Een sleutel van een gedeeld geheim ophalen](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

U kunt ook andere optionele waarden verzenden als URL-querytekenreeksen, zoals in dit voorbeeld:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

Met de parameter `file_limit` wordt de maximale bestandsgrootte in bytes opgegeven. Met de parameter `file_exts` worden de bestandsextensies opgegeven die mogen worden geüpload. Beide waarden zijn optioneel.

Er wordt een algemene limiet ingesteld in de toepassing voor de maximale bestandsgrootte en de toegestane bestandsextensies. Als wat u in het verzoek verzendt een ondergroep van de globale grenzen is, wordt het geëerd. De globale limieten zijn als volgt:

| Globale limiet | Waarde |
|--- |--- |
| Bestandsgrootte voor alle clients | 20 MB |
| Ondersteunde bestandsindelingen voor afbeeldingen die u wilt uploaden | BMP, GIF, JPG, PNG, PSD |

In het volgende HTML-formulier kan een gebruiker een element uploaden. In het formulier wordt de gebruiker gevraagd de volgende gegevens in te voeren:

* Een bedrijfsnaam.
* Een token voor uploaden.
* Een maximale bestandsgrootte.
* Een lijst met bestandsextensies.
* Bepaalt of het kleurprofiel en de bestandsnaam die aan het element zijn gekoppeld, moeten worden behouden.
* Of de achtergrond Uitnemen al dan niet wordt gebruikt. Als u Achtergrond uitnemen inschakelt, stelt u de Hoek, Tolerantie en Vulmethode in. Zie Achtergrond uitnemen in [Opties voor Beeldbewerking bij uploaden](image-editing-options-upload.md#image-editing-options-at-upload).
* De naam van het bestand dat moet worden geüpload

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

U kunt de HTML-broncode die aan het bovenstaande formulier is gekoppeld, weergeven door op de volgende koppeling te klikken:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Klik in Firefox met de rechtermuisknop in het browservenster en klik vervolgens op **Paginabron weergeven**. De code toont het overeenkomstige URL vraagkoord en de methode van de POST die in werking worden gesteld wanneer de gebruiker **Submit** klikt.

Als u de XML-reactie wilt weergeven in Internet Explorer, klikt u op **Weergave > Bron**. Als u de XML-reactie in Firefox wilt weergeven, klikt u op **Gereedschappen > Webontwikkelaar > Pagina-bron**. Firefox wordt aanbevolen voor het weergeven van XML-reacties.

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
>Het geüploade element (JPG, GIF, enzovoort) wordt geconverteerd naar de PTIFF-indeling en het antwoord verzendt een directe koppeling naar dat PTIFF-element.

Het middel is als elke andere bron ImageServing; U kunt er verwerkingsquery&#39;s op toepassen. De volgende URL vraagt bijvoorbeeld om een element dat naar de opgegeven breedte en hoogte wordt uitgerekt.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Verzend het element dat u wilt uploaden als multipart/form-post terwijl u de overige waarden verzendt als een URL-queryreeks. U kunt de volgende velden in de URL-queryreeks gebruiken om een element te uploaden:

| URL-parameter | Vereist of optioneel | Waarde |
|--- |--- |--- |
| op | Vereist | uploaden |
| upload_token | Vereist | Upload token voor de sleutel voor gedeeld geheim die aan het bedrijf is gekoppeld. |
| company_name | Vereist | Naam van het bedrijf dat de upload uitvoert. |
| file_limit | Optioneel | Bestandsgroottelimiet, in bytes, voor het element. |
| file_exts | Optioneel | Lijst met toegestane extensies voor het afbeeldingselementbestand. |
| preserve_colorProfile | Optioneel | Behoudt een ingesloten kleurprofiel terwijl het geüploade bestand wordt geconverteerd naar PTIFF-indeling. Mogelijke waarden zijn true of false. De standaardwaarde is false. |
| preserve_filename | Optioneel | De bestandsnaam van het geüploade element blijft behouden. Mogelijke waarden zijn true of false. De standaardwaarde is false. |

>[!NOTE]
>
>U moet het te uploaden element verzenden als het enige veld in een aanvraag voor een multipart-POST.

**Voorbeeld-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Toegestane HTTP-methode:**

POST

### Metagegevens van elementen ophalen voor afbeeldingen {#getting-asset-metadata-for-images}

U kunt `image_info` gebruiken om meta-gegevens voor activa terug te winnen die u uploadde, zoals aangetoond in het volgende voorbeeld:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Een voorbeeld van een geslaagde reactie ziet er als volgt uit:

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
|--- |--- |--- |
| op | Vereist | image_info |
| shared_geheime | Vereist | De gedeelde geheime sleutel voor het bedrijf. |
| image_name | Vereist | Naam van de afbeelding. |

**Voorbeeld-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Toegestane HTTP-methode:**

GET en POST

## Een vectorelement {#uploading-a-vector-asset} uploaden

Nadat u een uploadtoken hebt opgehaald dat gedurende een bepaalde periode geldig is, kunt u een vectorelement uploaden. U uploadt het element als multipart/form post terwijl het verzenden van de rest waarden als URL vraagkoord, zoals aangetoond in dit voorbeeld:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

De velden `upload_token` en `company_name` zijn vereist.

Zie [De uploadtoken](uploading-image-asset-or-vector.md#retrieving_the_upload_token) ophalen.

Zie [Een sleutel van een gedeeld geheim ophalen](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

U kunt ook andere optionele waarden verzenden als URL-querytekenreeksen, zoals in dit voorbeeld:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

Met de parameter `file_limit` wordt de maximale bestandsgrootte in bytes opgegeven. Met de parameter `file_exts` worden de bestandsextensies opgegeven die mogen worden geüpload. Beide waarden zijn optioneel.

Er wordt een algemene limiet ingesteld in de toepassing voor de maximale bestandsgrootte en de toegestane bestandsextensies. Als wat u in het verzoek verzendt een ondergroep van de globale grenzen is, wordt het geëerd. De globale limieten zijn als volgt:

| Globale limiet | Waarde |
|--- |--- |
| Bestandsgrootte voor alle clients | 20 MB |
| Ondersteunde vectorbestandsindelingen voor uploaden | AI, EPS, PDF (alleen wanneer de PDF eerder is geopend en opgeslagen in Adobe Illustrator CS6) |

In het volgende HTML-formulier kan een gebruiker een element uploaden. In het formulier wordt de gebruiker gevraagd de volgende gegevens in te voeren:

* Een bedrijfsnaam.
* Een token voor uploaden.
* Een maximale bestandsgrootte.
* Een lijst met bestandsextensies.
* Bepaalt of het kleurprofiel en de bestandsnaam die aan het element zijn gekoppeld, moeten worden behouden.
* Of de achtergrond Uitnemen al dan niet wordt gebruikt. Als u Achtergrond uitnemen inschakelt, stelt u de Hoek, Tolerantie en Vulmethode in. Zie Achtergrond uitnemen in [Opties voor Beeldbewerking bij uploaden](image-editing-options-upload.md#image-editing-options-at-upload).
* De naam van het bestand dat moet worden geüpload

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

De volgende HTML-code wordt weergegeven wanneer u met de rechtermuisknop in het browservenster klikt en vervolgens op **Bron weergeven** klikt voor het formulier dat in de illustratie wordt weergegeven. De code toont het overeenkomstige URL vraagkoord en de methode van de POST die in werking worden gesteld wanneer de gebruiker **Submit** klikt.

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
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Als u de XML-reactie in Internet Explorer wilt weergeven, klikt u op **Weergave** > **Bron**. Als u de XML-reactie in Firefox wilt weergeven, klikt u op **Weergave** > **Paginabron**. Firefox wordt aanbevolen voor het weergeven van XML-reacties.

Hier volgt een voorbeeldreactie van een geslaagde upload:

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
>Het geüploade element (AI, EPS, PDF enzovoort) wordt geconverteerd naar de FXG-indeling en het antwoord verstuurt een directe koppeling naar dat FXG-element.

Het middel is als elke andere Web-aan-druk middel; U kunt er verwerkingsquery&#39;s op toepassen. De volgende URL converteert bijvoorbeeld een FXG-bron naar een afbeelding van 500 x 500 png.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Verzend het element dat u wilt uploaden als multipart/form-post terwijl u de overige waarden verzendt als een URL-queryreeks. U kunt de volgende velden in de URL-queryreeks gebruiken om een element te uploaden:

| URL-parameter | Vereist of optioneel | Waarde |
|--- |--- |--- |
| op | Vereist | uploaden |
| upload_token | Vereist | Upload token voor de sleutel voor gedeeld geheim die aan het bedrijf is gekoppeld. |
| company_name | Vereist | Naam van het bedrijf dat de upload uitvoert. |
| file_limit | Optioneel | Bestandsgroottelimiet, in bytes, voor het element. |
| file_exts | Optioneel | Lijst met toegestane extensies voor het elementbestand. |

>[!NOTE]
>
>U moet het te uploaden element verzenden als het enige veld in een aanvraag voor een multipart-POST.

**Voorbeeld-URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Toegestane HTTP-methode:**

POST
