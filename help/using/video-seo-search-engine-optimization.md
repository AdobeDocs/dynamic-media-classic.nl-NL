---
title: Video-SEO (Optimalisatie zoekmachine)
description: Leer hoe u SEO-instellingen voor video kunt configureren in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# Video-SEO (Optimalisatie zoekmachine){#video-seo-search-engine-optimization}

SEO is het proces om het volume van verkeer aan een Website van onderzoeksmotoren te verbeteren. Terwijl zoekprogramma&#39;s uitblinken in het verzamelen van informatie over op tekst gebaseerde inhoud, kunnen ze niet voldoende informatie over video verkrijgen. Deze informatie moet aan hen worden verstrekt.

Met Adobe Dynamic Media Classic Video SEO kunt u videometagegevens toepassen om zoekprogramma&#39;s beschrijvingen van uw video&#39;s te bieden. Adobe Dynamic Media Classic biedt u de mogelijkheid om videositemaps en mRSS-feeds te maken. Deze standaard XML-bestanden worden gebruikt voor het verzenden van videogegevens naar zoekprogramma&#39;s:

* **Video Sitemap**: Maakt Google precies waar en wat de videoinhoud op een plaats is. Op Google kunnen dus volledig naar video&#39;s worden gezocht. Een videositemap kan bijvoorbeeld de actieve tijd en de categorieën video&#39;s opgeven. Voor informatie over VideoSitemaps, zie [ Video sitemaps en videoalternatieven sitemap ](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

* **mRSS (Media Echt Eenvoudige Syndicatie) voer**: Gebruikt door inhouduitgevers om media dossiers in Yahoo te voeren! Video zoeken. Voor informatie over de diervoeders van mRSS, zie [ Video sitemaps en de alternatieven van videositemap ](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

>[!NOTE]
>
>Google ondersteunt zowel het Video Sitemap- als het mRSS-feed-protocol voor het verzenden van informatie naar zoekmachines.

Adobe Dynamic Media Classic kan videobeelden Sitemaps en mRSS-feeds genereren op basis van metagegevens die bij elke video worden opgeslagen. Wanneer u videositemaps en mRSS-feeds maakt, bepaalt u welke metagegevensvelden van videobestanden moeten worden opgenomen. Op deze manier beschrijft u uw video&#39;s aan onderzoeksmotoren zodat de onderzoeksmotoren verkeer aan video&#39;s op uw Website nauwkeuriger kunnen leiden.

>[!NOTE]
>
>Voordat u een video-itemap of MRSS-feed maakt, moet u weten welke velden de zoekmachine in het XML-bestand nodig heeft en hoe u deze velden kunt structureren. Als u een geslaagde video-Sitemap of mRSS-feed wilt maken, moet deze voldoen aan de vereisten van het zoekprogramma.

Nadat u deze hebt gegenereerd, maakt Adobe Dynamic Media Classic rapporten over videoitems en MRSS-feeds. Deze rapporten zijn beschikbaar op de VideoSEO- pagina van het Rapport.

>[!NOTE]
>
>Voor de videobeelden Sitemaps en de feeds mRSS, vangt Adobe Dynamic Media Classic meta-gegevens slechts van video&#39;s die voor publicatie duidelijk zijn. Markeer video&#39;s voor publicatie om de bijbehorende metagegevens op te nemen in Video-items en MRSS-feeds.

## Video-SEO-instellingen kiezen

Selecteer Video SEO-instellingen voor Video Sitemaps en MRSS-feeds op de **[!UICONTROL Video Search Engine Optimization Settings]** -pagina. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]** om deze pagina op de algemene navigatiebalk te openen.

Kies in het gebied **[!UICONTROL General Setting]** of u videositemaps, mRSS-feeds of beide wilt genereren. Wijs in het gebied **[!UICONTROL Generation Settings]** metagegevensvelden toe aan invoervelden.

Nadat u de instellingen hebt gekozen, selecteert u **[!UICONTROL Save]** (of **[!UICONTROL Save & Generate]** ) om de videositemap, mRSS-feeds of beide te maken.

### Algemene instellingen instellen {#choosing-general-settings}

Kies een rapportmodus in de vervolgkeuzelijst **[!UICONTROL Generation Mode]** :

* **Video Sitemap**: Creeer een Video Sitemap.

* **mRSS Feed**: Creeer een (mRSS) voer van Media.

* **allebei**: Creeer beide soorten dossiers van XML.

* **weg**: Ophouden producerend VideoSitemaps en het voer van Media RSS (mRSS), verkies deze optie.

