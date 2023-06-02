---
title: Video's uploaden en coderen
description: Leer video's uploaden en coderen in Adobe Dynamic Media Classic.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '3862'
ht-degree: 1%

---

# Video&#39;s uploaden en coderen{#uploading-and-encoding-videos}

Als u één video of adaptieve videosets wilt maken voor levering op het web of op mobiele apparaten, uploadt u eerst uw primaire videobestanden naar Adobe Dynamic Media Classic. Adobe Dynamic Media Classic codeert video&#39;s naar MP4 en publiceert video in de volgende bestandsindelingen:

* **MP4** - Adobe Dynamic Media Classic raadt MP4 aan als de voorkeursindeling voor videobestanden. Gebruik MP4-bestanden voor het volgende:

   * HTTP Dynamic Streaming op desktops.
   * Live HTTP-streaming (streamingprotocol van Apple).
   * Progressieve video-levering aan mobiele Android™-, BlackBerry®- en Windows®-apparaten

   Adobe Dynamic Media Classic biedt twee workflows voor het uploaden van videobestanden:

* **Vooraf gecodeerde video&#39;s** - U uploadt MP4-bestanden rechtstreeks naar Adobe Dynamic Media Classic. Met deze workflow worden bestanden niet gecodeerd op het moment dat u ze uploadt. De bestanden worden vooraf gecodeerd ter voorbereiding op levering op het bureaublad en op mobiele apparaten.

