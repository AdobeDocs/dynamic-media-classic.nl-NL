---
title: Video-SEO (Optimalisatie zoekmachine)
seo-title: Video-SEO (Optimalisatie zoekmachine)
description: 'null'
seo-description: Leer hoe u video-SEO-instellingen configureert.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# Video-SEO (Optimalisatie zoekmachine){#video-seo-search-engine-optimization}

SEO is het proces om het volume van verkeer aan een Website van onderzoeksmotoren te verbeteren. Terwijl zoekmachines uitblinken in het verzamelen van informatie over op tekst gebaseerde inhoud, kunnen ze geen informatie over video adequaat verkrijgen tenzij deze informatie aan hen wordt verstrekt.

Met Dynamic Media Classic Video SEO kunt u videometagegevens gebruiken om zoekprogramma&#39;s beschrijvingen van uw video&#39;s te bieden. Met Dynamic Media Classic kunt u videositemaps en mRSS-feeds maken. Dit zijn standaard XML-bestanden voor het verzenden van videogegevens naar zoekprogramma&#39;s:

**Met Video Sitemap** wordt Google precies aangegeven waar en wat de video-inhoud op een site is. Daarom kunnen video&#39;s volledig worden doorzocht op Google. Een videositemap kan bijvoorbeeld de actieve tijd en de categorieën video&#39;s opgeven. Ga naar https://www.google.com/support/webmasters/bin/answer.py?answer=80471 voor informatie over videodemo&#39;s.

**MRSS-feed** (Media Echt eenvoudige syntaxis) Gebruikt door uitgevers van inhoud om mediabestanden naar Yahoo te sturen! Video zoeken. Zie https://www.rssboard.org/media-rss voor informatie over mRSS-feeds.

>[!NOTE]
>
>Google ondersteunt zowel het Video Sitemap- als het mRSS-feed-protocol voor het verzenden van informatie naar zoekmachines.

Met Dynamic Media Classic kunt u videositemaps en mRSS-feeds genereren op basis van metagegevens die bij elke video worden opgeslagen. Wanneer u videositemaps en mRSS-feeds maakt, bepaalt u welke metagegevensvelden van videobestanden moeten worden opgenomen. Op deze manier beschrijft u uw video&#39;s naar zoekprogramma&#39;s, zodat zoekprogramma&#39;s het verkeer naar video&#39;s op uw website nauwkeuriger kunnen sturen

>[!NOTE]
>
>Voordat u een video-itemap of MRSS-feed maakt, moet u weten welke velden de zoekmachine in het XML-bestand nodig heeft en hoe u deze velden kunt structureren. Als u een geslaagde video-Sitemap of mRSS-feed wilt maken, moet deze voldoen aan de vereisten van het zoekprogramma.

Dynamic Media Classic maakt rapporten over videositemaps en mRSS-feeds nadat u deze hebt gegenereerd. Deze rapporten zijn beschikbaar op het Video scherm van het Rapport SEO.

>[!NOTE]
>
>Voor de videobeelden Sitemaps en de feeds mRSS, vangen de Dynamische Klassieke Media slechts meta-gegevens van video&#39;s die voor publiceren duidelijk zijn. Markeer video&#39;s die u wilt publiceren om de bijbehorende metagegevens op te nemen in Video-items en MRSS-feeds.

## Video-SEO-instellingen kiezen {#choosing-video-seo-settings}

Kies Video SEO-instellingen voor Video Sitemaps en MRSS-feeds in het scherm Video Search Engine Optimization Settings. Kies Setup > Application Setup > Video SEO > Settings om dit scherm te openen.

Kies in het gedeelte Algemene instelling of u videositemaps, mRSS-feeds of beide wilt genereren. Wijs in het gedeelte Generatie-instellingen metagegevensvelden toe aan invoervelden.

Nadat u de instellingen hebt gekozen, klikt u op Genereren (of Opslaan en genereren) om de videositemap, MRSS-feeds of beide te maken.

### Algemene instellingen kiezen {#choosing-general-settings}

Voor de drop-down lijst van de Wijze van de Generatie, kies een rapportwijze:

**Videositemap** Een videositemap maken.

**mRSS-feed** Maak een Media RSS-feed (mRSS).

**Beide** maken beide typen XML-bestanden.

