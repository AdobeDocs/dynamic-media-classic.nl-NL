---
title: Video-SEO (Optimalisatie zoekmachine)
description: Leer hoe u video-SEO-instellingen configureert in Adobe Dynamic Media Classic.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 0%

---

# Video-SEO (Optimalisatie zoekmachine){#video-seo-search-engine-optimization}

SEO is het proces om het volume van verkeer aan een Website van onderzoeksmotoren te verbeteren. Terwijl zoekmachines uitblinken in het verzamelen van informatie over op tekst gebaseerde inhoud, kunnen ze geen informatie over video adequaat verkrijgen tenzij deze informatie aan hen wordt verstrekt.

Met Adobe Dynamic Media Classic Video SEO kunt u videometagegevens toepassen om zoekprogramma&#39;s beschrijvingen van uw video&#39;s te bieden. Met Adobe Dynamic Media Classic kunt u videositemaps en mRSS-feeds maken. Deze standaard XML-bestanden worden gebruikt voor het verzenden van videogegevens naar zoekprogramma&#39;s:

* **Video Sitemap**  - Hiermee wordt precies aangegeven waar en wat de video-inhoud op een site is. Op Google kunnen dus volledig naar video&#39;s worden gezocht. Een videositemap kan bijvoorbeeld de actieve tijd en de categorieën video&#39;s opgeven. Zie [Videositemaps en alternatieven voor videositemap](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1) voor meer informatie over videositemaps.

* **mRSS-feed**  (Media Echt eenvoudige syntaxis) - Gebruikt door uitgevers van inhoud om mediabestanden naar Yahoo te sturen! Video zoeken. Zie [Video-sitemaps en alternatieven voor videositemap](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1) voor informatie over mRSS-feeds.

>[!NOTE]
>
>Google ondersteunt zowel het Video Sitemap- als het mRSS-feed-protocol voor het verzenden van informatie naar zoekmachines.

Adobe Dynamic Media Classic kan videositemaps en mRSS-feeds genereren op basis van metagegevens die bij elke video worden opgeslagen. Wanneer u videositemaps en mRSS-feeds maakt, bepaalt u welke metagegevensvelden van videobestanden moeten worden opgenomen. Op deze manier beschrijft u uw video&#39;s naar zoekprogramma&#39;s, zodat zoekprogramma&#39;s het verkeer naar video&#39;s op uw website nauwkeuriger kunnen sturen

>[!NOTE]
>
>Voordat u een video-itemap of MRSS-feed maakt, moet u weten welke velden de zoekmachine in het XML-bestand nodig heeft en hoe u deze velden kunt structureren. Als u een geslaagde video-Sitemap of mRSS-feed wilt maken, moet deze voldoen aan de vereisten van het zoekprogramma.

Adobe Dynamic Media Classic maakt rapporten over videositemaps en mRSS-feeds nadat u deze hebt gegenereerd. Deze rapporten zijn beschikbaar op de VideoSEO- pagina van het Rapport.

>[!NOTE]
>
>Voor de videobeelden Sitemaps en de feeds mRSS, vangt Adobe Dynamic Media Classic slechts meta-gegevens van video&#39;s die voor publicatie worden gemerkt. Markeer video&#39;s die u wilt publiceren om de bijbehorende metagegevens op te nemen in Video-items en MRSS-feeds.

## Video-SEO-instellingen kiezen {#choosing-video-seo-settings}

Selecteer Video SEO-instellingen voor video-items en MRSS-feeds op de pagina **[!UICONTROL Video Search Engine Optimization Settings]**. Als u deze pagina wilt openen, gaat u op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]**.

Kies in het gebied **[!UICONTROL General Setting]** of u videositemaps, mRSS-feeds of beide wilt genereren. Wijs in het gebied **[!UICONTROL Generation Settings]** metagegevensvelden toe aan invoervelden.

Nadat u instellingen hebt gekozen, selecteert u **[!UICONTROL Save]** (of **[!UICONTROL Save & Generate]**) om de videositemap, mRSS-feeds of beide te maken.

### Algemene instellingen instellen {#choosing-general-settings}

Kies een rapportmodus in de vervolgkeuzelijst **[!UICONTROL Generation Mode]**:

* **Video Sitemap**  - Maak een videositemap.

* **mRSS-feed**  - Maak een Media RSS-feed (mRSS).

* **Beide**  - Maak beide typen XML-bestanden.

* **Kies deze optie uit** . U kunt de videositemaps en de RSS-feeds (mRSS) van Media niet meer genereren.