* **Primaire bronvideo&#39;s** - Upload primaire bronvideobestanden en codeer deze bestanden tijdens het uploaden naar MP4-bestanden. Gecodeerde video&#39;s krijgen het label &quot;Video&quot; in het deelvenster Bladeren. Adobe Dynamic Media Classic ondersteunt de codering van videobestanden in een groot aantal indelingen.

   * Zorg ervoor dat de primaire bronvideobestanden die u wilt coderen, worden ondersteund.

      Zie [Ondersteunde videobestandstypen voor codering](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Kies een voorinstelling voor videocodering.

      Zie [Videovoorinstellingen voor het coderen van videobestanden](application-setup.md#video-presets-for-encoding-video-files).

      Zie [Aanbevolen procedures voor videocodering](uploading-encoding-videos.md#best-practices-for-video-encoding).

Adobe Dynamic Media Classic genereert ook videominiaturen. Meer informatie over videominiaturen, hoe u de URL&#39;s opgeeft en posterframes wijzigt.

Zie [Werken met videominiaturen](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**U kunt als volgt video&#39;s uploaden en coderen:**

Voer een van de volgende handelingen uit.

*Als uw video&#39;s al zijn gecodeerd*

1. Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Upload]**.
1. Selecteer op de pagina Uploaden de optie **[!UICONTROL From Desktop]** tab.
1. Op de Upload pagina, in **[!UICONTROL Select Files for Upload]** deelvenster, selecteert u **[!UICONTROL Browse]**, navigeert u naar een MP4-videobestand en selecteert u **[!UICONTROL Open]**.
1. In de **[!UICONTROL Choose Folder Destination]** selecteert u een map voor het geüploade bestand.
1. Controleer op de pagina Uploaden of **[!UICONTROL Publish After Uploading]** is ingeschakeld.
1. Selecteren **[!UICONTROL Submit Upload]**.

*Als u uw video&#39;s wilt coderen met Adobe Dynamic Media Classic*

1. Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Upload]**.
1. Selecteer op de pagina Uploaden de optie **[!UICONTROL From Desktop]** tab.
1. In de **[!UICONTROL Select Files to Upload]** deelvenster, selecteert u **[!UICONTROL Browse]**, navigeert u naar een primair bronvideobestand en selecteert u **[!UICONTROL Open]**.
1. In de **[!UICONTROL Choose Folder Destination]** selecteert u een map voor het geüploade bestand.
1. Selecteer in de rechterbenedenhoek van de pagina de optie **[!UICONTROL Job Options]**,
1. Vouw in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL EVideo Options]** Voer vervolgens een van de volgende handelingen uit:

   * U kunt het beste **[!UICONTROL Adaptive Video Encoding]**. Zie [Adaptieve video (standaard)](application-setup.md#adaptive-video-default).
   * Optioneel. Als u afzonderlijke coderingsinstellingen wilt gebruiken, vouwt u **[!UICONTROL Single Encoding Presets]**en selecteert u vervolgens de gewenste coderingsopties voor Desktop, Mobile en Tablet.
Zie [Voorinstellingen voor videocodering op bureaublad](application-setup.md#desktop-video-encoding-presets), [Voorinstellingen voor mobiele videocodering](application-setup.md#mobile-video-encoding-presets), [Voorinstellingen voor videocodering van tablet](application-setup.md#tablet-video-encoding-presets).
1. Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL Save]**.
1. Controleer op de pagina Uploaden of **[!UICONTROL Publish After Uploading]** is ingeschakeld.
1. Selecteer in de rechterbenedenhoek van de pagina Uploaden de optie **[!UICONTROL Submit Upload]**.

*Als u een eerder geüpload videobestand opnieuw wilt coderen*

1. Navigeer in Adobe Dynamic Media Classic in het deelvenster Bladeren naar de video en selecteer deze.
1. Ga naar **[!UICONTROL File]** > **[!UICONTROL Reprocess]**.
1. Vouw in het dialoogvenster Elementen opnieuw verwerken het item uit **[!UICONTROL EVideo Options]** Voer vervolgens een van de volgende handelingen uit:
   * U kunt het beste de volgende methode gebruiken. Selecteren **Adaptieve video**.
Zie [Adaptieve video (standaard)](application-setup.md#adaptive-video-default).
   * Optioneel. Als u afzonderlijke coderingsinstellingen wilt gebruiken, vouwt u **[!UICONTROL Single Encoding Presets]**en selecteert u vervolgens de gewenste coderingsopties voor Desktop, Mobile en Tablet.
Zie [Voorinstellingen voor videocodering op bureaublad](application-setup.md#desktop-video-encoding-presets), [Voorinstellingen voor mobiele videocodering](application-setup.md#mobile-video-encoding-presets), [Voorinstellingen voor videocodering van tablet](application-setup.md#tablet-video-encoding-presets).
1. Selecteer in het dialoogvenster Elementen opnieuw verwerken de optie **[!UICONTROL Submit]**.

Wanneer u een voorinstelling voor adaptieve videocodering gebruikt of meerdere voorinstellingen voor enkele codering gebruikt, is het resultaat een adaptieve videoset die automatisch met meerdere videocoderingen wordt gemaakt. U kunt ook handmatig een adaptieve videoset maken door afzonderlijke video&#39;s te selecteren.

Alleen MP4- en M4V-bestandstypen worden gemaakt wanneer u automatisch of handmatig een adaptieve videoset genereert.

## Ondersteunde videobestandstypen voor codering {#supported-video-file-types-for-encoding}

De volgende tabel bevat een lijst met videobestandstypen (met toegestane videocodecs) die u naar de MP4- of OGV-indeling kunt coderen wanneer u bestanden uploadt. De tabel bevat bestandsindelingen en codecs:

* **Videobestandsindelingen** - Net als bij een ZIP-bestand bepaalt de indeling van videobestanden hoe de bestanden in het videobestand worden opgenomen. Een videobestand bevat meestal meerdere tracks (een videotrack (zonder audio) en een of meer audiotracks (zonder video) die met elkaar verweven en gesynchroniseerd zijn. De videobestandsindeling bepaalt hoe deze verschillende gegevenstracks en metagegevens worden ingedeeld.

* **Videocodecs** - Een videocodec beschrijft het algoritme waarmee een video wordt gecodeerd. Een videospeler decodeert de video volgens zijn codec en geeft vervolgens een reeks beelden, of kaders, op het scherm weer. Met codecs minimaliseert u de hoeveelheid informatie die videobestanden nodig hebben om video af te spelen. In plaats van informatie over elk afzonderlijk frame wordt alleen informatie over de verschillen tussen het ene frame en het volgende opgeslagen. Omdat de meeste video&#39;s weinig van het ene frame naar het andere veranderen, maken codecs hoge compressiesnelheden mogelijk, waardoor de bestanden kleiner worden.

   | Videobestandsindeling | Videocodecs |
   | --- | --- |
   | 3GP | H.263, H.264 |
   | AVI | DivX, DV |
   | M2P | MPEG-2 PS |
   | M2T | MPEG-2 TS |
   | M2TS | MPEG-2 TS |
   | M2V | MPEG-2 ES |
   | M4V | H.264 |
   | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
   | MP4 | H.264/MPEG-4 AVC |
   | MPEG | MPEG-2 SS |
   | MPG | MPEG-2 SS |
   | MTS | MPEG-2 |
   | ProRes | APCN, APCS, APCO, APCH, AP4H |
   | TS | DVCPro 50 |
   | VOB | MPEG-2 |
   | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

   >[!NOTE]
   >
   >Het scherm van Banen alarmeert u als u uploadt en probeert om een videodossier te coderen maar het dossier wordt verworpen omdat het een incompatibele codec of dossiercontainer bevat. Zie voor meer informatie [Taakbestanden controleren](checking-job-files.md).

## Aanbevolen procedures voor videocodering {#best-practices-for-video-encoding}

Hieronder vindt u tips voor het aanbevolen gebruik voor het coderen van bronvideobestanden in Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Bronvideobestanden {#source-video-files}

Wanneer u een videobestand codeert, gebruikt u een videobronbestand van de hoogst mogelijke kwaliteit. Gebruik geen eerder gecodeerde videobestanden omdat deze bestanden al zijn gecomprimeerd en als u verder codeert, wordt een video van subparkwaliteit gemaakt.

In de volgende tabel worden de aanbevolen grootte, hoogte-breedteverhouding en minimale bitsnelheid beschreven die uw bronvideobestanden moeten hebben wanneer u ze codeert:

| Grootte | Hoogte-breedteverhouding | Minimale bitsnelheid |
| --- | --- | --- |
| 1024 x 768 | 4:3 | 4500 kbps voor de meeste video&#39;s. |
| 1280 x 720 | 16:9 | 3000 - 6000 kbps, afhankelijk van de hoeveelheid beweging in de video. |
| 1920 x 1080 | 16:9 | 6000 - 8000 kbps, afhankelijk van de mate van beweging in de video. |

### De metagegevens van een bestand verkrijgen {#obtaining-a-file-s-metadata}

U kunt de metagegevens van een bestand verkrijgen door de metagegevens van het bestand te bekijken in Adobe Dynamic Media Classic, met een programma voor videobewerking of met een toepassing die is ontworpen voor het verkrijgen van metagegevens. Hieronder vindt u instructies voor het gebruik van MediaInfo, een toepassing van derden, voor het verkrijgen van de metagegevens van een videobestand:

1. Ga naar deze webpagina: [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. Selecteer en download het installatieprogramma voor de GUI-versie en volg de installatie-instructies.
1. Klik na de installatie met de rechtermuisknop op het videobestand (alleen Windows®) en selecteer MediaInfo, of open MediaInfo en sleep het videobestand naar de toepassing. U ziet alle metagegevens die aan het videobestand zijn gekoppeld, inclusief de breedte, hoogte en fps.

### Hoogte-breedteverhouding {#aspect-ratio}

Wanneer u een voorinstelling voor videocodering kiest of maakt voor uw primaire videobestand, moet u ervoor zorgen dat de voorinstelling dezelfde hoogte-breedteverhouding heeft als het primaire videobestand. De *hoogte-breedteverhouding* is de verhouding tussen de breedte en de hoogte van de video.

Als u de hoogte-breedteverhouding van een videobestand wilt bepalen, vraagt u de metagegevens van het bestand op en noteert u de breedte en hoogte van het bestand (zie [De metagegevens van een bestand verkrijgen](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Gebruik vervolgens deze formule om de hoogte-breedteverhouding te bepalen:

width/height = hoogte-breedteverhouding

In de volgende tabel wordt beschreven hoe de resultaten van de formule worden omgezet in algemene opties voor de hoogte-breedteverhouding:

| Resultaat van formule | Hoogte-breedteverhouding |
| --- | --- |
| 1.33 | 4:3 |
| 0.75 | 3:4 |
| 1.78 | 16:9 |
| 0.56 | 9:16 |

Een video van 1440 x 1080 hoogte heeft bijvoorbeeld een hoogte-breedteverhouding van 1440/1080 of 1,33. In dit geval kiest u een voorinstelling voor videocodering met een hoogte-breedteverhouding van 4:3 om het videobestand te coderen.

### Gegevenssnelheid {#data-rate}

De *gegevenssnelheid* (ook wel *bitsnelheid*) is de hoeveelheid gegevens die is gecodeerd om één seconde video af te spelen. De gegevenssnelheid wordt gemeten in kilobits per seconde (Kbps).

>[!NOTE]
>
>Omdat in alle codecs compressie met verlies wordt gebruikt, is de gegevenssnelheid de belangrijkste factor voor de videokwaliteit. Bij compressie met verlies neemt de kwaliteit af naarmate u een videobestand comprimeert. Daarom zijn alle andere eigenschappen gelijk (de resolutie, framesnelheid en codec), hoe lager de gegevenssnelheid, hoe lager de kwaliteit van het gecomprimeerde bestand.

Wanneer u een voorinstelling voor videocodering kiest, moet u rekening houden met de verbindingssnelheid van de eindgebruiker van het doel. Kies een voorinstelling met een gegevenssnelheid van 80 procent van die snelheid. Als de verbindingssnelheid van de eindgebruiker van het doel bijvoorbeeld 1000 Kbps is, is de beste voorinstelling een snelheid met een videogegevenssnelheid van 800 Kbps.

In deze tabel wordt de gegevenssnelheid beschreven van standaardverbindingssnelheden.

| Snelheid (Kbps) | Verbindingstype |
| --- | --- |
| 256 | Inbelverbinding. |
| 800 | Normale mobiele verbinding. Kies hiervoor een gegevenssnelheid tussen 400 en maximaal 800 voor 3G-ervaringen. |
| 2000 | Standaardbreedbandverbinding voor desktops. Voor deze verbinding, richt een gegevenstarief in de waaier 800-2000 Kbps, met de meeste doelstellingen gemiddeld 1200-1500 Kbps. |
| 5000 | Typische breedbandverbinding. Codering in dit bovenste bereik wordt niet aanbevolen, omdat de video bij deze snelheid niet beschikbaar is voor de meeste consumenten. |

### Resolutie {#resolution}

*Resolutie* Hiermee worden de hoogte en breedte van een videobestand in pixels beschreven. De meeste bronvideo wordt opgeslagen met een hoge resolutie (bijvoorbeeld 1920 x 1080). Voor streamingdoeleinden wordt bronvideo gecomprimeerd tot een lagere resolutie (640 x 480 of lager).

Resolutie en gegevenssnelheid zijn twee geïntegreerde gekoppelde factoren die de videokwaliteit bepalen. Als u dezelfde videokwaliteit wilt behouden, geldt dat hoe hoger het aantal pixels in een videobestand (hoe hoger de resolutie), hoe hoger de gegevenssnelheid. Neem bijvoorbeeld het aantal pixels per frame in een videobestand met een resolutie van 320 x 240 en een resolutie van 640 x 480:

| Resolutie | Pixels per frame |
| --- | --- |
| 320 x 240 | 76,800 |
| 640 x 480 | 307,200 |

Het bestand van 640 x 480 heeft vier keer zoveel pixels per frame. Als u voor deze twee voorbeeldresoluties dezelfde gegevenssnelheid wilt bereiken, past u viermaal de compressie toe op het bestand van 640 x 480, waardoor de kwaliteit van de video kan afnemen. Daarom levert een videogegevenssnelheid van 250 Kbps beelden van hoge kwaliteit bij een resolutie van 320 x 240, maar niet bij een resolutie van 640 x 480.

>[!NOTE]
>
>Over het algemeen geldt dat hoe hoger de gegevenssnelheid, hoe beter de video wordt weergegeven en hoe hoger de resolutie die u gebruikt, hoe hoger de gegevenssnelheid waarmee u de weergavekwaliteit wilt behouden (in vergelijking met lagere resoluties).

Omdat de resolutie en de gegevenssnelheid zijn gekoppeld, hebt u twee opties bij het coderen van video:

* Kies een gegevenssnelheid en codeer vervolgens met de hoogste resolutie die het beste lijkt bij de gekozen gegevenssnelheid.
* Kies een resolutie en codeer met de gegevenssnelheid die nodig is voor video van hoge kwaliteit met de gekozen resolutie.

Wanneer u een voorinstelling voor videocodering kiest (of maakt) voor uw primaire videobestand, gebruikt u deze tabel om de juiste resolutie in te stellen:

| Resolutie | Hoogte (pixels) | Schermgrootte |
| --- | --- | --- |
| 240p | 240 | Glanzend scherm |
| 300p | 300 | Klein scherm, meestal voor mobiele apparaten |
| 360p | 360 | Klein scherm |
| 480p | 480 | Standaardscherm |
| 720p | 720 | Groot scherm |
| 1080p | 1080 | High-definition groot scherm |

### Fps (frames per seconde) {#fps-frames-per-second}

In de Verenigde Staten en Japan wordt de meeste video opgenomen met een snelheid van 29,97 frames per seconde (fps); in Europa wordt de meeste video opgenomen met 25 fps. Film wordt opgenomen bij 24 fps.

Kies een voorinstelling voor videocodering die overeenkomt met de fps-snelheid van het primaire videobestand. Als uw primaire video bijvoorbeeld 25 fps is, kiest u een coderingsvoorinstelling met 25 fps. Standaard wordt voor alle aangepaste codering de fps van het primaire videobestand gebruikt. Daarom hoeft u de fps-instelling niet expliciet op te geven wanneer u een voorinstelling voor videocodering maakt.

### Afmetingen videocodering {#video-encoding-dimensions}

Voor optimale resultaten selecteert u de coderingsafmetingen, zodat de bronvideo een volledig veelvoud van alle gecodeerde video&#39;s is.

Als u deze verhouding wilt berekenen, deelt u de bronbreedte door de gecodeerde breedte om de breedteverhouding op te halen. Vervolgens deelt u de bronhoogte door de gecodeerde hoogte om de hoogte-breedteverhouding te bepalen.

Als de resulterende verhouding een geheel geheel getal is, betekent dit dat de video optimaal wordt geschaald. Als de resulterende verhouding geen geheel geheel getal is, is dit van invloed op de videokwaliteit doordat pixelartefacten overblijven op het scherm. Dit effect is vooral opvallend wanneer de video tekst heeft.

Stel dat uw bronvideo bijvoorbeeld 1920 x 1080 is. In de volgende tabel bieden de drie gecodeerde video&#39;s de optimale coderingsinstellingen.

| Videotype | Breedte x hoogte | Breedteverhouding | Hoogteverhouding |
| --- | --- | --- | --- |
| Bron | 1920 x 1080 | 1 | 1 |
| Gecodeerd | 960 x 540 | 2 | 2 |
| Gecodeerd | 640 x 360 | 3 | 3 |
| Gecodeerd | 480 x 270 | 4 | 4 |

### Gecodeerde videobestandsindeling {#encoded-video-file-format}

Adobe Dynamic Media Classic raadt u aan voorinstellingen voor MP4 H.264-videocodering te gebruiken. Omdat MP4-bestanden de H.264-videocodec gebruiken, biedt deze video van hoge kwaliteit, maar met een gecomprimeerde bestandsgrootte.

## Werken met voorinstellingen voor videocodering {#working-with-video-encoding-presets}

Primaire videobestanden die zijn gemaakt met videoproductieapparatuur en videobewerkingssoftware zijn vaak te groot en niet geschikt voor levering aan onlinebestemmingen. Als u digitale video wilt omzetten in de juiste indeling en de specificaties voor afspelen op verschillende schermen, kunt u *transcode* videobestanden (een proces dat ook wel bekend staat als *coderen*). Tijdens het coderingsproces wordt de video gecomprimeerd tot een kleinere, efficiënte bestandsgrootte voor een optimale weergave op het web en op mobiele apparaten.

Zie [Video&#39;s uploaden en coderen](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic biedt u een bibliotheek met vooraf gedefinieerde voorinstellingen voor videocodering die de meest gebruikte coderingsinstellingen weerspiegelen. Deze coderingsvoorinstellingen zijn geoptimaliseerd voor afspelen op doelschermen. Daarnaast kunnen beheerders hun eigen voorinstellingen voor videocodering maken om de grootte en afspeelkwaliteit van video&#39;s aan eindgebruikers aan te passen. Alle voorinstellingen voor videocodering, ongeacht of deze uit Adobe Dynamic Media Classic komen of op maat zijn gemaakt, voor uitvoervideo in de MP4-bestandsindeling.

In het scherm Voorinstellingen video kunnen beheerders videocodering instellen en beheren. Ze kunnen het volgende doen:

* Voorinstellingen voor videocodering activeren en deactiveren.
* Maak een voorinstelling voor videocodering.
* Voorinstellingen voor videocodering bewerken.
* Videovoorinstellingen verwijderen.

Alle video&#39;s die u uploadt naar Adobe Dynamic Media Classic of die u codeert in Adobe Dynamic Media Classic, worden beschouwd als &#39;video&#39;. Met andere woorden, deze asset-classificatie betekent dat u de video kunt afspelen op desktops, mobiele apparaten of beide. U kunt bijvoorbeeld een voorvertoning van deze typen video&#39;s weergeven in Adobe Dynamic Media Classic. U kunt ook URL&#39;s (met de functie URL kopiëren) en code genereren die u kunt insluiten (met de functie Code insluiten) voor gebruik met videospelers, websites enzovoort.

Zie [Video&#39;s voorvertonen in een videoviewer](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Zie [Een video-URL koppelen aan een mobiele site of website](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Zie [De videoviewer insluiten op een webpagina](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Voor video-elementen die u uploadt en codeert in Adobe Dynamic Media Classic, wordt video geleverd in de volgende bestandsindeling:

**MP4 H.264** Gebruik MP4-bestanden voor het volgende:

* HTTP Dynamic Streaming op desktops.
* HLS (Live HTTP-streaming, Apple-streamingprotocol).
* Progressieve video-levering aan mobiele Android™-, BlackBerry®- en Windows®-apparaten.

Alle andere video-indelingen en codec worden beschouwd als primaire video. Deze middelenclassificatie betekent dat de video een bronvideobestand is en niet kan worden gebruikt voor weergave op desktops of mobiele apparaten. U kunt deze typen video&#39;s bijvoorbeeld niet voorvertonen in Adobe Dynamic Media Classic. U kunt ook geen URL&#39;s kopiëren of code insluiten voor gebruik in videospelers, websites enzovoort.

### De lijst met videocoderingsvoorinstellingen filteren {#filtering-the-list-of-video-encoding-presets}

De pagina Voorinstellingen video en de pagina Voorinstellingen adaptieve video bestaan uit een tabel met de actieve status, de naam van de voorinstelling, het beoogde afspeelapparaat, de videogrootte en de gegevenssnelheid van elke voorinstelling voor video.

U kunt de lijst verfijnen door ervoor te kiezen om op zowel, Actief als Inactief te filteren, om alle videovoorinstellingen te zien of de lijst te beperken tot actieve of inactieve voorinstellingen.

U kunt ook filteren op basis van een afspeelapparaatoptie om de lijst te beperken tot videovoorinstellingen die zijn ontworpen voor het afspelen van video&#39;s op alle apparaten, computers, mobiele apparaten of tablets.

**De lijst met videocoderingsvoorinstellingen filteren:**

1. Ga in Adobe Dynamic Media Classic op de Global Navigation Bar naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]** of **[!UICONTROL Single Encoding Presets]**.

   De pagina&#39;s voor Adaptieve videovoorinstellingen en Eén codering bevatten een tabel met de status Actief, Naam voorinstelling, het beoogde afspeelapparaat, de videoafmetingen en de gegevenssnelheid van elke videovoorinstelling.

1. Op de Enige Coderende Vooraf ingestelde pagina genoemd Video vooraf instelt, op de Video vooraf instelt toolbar, gebruik de twee drop-down lijsten om de lijst van voorinstellingen in de lijst te verfijnen die op Actieve status, en playbackapparaat wordt gebaseerd.

   * Kies in de eerste, smallere vervolgkeuzelijst de optie **[!UICONTROL Both]** om alle videovoorinstellingen weer te geven of kies **[!UICONTROL Active]** of **[!UICONTROL Inactive]** U kunt de lijst ook beperken tot actieve of inactieve voorinstellingen.
   * Kies in de tweede, bredere vervolgkeuzelijst een afspeelapparaatoptie om de lijst te beperken tot videovoorinstellingen die zijn ontworpen voor het afspelen van video&#39;s op desktops. of voor het afspelen van video&#39;s op mobiele apparaten of tablets.

### Voorinstellingen voor videocodering activeren of deactiveren {#activating-or-deactivating-video-encoding-presets}

Geactiveerde videovoorinstellingen worden weergegeven in het dialoogvenster Taakopties uploaden. Het dialoogvenster wordt weergegeven wanneer een gebruiker videobestanden uploadt tijdens het uploaden. Ze kunnen kiezen uit een lijst met alle geactiveerde coderingsvoorinstellingen.

1. Ga in Adobe Dynamic Media Classic op de Global Navigation Bar naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Voer een van de volgende handelingen uit:

   * Selecteren **[!UICONTROL Adaptive Video Presets]**.
   * Selecteren **[!UICONTROL Single Encoding Presets]**.

1. Voer een van de volgende handelingen uit:

   * Als u een videovoorinstelling wilt activeren, selecteert u op de pagina met voorinstellingen onder de kolom Actief het vakje naast de naam van een voorinstelling.
   * Als u een videovoorinstelling wilt deactiveren, schakelt u het vakje naast de videovoorinstellingen die u inactief wilt maken uit.

      >[!NOTE]
      >
      >Inactieve videovoorinstellingen worden niet weergegeven in het dialoogvenster Opties voor uploaden.

1. Selecteer in de rechterbenedenhoek van de pagina de optie **[!UICONTROL Close]**.

### Een voorinstelling voor videocodering toevoegen of bewerken {#adding-or-editing-a-video-encoding-preset}

U kunt uw eigen aangepaste, enkelvoudige coderingsvideovoorinstellingen maken en deze toevoegen aan de tabel Video-voorinstellingen. U kunt ook alle vooraf gedefinieerde voorinstellingen voor één codering wijzigen die bij Adobe Dynamic Media Classic worden geleverd, op voorwaarde dat u de bewerkte voorinstelling opslaat met een nieuwe naam.

Adobe Dynamic Media Classic heeft maximale limieten ingesteld voor de doelgegevenssnelheid, resolutie-hoogte en resolutie-breedte voor een goede afspeelervaring. Er worden waarschuwingsberichten weergegeven als u deze limieten overschrijdt:

* Voor het afspelen van een computer gelden de volgende limieten: (Breedte/16) &#42; (Hoogte/16) &lt; 8192.
* Voor afspelen op mobiele apparaten gelden de volgende limieten: (Breedte/16) &#42; (Hoogte/16) &lt; 660; doelgegevenssnelheid &lt; 4000.
* Voor het afspelen van tablets gelden de volgende limieten: (Breedte/16) &#42; (Hoogte/16) &lt; 3600.

**Een voorinstelling voor videocodering toevoegen of bewerken:**

1. Ga in Adobe Dynamic Media Classic op de Global Navigation Bar naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Selecteren **[!UICONTROL Single Encoding Presets]**.
1. Voer op de pagina Voorinstellingen video een van de volgende handelingen uit:

   * Selecteer op de werkbalk Voorinstellingen video de optie **[!UICONTROL Add]** zodat u een videovoorinstelling kunt toevoegen.
   * Selecteer een videovoorinstelling. Selecteer in de werkbalk de optie **[!UICONTROL Edit]**.

      U kunt vooraf gedefinieerde Adobe Dynamic Media Classic-voorinstellingen niet bewerken. u kunt alleen een voorinstelling maken op basis van een bestaande voorinstelling als u **[!UICONTROL Save As]**.

1. Stel op de pagina Voorinstelling video toevoegen of Voorinstelling video bewerken de gewenste opties voor videovoorinstellingen in.

   Zie [Aanbevolen procedures voor videocodering](uploading-encoding-videos.md#best-practices-for-video-encoding) voor aanbevolen instellingen.

   | Voorinstelling video, optie | Beschrijving |
   | --- | --- |
   | Naam voorinstelling | Voer een beschrijvende naam in voor de videovoorinstelling. De naam die u invoert, wordt weergegeven in het dialoogvenster Taakopties uploaden, waarin gebruikers opties voor transcodering kiezen. |
   | Beschrijving | Beschrijf de videovoorinstelling. Wat u invoert, verschijnt als knopinfo wanneer u de aanwijzer over de naam van de voorinstelling in het dialoogvenster Taakopties uploaden verplaatst, waarin gebruikers opties voor transcodering kiezen. |
   | Afspeelapparaat | Kies het apparaat waarop de video moet worden afgespeeld. De opties zijn Computer (desktops), Mobiel (iPhone, iPad, Android™). of Tablet (alleen iPad). Deze instelling bepaalt automatisch de juiste video- en audiocodec die tijdens het coderen wordt gebruikt. |
   | Doelgegevenssnelheid | Voer de gemiddelde snelheid van de internetverbinding (in kilobits per seconde) van de eindgebruiker in. U kunt de snelheid invoeren of de schuifregelaar slepen om deze in te voeren. Het spectrum van de Snelheid van de Verbinding van de Gebruiker maakt een lijst van typische snelheden voor breedband, DSL, mobiel, en dial-up verbindingen. Deze instelling bepaalt automatisch de gecombineerde video- en audiogegevenssnelheid. Met andere woorden, de hoeveelheid gegevens die wordt gecodeerd om één seconde van videoplayback te maken. Hoe hoger de gegevenssnelheid, hoe beter de kwaliteit van de resulterende video. Te hoge gegevenssnelheden resulteren echter in grote bestanden die een subpariteit weergeven voor gebruikers met een lage bandbreedte. U kunt het beste een evenwicht vinden tussen hoge en lage gegevenssnelheden. Doel is een weergave van goede kwaliteit te maken zonder gebruikers met een smalle bandbreedte van elkaar te vervreemden. |
   | Hoogte-breedteverhouding | De verhouding is de verhouding tussen de breedte en de hoogte van de video. De eerste twee onderstaande hoogte-breedteverhoudingen worden vaak gebruikt om video horizontaal weer te geven:<ul><li> 4:3 - Wordt gebruikt voor bijna alle standaarddefinitie van tv-inhoud.</li><li>16:9 - Wordt gebruikt voor vrijwel alle breedbeeldinhoud en films op HDTV (High-Definition Television).</li><li>Automatisch schalen - (standaard) Eén coderingsvoorinstelling die met een willekeurige hoogte-breedteverhouding werkt om video&#39;s te maken die u kunt afspelen op mobiele apparaten, tablets en desktops. Geüploade bronvideo&#39;s die met deze voorinstelling zijn gecodeerd, worden ingesteld met een vaste hoogte. De breedte wordt echter automatisch geschaald om de hoogte-breedteverhouding van de video te behouden (hoogte-breedteverhouding).</li><li>Aangepast - Wordt gebruikt wanneer u een niet-standaardvideogrootte wilt definiëren.</li><li>De door u gekozen hoogte-breedteverhouding bepaalt de breedte- en hoogteinstellingen voor de resolutiegrootte. de breedte- en hoogtewaarde worden automatisch geschaald naar de juiste hoogte-breedteverhouding.</li></ul> |
   | Formaat resolutie | De grootte wordt bepaald door de resolutiegrootte, die wordt uitgedrukt door het aantal pixels breed en het aantal pixels hoog. Voer een breedte- en hoogtewaarde in pixels in of sleep de schuifregelaar om deze waarden in te voeren. Het spectrum Resolutie geeft een overzicht van de typische resolutiegrootten. De waarden voor breedte en hoogte passen automatisch de geselecteerde hoogte-breedteverhouding toe. Als u bijvoorbeeld 4:3 selecteert als hoogte-breedteverhouding en 400 invoert als breedte, wordt 300 automatisch ingevoerd als hoogte. Als u voor de instelling Verhouding automatisch schalen hebt geselecteerd, wordt de waarde voor Breedte voor de resolutiegrootte automatisch ingesteld op Automatisch. Selecteren **[!UICONTROL Preview]** zodat u een browservenster kunt openen en uw resolutieopties kunt bekijken. |
   | Achtervoegsel van bestand coderen | Voer een achtervoegsel in. Dit achtervoegsel wordt toegevoegd aan het resulterende gecodeerde videobestand. U kunt een koppelteken en een onderstrepingsteken in de naam invoeren; spaties en speciale tekens zijn niet toegestaan. |
   | Overige instellingen | Adobe Dynamic Media Classic bepaalt automatisch alle andere coderingsinstellingen volgens de richtlijnen voor het coderen van aanbevolen waarden. |

1. Voer een van de volgende handelingen uit:

   * Selecteren **[!UICONTROL Save]** als u een videovoorinstelling hebt toegevoegd of bewerkt.
   * Selecteren **[!UICONTROL Save As]** als u een videovoorinstelling hebt toegevoegd door te beginnen met een bestaande voorinstelling.

### Een voorinstelling voor videocodering verwijderen {#deleting-a-video-encoding-preset}

Beheerders kunnen aangepaste videovoorinstellingen verwijderen. Videovoorinstellingen die bij Adobe Dynamic Media Classic worden geleverd, kunnen niet worden verwijderd.

1. Ga in Adobe Dynamic Media Classic op de Global Navigation Bar naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Selecteren **[!UICONTROL Single Encoding Presets]**.
1. Selecteer op de pagina Voorinstellingen video een voorinstelling voor video in de tabel die u niet langer wilt of nodig hebt.
1. Selecteer op de werkbalk Voorinstellingen video de optie **[!UICONTROL Delete]**.
1. Selecteer in het dialoogvenster Voorinstelling verwijderen de optie **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Snel starten: Video in Adobe Dynamic Media Classic](quick-start-video.md#quick-start-video)
>* [Video&#39;s uploaden en coderen](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Werken met voorinstellingen voor videoviewers](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [Videovoorinstellingen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) trainingsvideo

