---
title: "Snel starten: Video in Adobe Dynamic Media Classic"
description: Een inleiding en Snel aan de Video van Adobe Dynamic Media Classic beginnen om u te helpen snel aan de slag gaan.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# Snel starten: Video in Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video is een end-to-end oplossing waarmee u eenvoudig Adaptieve video van hoge kwaliteit kunt publiceren voor streaming op meerdere schermen, zoals desktopcomputers, iOS, Android™, BlackBerry® en mobiele apparaten van Windows®. Een adaptieve videoreeks groepeert versies van de zelfde video die bij verschillende beetjetarieven en formaten zoals 400 kbps, 800 kbps, en 1000 kbps worden gecodeerd. De desktopcomputer of het mobiele apparaat detecteert de beschikbare bandbreedte.

Op een mobiel iOS-apparaat wordt bijvoorbeeld een bandbreedte gedetecteerd, zoals 3G, 4G of Wi-Fi. Vervolgens wordt automatisch de naar rechts gecodeerde video geselecteerd bij de verschillende bitsnelheden van de video in de adaptieve videoset. De video wordt gestreamd naar desktops, mobiele apparaten of tablets.

Bovendien wordt de videokwaliteit automatisch dynamisch geschakeld als de netwerkomstandigheden veranderen op het bureaublad of op het mobiele apparaat. Als een klant de modus Volledig scherm op een desktopcomputer inschakelt, reageert de Adaptive Video Set met een betere resolutie, waardoor de kijkervaring van de klant wordt verbeterd. Met Adaptieve videosets kunt u het best afspelen. Dit is het meest geschikt voor klanten die Adobe Dynamic Media Classic Video op meerdere schermen en apparaten afspelen.

De logica die een videospeler gebruikt om te bepalen welke gecodeerde video moet worden afgespeeld of tijdens het afspelen moet worden geselecteerd, is gebaseerd op het volgende algoritme:

1. De videospeler laadt het eerste videofragment op basis van de bitsnelheid die het dichtst bij de waarde ligt die voor de beginbitsnelheid is ingesteld in de speler zelf.
1. De videospelerschakelaars die op veranderingen in de bandbreedtesnelheid worden gebaseerd die de volgende criteria gebruiken:

   1. De speler kiest de hoogste bandbreedtestroom onder of gelijk aan de geschatte bandbreedte.
   1. De speler overweegt slechts 80% van de beschikbare bandbreedte. Als er echter een overstap wordt gemaakt, is het conservatiever bij slechts 70% om overschatting te voorkomen en onmiddellijk terug te keren.

Zie de logica van het algoritme op [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) voor technische informatie hierover.

Adobe Dynamic Media Classic ondersteunt het volgende voor het beheer van afzonderlijke video&#39;s en Adaptieve videosets:

* Video uploaden vanaf een groot aantal ondersteunde video-indelingen. En het uploaden van audio-indelingen en het coderen van video naar MP4 H.264 formaat voor playback over veelvoudige schermen. U kunt vooraf gedefinieerde Adobe Dynamic Media Classic Adaptive Video-voorinstellingen, voorinstellingen voor één videocodering gebruiken of uw eigen codering aanpassen om de kwaliteit en de grootte van de video te bepalen.