Kies in de vervolgkeuzelijst **[!UICONTROL Automatic/Manual Mode]** of u automatisch of handmatig wilt genereren:

* **Automatische modus**  - Adobe Dynamic Media Classic genereert elke dag automatisch één videosap, Media RSS-feed (mRSS) of beide. Selecteer de optie **[!UICONTROL Mark for Publish]** om het XML-bestand dat door Adobe Dynamic Media Classic wordt gegenereerd, automatisch te markeren voor publicatie.

   * **Markeren voor** PublishMarks voor het publiceren van het XML-bestand dat wordt gegenereerd.

* **Handmatige modus**  - Adobe Dynamic Media Classic genereert de video-Sitemap, de Media RSS-feed (mRSS) of beide wanneer u  **[!UICONTROL Generate]** of  **[!UICONTROL Save & Generate]** in het scherm Optimalisatie-instellingen voor videozoekopdrachten selecteert. Kies ook de volgende opties:

   * **Geen verdere instellingen**  - markeert het gegenereerde XML-bestand niet voor publicatie.

   * **Markeren voor publicatie**  - Markeringen voor publicatie van het gegenereerde XML-bestand.

   * **Partiële generatie**  toestaan - Zoekprogramma&#39;s kunnen een XML-bestand afwijzen als het geen volledige metagegevens voor alle video&#39;s bevat. Met deze optie wordt het XML-bestand gegenereerd, zelfs als voor bepaalde video&#39;s geen metagegevens beschikbaar zijn. Een waarschuwing wordt geregistreerd op het scherm van het Rapport. Kies deze optie als u het XML-bestand wilt exporteren en de ontbrekende gegevens handmatig wilt verwerken.

### Generatie-instellingen kiezen {#choosing-generation-settings}

In het gedeelte Instellingen genereren worden invoervelden voor de videospecificatie, of de mRSS-feed of beide vermeld en in het deelvenster Metagegevens worden de namen van metagegevensvelden weergegeven. In het gedeelte Algemene instellingen kunt u invoervelden toewijzen aan metagegevensvelden. Op deze manier geeft u aan Adobe Dynamic Media Classic door waar u metagegevens voor de videositemap en/of mRSS-feed wilt ophalen.

1. Kies een metagegevensweergave in het menu Weergaven Metagegevens. Nadat u een weergave hebt gekozen, worden de namen van metagegevensvelden weergegeven in het deelvenster Metagegevens.
Zie [Metagegevensweergaven](application-setup.md#metadata_views).
1. Sleep namen van metagegevensvelden van het deelvenster Metagegevens naar de invoervelden Openingspagina, Titel, Beschrijving, Labels en Categorie. De velden Openingspagina, Titel en Beschrijving zijn vereist.

   >[!NOTE]
   >
   >U kunt ook handmatig gegevens invoeren in invoervelden.

1. Voer een van de volgende handelingen uit:

   * Als u uw instellingen wilt opslaan zonder het XML-bestand te genereren, selecteert u **[!UICONTROL Save]**.
   * Selecteer **[!UICONTROL Save & Generate]** om het bestand op te slaan en te genereren.

      Het XML-bestand wordt gegenereerd en opgenomen in het taaklogbestand. Video Sitemap (video-sitemap) en een Media RSS-feed (mRSS) worden opgeslagen in de hoofdmap van uw bedrijf.

>[!NOTE]
>
>Publiceer de videospecificaties of de MRSS-feed voordat u deze kunt verzenden naar zoekprogramma&#39;s. Video Sitemap en Media RSS (mRSS) de voederdossiers worden opgeslagen in de wortelomslag van het bedrijf. Markeer deze XML-bestanden voor publicatie, indien nodig, en selecteer **[!UICONTROL Publish]**.

## Video-items en RSS-Feed-bestanden verzenden naar een zoekprogramma {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video Sitemap en Media RSS (mRSS) de voederdossiers worden opgeslagen in de wortelomslag van het bedrijf:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieer een van deze URL&#39;s naar de webstramiengereedschappen van het zoekprogramma om het bestand Video Sitemap of Media RSS (mRSS) naar zoekprogramma&#39;s te verzenden.

## Video SEO-rapporten weergeven {#viewing-video-seo-reports}

Bekijk video SEO rapporten op de Videopagina van het Rapport van de Optimalisering van de Motor van het Onderzoek. Als u deze pagina wilt openen, gaat u op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]**.

Als de fouten voorkwamen toen een rapport werd geproduceerd, zijn zij vermeld op de pagina van het Rapport.