Kies in de vervolgkeuzelijst **[!UICONTROL Automatic/Manual Mode]** of u automatisch of handmatig wilt genereren:

* **Automatische Wijze**: Adobe Dynamic Media Classic produceert automatisch één VideoSitemap, (mRSS) voer van Media RSS, of allebei, elke dag. Selecteer de optie **[!UICONTROL Mark for Publish]** zodat u het door Adobe Dynamic Media Classic gegenereerde XML-bestand automatisch kunt markeren voor publicatie.

   * **Teken voor Publish** Tekens voor publiceer het dossier van XML dat wordt geproduceerd.

* **Handmatige Wijze**: Adobe Dynamic Media Classic produceert de VideoSitemap, (mRSS) voer van Media RSS, of allebei, wanneer u **[!UICONTROL Generate]** of **[!UICONTROL Save & Generate]** in het Video scherm van de Montages van de Optimalisering van het Onderzoek selecteert. Kies ook de volgende opties:

   * **Geen Verdere Montages**: Merk voor publiceer niet het dossier van XML dat wordt geproduceerd.

   * **Teken voor Publish**: De markeringen voor publiceren het dossier van XML dat wordt geproduceerd.

   * **staat Gedeeltelijke Generatie** toe: De motoren van het onderzoek kunnen een dossier van XML verwerpen als het volledige meta-gegevensinformatie voor alle video&#39;s niet bevat. Met deze optie wordt het XML-bestand gegenereerd, zelfs als voor bepaalde video&#39;s geen metagegevens beschikbaar zijn. Een waarschuwing wordt geregistreerd op het scherm van het Rapport. Kies deze optie als u het XML-bestand wilt exporteren en de ontbrekende gegevens handmatig wilt verwerken.

### Generatie-instellingen kiezen {#choosing-generation-settings}

In het gedeelte Instellingen genereren worden invoervelden weergegeven voor de videositemap, de mRSS-feed of beide. In het deelvenster Metagegevens worden de namen van metagegevensvelden weergegeven. In het gedeelte Algemene instellingen kunt u invoervelden toewijzen aan metagegevensvelden. Op deze manier geeft u Adobe Dynamic Media Classic de locatie op waar u metagegevens voor de videositemap en/of MRSS-feed wilt verkrijgen.

1. Kies een metagegevensweergave in het menu Weergaven Metagegevens. Nadat u een weergave hebt gekozen, worden de namen van metagegevensvelden weergegeven in het deelvenster Metagegevens.
Zie {de meningen van 0} Meta-gegevens [.](application-setup.md#metadata_views)
1. Sleep namen van metagegevensvelden van het deelvenster Metagegevens naar de invoervelden Openingspagina, Titel, Beschrijving, Labels en Categorie. De velden Openingspagina, Titel en Beschrijving zijn vereist.

   >[!NOTE]
   >
   >U kunt ook handmatig gegevens invoeren in invoervelden.

1. Voer een van de volgende handelingen uit:

   * Selecteer **[!UICONTROL Save]** als u uw instellingen wilt opslaan zonder het XML-bestand te genereren.
   * Selecteer **[!UICONTROL Save & Generate]** om het bestand op te slaan en te genereren.

     Het XML-bestand wordt gegenereerd en opgenomen in het taaklogbestand. Video Sitemap (video-sitemap) en een Media RSS-feed (mRSS) worden opgeslagen in de hoofdmap van uw bedrijf.

>[!NOTE]
>
>Publiceer de videospecificaties of de MRSS-feed voordat u deze kunt verzenden naar zoekprogramma&#39;s. Video Sitemap en Media RSS (mRSS) de voederdossiers worden opgeslagen in de wortelomslag van het bedrijf. Markeer deze XML-bestanden voor publicatie, indien nodig, en selecteer **[!UICONTROL Publish]** .

## Video-items en RSS-Feed-bestanden verzenden naar een zoekprogramma {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video Sitemap en Media RSS (mRSS) de voederdossiers worden opgeslagen in de wortelomslag van het bedrijf:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieer een van deze URL&#39;s naar de webstramiengereedschappen van het zoekprogramma om het bestand Video Sitemap of Media RSS (mRSS) naar zoekprogramma&#39;s te verzenden.

## Video SEO-rapporten weergeven {#viewing-video-seo-reports}

Bekijk video SEO rapporten op de Videopagina van het Rapport van de Optimalisering van de Motor van het Onderzoek van het Onderzoek. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]** om deze pagina op de algemene navigatiebalk te openen.

Als de fouten voorkwamen toen een rapport werd geproduceerd, zijn zij vermeld op de pagina van het Rapport.
