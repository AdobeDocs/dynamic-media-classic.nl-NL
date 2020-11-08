---
title: Video gebruiken op uw websites en mobiele sites
seo-title: Video gebruiken op uw websites en mobiele sites
description: 'null'
seo-description: Leer hoe u video implementeert op uw websites en mobiele sites.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1689'
ht-degree: 1%

---


# Video gebruiken op uw websites en mobiele sites{#deploying-video-to-your-websites-and-mobile-sites}

Websites, mobiele sites en bureaubladtoepassingen hebben via URL-tekenreeksen of ingesloten code toegang tot Dynamic Media Classic-serverinhoud, zoals video. Dynamic Media Classic activeert deze URL-tekenreeksen tijdens het publicatieproces. Als u de URL-tekenreeks of insluitcode voor uw video wilt plaatsen in uw webpagina&#39;s, mobiele pagina&#39;s en bureaubladtoepassingen, kopieert u deze vanuit Dynamic Media Classic.

>[!NOTE]
>
>De URL of insluitcode is pas actief als u het element publiceert.

## Video publiceren {#publishing-video}

Wanneer u een video publiceert, kunnen Dynamic Media Classic Servers video&#39;s leveren aan uw website, mobiele site of toepassing.

Er zijn twee verschillende methoden waarmee u video kunt publiceren:

* **Video&#39;s automatisch en direct tijdens het uploaden publiceren**

   Tijdens het uploaden van video&#39;s kan Dynamic Media Classic automatisch video&#39;s publiceren wanneer deze worden geüpload en gecodeerd. Als u de mogelijkheid hebt om onmiddellijk te publiceren, hoeft u video&#39;s niet afzonderlijk te publiceren.

* **Video na het uploaden handmatig publiceren**

   Als u video&#39;s niet meteen wilt publiceren, kunt u de video&#39;s op elk gewenst moment handmatig publiceren.

Nadat u video&#39;s publiceert, activeert Dynamic Media Classic de URL-tekenreeksen voor uw HTML-pagina of toepassingscode.

**Video publiceren**

1. Voer een van de volgende handelingen uit:

   * Als u video&#39;s automatisch en direct wilt publiceren tijdens het uploaden, klikt u in het scherm Uploaden op **Publiceren na het uploaden**. U bent klaar; er zijn geen verdere stappen nodig .
   * Als u video&#39;s na het uploaden handmatig wilt publiceren, selecteert u de video&#39;s in het deelvenster Bladeren en klikt u vervolgens op **Publiceren** op de algemene navigatiebalk.

## Een video-URL koppelen aan een mobiele site of website {#linking-a-video-url-to-a-mobile-site-or-a-website}

Nadat u een video hebt gepubliceerd, kunt u de URL verkrijgen voor gebruik in uw website, mobiele site of bureaubladtoepassing. Gebruik de video-URL wanneer u video wilt weergeven in een pop-upvenster of in een modaal venster vóór de webpagina.

Wanneer een klant op de koppeling klikt, worden hun apparaat, bandbreedte en schermgrootte automatisch gedetecteerd. De juiste video wordt weergegeven om te worden afgespeeld in een vooraf gedefinieerde viewer voor desktop of in de native videospeler van het mobiele apparaat voor smartphones en tablets.