Zie [Aangepaste videovoorinstellingen activeren of deactiveren](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Zie ook [Videovoorinstellingen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) trainingsvideo.

Wanneer een adaptieve videoset wordt gegenereerd, bevat deze MP4-video&#39;s.

>[!NOTE]
>
>Primaire video&#39;s/bronvideo&#39;s en andere bronvideo zijn *niet* toegevoegd aan een adaptieve videoset.

* Video ondertiteling in de de kijkers van Univeral_HTML5_Video, Universal_HTML5_MixedMedia_donker, en Universal_HTML5_MixedMedia_light en videohoofdstuknavigatie in Univeral_HTML5_Video, Universal_HTML5_MixedMedia_donker, en Universal_HTML5_MixedMedia_light.

  Zie [Bijschriften toevoegen aan een video](adding-captions-video.md).

  Zie [Hoofdstukmarkeringen aan een video toevoegen](adding-chapter-markers-video.md).

* Video organiseren, doorbladeren en doorzoeken met volledige metagegevensondersteuning voor een efficiënt beheer van video-elementen.
* Lever Adaptieve videosets naar het web en naar desktops en mobiele apparaten, zoals de iPhone, iPad, Android™, BlackBerry® en Windows®-telefoon.

  Adaptieve videostreaming wordt ondersteund op verschillende iOS-platforms.

  Zie de nieuwste ondersteuning in de [Referentiehandleiding voor Adobe Viewers](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic ondersteunt het afspelen van mobiele video voor MP4 H.264-video. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  U kunt Windows®-apparaten die deze video-indeling ondersteunen als volgt vinden:

  [Ondersteunde video-indelingen op Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* De video afspelen met gebruik van voorinstellingen voor Adobe Dynamic Media Classic Viewer, waaronder de volgende:

   * Enkele videoviewers.
   * Gemengde Media-viewers die zowel video- als afbeeldingsinhoud combineren.

* Configureer videospelers om aan uw brandingbehoeften te voldoen.
* Integreer video op uw website, mobiele site of mobiele toepassing met een eenvoudige URL of Embed Code.

Bekijk de volgende trainingsvideo&#39;s:
* [Overzicht van MP4-video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4-videovoorvertoning](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4-video uploaden](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Overzicht van streaming](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Snel starten**

De volgende stapsgewijze beschrijving van de workflow is ontworpen om u te helpen snel aan de slag te gaan met Adaptive Video Sets in Adobe Dynamic Media Classic. Na elke stap, is er een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

## 1. Video&#39;s uploaden en coderen

U kunt adaptieve videosets uploaden en genereren aan de hand van een van de volgende twee scenario&#39;s:

* **Vooraf gecodeerde video&#39;s uploaden**: Als uw video&#39;s al extern zijn gecodeerd vanuit Adobe Dynamic Media Classic, selecteert u op de algemene navigatiebalk de optie **[!UICONTROL Upload]**. Blader naar en upload MP4-videobestanden rechtstreeks naar Adobe Dynamic Media Classic. Ga vervolgens naar **[!UICONTROL Build]** > **[!UICONTROL Adaptive Video Sets]**. Blader naar uw videobestanden. Sleep de gewenste videobestanden naar de tabel Adaptive Video Set en sla deze op.
* **Primaire bronvideo&#39;s uploaden**: Als uw video&#39;s niet zijn gecodeerd, selecteert u op de algemene navigatiebalk de optie **[!UICONTROL Upload]** primaire videobronbestanden (niet-MP4) uploaden. Adobe Dynamic Media Classic codeert ze voor u naar MP4-bestanden. In de **[!UICONTROL Upload Job Options]** dialoogvenster, onder **[!UICONTROL EVideo Options]**, selecteert u **[!UICONTROL Adaptive Video]**.

  Met deze voorkeursoptie kunt u Adaptieve videosets maken. De juiste coderingsvoorinstelling wordt automatisch toegepast op de video, ongeacht of dit 16:9 of 4:3 is, om de afmetingen te laten overeenkomen van de video die u hebt geüpload. Wanneer u de uploadtaak verzendt, wordt automatisch een adaptieve videoset gemaakt die drie coderingsvideo-instellingen in de juiste hoogte-breedteverhouding bevat.

  Of in dezelfde **[!UICONTROL Job Options]** dialoogvenster, onder **[!UICONTROL EVideo Options]**, uitbreiden **[!UICONTROL Single Encoding Presets]**. Selecteer de gewenste voorinstellingen voor videocodering. U kunt **Desktop**, **Mobiel (iPhone, iPad, Android™)**, en **Tablet (iPad, Android™)** om de MP4-bestanden te maken.

* Of u kunt een primaire video opnieuw verwerken met de opdracht **[!UICONTROL Reprocessing]** gebruiken. De zojuist gecodeerde video&#39;s worden toegevoegd aan de bestaande adaptieve videoset.

Zie [Video&#39;s uploaden en coderen](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optioneel**

Adobe Dynamic Media Classic beschikt over een groot aantal vooraf gedefinieerde voorinstellingen voor videocodering. Deze vooraf gedefinieerde voorinstellingen weerspiegelen de meest gangbare instellingen voor videocodering die vandaag worden gebruikt en zijn geoptimaliseerd voor afspelen op doelpagina&#39;s.

Als verdere aanpassingen nodig zijn, kunnen beheerders echter videovoorinstellingen maken om de grootte en de afspeelervaring van Video&#39;s aan de eindgebruikers aan te passen. Beheerders kunnen videovoorinstellingen toevoegen en beheren via de pagina Voorinstellingen video die onder **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Single Encoding Presets]**. De pagina Voorinstellingen video biedt opties voor het toevoegen, bewerken, verwijderen en activeren van videovoorinstellingen.

Zie [Werken met voorinstellingen voor videocodering](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Video&#39;s voorvertonen in een videoviewer

Als u wilt zien hoe een video wordt afgespeeld voor eindgebruikers op een bureaublad, uw website of een mobiel apparaat, selecteert u de video in het deelvenster Bladeren. Selecteer vervolgens **[!UICONTROL Preview]**.

Zie [Video&#39;s voorvertonen in een videoviewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

U kunt de video afspelen op de pagina Voorvertoning. U kunt ook verschillende videoviewers kiezen om te zien hoe uw video er in verschillende spelers uitziet. U kunt de HTML5-videospeler het beste gebruiken voor weergave op meerdere schermen op een desktopcomputer, tablet of mobiel apparaat.

**Optioneel**

Aanpassing voorinstelling viewer: Adobe Dynamic Media Classic biedt vooraf gedefinieerde viewervoorinstellingen voor het afleveren van video. Deze voorinstellingen bepalen de vormgeving van de viewer en de werking van de afspeelbesturingselementen. Beheerders kunnen voorinstellingen voor viewers toevoegen en beheren via de pagina Voorinstellingen voor viewer om de videoviewer aan te passen. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. De pagina Voorinstellingen viewer bevat opdrachten voor het toevoegen, bewerken, verwijderen en activeren van voorinstellingen van viewers.

Zie [Werken met voorinstellingen voor video-viewers](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Zie ook [Videovoorinstellingen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) trainingsvideo.

## 3. Video&#39;s distribueren naar uw websites en mobiele sites

Als u video wilt integreren in uw website, kunt u een van de volgende handelingen uitvoeren:

* Geef de video weer in een eigen pop-upvenster of in een modaal venster. Gebruik in dat geval de opdracht **[!UICONTROL Copy URL]** gebruiken.

  Als u de URL voor een video wilt opvragen, selecteert u deze in de rasterweergave of de lijstweergave in het deelvenster Bladeren. Selecteren **[!UICONTROL Preview]** en selecteer vervolgens **[!UICONTROL Copy URL]** aan het recht van `Universal_HTML5_Viewer`.

  Wanneer u **[!UICONTROL Copy URL]**, wordt de URL naar het klembord gekopieerd. Plaats deze code in de HTML van uw website, mobiele site of toepassing.

  >[!NOTE]
  >
  >URL&#39;s worden pas geactiveerd nadat u de video of de adaptieve videoset hebt gepubliceerd.

* Geef de video weer die is ingesloten op de webpagina, in welk geval de optie **[!UICONTROL Embed Code]** gebruiken.

  Als u de insluitcode voor een video wilt verkrijgen, selecteert u de video in het deelvenster Bladeren in de rasterweergave of de lijstweergave. Ga naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**. Selecteer onder de kolom Acties van de tabel de optie **[!UICONTROL Embed Code]** aan het recht van `Universal_HTML5_Video`. Het bewerken van de code is niet toegestaan.

  Selecteren **[!UICONTROL Close]** en plak de insluitcode in een of meer van uw webpagina&#39;s.

  >[!NOTE]
  >
  >De insluitcode wordt alleen geactiveerd nadat u de video of de adaptieve videoset hebt gepubliceerd.

Zie [Video distribueren naar uw websites en mobiele sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Aanbevolen procedures voor videocodering](uploading-encoding-videos.md#best_practices_for_video_encoding)
