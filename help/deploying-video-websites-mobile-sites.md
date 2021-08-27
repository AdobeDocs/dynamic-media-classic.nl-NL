---
title: Video distribueren naar uw websites en mobiele sites
description: Leer hoe u video vanaf Adobe Dynamic Media Classic kunt implementeren op uw websites en mobiele sites.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 1%

---

# Video distribueren naar uw websites en mobiele sites{#deploying-video-to-your-websites-and-mobile-sites}

Websites, mobiele sites en bureaubladtoepassingen hebben via URL-tekenreeksen of ingesloten code toegang tot Adobe Dynamic Media Classic-serverinhoud, zoals video. Adobe Dynamic Media Classic activeert deze URL-tekenreeksen tijdens het publicatieproces. Als u de URL-tekenreeks of insluitcode voor uw video wilt plaatsen in uw webpagina&#39;s, mobiele pagina&#39;s en bureaubladtoepassingen, kopieert u deze vanuit Adobe Dynamic Media Classic.

>[!NOTE]
>
>De URL of insluitcode is pas actief als u het element publiceert.

## Video publiceren {#publishing-video}

Als u een video publiceert, kunnen Adobe Dynamic Media Classic Servers video leveren aan uw website, mobiele site of toepassing.

Er zijn twee verschillende methoden waarmee u video kunt publiceren:

* **Video&#39;s automatisch en direct publiceren tijdens het uploaden**  - Als onderdeel van het video-uploadproces kan Adobe Dynamic Media Classic video&#39;s automatisch publiceren wanneer ze worden geüpload en gecodeerd. Als u de mogelijkheid hebt om onmiddellijk te publiceren, hoeft u video&#39;s niet afzonderlijk te publiceren.

* **Video handmatig publiceren na het uploaden**  - Als u video&#39;s niet meteen wilt publiceren, kunt u de video&#39;s op elk gewenst moment handmatig publiceren.

Nadat u video&#39;s publiceert, activeert Adobe Dynamic Media Classic de URL-tekenreeksen voor uw HTML-pagina of toepassingscode.

**Video publiceren:**

1. Voer een van de volgende handelingen uit:

   * Als u video&#39;s automatisch en direct wilt publiceren tijdens het uploaden, selecteert u **[!UICONTROL Publish after uploading]** op de pagina Uploaden. U bent klaar; er zijn geen verdere stappen nodig .
   * Als u video&#39;s na het uploaden handmatig wilt publiceren, selecteert u in het deelvenster Bladeren de video&#39;s en selecteert u **Publiceren** op de algemene navigatiebalk.

## Een video-URL koppelen aan een mobiele site of website {#linking-a-video-url-to-a-mobile-site-or-a-website}

Nadat u een video hebt gepubliceerd, kunt u de URL verkrijgen voor gebruik in uw website, mobiele site of bureaubladtoepassing. Gebruik de video-URL wanneer u video wilt weergeven in een pop-upvenster of in een modaal venster vóór de webpagina.

Wanneer een klant de koppeling selecteert, worden het apparaat, de bandbreedte en de schermgrootte van de koppeling automatisch gedetecteerd. De juiste video wordt weergegeven om te worden afgespeeld in een vooraf gedefinieerde viewer voor desktop of in de native videospeler van het mobiele apparaat voor smartphones en tablets.