**Uit** Kies deze optie om te stoppen met het genereren van videositemaps en een Media RSS-feeds (mRSS).

Kies in de vervolgkeuzelijst Automatische modus/Handmatige modus of u automatisch of handmatig wilt genereren:

**Met Automatische modus** Dynamische media Classic worden elke dag automatisch één videositemap, Media RSS-feed (mRSS) of beide gegenereerd. Kies de optie Markeren voor publiceren om het XML-bestand dat Dynamic Media Classic genereert, automatisch te markeren voor publicatie.

**Met de modus** Handmatig Dynamic Media Classic wordt de feed Video Sitemap, Media RSS (mRSS) of beide gegenereerd wanneer u op Genereren of Opslaan en genereren klikt in het scherm Optimalisatie-instellingen voor video zoeken. Kies ook de volgende opties:

**Geen andere instellingen** markeert het gegenereerde XML-bestand niet voor publicatie.

**Markeren voor publicatietekens** om het gegenereerde XML-bestand te publiceren.

**Zoekprogramma&#39;s voor gedeeltelijke generatie** toestaan kan een XML-bestand afwijzen als het niet alle metagegevens voor alle video&#39;s bevat. Met deze optie wordt het XML-bestand gegenereerd, zelfs als er voor bepaalde video&#39;s geen metagegevens beschikbaar zijn. Een waarschuwing wordt geregistreerd op het scherm van het Rapport. Kies deze optie als u het XML-bestand wilt exporteren en de ontbrekende gegevens handmatig wilt verwerken.

### Generatie-instellingen kiezen {#choosing-generation-settings}

In het gebied Instellingen genereren worden invoervelden voor de videospecificatie en/of de MRSS-feed weergegeven en in het deelvenster Metagegevens worden de namen van metagegevensvelden weergegeven. In het gedeelte Algemene instellingen kunt u invoervelden toewijzen aan metagegevensvelden. Op deze manier geeft u aan Dynamic Media Classic door waar u metagegevens voor de videositemap en/of mRSS-feed kunt ophalen.

1. Kies een metagegevensweergave in het menu Weergaven Metagegevens. Nadat u een weergave hebt gekozen, worden de namen van metagegevensvelden weergegeven in het deelvenster Metagegevens. (Zie Weergaven van [metagegevens voor informatie over weergaven van metagegevens](application-setup.md#metadata_views).)
1. Sleep namen van metagegevensvelden van het deelvenster Metagegevens naar de invoervelden Openingspagina, Titel, Beschrijving, Labels en Categorie. De velden Openingspagina, Titel en Beschrijving zijn vereist.

   >[!NOTE]
   >
   >U kunt ook handmatig gegevens invoeren in invoervelden.

1. Klik op Opslaan (om uw instellingen op te slaan zonder het XML-bestand te genereren), Genereren (om het XML-bestand te genereren) of Opslaan en genereren (om het bestand op te slaan en te genereren).

   Het XML-bestand wordt gegenereerd en opgenomen in het taaklogbestand. Video Sitemap (video-sitemap) en een Media RSS-feed (mRSS) worden opgeslagen in de hoofdmap van uw bedrijf.

>[!NOTE]
>
>U moet de videospecificaties of de MRSS-feed publiceren voordat u deze kunt verzenden naar zoekprogramma&#39;s. Video Sitemap en Media RSS (mRSS) de voederdossiers worden opgeslagen in de wortelomslag van het bedrijf. Markeer deze XML-bestanden voor publicatie, indien nodig, en klik op Publiceren.

## Video Sitemap- en MRSS-Feed-bestanden verzenden naar zoekprogramma&#39;s {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video Sitemap en Media RSS (mRSS) de voederdossiers worden opgeslagen in de wortelomslag van het bedrijf:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieer een van deze URL&#39;s naar de webstramiengereedschappen van het zoekprogramma om het bestand Video Sitemap of Media RSS (mRSS) naar zoekprogramma&#39;s te verzenden.

## Video SEO-rapporten weergeven {#viewing-video-seo-reports}

Bekijk video SEO rapporten over het scherm van het Rapport van de Optimalisering van de Motor van het Onderzoek Video. Klik op Setup > Application Setup > Video SEO > Reports om dit scherm te openen.

Als de fouten voorkwamen toen een rapport werd geproduceerd, zijn zij vermeld op het scherm van het Rapport.
