---
title: '"Snel starten: Video"'
description: Een inleiding en Snel aan de Adobe van de Klassieke Video van Dynamic Media om u te helpen snel aan de slag gaan.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Klassiek,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# Snel starten: Video{#quick-start-video}

Adobe Dynamic Media Classic Video is een end-to-end oplossing waarmee u eenvoudig Adaptieve video van hoge kwaliteit kunt publiceren voor streaming op meerdere schermen, waaronder mobiele apparaten voor desktops, iOS, Android™, BlackBerry® en Windows®. Een adaptieve videoreeks groepeert versies van de zelfde video die bij verschillende beetjetarieven en formaten zoals 400 kbps, 800 kbps, en 1000 kbps worden gecodeerd. De desktopcomputer of het mobiele apparaat detecteert de beschikbare bandbreedte.

Op een mobiel iOS-apparaat detecteert het bijvoorbeeld een bandbreedte zoals 3G, 4G of Wi-Fi. Vervolgens wordt automatisch de naar rechts gecodeerde video geselecteerd bij de verschillende bitsnelheden van de video in de adaptieve videoset. De video wordt gestreamd naar desktops, mobiele apparaten of tablets.

Bovendien wordt de videokwaliteit automatisch dynamisch geschakeld als de netwerkomstandigheden veranderen op het bureaublad of op het mobiele apparaat. Ook, als een klant volledig-schermwijze op een Desktop ingaat, antwoordt de Adaptieve VideoReeks door een betere resolutie te gebruiken, verbeterend de het bekijken van de klant ervaring. Met Adaptieve videosets kunt u de best mogelijke weergave bieden voor klanten die Dynamic Media Classic-video op meerdere schermen en apparaten afspelen.

De logica die een videospeler gebruikt om te bepalen welke gecodeerde video moet worden afgespeeld of tijdens het afspelen moet worden geselecteerd, is gebaseerd op het volgende algoritme:

1. Videospeler laadt het eerste videofragment op basis van de bitsnelheid die het dichtst bij de waarde ligt die is ingesteld voor de &#39;initiële bitsnelheid&#39; in de speler zelf.
1. De videospelerschakelaars die op veranderingen in de bandbreedtesnelheid worden gebaseerd die de volgende criteria gebruiken:

   1. De speler kiest de hoogste bandbreedtestroom onder of gelijk aan de geschatte bandbreedte.
   1. De speler overweegt slechts 80% van de beschikbare bandbreedte. Als het echter overschakelt, is het conservatiever bij slechts 70% om overschatting te voorkomen en onmiddellijk terug te moeten schakelen.

Zie de logica van het algoritme op [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) voor technische informatie over het.

Dynamic Media Classic ondersteunt het volgende voor het beheer van afzonderlijke video- en adaptieve videosets:

* Video uploaden van diverse ondersteunde video-indelingen en audio-indelingen en video coderen naar MP4 H.264-indeling, zodat deze op meerdere schermen kan worden afgespeeld. U kunt vooraf gedefinieerde Dynamic Media Classic adaptieve videovoorinstellingen, voorinstellingen voor één videocodering gebruiken of uw eigen codering aanpassen om de kwaliteit en de grootte van de video te bepalen.

   Wanneer een adaptieve videoset wordt gegenereerd, bevat deze MP4-video&#39;s.

   >[!NOTE]
   >
   >Master/bronvideo&#39;s en andere bronopmaakvideo worden *niet* toegevoegd aan een adaptieve videoset.

* Video-ondertiteling in de viewers Univeral_HTML5_Video, Universal_HTML5_MixedMedia_donker en Universal_HTML5_MixedMedia_light en de navigatie in videohoofdstukken in de viewers Univeral_HTML5_Video, Universal_HTML5_MixedMedia_donker en Universal_HTML5_MixedMedia_light.

   Zie [Bijschriften toevoegen aan video](adding-captions-video.md).

   Zie [Hoofdstukmarkeringen toevoegen aan video](adding-chapter-markers-video.md).