Zie ook [De videoviewer insluiten op een webpagina](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Een video-URL koppelen aan een mobiele site of website:**

1. Selecteer **[!UICONTROL Video]** of **[!UICONTROL Adaptive Video Set]** in de vervolgkeuzelijst **[!UICONTROL Show]** in het deelvenster Asset Browse.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap met de video of de adaptieve videoset die u wilt koppelen.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteer **[!UICONTROL Grid View]** of **[!UICONTROL List View]**. Dubbelklik in het deelvenster Asset Browse op de videominiatuur van één element om dit te openen in de gedetailleerde weergave. Selecteer in de URL&#39;s en het deelvenster Code insluiten rechts onder HTTP-streaming **[!UICONTROL Copy URL]** rechts van de gewenste viewer. U kunt het beste de URL kopiëren die is gekoppeld aan de `Universal_HTML5_Video`-viewer.
   * Selecteer **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel in de Viewer List. U kunt het beste de URL kopiëren die is gekoppeld aan de `Universal_HTML5_Video`-viewer.

   * Selecteer **[!UICONTROL List View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens rechts van de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel in de Viewer List. U kunt het beste de URL kopiëren die is gekoppeld aan de `Universal_HTML5_Video`-viewer.

   * Selecteer **[!UICONTROL Grid View]**, **[!UICONTROL List View]** of **[!UICONTROL Detail View]**. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel in de Viewer List. U kunt het beste de URL kopiëren die is gekoppeld aan de `Universal_HTML5_Video`-viewer.

1. Plak de URL-koppeling voor de HTML5-video op uw website en mobiele site.

## De videoviewer insluiten op een webpagina {#embedding-the-video-viewer-on-a-web-page}

Gebruik de functie Code insluiten als u de video wilt afspelen die is ingesloten op de webpagina. U kopieert de insluitcode naar het klembord, zodat u deze op uw webpagina&#39;s kunt plakken. Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

Zie ook [Een video-URL koppelen aan een mobiele site of een website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**De videoviewer insluiten op een webpagina:**

1. Selecteer **[!UICONTROL Video]** of **[!UICONTROL Adaptive Video Set]** in de vervolgkeuzelijst Tonen in het deelvenster Asset Browse.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap met de video of de adaptieve videoset waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteer **[!UICONTROL Grid View]** of **[!UICONTROL List View]**. Dubbelklik in het deelvenster Asset Browse op de videominiatuur van één element om dit te openen in de gedetailleerde weergave. Selecteer in de URL&#39;s en het deelvenster Code insluiten rechts onder HTTP-streaming **[!UICONTROL Embed Code]** rechts van de gewenste viewer. Als beste praktijken, selecteer **[!UICONTROL Embed Code]** die met `Universal_HTML5_Video` kijker wordt geassocieerd.
   * Selecteer **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en selecteer **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** onder de miniatuurafbeelding van de video.

      Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel in de Viewer List. Als beste praktijken, selecteer **[!UICONTROL Embed Code]** die met `Universal_HTML5_Video` kijker wordt geassocieerd.

   * Selecteer **[!UICONTROL List View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens rechts van de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel in de Viewer List. Als beste praktijken, selecteer **[!UICONTROL Embed Code]** die met `Universal_HTML5_Video` kijker wordt geassocieerd.

   * Selecteer **[!UICONTROL Grid View]**, **[!UICONTROL List View]** of **[!UICONTROL Detail View]**. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel in de Viewer List. Als beste praktijken, selecteer **[!UICONTROL Embed Code]** die met `Universal_HTML5_Video` kijker wordt geassocieerd.

1. Selecteer **[!UICONTROL Copy to Clipboard]** in het dialoogvenster Code insluiten.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Selecteer **[!UICONTROL Close]**.
1. Plak de insluitcode in uw webpagina&#39;s.

### Insluitcode implementeren voor het gebruik van HTML5-video met MP4-video-elementen {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Als u de Adobe Dynamic Media Classic HTML5-videospeler niet gebruikt, maar in plaats daarvan de native HTML5 `<video>`-tag met MP4-video-elementen wilt gebruiken, kunt u het volgende voorbeeld van de ingesloten code gebruiken:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Vervang `"S7 video thumbnail URL"` door de URL van de miniatuur van de video. Dit is de miniatuurafbeelding van de video die de gebruiker ziet voordat de video wordt afgespeeld.

   Zie [URL&#39;s van videominiaturen verkrijgen](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Vervang `"S7 OGG video asset URL (no player)"` door de progressieve URL van de video voor OGG video.

   Zie [Een video-URL koppelen aan een mobiele site of een website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Vervang `"S7 MP4 mobile progressive video asset URL (no player)"` door de progressieve URL voor mobiele apparaten van de video.

   Zie [Een video-URL koppelen aan een mobiele site of een website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Video implementeren met een externe videospeler {#deploying-video-using-a-third-party-video-player}

Als u een videospeler van derden of een aangepaste videospeler gebruikt in plaats van een Adobe Dynamic Media Classic-videoviewer, krijgt u de directe video-URL die geschikt is voor videostreaming met meerdere bitsnelheden of progressief downloaden met HLS.

**Video implementeren met een externe videospeler:**

1. Ga in Adobe Dynamic Media Classic op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.
1. Voer afhankelijk van het type URL dat u wilt gebruiken een van de volgende taken uit:

* Een directe URL voor HLS-streaming video (multi-bitsnelheid) genereren

   Construct u op de pagina **[!UICONTROL Application General Settings]** in de groep **[!UICONTROL Servers]** in het tekstveld **[!UICONTROL Published Server Name]** de directe URL. Gebruik de volgende syntaxis: `server/is/content/company/folder/filename.m3u8`

   Stel dat de naam van de gepubliceerde server `https://s7d9.scene7.com/.` Met de syntaxis in stap 2 is, kan de directe URL er als volgt uitzien:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Een directe URL voor HLS-streaming video (enkele bitsnelheid) genereren

   construeer op de pagina **[!UICONTROL Application General Settings]** in de groep **[!UICONTROL Servers]** in het tekstveld **[!UICONTROL HLS Streaming Server Name]** de directe URL met behulp van de volgende syntaxis:

   `server/company/folder/filename.ext.m3u8`

   Stel dat de naam van de HLS-streamingserver `https://s7mbrstream.scene7.com/hls-vod/` is. Met de syntaxis in stap 2 kan de directe URL er als volgt uitzien:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Een direct progressieve video-URL genereren

   construeer op de pagina **[!UICONTROL Application General Settings]** in de groep **[!UICONTROL Servers]** in het tekstveld **[!UICONTROL Progressive Video Server Name]** de directe eVideo-URL met behulp van de volgende syntaxis:

   `server/company/folder/filename`

   Stel dat de naam van de progressieve videoserver `https://s7d9.scene7.com/is/content/` is. Met de syntaxis in stap 2 kan de directe URL er als volgt uitzien:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Werken met videominiaturen {#working-with-video-thumbnails}

Adobe Dynamic Media Classic genereert miniaturen voor gecodeerde video&#39;s en vooraf gecodeerde video&#39;s. U kunt videominiaturen gebruiken zoals elk afbeeldingselement. Bovendien kunt u URLs voor de videoduimnagels verkrijgen die Adobe Dynamic Media Classic produceert en deze URLs buiten Adobe Dynamic Media Classic opstelt. U kunt bijvoorbeeld de miniaturen in zoekresultaten, verwante videobestanden en videoafspeellijsten op een website implementeren.

Miniaturen worden gegenereerd op basis van het eerste heterogene frame (niet een volledig zwart frame, of een helemaal wit frame enzovoort) van de video.

### URL&#39;s met videominiaturen verkrijgen {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic genereert automatisch videominiaturen tijdens het uploaden. De miniaturen worden weergegeven in de Lijstweergave en de Rasterweergave in het deelvenster Bladeren.

Als u URL&#39;s voor videominiaturen wilt genereren, voert u een publicatiebewerking uit.

Zie [Video publiceren](deploying-video-websites-mobile-sites.md#publishing_video).

Na publicatie kunt u videominiaturen-URL&#39;s opvragen in de gedetailleerde weergave in de URL&#39;s en het deelvenster Code insluiten. Selecteer **[!UICONTROL Copy URL]** rechts van de videominiatuur zodat u de URL ervan kunt kopiëren.

### Posterframes in videoviewers wijzigen {#modifying-poster-frames-in-video-viewers}

Het *posterframe* is het eerste frame dat in videoviewers wordt weergegeven voordat de video wordt afgespeeld. Adobe Dynamic Media Classic gebruikt videominiaturen als posterframes.

U kunt afbeeldingsaanpassingen toepassen op het posterframe. U kunt bijvoorbeeld het posterframe uitsnijden of transparant maken. Als u het posterframe wilt wijzigen, opent u het configuratiescherm voor de videoviewer en voert u modifiers in de sectie Modifiers voor posterafbeelding in.

Zie [Een voorinstelling voor een videoviewer toevoegen of bewerken](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Zie [Handleiding voor beeldservers](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

U kunt videominiaturen ook wijzigen door modifiers toe te voegen aan videominiaturen-URL&#39;s.

>[!MORELIKETHIS]
>
>* [Bestanden publiceren](publishing-files.md#publishing_files)