Zie ook [De videoviewer insluiten op een webpagina](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Een video-URL koppelen aan een mobiele site of website**

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Middelen bladeren op **Video** of **Adaptieve videoset**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap met de video of de adaptieve videoset die u wilt koppelen.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **Rasterweergave** of **Lijstweergave**. Dubbelklik in het deelvenster Asset Browse op de videominiatuur van één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en het deelvenster Code insluiten rechts onder HTTP-streaming op URL **** kopiëren rechts van de gewenste viewer. U kunt het beste de URL kopiëren die aan de `Universal_HTML5_Video` viewer is gekoppeld.
   * Klik op **Rasterweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens onder de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik op URL **** kopiëren onder de kolom Handelingen van de tabel in de Viewer List. U kunt het beste de URL kopiëren die aan de `Universal_HTML5_Video` viewer is gekoppeld.

   * Klik op **Lijstweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik op URL **** kopiëren onder de kolom Handelingen van de tabel in de Viewer List. U kunt het beste de URL kopiëren die aan de `Universal_HTML5_Video` viewer is gekoppeld.

   * Klik op **Rasterweergave**, **Lijstweergave** of **Gedetailleerde weergave**. Klik op dezelfde werkbalk op **Voorvertoning** > **Viewer List**.

      Klik op URL **** kopiëren onder de kolom Handelingen van de tabel in de Viewer List. U kunt het beste de URL kopiëren die aan de `Universal_HTML5_Video` viewer is gekoppeld.

1. Plak de URL-koppeling voor de HTML5-video op uw website en mobiele site.

## De videoviewer insluiten op een webpagina {#embedding-the-video-viewer-on-a-web-page}

Gebruik de functie Code insluiten als u de video wilt afspelen die is ingesloten op de webpagina. U kopieert de insluitcode naar het klembord, zodat u deze op uw webpagina&#39;s kunt plakken. Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

Zie ook Een video-URL [koppelen aan een mobiele site of website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**De videoviewer insluiten op een webpagina**

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Middelen bladeren op **Video** of **Adaptieve videoset**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap met de video of de adaptieve videoset waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **Rasterweergave** of **Lijstweergave**. Dubbelklik in het deelvenster Asset Browse op de videominiatuur van één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en het deelvenster Code insluiten rechts onder HTTP-streaming op Code **** insluiten rechts van de gewenste viewer. U kunt het beste op Code **** insluiten klikken die aan de `Universal_HTML5_Video` viewer is gekoppeld.
   * Klik op **Rasterweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens onder de afbeelding van de videominiatuur op **Voorvertoning** > **Viewer List**.

      Klik op de pagina Viewer List onder de kolom Acties van de tabel op Code **** insluiten. U kunt het beste op Code **** insluiten klikken die aan de `Universal_HTML5_Video` viewer is gekoppeld.

   * Klik op **Lijstweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik op de pagina Viewer List onder de kolom Acties van de tabel op Code **** insluiten. U kunt het beste op Code **** insluiten klikken die aan de `Universal_HTML5_Video` viewer is gekoppeld.

   * Klik op **Rasterweergave**, **Lijstweergave** of **Gedetailleerde weergave**. Klik op dezelfde werkbalk op **Voorvertoning** > **Viewer List**.

      Klik op de pagina Viewer List onder de kolom Acties van de tabel op Code **** insluiten. U kunt het beste op Code **** insluiten klikken die aan de `Universal_HTML5_Video` viewer is gekoppeld.

1. Klik in het dialoogvenster Code insluiten op **Kopiëren naar klembord**.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Klik op **Sluiten**.
1. Plak de insluitcode in uw webpagina&#39;s.

### Insluitcode implementeren voor het gebruik van HTML5-video met MP4-video-elementen {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Als u de Dynamic Media Classic HTML5-videospeler niet gebruikt, maar in plaats daarvan de native HTML5- `<video>` tag met MP4-video-elementen wilt gebruiken, kunt u het volgende voorbeeld van de ingesloten code gebruiken:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Vervangen `"S7 video thumbnail URL"` door de URL van de miniatuur van de video. Dit is de miniatuurafbeelding van de video die een gebruiker ziet voordat hij of zij de video afspeelt.

   Zie URL&#39;s met videominiaturen [verkrijgen](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Vervangen `"S7 OGG video asset URL (no player)"` door de progressieve URL van de video voor OGG-video.

   Zie Een video-URL [koppelen aan een mobiele site of website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Vervangen `"S7 MP4 mobile progressive video asset URL (no player)"` door de progressieve URL van de video voor mobiele apparaten.

   Zie Een video-URL [koppelen aan een mobiele site of website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Video implementeren met een externe videospeler {#deploying-video-using-a-third-party-video-player}

Als u een videospeler van derden of een aangepaste ingebouwde videospeler in plaats van een Dynamic Media Classic-videoviewer gebruikt, kunt u de directe video-URL verkrijgen die geschikt is voor videostreaming met meerdere bitsnelheden van HLS of progressief downloaden.

**Video implementeren met een externe videospeler**

1. Klik in Dynamic Media Classic op de algemene navigatiebalk op **Instellen** > **Toepassingsinstelling** > **Algemene instellingen**.
1. Voer afhankelijk van het type URL dat u wilt gebruiken een van de volgende taken uit:
* Een directe URL voor HLS-streaming video (multi-bitsnelheid) genereren

   Voor de pagina van de Montages **van de Algemene** Toepassing, in de groep van **Servers** , op het **Gepubliceerde de tekstgebied van de Naam** van de Server, construeert direct URL gebruikend de volgende syntaxis: `server/is/content/company/folder/filename.m3u8`
Stel dat de naam van de gepubliceerde server de syntaxis in stap 2 gebruikt, de directe URL er als volgt uitziet: `https://s7d9.scene7.com/.`
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Een directe URL voor HLS-streaming video (enkele bitsnelheid) genereren

   Constructeer op de pagina Algemene instellingen **van de** toepassing in de groep **Servers** in het tekstveld Naam **van** HLS-streamingserver de directe URL met behulp van de volgende syntaxis:
   `server/company/folder/filename.ext.m3u8`
Stel dat de naam van de HLS-streamingserver `https://s7mbrstream.scene7.com/hls-vod/`is. Met de syntaxis in stap 2 kan de directe URL er als volgt uitzien:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Een direct progressieve video-URL genereren

   Construct u op de pagina Algemene instellingen **van** toepassing in de groep **Servers** in het tekstveld Naam **van** progressieve videoclip de directe eVideo-URL met behulp van de volgende syntaxis: `server/company/folder/filename`
Stel dat de naam van de progressieve videoserver `https://s7d9.scene7.com/is/content/`is. Met de syntaxis in stap 2 kan de directe URL er als volgt uitzien:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Werken met videominiaturen {#working-with-video-thumbnails}

Met Dynamic Media Classic worden miniaturen voor gecodeerde video&#39;s en vooraf gecodeerde video&#39;s gegenereerd. U kunt videominiaturen gebruiken zoals elk afbeeldingselement. Bovendien kunt u URLs voor de videoduimnagels verkrijgen die de Dynamische Klassieke Media deze URLs buiten Dynamische Klassiek van Media produceert en opstelt. U kunt bijvoorbeeld de miniaturen in zoekresultaten, verwante videobestanden en videoafspeellijsten op een website implementeren.

Miniaturen worden gegenereerd op basis van het eerste heterogene frame (niet een volledig zwart frame, of een helemaal wit frame enzovoort) van de video.

### URL&#39;s met videominiaturen ophalen {#obtaining-video-thumbnail-urls}

Dynamic Media Classic genereert automatisch videominiaturen tijdens het uploadproces. De miniaturen worden weergegeven in de lijstweergave en de rasterweergave van het deelvenster Bladeren.

Als u URL&#39;s voor videominiaturen wilt genereren, voert u een publicatiebewerking uit.

Zie Video [](deploying-video-websites-mobile-sites.md#publishing_video)publiceren.

Na publicatie kunt u videominiaturen-URL&#39;s opvragen in de gedetailleerde weergave in de URL&#39;s en het deelvenster Code insluiten. Klik op URL **** kopiëren rechts van de videominiatuur om de URL te kopiëren

### Posterframes wijzigen in videoviewers {#modifying-poster-frames-in-video-viewers}

Het *posterframe* is het eerste frame dat in videoviewers wordt weergegeven voordat de video wordt afgespeeld. Dynamic Media Classic gebruikt videominiaturen als posterframes.

U kunt afbeeldingsaanpassingen toepassen op het posterframe. U kunt bijvoorbeeld het posterframe uitsnijden of transparant maken. Als u het posterframe wilt wijzigen, opent u het configuratiescherm voor de videoviewer en voert u modifiers in de sectie Modifiers voor posterafbeelding in.

Zie Een voorinstelling voor [een videoviewer](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)toevoegen of bewerken.

Zie [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

U kunt videominiaturen ook wijzigen door modifiers toe te voegen aan videominiaturen-URL&#39;s.

>[!MORELIKETHIS]
>
>* [Bestanden publiceren ](publishing-files.md#publishing_files)