* Video organiseren, doorbladeren en doorzoeken met volledige metagegevensondersteuning voor een efficiënt beheer van video-elementen.
* Lever Adaptieve videosets naar het web en naar desktops en mobiele apparaten, waaronder de iPhone, iPad, Android™, BlackBerry® en Windows®-telefoon.

   Adaptieve videostreaming wordt ondersteund op verschillende iOS-platforms.

   Zie de nieuwste ondersteuning in de [Referentiehandleiding voor Adobe-viewers](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Dynamic Media Classic ondersteunt het afspelen van mobiele video voor MP4 H.264-video. U kunt op de volgende website naar BlackBerry®-apparaten zoeken die deze video-indeling ondersteunen:

   Zie [Ondersteunde video-indelingen op BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   U kunt Windows®-apparaten die deze video-indeling ondersteunen als volgt vinden:

   Zie [Ondersteunde video-indelingen op Windows® Phone](https://docs.microsoft.com/en-us/).

* Speel de video af met gebruik van Dynamic Media Classic Viewer Presets, waaronder de volgende:

   * Afzonderlijke videoviewers.
   * Gemengde Media-viewers die zowel video- als afbeeldingsinhoud combineren.

* Configureer videospelers om aan uw brandingbehoeften te voldoen.
* Video met een eenvoudige URL of insluitcode integreren in uw website, mobiele site of mobiele toepassing.

**Snel starten**

De volgende stapsgewijze workflowbeschrijving is ontworpen om u te helpen snel aan de slag te gaan met adaptieve videosets in Dynamic Media Classic. Na elke stap is een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

## 1. Video&#39;s uploaden en coderen

U kunt adaptieve videosets uploaden en genereren aan de hand van een van de volgende twee scenario&#39;s:

* **Vooraf gecodeerde video**  uploaden - Als uw video&#39;s al buiten Dynamic Media Classic zijn gecodeerd, klikt u op de algemene navigatiebalk  **[!UICONTROL Upload]** om naar MP4-videobestanden te bladeren en deze rechtstreeks te uploaden naar Dynamic Media Classic. Klik vervolgens op **[!UICONTROL Build]** > **[!UICONTROL Adaptive Video Sets]**. Blader naar uw videobestanden. Sleep de gewenste videobestanden naar de tabel Adaptive Video Set en sla deze op.
* **Master bronvideo**  uploaden - Als uw video&#39;s niet zijn gecodeerd, klikt u op de algemene navigatiebalk  **[!UICONTROL Upload]** om master videobronbestanden (niet-MP4) te uploaden en laat u deze via Dynamic Media Classic coderen naar MP4-bestanden. Selecteer **[!UICONTROL Adaptive Video]** onder **[!UICONTROL EVideo Options]** in het dialoogvenster **[!UICONTROL Upload Job Options]**.

   Met deze voorkeursoptie kunt u een adaptieve videoset maken die automatisch de juiste coderingsvoorinstelling op de video toepast, ongeacht of deze 16:9 of 4:3 is, zodat deze overeenkomt met de afmetingen van de video die u hebt geüpload. Wanneer u de uploadtaak verzendt, wordt automatisch een adaptieve videoset gemaakt die drie videocoderingen in de juiste hoogte-breedteverhouding bevat.

   Of vouw **[!UICONTROL Single Encoding Presets]** in hetzelfde **[!UICONTROL Job Options]** dialoogvenster onder **[!UICONTROL EVideo Options]** uit. Selecteer de afzonderlijke voorinstellingen voor videocodering die u wilt instellen op **Desktop**, **Mobiel (iPhone, iPad, Android™)** en **Tablet (iPad, Android™)**, zodat u de MP4-bestanden maakt.

* Of u kunt een master video opnieuw verwerken met de functie **[!UICONTROL Reprocess]**. De zojuist gecodeerde video&#39;s worden toegevoegd aan de bestaande adaptieve videoset.

Zie [Video&#39;s uploaden en coderen](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optioneel**

Dynamic Media Classic bevat een groot aantal vooraf gedefinieerde voorinstellingen voor videocodering. Deze vooraf gedefinieerde voorinstellingen weerspiegelen de meest gangbare instellingen voor videocodering die vandaag worden gebruikt en zijn geoptimaliseerd voor afspelen op doelpagina&#39;s.

Als verdere aanpassingen nodig zijn, kunnen beheerders echter videovoorinstellingen maken om de grootte en de afspeelervaring van Video&#39;s aan de eindgebruikers aan te passen. Beheerders kunnen videovoorinstellingen toevoegen en beheren via de pagina Voorinstellingen video die beschikbaar is onder **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Single Encoding Presets]**. De pagina Voorinstellingen video biedt opties voor het toevoegen, bewerken, verwijderen en activeren van videovoorinstellingen.

Zie [Werken met voorinstellingen voor videocodering](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Video&#39;s voorvertonen in een videoviewer

Als u wilt zien hoe een video wordt afgespeeld voor eindgebruikers op een desktopcomputer, uw website of een mobiel apparaat, selecteert u de video in het deelvenster Bladeren en klikt u op **[!UICONTROL Preview]**.

Zie [Video&#39;s voorvertonen in een videoviewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

U kunt de video afspelen op de voorvertoningspagina. U kunt ook verschillende videoviewers kiezen om te zien hoe uw video er in verschillende spelers uitziet. U kunt de HTML5-videospeler het beste gebruiken voor weergave op meerdere schermen op computers, tablets en mobiele apparaten.

**Optioneel**

Aanpassing van voorinstellingen viewer - Dynamic Media Classic biedt vooraf gedefinieerde voorinstellingen voor viewers voor het afleveren van video. Deze voorinstellingen bepalen de vormgeving van de viewer en de werking van de afspeelbesturingselementen. Beheerders kunnen voorinstellingen voor viewers toevoegen en beheren via de pagina Voorinstellingen voor viewer om de videoviewer aan te passen. Als u deze pagina wilt openen, klikt u in de rechterbovenhoek van Dynamic Media Classic op **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. De pagina Voorinstellingen viewer bevat opdrachten voor het toevoegen, bewerken, verwijderen en activeren van voorinstellingen van viewers.

Zie [Werken met voorinstellingen voor videoviewers](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

## 3. Video&#39;s gebruiken voor uw websites en mobiele sites

Als u video wilt integreren in uw website, kunt u een van de volgende handelingen uitvoeren:

* Geef de video weer in een eigen pop-upvenster of in een modaal venster. In dat geval gebruikt u de functie **[!UICONTROL Copy URL]**.

   Als u de URL voor een video wilt opvragen, selecteert u deze in de rasterweergave of lijstweergave in het deelvenster Bladeren. Klik **[!UICONTROL Preview]**, en klik dan **[!UICONTROL Copy URL]** rechts van `Universal_HTML5_Viewer`.

   Wanneer u **[!UICONTROL Copy URL]** klikt, wordt URL gekopieerd aan het Klembord. Plaats deze code in de HTML van uw website, mobiele site of toepassing.

   >[!NOTE]
   >
   >URL&#39;s worden alleen geactiveerd nadat u de video of de adaptieve videoset hebt gepubliceerd.

* Geef de video weer die is ingesloten op de webpagina, in welk geval de functie **[!UICONTROL Embed Code]** wordt gebruikt.

   Als u de insluitcode voor een video wilt verkrijgen, selecteert u de video in het deelvenster Bladeren in de rasterweergave of de lijstweergave. Klik op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**. Klik in de kolom Acties van de tabel op **[!UICONTROL Embed Code]** rechts van `Universal_HTML5_Video`. Het bewerken van de code is niet toegestaan.

   Klik op **[!UICONTROL Close]** en plak de insluitcode in uw webpagina&#39;s.

   >[!NOTE]
   >
   >Insluitcode wordt alleen geactiveerd nadat u de video of adaptieve videoset hebt gepubliceerd.

Zie [Video distribueren naar uw websites en mobiele sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Aanbevolen procedures voor videocodering](uploading-encoding-videos.md#best_practices_for_video_encoding)

