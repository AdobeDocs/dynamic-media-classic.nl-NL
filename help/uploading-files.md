---
title: Bestanden uploaden
seo-title: Bestanden uploaden
description: 'null'
seo-description: Leer hoe u bestanden kunt uploaden.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '3855'
ht-degree: 0%

---


# Bestanden uploaden{#uploading-files}

Voordat u bestanden met elementen uploadt naar Dynamic Media Classic, moet u controleren of de elementbestanden een juiste naam hebben en of de mapstructuur op de gewenste manier is ingesteld en ingedeeld. U kunt bestanden uploaden vanaf een door Dynamic Media Classic geleverde FTP-site of rechtstreeks vanaf uw computer of netwerk. Dynamic Media Classic biedt opties voor het optimaliseren van bestanden terwijl u deze uploadt. Als u Adobe Dynamic Media Classic-bureaubladtoepassing hebt geïnstalleerd, kunt u bestanden en mappen uploaden door deze rechtstreeks vanaf uw bureaublad te slepen. (Zie [Algemene instellingen van toepassing](application-setup.md#general_settings).)

## Elementen en mappen voorbereiden voor het uploaden van {#preparing-your-assets-and-folders-for-uploading}

Voordat u elementen uploadt naar Dynamic Media Classic, moet u ervoor zorgen dat deze de juiste indeling en grootte hebben. U moet ook de Klassieke Dynamic Media-regels voor het benoemen van elementen in acht nemen. Door een maporganisatie en -structuur voor de bestanden in te stellen, zorgt u ervoor dat u bestanden gemakkelijk kunt vinden en ermee kunt werken.

### Ondersteunde bestandsindelingen {#supported-asset-file-formats}

In deze tabel worden de bestandsindelingen weergegeven die door Dynamic Media Classic worden ondersteund. Zie [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en) voor informatie over ondersteunde Camera Raw bestanden.

| Indelingen voor elementbestanden | Beschrijving |
|--- |--- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Style Sheet | CSS |
| Kleurprofielen | ICC, ICM |
| Lettertypen | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Afbeeldingen | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (alleen Windows), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG en Camera Raw |
| PostScript | EPS, PS |
| Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Ondersteuning voor TAR- en ZIP-upload bevat een selectievakje om aan te geven of u de bestanden wilt uitpakken.

### Niet-ondersteunde afbeeldingsindelingen in Dynamic Media {#unsupported-image-formats-dynamic-media}

In de volgende lijst worden de subtypen van rasterafbeeldingsbestandsindelingen beschreven die *niet* worden ondersteund in Dynamic Media.

Zie ook [Niet-ondersteunde bestandsindelingen detecteren voor Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* PNG-bestanden met een IDAT-segmentgrootte groter dan 100 MB.
* PSB-bestanden.
* PSD-bestanden met een andere kleurruimte dan CMYK, RGB, Grijswaarden of Bitmap worden niet ondersteund. DuoTone-, Lab- en Geïndexeerde kleurruimten worden niet ondersteund.
* PSD-bestanden met een bitdiepte groter dan 16.
* TIFF-bestanden met zwevende-kommagegevens.
* TIFF-bestanden met LAB-kleurruimte.

### Elementen {#asset-types}

Voor optimale resultaten met het Dynamic Media Classic-platform moet u de aanbevolen bestandsindelingen en -grootten gebruiken. In deze tabel worden de elementtypen weergegeven, waarvan sommige de aanbevolen indelingen en bestandsgrootten hebben voor veelgebruikte elementen.

| Type element | Beschrijving/Recommendations |
|--- |--- |
| Audio | Invoergeluidsindelingen voor audio-elementen zijn AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. U kunt audio naar de volgende indelingen transcoderen: MP3, AAC en HE-AAC. |
| Afbeeldingen (voor Afbeeldingsgrootte, Zoomen, Afbeeldingssets, Spin-sets) | Afbeeldingen moeten ten minste 2000 pixels groot zijn; De meeste afbeeldingen hebben een grootte van 1500 tot 2500 pixels in de langste afmeting. Het wordt aanbevolen afbeeldingen zonder verlies in te stellen, zoals TIFF- en PNG-bestanden. Als u een JPEG-afbeelding gebruikt, gebruikt u de instellingen voor de hoogste kwaliteit. GIF-bestanden met animatie worden op dezelfde manier verwerkt als andere statische inhoud. |
| eCatalogs | Gebruik PDF-bestanden met hoge resolutie die zijn gemaakt in Adobe® Acrobat® of een Creative Suite-toepassing die is opgeslagen als &#39;geschikt voor drukpers&#39;. PDF&#39;s bevatten alle benodigde lettertypen, afbeeldingen, maskers en grafische elementen waarnaar wordt verwezen, zoals enkele pagina&#39;s, spreads met twee pagina&#39;s of in een indeling met meerdere pagina&#39;s. Volgorde uw pagina&#39;s door de dossiers in alfanumerieke orde te noemen. Plaats alle PDF&#39;s voor uw eCatalog in één map, zodat u ze eenvoudig kunt uploaden. U kunt opties voor uitsnijden selecteren bij het uploaden om het bijsnijdgebied van PDF&#39;s te verwijderen, zoals snijtekens, registratiedoelen of kleurenbalken. De meeste PDF-bestanden die klaar zijn voor drukken bevinden zich in de CMYK-kleurruimte. Het is daarom belangrijk dat u het CMYK ICC-kleurprofiel opgeeft dat wordt gebruikt bij uw PDF-bestanden. |
| Sjablonen | Een gelaagde afbeelding of lay-outontwerp dat tekst, afbeeldingen en lagen kan bevatten. Afbeeldingslagen, tekstreeksen en kenmerken, zoals kleur en grootte, kunnen worden geparametereerd zodat variabele gegevens kunnen worden aangepast. Afbeeldingsvereisten voor gebruik in sjablonen zijn gelijk aan die voor andere afbeeldingen. Bereid uw afbeeldingen voor in Photoshop of een ander beeldbewerkingsprogramma. Sla elke afbeelding op als een afgevlakt transparant bestand in de TIFF- of PNG-indeling. Zorg ervoor dat de afbeeldingsresolutie geschikt is voor het verwachte gebruik. Afbeeldingen die u wilt afdrukken, moeten 300 ppi zijn. |
| Video&#39;s | Dynamic Media Classic ondersteunt videobestanden die zijn opgeslagen in de OGV- en MP4-indeling. U kunt bestanden tijdens het uploaden naar MP4-indeling transcoderen.Zie [Ondersteunde bestandsindelingen voor elementen](#supported-static-file-formats). |
| Lettertypen | Geüpload TrueType, Type1 (alleen Windows), OpenType-lettertypen en PhotoFonts |
| Afbeeldingen | Afbeeldingen en gelaagde afbeeldingsbestanden. |
| Afbeeldingssets en stalensets | Een reeks verwante afbeeldingen die in een viewer kunnen worden weergegeven. |
| ICC-profielen | Een kleurprofiel dat u kunt gebruiken om een geüploade afbeelding vanuit de bronkleurruimte om te zetten in een andere kleurruimte. |
| Vignetten | Afbeeldingen die zijn gemaakt met het programma voor het schrijven van afbeeldingen en verwante bestanden. |
| Inhoudsbestanden | Adobe InDesign-, Illustrator- of Photoshop-inhoudsbestanden. |
| FXG-bestanden | Afbeeldingsindelingsbestanden met een resolutie-onafhankelijke indeling die u kunt gebruiken om aanpasbare sjablonen te maken voor uitvoer naar afdrukken, web, e-mail, bureaublad en apparaten. |
| SVG-bestanden | Schaalbare vectorafbeeldingsbestanden die servers van Image Serving kunnen renderen. |
| XML-bestanden | Bestanden die voorbewerkingsregels definiëren die worden gebruikt om het pad te wijzigen en delen van verzoeken te zoeken. |
| Cascading Style Sheet-bestanden. | CSS-skins uploaden om HTML5-viewers aan te passen. |
| JavaScript-bestanden | JavaScript-bestanden worden gebruikt voor viewerinstrumentatie voor het bevatten van accountgegevens. Adobe Security raadt dit alleen aan voor clientaccounts die een afzonderlijk domein in gebruik hebben voor levering (om cross-site scripting te voorkomen). |

>[!NOTE]
>
>Wanneer u afbeeldingsbestanden en PDF&#39;s uploadt naar Dynamic Media Classic, worden deze bronbestanden door het systeem geconverteerd naar P-TIFF (Pyramid TIFF)-bestanden. Deze P-TIFF&#39;s zijn de bestanden die later worden gepubliceerd naar Dynamic Media Image Servers. Dynamic Media Classic gebruikt de Piramid Tiff-bestandsindeling omdat deze diverse zoomverhoudingen bevat waarmee u snel kunt inzoomen bij weergave met een Dynamic Media Classic Zoom Viewer.

### Ondersteunde statische bestandsindelingen {#supported-static-file-formats}

Dynamic Media Classic ondersteunt verschillende statische bestandsindelingen. Statische inhoud is elk element dat &#39;as-is&#39; wordt gepubliceerd, zoals CSS, PDF, SVG, XML enzovoort.

De volgende bestandstypen kunnen worden gepubliceerd:

* Geanimeerde GIF
* Audiobestanden
* CSS
* JavaScript (wanneer het bedrijf met zijn eigen domein wordt gevormd)
* Master video
* PDF (als PDF specifiek is gemarkeerd voor publiceren na uploaden, om levering van alle PDF&#39;s voor bestaande eCatalog/PDF-workflow te voorkomen)
* PrX-video
* SVG
* XML
* ZIP

Dynamic Media Classic beschikt niet over de optie om een voorbeeld-URL van statische inhoud te genereren.

### Bestandsnaamvereisten {#filename-requirements}

Omdat bestandsextensies tijdens het uploaden worden verwijderd uit bestandsnamen, staat het systeem niet toe dat bestanden dezelfde hoofdnaam hebben. In het klassieke Dynamic Media-systeem wordt de bestandsnaam van het element minus de bestandsextensie de element-id voor het element. Daarom kunnen geen twee elementen dezelfde naam hebben.

Zorg ervoor dat alle gebruikers in uw bedrijf deze regels voor het benoemen van bestanden begrijpen:

* Element-id&#39;s met dezelfde exacte naam zijn niet toegestaan in het systeem.
* Namen van element-id zijn hoofdlettergevoelig.
* Als beste praktijken, zorg ervoor dat activa IDs geen lege ruimten (bijvoorbeeld, zwarte jasje.tif en blauw jpg) bevat. Dynamic Media Classic ASCII codeert lege spaties in elementnamen wanneer elementnamen worden gebruikt om URL-tekenreeksen samen te stellen. Deze ASCII-codes zijn moeilijk leesbaar, waardoor het lezen van URL&#39;s moeilijker kan worden.
* Taalspecifieke tekens zijn toegestaan in bestandsnamen. De volgende tekens zijn echter niet toegestaan in bestandsnamen:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Als een bestandsnaam een of meer van de bovenstaande tekens bevat, worden de tekens tijdens het uploaden uit de bestandsnaam verwijderd.

In de meeste gevallen kan de bestandsnaam van een element hetzelfde zijn als het itemnummer, de SKU-code van het product of een andere naam als in het volgende voorbeeld:

| Item | Bestandsnaam | Element-id |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Maporganisatie en -structuur {#folder-organization-and-structure}

Organiseer en structureer mappen en submappen voor uw inhoud in Dynamic Media Classic voordat u uw inhoud uploadt naar het systeem. Het plannen op deze manier heeft twee belangrijke voordelen:

* Wanneer u de inhoud via FTP uploadt naar Dynamic Media Classic, kunt u het systeem de mapstructuur laten repliceren tijdens het uploaden. Op deze manier wordt uw inhoud in dezelfde mappen en submappen in Dynamic Media Classic geordend als op uw computer of netwerk. (Als u de mapstructuur in Dynamic Media Classic wilt repliceren, selecteert u de optie Submappen opnemen wanneer u elementen uploadt via FTP.)
* Het is veel moeilijker om mappen in het systeem opnieuw te ordenen nadat bestanden zijn geüpload dan met een zorgvuldig overwogen mapstructuur te beginnen.

De benadering en structuur van mapnamen die u kiest voor het opslaan van uw inhoud op de Dynamic Media Classic, zijn afhankelijk van de behoeften van uw organisatie. Hier volgen enkele voorbeelden van mapstructuren:

**SKU-** basedFolders worden genoemd volgens SKUs of puntaantallen. Er worden bijvoorbeeld aparte mappen gemaakt voor alle reeksen 0, 20 en 30 cijfers.

**Merk-** basedVoor fabrikanten met meerdere merklijnen en detailhandelaren die andere merken van andere bedrijven op de markt brengen, scheidt dossiers in productomslagen die voor verschillende merken worden genoemd.

**Project-** basedFolders worden georganiseerd volgens rollout/drop datum of projectnaam. Klanten die vooral eCatalogi produceren, zijn voor deze aanpak.

**Spiegelen van** maphiërarchie van websitesDeze mapstructuur weerspiegelt de mapstructuur van de website, met de mappen die bijvoorbeeld voor productcategorieën zijn genoemd.

## Bestanden {#uploading-your-files} uploaden

U kunt afzonderlijke bestanden uploaden vanaf het bureaublad of mappen uploaden via FTP. Als u meer dan 100 MB dossiers wilt uploaden of volledige omslagen en subfolders uploaden, selecteer **VIA FTP** tabel.

Dynamic Media Classic stuurt u een e-mailbericht om te bevestigen wanneer uw uploadtaak begint en eindigt en om u op de hoogte te stellen van eventuele problemen.

Tijdens (of direct na) een grote uploadtaak kunnen sommige nieuwe items het bericht &quot;Afbeelding nog niet geoptimaliseerd&quot; weergeven. Dit bericht wordt weergegeven omdat de bestanden nog niet volledig zijn verwerkt en aan Dynamic Media Classic zijn toegevoegd. U kunt deze bestanden later optimaliseren. (Zie [Bestanden optimaliseren](application-setup.md#optimize_files).)

### Bestanden uploaden via het tabblad FROM DESKTOP {#upload-files-using-sps-desktop-application}

Met de Dynamic Media Classic Desktop-toepassing kunt u bestanden en mappen uploaden door te slepen.

1. Klik in de Dynamic Media Classic Desktop-toepassing op de algemene navigatiebalk op **Uploaden**.
1. Voor de Upload pagina, klik **VAN BUREAUBLAD** tabel.
1. Klik links op de pagina Uploaden in het gebied **Bestanden selecteren voor uploaden** op **Bladeren** om de bestanden of mappen te selecteren die u wilt uploaden en klik vervolgens op **Openen**.
1. Navigeer rechts van de pagina Uploaden in het gebied **Kies Mapdoel** naar een doelmap waar u de geüploade bestanden of mappen wilt toevoegen.
1. (Optioneel) Geef onder aan de uploadpagina in het veld **Taaknaam** de nieuwe naam van de uploadtaak op. U kunt ook gewoon de door het systeem gegenereerde standaardnaam gebruiken die Dynamic Media Classic biedt. De baan en andere upload en het publiceren banen worden geregistreerd op de pagina van Banen, waar u de status van banen kunt controleren.
Zie [Taakbestanden controleren](checking-job-files.md#checking_job_files).
1. (Optioneel) Selecteer **Publiceren na uploaden** onder aan de pagina Uploaden als u de elementen die u uploadt automatisch wilt publiceren.
Wanneer u bestanden publiceert, worden deze naar live servers verzonden. URL&#39;s voor deze bestanden kunnen vervolgens worden gebruikt op externe websites en toepassingen. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
1. (Optioneel) Selecteer onder aan de uploadpagina **Overschrijven in een map, dezelfde naam voor basiselementen ongeacht de extensie** als u wilt dat de bestanden die u uploadt, bestaande bestanden vervangen door dezelfde naam. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
De naam van deze optie kan verschillen, afhankelijk van de instellingen in **Toepassingsinstellingen > Algemene instellingen > Uploaden naar toepassing > Afbeeldingen overschrijven**.
1. Klik in de rechterbenedenhoek van de uploadpagina op **Taakopties** en geef vervolgens de gewenste opties op.

   Zie [Opties voor uploaden](uploading-files.md#upload_options).

1. Klik in het dialoogvenster Taakopties uploaden op **Opslaan**.
1. Klik in de rechterbenedenhoek van de uploadpagina op **Uploaden verzenden**.
Als u de voortgang van het uploaden wilt zien, klikt u op **Jobs** op de algemene navigatiebalk. U kunt blijven werken in Dynamic Media Classic en op elk gewenst moment terugkeren naar de pagina Taken om een actieve taak te controleren. Als u een uploadtaak die wordt uitgevoerd wilt annuleren, selecteert u **Annuleren** naast de duur van de upload.

### Bestanden uploaden via het tabblad VIA FTP {#upload-files-using-via-ftp}

1. Meld u aan bij de Klassieke FTP-site van Dynamic Media die specifiek is voor uw specifieke regio. Gebruik de FTP-gebruikersnaam en het wachtwoord die u van de beheerder hebt ontvangen.
1. Klik in Dynamic Media Classic op de algemene navigatiebalk op **Uploaden**.
1. Klik op het tabblad **VIA FTP** op de pagina Uploaden.
1. Kies links op de pagina Uploaden in het gebied **FTP-map kiezen voor uploaden** een FTP-map waaruit u bestanden wilt uploaden.
1. Kies rechts van de uploadpagina in het gebied **Kies Adobe Dynamic Media-mapbestemming** een doelmap in Dynamic Media Classic.
1. (Optioneel) Geef onder aan de uploadpagina in het veld **Taaknaam** de nieuwe naam van de uploadtaak op. U kunt ook gewoon de door het systeem gegenereerde standaardnaam gebruiken die Dynamic Media Classic biedt. De baan en andere upload en het publiceren banen worden geregistreerd op de pagina van Banen, waar u de status van banen kunt controleren.
Zie [Taakbestanden controleren](checking-job-files.md#checking_job_files).
1. (Optioneel) Selecteer **Publiceren na uploaden** onder aan de pagina Uploaden als u de elementen die u uploadt automatisch wilt publiceren.
Wanneer u bestanden publiceert, worden deze naar live servers verzonden. URL&#39;s voor deze bestanden kunnen vervolgens worden gebruikt op externe websites en toepassingen. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
1. (Optioneel) Selecteer onder aan de uploadpagina **Overschrijven in een map, dezelfde naam voor basiselementen ongeacht de extensie** als u wilt dat de bestanden die u uploadt, bestaande bestanden vervangen door dezelfde naam. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
De naam van deze optie kan verschillen, afhankelijk van de instellingen in **Toepassingsinstellingen > Algemene instellingen > Uploaden naar toepassing > Afbeeldingen overschrijven**.
1. (facultatief; Deze optie is alleen beschikbaar als u onder aan de uploadpagina op de tab **VIA FTP** hebt geklikt. Selecteer **ZIP- of Tar-bestanden bij uploaden decomprimeren** als u alle bestanden automatisch wilt extraheren uit uw geüploade ZIP- of TAR-bestand. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.
1. Klik in de rechterbenedenhoek van de uploadpagina op **Taakopties** en geef vervolgens de gewenste opties op.

   Zie [Opties voor uploaden](uploading-files.md#upload_options).

1. Klik in het dialoogvenster Taakopties uploaden op **Opslaan**.
1. Klik in de rechterbenedenhoek van de uploadpagina op **Uploaden verzenden**.

   Klik op **Jobs** om de voortgang van het uploaden te zien. De pagina van Banen toont u de vooruitgang van het uploaden. U kunt blijven werken in Dynamic Media Classic en op elk gewenst moment terugkeren naar de pagina Taken om een actieve taak te controleren.

Als u een actieve uploadtaak wilt annuleren, klikt u op **Annuleren** naast de duur van de upload.

## Dialoogvenster Taakopties uploaden {#upload-options}

Bij het uploaden van bestanden kunt u uit de volgende opties kiezen in het dialoogvenster Opties voor uploaden:

* **JOB**  - Klik  **** JOB om opties te kiezen die de volledige uploadtaak beïnvloeden.

   U kunt ook *standaardopties* voor het uploaden van taken kiezen met het dialoogvenster **Standaardopties voor uploaden** in Algemene instellingen. Klik **Setup > Toepassingsinstellingen > Algemene instellingen > Standaardopties voor uploaden** en stel de gewenste standaardopties in.

   * **Wanneer** — De optie  **** Wanneer is alleen beschikbaar als u het  **VIA** FTP-tabblad hebt geselecteerd.
      * **Eenmalig**  — Geef een uploadtaak op die één keer wordt uitgevoerd. U kunt onder andere de volgende opties kiezen:
         * **Nu**  - Hiermee wordt de uploadtaak direct uitgevoerd nadat u op  **** Opslaan in het dialoogvenster Opties voor uploaden hebt geklikt en vervolgens op  **Uploaden** verzenden op de pagina Uploaden klikt.
         * **Plan voor Later** : selecteer het jaar, de maand, de dag, en de tijd (in stappen van 15 minuten) dat u de uploadtaak wilt uitvoeren.
      * **Herhalend**  - specificeer een uploadbaan die dagelijks, wekelijks, of maandelijks loopt. Of pas de uploadtaak aan uw eigen specificaties aan.
         * **Dagelijks** : stel de tijd in waarop de taak elke dag moet worden uitgevoerd. Als u wilt dat de taak slechts van maandag tot en met vrijdag wordt uitgevoerd, selecteert u **Alleen weekdagen**.
         * **Wekelijks** : kies een specifieke dag van de week en tijd die u de baan wilt lopen.
         * **Maandelijks** — Kies een specifieke dag van de maand of dag van de week, inclusief de begintijd, waarop u de taak wilt uitvoeren.
         * **Aangepast**  - Pas een upload- of publicatietaakinterval aan uw eigen specificaties aan. Zie [Een aangepaste upload- of publiceertaaktijdinterval maken](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Publiceren na uploaden** — Beschikbaar als u het  **tabblad FROM** DESKTOP of  **VIA** FTPtab hebt geselecteerd. Selecteer deze optie als u de elementen die u uploadt automatisch wilt publiceren. Wanneer u bestanden publiceert, worden deze naar live servers verzonden. URL&#39;s voor deze bestanden kunnen vervolgens worden gebruikt op externe websites en toepassingen. Deze optie is ook beschikbaar op de Upload pagina.

   * **Overschrijf in een willekeurige map dezelfde naam voor basiselementen, ongeacht de extensie** . Beschikbaar als u  **FROM** DESKTOPtab of  **VIA** FTPtab hebt geselecteerd. Selecteer deze optie als u wilt dat de bestanden die u uploadt, bestaande bestanden met dezelfde naam vervangen. Deze optie is ook beschikbaar op de Upload pagina. De naam van deze optie kan verschillen, afhankelijk van de instellingen in **Toepassingsinstellingen > Algemene instellingen > Uploaden naar toepassing > Afbeeldingen overschrijven**.

   * **ZIP- of Tar-bestanden bij uploaden**  decomprimeren - Beschikbaar als u  **FROM** DESKTOPtab of  **VIA** FTPtab hebt geselecteerd.
Selecteer deze optie als u automatisch alle bestanden uit het geüploade ZIP- of TAR-bestand wilt extraheren. Deze optie is ook beschikbaar in het dialoogvenster Taakopties.

   * **Inclusief submappen**  - alleen beschikbaar als u het  **VIA** FTPtab hebt geselecteerd.
Selecteer deze optie als u submappen wilt uploaden van de map die u wilt uploaden. De namen van de map en de submappen die u uploadt, worden automatisch ingevoerd in Dynamic Media Classic.

   * **Metagegevensbestanden**  verwerken - Alleen beschikbaar als u  **VIA** FTPtab hebt geselecteerd. Selecteer deze optie als u een door tabs gescheiden of XML-bestand wilt uploaden om metagegevens aan meerdere elementen toe te voegen.
Zie [Metagegevens importeren (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPTIONS**  UITSNIJDEN - Als u pixels in witruimte automatisch wilt uitsnijden in een afbeelding, opent u het menu Uitsnijden, kiest u Handmatig en voert u pixelmetingen in in de velden Boven, Rechts, Onder en Links om van de zijkanten uit te snijden. U kunt ook Bijsnijden kiezen in het menu Uitsnijden en de volgende opties kiezen:

   * **Wegsnijden op basis van**  - Bepaal of u wilt uitsnijden op basis van kleur of transparantie:

      * **Kleur** : kies de optie Kleur. Selecteer vervolgens het menu Hoek en kies de hoek van de afbeelding met de kleur die het beste overeenkomt met de kleur voor de witruimte die u wilt uitsnijden.

         Bijsnijden op basis van kleur: Geef 0 op om alleen pixels uit te snijden als deze exact overeenkomen met de kleur die u in de hoek van de afbeelding hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

      * **Transparantie**  - Kies de optie Transparantie.

         Bijsnijden op basis van transparantie: Geef 0 op om alleen pixels uit te snijden als deze volledig transparant zijn; De cijfers dichter aan 1 staan voor meer transparantie.

      * **Tolerantie**  - Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven.

* **OPTIONS**  VAN KLEURPROFIEL: kies een kleurconversie wanneer u geoptimaliseerde bestanden maakt die worden gebruikt voor Klassieke, dynamische Dynamic Media-levering:

   * **Standaardkleurbehoud** : behoudt de kleuren van de bronafbeelding wanneer de afbeeldingen kleurruimtegegevens bevatten; er is geen kleurconversie. In bijna alle afbeeldingen van vandaag is het juiste kleurprofiel al ingesloten. Als een CMYK-bronafbeelding echter geen ingesloten kleurprofiel bevat, worden de kleuren omgezet in de kleurruimte sRGB (standaard rood-groen-blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

   * **Oorspronkelijke kleurruimte**  behouden - Behoudt de oorspronkelijke kleuren zonder kleurconversie op het punt van inname in Dynamic Media Classic. Voor afbeeldingen zonder een ingesloten kleurprofiel wordt de vereiste kleurconversie voor het verwerken van aanvragen voor de afbeelding uitgevoerd met de standaardkleurprofielen die zijn geconfigureerd in de Publicatie-instellingen. Deze kleurprofielen worden mogelijk niet uitgelijnd met de kleur in de bestanden die met deze optie zijn gemaakt. Daarom wordt u aangeraden de optie Standaardkleurbehoud te gebruiken.

   * **Aangepast van > naar**  - opent menu&#39;s zodat u een optie kunt kiezen voor Omzetten van en Omzetten in kleurruimte. Deze geavanceerde optie negeert alle kleurinformatie die in het bronbestand is ingesloten. Selecteer deze optie alleen als alle afbeeldingen die u verzendt onjuiste of ontbrekende kleurprofielgegevens bevatten.

* **OPTIONS**  VOOR AFBEELDINGSBEWERKING: u kunt de  &lt;> knipmaskers in afbeeldingen behouden en een kleurprofiel kiezen.
Zie [Opties voor het bewerken van afbeeldingen tijdens het uploaden](image-editing-options-upload.md#image-editing-options-at-upload).

* **POSTSCRIPT-OPTIONS** : u kunt PostScript® rasteren, bestanden uitsnijden, transparante achtergronden behouden, een resolutie kiezen en een kleurruimte kiezen.
Zie [Werken met PostScript- en Illustrator-bestanden](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **PHOTOSHOP OPTIONS** : u kunt sjablonen maken van Adobe® Photoshop®-bestanden, lagen behouden, opgeven hoe lagen worden benoemd, tekst uitnemen en opgeven hoe afbeeldingen in sjablonen worden verankerd.
Zie [Uploadopties voor PSD](psd-files.md#psd_upload_options).

* **PDF-OPTIONS** : u kunt de bestanden rasteren, zoekwoorden en koppelingen extraheren, automatisch een eCatalog genereren, de resolutie instellen en een kleurruimte kiezen.
Zie [Opties voor PDF-upload](pdfs.md#pdf_upload_options).

* **ILLUSTRATOR-OPTIONS** : u kunt Adobe Illustrator®-bestanden rasteren, transparante achtergronden behouden, een resolutie kiezen en een kleurruimte kiezen.
Zie [Werken met PostScript- en Illustrator-bestanden](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO-OPTIONS** : u kunt een videobestand transcoderen door een videovoorinstelling te kiezen.
Zie [Werken met voorinstellingen voor videocodering](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **AANVULLENDE METAGEGEVENS** : voer trefwoorden in die de bestanden beschrijven die u wilt uploaden. Trefwoorden scheiden door komma&#39;s. Met trefwoorden kunt u gemakkelijker naar elementen zoeken.
Zie [Een geavanceerde zoekopdracht uitvoeren](searching-assets.md#conducting_an_advanced_search).

* **VOORINSTELLINGEN**  VOOR BATCH-SET: als u een Afbeeldingsset, Centrifugeerset met meerdere assen of Staalset wilt maken van de geüploade bestanden, klikt u op de kolom Actief voor de voorinstelling die u wilt gebruiken. U kunt meerdere voorinstellingen selecteren. U maakt de voorinstellingen op de pagina Voorinstellingen voor toepassingsinstellingen/batchsets.
Zie [Voorinstellingen batchset](application-setup.md#batch_set_presets).

* **GEAVANCEERD**  - Zie Uploaden  [volgen met een andere taak](uploading-files.md#follow-an-upload-with-another-job).

## Uploaden met een andere taak volgen {#follow-an-upload-with-another-job}

Wanneer u items uploadt via FTP, kunt u een volgende taak plannen die moet beginnen zodra het uploaden is voltooid. (Als andere taken op dat moment moeten beginnen, wordt de taak die u hier instelt, na deze taken in de wachtrij geplaatst.)

De nieuwe baan verzendt een bericht naar het adres u specificeert zodat de code bij die plaats kan worden teweeggebracht. Deze vervolgpublicatietaak gebruikt dezelfde naam als de uploadtaak, maar met de tekst *Pub_* toegevoegd aan het begin.

**Een upload volgen met een andere taak**

1. Klik **Upload**, dan klik **VIA FTP** tabel.
1. Klik in de rechterbenedenhoek van de uploadpagina op **Taakopties**.
1. Vouw in het dialoogvenster Taakopties uploaden de sectie **ADVANCED** uit.
1. Kies een van de volgende opties in de vervolgkeuzelijst **Uploaden volgen met een andere taak**:

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
   >Regelmatig geplande taken kunnen er niet toe leiden dat bestanden worden gepubliceerd.

>[!MORELIKETHIS]
>
>* [Werken met middelenmappen](asset-folders.md#working_with_asset_folders)
>* [Herhalende upload- en publicatietaken afhandelen](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Een upload- of publicatietaak gebruiken als trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

