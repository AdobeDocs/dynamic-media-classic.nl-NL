---
title: Bestanden uploaden
description: Leer hoe u bestanden uploadt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '3657'
ht-degree: 0%

---

# Bestanden uploaden{#uploading-files}

Voordat u bestanden met elementen uploadt naar Adobe Dynamic Media Classic, moet u controleren of de elementbestanden een juiste naam hebben. En zorg ervoor dat uw omslagstructuur opstelling en georganiseerd is zoals u wilt. U kunt bestanden uploaden vanaf een door Adobe Dynamic Media Classic verschafte FTP-site of rechtstreeks vanaf uw computer of netwerk. Adobe Dynamic Media Classic biedt opties voor het optimaliseren van bestanden tijdens het uploaden. Als u de Adobe Dynamic Media Classic Desktop-toepassing hebt geïnstalleerd, kunt u bestanden en mappen uploaden door deze rechtstreeks vanaf uw bureaublad te slepen. Zie [Algemene instellingen van toepassing](application-setup.md#general_settings).

## Elementen en mappen voorbereiden voor uploaden {#preparing-your-assets-and-folders-for-uploading}

Voordat u elementen uploadt naar Adobe Dynamic Media Classic, moet u controleren of ze de juiste indeling en grootte hebben. U moet ook de Adobe Dynamic Media Classic-regels voor het benoemen van elementen in acht nemen. Door een maporganisatie en -structuur voor de bestanden in te stellen, zorgt u ervoor dat u bestanden gemakkelijk kunt vinden en ermee kunt werken.

### Ondersteunde bestandsindelingen {#supported-asset-file-formats}

In deze tabel worden de bestandsindelingen weergegeven die door Adobe Dynamic Media Classic worden ondersteund. Zie voor informatie over ondersteunde Camera Raw bestanden [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Indelingen voor elementbestanden | Beschrijving |
| --- | --- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Style Sheet | CSS |
| Kleurprofielen | ICC, ICM |
| Lettertypen | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Afbeeldingen | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (alleen Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG en Camera Raw |
| PostScript | EPS, PS |
| Adobe Dynamic Media Classic-ontwerpen van afbeeldingen | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Ondersteuning voor TAR- en ZIP-upload bevat een selectievakje om aan te geven of u de bestanden wilt uitpakken.

### Niet-ondersteunde afbeeldingsindelingen in Dynamic Media {#unsupported-image-formats-dynamic-media}

In de volgende lijst worden de subtypen beschreven van de bestandsindelingen voor rasterafbeeldingen die *niet* ondersteund in Dynamic Media.

Zie ook [Niet-ondersteunde bestandsindelingen detecteren voor Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* PNG-bestanden met een IDAT-segmentgrootte groter dan 100 MB.
* PSB-bestanden
* PSD-bestanden met een andere kleurruimte dan CMYK, RGB, Grijswaarden of Bitmap worden niet ondersteund. DuoTone-, Lab- en Geïndexeerde kleurruimten worden niet ondersteund.
* PSD-bestanden met een bitdiepte groter dan 16.
* TIFF-bestanden met zwevende-kommagegevens.
* TIFF-bestanden met Lab-kleurruimte.

### Elementen {#asset-types}

Voor optimale resultaten met het Adobe Dynamic Media Classic-programma moet u de aanbevolen bestandsindelingen en -grootten gebruiken. In deze tabel worden de elementtypen weergegeven, waarvan sommige de aanbevolen indelingen en bestandsgrootten hebben voor veelgebruikte elementen.

| Type element | Beschrijving/Recommendations |
| --- | --- |
| Audio | Invoergeluidsindelingen voor audio-elementen zijn AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. U kunt audio naar de volgende indelingen transcoderen: MP3, AAC en HE-AAC. |
| Afbeeldingen (voor Afbeeldingsgrootte, Zoomen, Afbeeldingssets, Spin-sets) | Afbeeldingen moeten ten minste 2000 pixels groot zijn. De meeste afbeeldingen hebben een maximale grootte van 1500 tot 2500 pixels. Het wordt aanbevolen afbeeldingen zonder verlies in te stellen, zoals TIFF- en PNG-bestanden. Als u een JPEG-afbeelding gebruikt, gebruikt u de instellingen voor de hoogste kwaliteit. Animate GIF-bestanden worden op dezelfde manier verwerkt als andere statische inhoud. |
| eCatalogs | Gebruik PDF-bestanden met hoge resolutie die zijn gemaakt in Adobe Acrobat of een Adobe-Creative Suite-toepassing die is opgeslagen als &#39;geschikt voor drukpers&#39;. PDF bevatten alle benodigde lettertypen, afbeeldingen en maskers. En neem alle benodigde grafische elementen waarnaar wordt verwezen op, zoals enkele pagina&#39;s, spreads met twee pagina&#39;s of in een indeling met meerdere pagina&#39;s. Volgorde uw pagina&#39;s door de dossiers in alfanumerieke orde te noemen. Plaats alle PDF voor uw eCatalog in één enkele omslag voor gemak om te uploaden. U kunt opties voor uitsnijden selecteren bij het uploaden om het bijsnijdgebied te verwijderen uit PDF, zoals snijtekens, registratiedoelen of kleurenbalken. De meeste PDF-bestanden die klaar zijn voor gebruik op de drukpers bevinden zich in de CMYK-kleurruimte. Het is daarom belangrijk dat u het CMYK ICC-kleurprofiel opgeeft dat wordt gebruikt bij de PDF-bestanden. |
| Sjablonen | Een gelaagde afbeelding of lay-outontwerp dat tekst, afbeeldingen en lagen kan bevatten. Afbeeldingslagen, tekstreeksen en kenmerken, zoals kleur en grootte, kunnen worden geparametereerd zodat variabele gegevens kunnen worden aangepast. Afbeeldingsvereisten voor gebruik in sjablonen zijn gelijk aan die voor andere afbeeldingen. Bereid uw afbeeldingen voor in Photoshop of een ander beeldbewerkingsprogramma. Sla elke afbeelding op als een afgevlakt transparant bestand in TIFF- of PNG-indeling. Zorg ervoor dat de afbeeldingsresolutie geschikt is voor het verwachte gebruik. Afbeeldingen die u wilt afdrukken, zijn 300 ppi. |
| Video&#39;s | Adobe Dynamic Media Classic ondersteunt videobestanden die zijn opgeslagen in de indeling OGV en MP4. U kunt bestanden tijdens het uploaden naar MP4-indeling transcoderen. Zie [Ondersteunde bestandsindelingen](#supported-static-file-formats). |
| Lettertypen | Uploaded TrueType, `Type1` (Alleen Windows®), OpenType®-lettertypen en PhotoFonts. |
| Afbeeldingen | Afbeeldingen en gelaagde afbeeldingsbestanden. |
| Afbeeldingssets en stalensets | Een reeks verwante afbeeldingen die in een viewer kunnen worden weergegeven. |
| ICC-profielen | Een kleurprofiel dat u kunt gebruiken om een geüploade afbeelding vanuit de bronkleurruimte om te zetten in een andere kleurruimte. |
| Vignetten | Afbeeldingen die zijn gemaakt met het programma Image Authoring en verwante bestanden. |
| Inhoudbestanden | Adobe InDesign, Illustrator of Photoshop-inhoudsbestanden. |
| FXG-bestanden | Afbeeldingsindelingsbestanden met een resolutie-onafhankelijke indeling die u kunt gebruiken om aanpasbare sjablonen te maken voor uitvoer naar afdrukken, web, e-mail, bureaublad en apparaten. |
| SVG-bestanden | Schaalbare vectorafbeeldingsbestanden die servers van Image Serving kunnen renderen. |
| XML-bestanden | Bestanden die voorbewerkingsregels definiëren die worden gebruikt om het pad te wijzigen en delen van verzoeken te zoeken. |
| Cascading Style Sheet-bestanden. | CSS-skins uploaden om HTML5-viewers aan te passen. |
| JavaScript-bestanden | JavaScript-bestanden worden gebruikt voor viewerinstrumentatie voor het bevatten van accountgegevens. De Veiligheid van de Adobe adviseert dit activatype slechts voor cliëntrekeningen die een afzonderlijk domein in gebruik voor levering hebben (om dwars-plaats scripting te vermijden). |

>[!NOTE]
>
>Wanneer u afbeeldingsbestanden en PDF uploadt naar Adobe Dynamic Media Classic, zet het systeem deze bronbestanden om in P-TIFF (Pyramid TIFF)-bestanden. Deze P-TIFF-bestanden zijn de bestanden die later worden gepubliceerd naar Dynamic Media Image Servers. Adobe Dynamic Media Classic gebruikt de Piramid Tiff-bestandsindeling omdat deze diverse zoomverhoudingen bevat waarmee u snel kunt inzoomen bij weergave met een Adobe Dynamic Media Classic Zoom Viewer.

### Ondersteunde statische bestandsindelingen {#supported-static-file-formats}

Adobe Dynamic Media Classic ondersteunt verschillende statische bestandsindelingen. Statische inhoud is elk element dat &#39;as-is&#39; wordt gepubliceerd, zoals CSS, PDF, SVG en XML.

De volgende bestandstypen kunnen worden gepubliceerd:

* Geanimeerd GIF
* Audiobestanden
* CSS
* JavaScript (wanneer het bedrijf met zijn eigen domein wordt gevormd)
* Primaire video
* PDF (wanneer PDF is gemarkeerd voor publicatie na uploaden, om te voorkomen dat alle PDF voor bestaande eCatalog/PDF-workflow worden geleverd)
* PrX-video
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic biedt geen optie om een voorbeeld-URL van statische inhoud te genereren.

### Bestandsnaamvereisten {#filename-requirements}

Omdat bestandsextensies tijdens het uploaden worden verwijderd uit bestandsnamen, staat het systeem niet toe dat bestanden dezelfde hoofdnaam hebben. In het Adobe Dynamic Media Classic-systeem wordt de bestandsnaam van het element minus de bestandsnaamextensie de element-id voor het element. Daarom kunnen geen twee elementen dezelfde naam hebben.

Zorg ervoor dat alle gebruikers in uw bedrijf deze regels voor het noemen van dossiers begrijpen:

* Element-id&#39;s met dezelfde naam zijn niet toegestaan in het systeem.
* Namen van element-id zijn hoofdlettergevoelig.
* Als beste praktijken, zorg ervoor dat activa IDs geen lege ruimten (bijvoorbeeld, zwarte jasje.tif en blauw jpg) bevat. Adobe Dynamic Media Classic ASCII codeert lege spaties in elementnamen wanneer elementnamen worden gebruikt om URL-tekenreeksen samen te stellen. Deze ASCII-codes zijn moeilijk leesbaar, waardoor het lezen van URL&#39;s moeilijker kan worden.
* Taalspecifieke tekens zijn toegestaan in bestandsnamen. De volgende tekens zijn echter niet toegestaan in bestandsnamen:

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  Als een bestandsnaam een of meer van de bovenstaande tekens bevat, worden de tekens tijdens het uploaden uit de bestandsnaam verwijderd.

Gewoonlijk kan de bestandsnaam van een element hetzelfde zijn als het itemnummer, de product-SKU of een andere naam als in het volgende voorbeeld:

| Item | Bestandsnaam | Element-id |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Maporganisatie en -structuur {#folder-organization-and-structure}

Organiseer en structureer mappen en submappen voor uw inhoud in Adobe Dynamic Media Classic voordat u de inhoud uploadt naar het systeem. Het plannen op deze manier heeft twee belangrijke voordelen:

* Wanneer u de inhoud via FTP uploadt naar Adobe Dynamic Media Classic, kunt u het systeem de mapstructuur laten repliceren tijdens het uploaden. Op deze manier wordt uw inhoud in dezelfde mappen en submappen in Adobe Dynamic Media Classic geordend als op uw computer of netwerk. (Als u de mapstructuur in Adobe Dynamic Media Classic wilt repliceren, selecteert u de optie Submappen opnemen wanneer u elementen uploadt via FTP.)
* Het is veel moeilijker om mappen in het systeem opnieuw te ordenen nadat bestanden zijn geüpload dan met een zorgvuldig overwogen mapstructuur te beginnen.

De methode en structuur voor het benoemen van mappen die u kiest voor het opslaan van uw inhoud op de Adobe Dynamic Media Classic, zijn afhankelijk van de behoeften van uw organisatie. Hier volgen enkele voorbeelden van mapstructuren:

**op SKU gebaseerd**: Mappen krijgen een naam op basis van SKU&#39;s of itemnummers. Er worden bijvoorbeeld aparte mappen gemaakt voor alle reeksen 0-, 20- en 30-cijfers.

**Op merk gebaseerd**: Voor fabrikanten met meerdere merklijnen en detailhandelaren die andere merken van andere bedrijven op de markt brengen, scheidt u bestanden in productmappen die voor verschillende merken worden genoemd.

**Projectgebaseerd**: Mappen worden ingedeeld op basis van de datum van de implementatie/neerzetbewerking of de naam van het project. Klanten die vooral eCatalogi produceren, zijn voor deze aanpak.

**Spiegelen van maphiërarchie van websites**: Deze mapstructuur weerspiegelt de mapstructuur van de website, met de mappen die bijvoorbeeld voor productcategorieën zijn benoemd.

## Bestanden uploaden {#uploading-your-files}

U kunt afzonderlijke bestanden uploaden vanaf het bureaublad of via FTP mappen uploaden. Als u meer dan 100 MB dossiers of uploadt volledige omslagen en subfolders wilt uploaden, selecteer **VIA FTP** tab.

Adobe Dynamic Media Classic stuurt je een e-mailbericht om te bevestigen wanneer je uploadtaak begint en eindigt en om je op de hoogte te stellen van eventuele problemen.

Tijdens (of direct na) een grote uploadtaak kunnen sommige nieuwe items het bericht &quot;Afbeelding nog niet geoptimaliseerd&quot; weergeven. Dit bericht wordt weergegeven omdat de bestanden nog niet volledig zijn verwerkt en aan Adobe Dynamic Media Classic zijn toegevoegd. U kunt deze bestanden later optimaliseren. Zie [Bestanden optimaliseren](application-setup.md#optimize_files).

### Bestanden uploaden met het tabblad Van bureaublad {#upload-files-using-sps-desktop-application}

Met de Adobe Dynamic Media Classic Desktop-toepassing kunt u bestanden en mappen uploaden door te slepen.

1. Selecteer in de Adobe Dynamic Media Classic Desktop-toepassing op de algemene navigatiebalk de optie **[!UICONTROL Upload]**.
1. Selecteer op de pagina Uploaden de optie **[!UICONTROL From Desktop]** tab.
1. Aan de linkerkant van de pagina Uploaden, in het dialoogvenster **[!UICONTROL Select Files for Upload]** gebied, selecteren **[!UICONTROL Browse]** om de bestanden of mappen te selecteren die u wilt uploaden, selecteert u vervolgens **[!UICONTROL Open]**.
1. Aan de rechterkant van de pagina Uploaden, in de gekozen **Mapdoel** navigeer naar een doelmap waar u de geüploade bestanden of mappen wilt toevoegen.
1. (Optioneel) Voer onder aan de pagina Uploaden in het tekstveld Taaknaam de nieuwe naam van de uploadtaak in. U kunt ook gewoon de standaardnaam gebruiken die door het systeem wordt gegenereerd en die door Adobe Dynamic Media Classic wordt opgegeven. Upload- en publicatietaken worden opgenomen op de pagina Taken, waar u de status van taken kunt controleren. Zie [Taakbestanden controleren](checking-job-files.md#checking_job_files).
1. (Optioneel) Selecteer onder aan de pagina Uploaden de optie **[!UICONTROL Publish After Uploading]** zodat u de elementen die u uploadt automatisch kunt publiceren.
Wanneer u bestanden publiceert, worden deze naar live servers verzonden. URL&#39;s voor deze bestanden kunnen vervolgens worden gebruikt op externe websites en toepassingen. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
1. (Optioneel) Selecteer onder aan de pagina Uploaden de optie **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** als u wilt dat de bestanden die u uploadt, bestaande bestanden met dezelfde naam vervangen. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
De naam van deze optie kan verschillen, afhankelijk van de instellingen in **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Selecteer in de rechterbenedenhoek van de pagina Uploaden de optie **[!UICONTROL Job Options]** en geeft u de gewenste opties op.

   Zie [Uploadopties](uploading-files.md#upload_options).

1. Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL Save]**.
1. Selecteer in de rechterbenedenhoek van de pagina Uploaden de optie **[!UICONTROL Submit Upload]**.
Selecteer **[!UICONTROL Jobs]** op de algemene navigatiebalk. U kunt blijven werken in Adobe Dynamic Media Classic. Keer op elk ogenblik op de pagina van Banen terug om een lopende baan te herzien. Als u een actieve uploadtaak wilt annuleren, selecteert u **[!UICONTROL Cancel]** naast de tijd van de Duur.

### Bestanden uploaden via het tabblad VIA FTP {#upload-files-using-via-ftp}

1. Meld u aan bij de FTP-site van Adobe Dynamic Media Classic die specifiek is voor uw specifieke regio. Gebruik de FTP-gebruikersnaam en het wachtwoord die u van de beheerder hebt ontvangen.
1. Selecteer in Adobe Dynamic Media Classic op de algemene navigatiebalk de optie **[!UICONTROL Upload]**.
1. Selecteer op de pagina Uploaden de optie **[!UICONTROL VIA FTP]** tab.
1. Aan de linkerkant van de pagina Uploaden, in het dialoogvenster **[!UICONTROL Choose FTP Folder For Upload]** , kiest u een FTP-map waaruit u bestanden wilt uploaden.
1. Aan de rechterkant van de pagina Uploaden, in de gekozen **[!UICONTROL Adobe Dynamic Media Folder Destination]** in Adobe Dynamic Media Classic.
1. (Optioneel) Voer onder aan de pagina Uploaden in het tekstveld Taaknaam de nieuwe naam van de uploadtaak in. U kunt ook gewoon de standaardnaam gebruiken die door het systeem wordt gegenereerd en die door Adobe Dynamic Media Classic wordt opgegeven. Upload- en publicatietaken worden opgenomen op de pagina Taken, waar u de status van taken kunt controleren.
Zie [Taakbestanden controleren](checking-job-files.md#checking_job_files).
1. (Optioneel) Selecteer onder aan de pagina Uploaden de optie **[!UICONTROL Publish After Upload]** zodat u de elementen die u uploadt automatisch kunt publiceren.
Wanneer u bestanden publiceert, worden deze naar live servers verzonden. URL&#39;s voor deze bestanden kunnen vervolgens worden gebruikt op externe websites en toepassingen. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
1. (Optioneel) Selecteer onder aan de pagina Uploaden de optie **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** als u wilt dat de bestanden die u uploadt, bestaande bestanden met dezelfde naam vervangen. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
De naam van deze optie kan verschillen, afhankelijk van de instellingen in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Optioneel; alleen beschikbaar als u de optie **[!UICONTROL VIA FTP]** tab. Selecteer onder aan de pagina Uploaden de optie **[!UICONTROL Uncompress Zip or Tar Files on Upload]** zodat u automatisch alle bestanden uit uw geüploade ZIP- of TAR-bestand kunt extraheren. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
1. Selecteer in de rechterbenedenhoek van de pagina Uploaden de optie **[!UICONTROL Job Options]** en geeft u de gewenste opties op.

   Zie [Uploadopties](uploading-files.md#upload_options).

1. Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL Save]**.
1. Selecteer in de rechterbenedenhoek van de pagina Uploaden de optie **[!UICONTROL Submit Upload]**.

   Als u de voortgang van het uploaden wilt zien, selecteert u op de algemene navigatiebalk de optie **[!UICONTROL Jobs]**. De pagina van Banen toont u de vooruitgang van het uploaden. U kunt blijven werken in Adobe Dynamic Media Classic. Keer op elk ogenblik op de pagina van Banen terug om een lopende baan te herzien.

Als u een actieve uploadtaak wilt annuleren, selecteert u **[!UICONTROL Cancel]** naast de tijd van de Duur.

## Opties voor uploaden, dialoogvenster {#upload-options}

Bij het uploaden van bestanden kunt u uit de volgende opties kiezen in het dialoogvenster Opties voor uploaden:

* **JOB**: Select **[!UICONTROL JOB]** om opties te kiezen die de volledige uploadtaak beïnvloeden.

  U kunt ook *default* opties voor het uploaden van taken met behulp van de **[!UICONTROL Default Upload Options]** in Algemene instellingen. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Default Upload Options]** Stel vervolgens de gewenste standaardopties in.

   * **[!UICONTROL When]**: Deze optie is alleen beschikbaar als u de optie **[!UICONTROL VIA FTP]** tab.
      * **[!UICONTROL One-Time]**: Geef een uploadtaak op die één keer wordt uitgevoerd. U kunt onder andere de volgende opties kiezen:
         * **[!UICONTROL Now]**: Voert de uploadtaak direct uit nadat u deze hebt geselecteerd **[!UICONTROL Save]** in het dialoogvenster Opties voor uploaden selecteert u vervolgens **[!UICONTROL Submit Upload]** op de uploadpagina.
         * **[!UICONTROL Schedule For Later]**: Selecteer het jaar, de maand, de dag en de tijd (in stappen van 15 minuten) waarop u de uploadtaak wilt uitvoeren.
      * **[!UICONTROL Recurring]**: Geef een uploadtaak op die dagelijks, wekelijks of maandelijks wordt uitgevoerd. Of pas de uploadtaak aan uw eigen specificaties aan.
         * **[!UICONTROL Daily]**: Stel de tijd in waarop de taak elke dag moet worden uitgevoerd. Als u de taak slechts van maandag tot en met vrijdag wilt uitvoeren, selecteert u **[!UICONTROL Weekdays Only]**.
         * **[!UICONTROL Weekly]**: Kies een specifieke dag van de week en tijd waarop de taak moet worden uitgevoerd.
         * **[!UICONTROL Monthly]**: Kies een specifieke dag van de maand of de dag van de week, inclusief de begintijd, waarop de taak moet worden uitgevoerd.
         * **[!UICONTROL Custom]**: Pas een upload- of publiceertaaktijdinterval aan uw eigen specificaties aan. Zie [Een aangepast tijdinterval voor uploaden of publiceren maken](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Publish After Uploading]**: Beschikbaar als u een van de **[!UICONTROL FROM DESKTOP]** of de **[!UICONTROL VIA FTP]** tab. Selecteer deze optie zodat u de elementen die u uploadt automatisch kunt publiceren. Wanneer u bestanden publiceert, worden deze naar live servers verzonden. URL&#39;s voor deze bestanden kunnen vervolgens worden gebruikt op externe websites en toepassingen. Deze optie is ook beschikbaar op de Upload pagina.

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]**: Beschikbaar als u een van de **[!UICONTROL FROM DESKTOP]** of de **[!UICONTROL VIA FTP]** tab. Selecteer deze optie als u wilt dat de bestanden die u uploadt, bestaande bestanden met dezelfde naam vervangen. Deze optie is ook beschikbaar op de Upload pagina. De naam van deze optie kan verschillen, afhankelijk van de instellingen in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.

   * **[!UICONTROL Uncompress Zip or Tar Files on Upload]**: Beschikbaar als u een van de **[!UICONTROL FROM DESKTOP]** of de **[!UICONTROL VIA FTP]** tab.
Selecteer deze optie zodat u automatisch alle bestanden kunt extraheren uit het geüploade ZIP- of TAR-bestand. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.

   * **[!UICONTROL Include subfolders]**: Alleen beschikbaar als u de optie **[!UICONTROL VIA FTP]** tab.
Selecteer deze optie als u submappen wilt uploaden van de map die u wilt uploaden. De namen van de map en de submappen die u uploadt, worden automatisch ingevoerd in Adobe Dynamic Media Classic.

   * **[!UICONTROL Process metadata files]**: Alleen beschikbaar als u een van de **[!UICONTROL VIA FTP]** tab. Selecteer deze optie als u een door tabs gescheiden of XML-bestand wilt uploaden om metagegevens aan meerdere elementen toe te voegen.
Zie [Metagegevens importeren (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Opties voor uitsnijden**: snijd automatisch pixels in witruimte uit een afbeelding. Open de **[!UICONTROL Crop]** menu, selecteert u **[!UICONTROL Manual]** en voert u pixelmetingen in in de tekstvelden Boven, Rechts, Onder en Links om vanaf de zijkanten uit te snijden. U kunt ook **[!UICONTROL Trim]** in het menu Uitsnijden en kies de volgende opties:

   * **[!UICONTROL Trim Away Based On]**: Kies of u wilt uitsnijden op basis van kleur of transparantie:
      * **[!UICONTROL Color]**: Kies de optie Kleur. Selecteer vervolgens het menu Hoek en kies de hoek van de afbeelding met de kleur die het beste overeenkomt met de kleur voor de witruimte die u wilt uitsnijden.
Bijsnijden op basis van kleur: geef 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de afbeelding hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.
      * **[!UICONTROL Transparency]**: Kies de optie **[!UICONTROL Transparency]** -optie.
Bijsnijden op basis van transparantie: geef 0 op om pixels alleen bij te snijden als ze transparant zijn; getallen dichter bij 1 zorgen voor meer transparantie.
      * **[!UICONTROL Tolerance]**: Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven.

* **Opties voor kleurprofielen**: Kies een kleurconversie wanneer u geoptimaliseerde bestanden maakt die worden gebruikt voor dynamische levering via Adobe Dynamic Media Classic:

   * **[!UICONTROL Default Color Preservation]**: Hiermee blijven de kleuren van de bronafbeelding behouden wanneer de afbeeldingen kleurruimte-informatie bevatten. Er is geen kleuromzetting. In bijna alle afbeeldingen van vandaag is het juiste kleurprofiel al ingesloten. Als een CMYK-bronafbeelding echter geen ingesloten kleurprofiel bevat, worden de kleuren omgezet in de kleurruimte sRGB (standaard rood-groen-blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.
   * **[!UICONTROL Keep Original Color Space]**: Behoudt de oorspronkelijke kleuren zonder kleurconversie op het punt van inname in Adobe Dynamic Media Classic. Voor afbeeldingen zonder ingesloten kleurprofiel wordt de vereiste kleurconversie voor het verwerken van aanvragen voor de afbeelding uitgevoerd met de standaardkleurprofielen die zijn geconfigureerd in de Publicatie-instellingen. Deze kleurprofielen worden niet altijd uitgelijnd met de kleuren in de bestanden die met deze optie zijn gemaakt. Daarom wordt u aangeraden de optie Standaardkleurbehoud te gebruiken.
   * **[!UICONTROL Custom From]** > **[!UICONTROL To]**: Hiermee opent u menu&#39;s, zodat u een **[!UICONTROL Convert From]** en **[!UICONTROL Convert To]** kleurruimte. Deze geavanceerde optie negeert alle kleurinformatie die in het bronbestand is ingesloten. Selecteer deze optie alleen als alle afbeeldingen die u verzendt onjuiste of ontbrekende kleurprofielgegevens bevatten.

* **Opties voor het bewerken van afbeeldingen**: U kunt de knipmaskers &lt;> in afbeeldingen behouden en een kleurprofiel kiezen.
Zie [Opties voor het verfijnen van afbeeldingen tijdens het uploaden](image-editing-options-upload.md#image-editing-options-at-upload).

* **Opties voor PostScript®**: U kunt PostScript®-bestanden rasteren, bestanden uitsnijden, transparante achtergronden behouden, een resolutie kiezen en een kleurruimte kiezen.
Zie [Werken met PostScript- en Illustrator-bestanden](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop-opties**: U kunt sjablonen maken van Adobe® Photoshop®-bestanden, lagen behouden, opgeven hoe lagen worden benoemd, tekst extraheren en opgeven hoe afbeeldingen in sjablonen worden verankerd.
Zie [Uploadopties voor PSD](psd-files.md#psd_upload_options).

* **PDF-opties**: U kunt de bestanden rasteren, zoekwoorden en koppelingen extraheren, automatisch een eCatalog genereren, de resolutie instellen en een kleurruimte kiezen.
Zie [Uploadopties voor PDF](pdfs.md#pdf_upload_options).

* **Illustrator-opties**: U kunt Adobe Illustrator®-bestanden rasteren, transparante achtergronden behouden, een resolutie kiezen en een kleurruimte kiezen.
Zie [Werken met PostScript- en Illustrator-bestanden](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO-opties**: U kunt een videobestand transcoderen door een videovoorinstelling te kiezen.
Zie [Werken met voorinstellingen voor videocodering](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Meer metagegevens**: Voer trefwoorden in die de bestanden beschrijven die u wilt uploaden. Trefwoorden worden door komma&#39;s van elkaar gescheiden. Met trefwoorden kunt u gemakkelijker naar elementen zoeken.
Zie [Een geavanceerde zoekopdracht uitvoeren](searching-assets.md#conducting_an_advanced_search).
Zie ook [Trefwoorden uploaden](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) trainingsvideo.

* **Voorinstellingen batchset**: Als u een Afbeeldingsset, Puntset of Staalset wilt maken van de geüploade bestanden, selecteert u de optie **[!UICONTROL Active]** voor de voorinstelling die u wilt gebruiken. U kunt meerdere voorinstellingen selecteren. U kunt de voorinstellingen maken op de pagina Voorinstellingen voor toepassingsinstellingen/batchsets.
Zie [Voorinstellingen batchset](application-setup.md#batch_set_presets).

* **Geavanceerd**: Zie [Uploaden met een andere taak volgen](uploading-files.md#follow-an-upload-with-another-job).

## Uploaden met een andere taak volgen {#follow-an-upload-with-another-job}

Wanneer u items uploadt met gebruik van FTP, kunt u een volgende taak plannen die moet beginnen wanneer het uploaden is voltooid. Als andere taken volgens de planning moeten beginnen, worden de taken die u hier plant, na deze taken in de wachtrij geplaatst.

De nieuwe baan verzendt een bericht naar het adres dat u specificeert zodat de code bij die plaats kan worden teweeggebracht. Deze vervolgpublicatietaak gebruikt dezelfde naam als de uploadtaak, maar met de tekst *Pub_* toegevoegd aan het begin.

**Een upload volgen met een andere taak:**

1. Selecteren **[!UICONTROL Upload]** en selecteert u vervolgens de **[!UICONTROL VIA FTP]** tab.
1. Selecteer in de rechterbenedenhoek van de pagina Uploaden de optie **[!UICONTROL Job Options]**.
1. Vouw in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL ADVANCED]** sectie.
1. Kies een van de volgende opties in het menu **[!UICONTROL Follow Upload with another job]** vervolgkeuzelijst:

   * Geen
   * HTTP-aanvraag
   * Publiceren van afbeeldingsserver
   * Publiceren van rendering van afbeeldingen
   * Video publiceren

1. Geef het HTTP-adres op.
1. Geef op of u alleen wilt werken als er bestanden zijn geüpload.
1. Geef aan of u deze aanvraag wilt uitvoeren telkens wanneer deze taak is voltooid, of alleen wanneer bestanden zijn gepubliceerd.

   >[!NOTE]
   >
   >Regelmatig geplande taken kunnen er soms toe leiden dat er geen bestanden worden gepubliceerd.

>[!MORELIKETHIS]
>
>* [Werken met middelenmappen](asset-folders.md#working_with_asset_folders)
>* [Terugkerende upload- en publicatietaken verwerken](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Een upload- of publicatietaak gebruiken als trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
