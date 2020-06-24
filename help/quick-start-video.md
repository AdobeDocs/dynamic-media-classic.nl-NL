---
title: '"Snel starten: Video"'
seo-title: '"Snel starten: Video"'
description: 'null'
seo-description: Een inleiding en Snel aan Video beginnen om u te helpen snel aan de slag gaan.
uuid: bf0ecf87-a1f2-4e83-8041-df5192dd26a1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6cef541b-e9df-48eb-9a16-ca3e1f07238e
translation-type: tm+mt
source-git-commit: 74238f90f45f0fb9a4566915a20a1d41dfb69fe1
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 0%

---


# Snel starten: Video{#quick-start-video}

Adobe Dynamic Media Classic Video is een end-to-end oplossing waarmee u eenvoudig Adaptieve video van hoge kwaliteit kunt publiceren voor streaming op meerdere schermen, waaronder desktopcomputers, iOS, Android, Blackberry en mobiele Windows-apparaten. Een adaptieve videoreeks groepeert versies van de zelfde video die bij verschillende beetjetarieven en formaten zoals 400 kbps, 800 kbps, en 1000 kbps worden gecodeerd. De desktopcomputer of het mobiele apparaat detecteert de beschikbare bandbreedte.

Op een mobiel iOS-apparaat detecteert het bijvoorbeeld een bandbreedte zoals 3G, 4G of Wi-Fi. Vervolgens wordt automatisch de naar rechts gecodeerde video geselecteerd bij de verschillende bitsnelheden van de video in de adaptieve videoset. De video wordt gestreamd naar desktops, mobiele apparaten of tablets.

Bovendien wordt de videokwaliteit automatisch dynamisch geschakeld als de netwerkomstandigheden veranderen op het bureaublad of op het mobiele apparaat. Ook, als een klant volledig-schermwijze op een Desktop ingaat, antwoordt de Adaptieve VideoReeks door een betere resolutie te gebruiken, daardoor verbeterend de het bekijken van de klant ervaring. Het gebruik van Adaptieve videosets biedt u de best mogelijke weergave voor klanten die Dynamic Media Klassieke video op meerdere schermen en apparaten afspelen.

De logica die een videospeler gebruikt om te bepalen welke gecodeerde video moet worden afgespeeld of tijdens het afspelen moet worden geselecteerd, is gebaseerd op het volgende algoritme:

1. Videospeler laadt het eerste videofragment op basis van de bitsnelheid die het dichtst bij de waarde ligt die is ingesteld voor de &#39;initiële bitsnelheid&#39; in de speler zelf.
1. De videospelerschakelaars die op veranderingen in de bandbreedtesnelheid worden gebaseerd die de volgende criteria gebruiken:

   1. De speler kiest de hoogste bandbreedtestroom onder of gelijk aan de geschatte bandbreedte.
   1. De speler overweegt slechts 80% van de beschikbare bandbreedte. Nochtans, als het overschakelt, is het gespreksverrijker bij slechts 70% om te vermijden overschatend en het moeten onmiddellijk terugschakelen.

Zie de logica van het algoritme op [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) voor technische informatie over het.

Voor het beheren van enige video en Adaptieve videosets biedt Dynamic Media Classic ondersteuning voor het volgende:

* Video uploaden van diverse ondersteunde video-indelingen en audio-indelingen en video coderen naar MP4 H.264-indeling, zodat deze op meerdere schermen kan worden afgespeeld. U kunt vooraf gedefinieerde Dynamic Media gebruiken Klassieke aangepaste videovoorinstellingen, voorinstellingen voor één videocodering of uw eigen codering aanpassen om de kwaliteit en de grootte van de video te bepalen.

   Wanneer een adaptieve videoset wordt gegenereerd, bevat deze MP4-video&#39;s.

   `**Note:**` Stramien-/bronvideo&#39;s en andere bronopmaakvideo worden *niet* toegevoegd aan een adaptieve videoset.

* Video-ondertiteling in de viewers Univeral_HTML5_Video, Universal_HTML5_MixedMedia_donker en Universal_HTML5_MixedMedia_light en de navigatie in videohoofdstukken in de viewers Univeral_HTML5_Video, Universal_HTML5_MixedMedia_donker en Universal_HTML5_MixedMedia_light.

   Zie Bijschriften [toevoegen aan video](adding-captions-video.md).

   Zie Hoofdstukmarkeringen [toevoegen aan video](adding-chapter-markers-video.md).

* Video organiseren, doorbladeren en doorzoeken met volledige metagegevensondersteuning voor een efficiënt beheer van video-elementen.
* Lever Adaptieve videosets naar het web, naar desktops en mobiele apparaten, waaronder de iPhone, iPad, Android™, Blackberry en Windows-telefoon.

   Adaptieve videostreaming wordt ondersteund op verschillende iOS-platforms.

   Raadpleeg de nieuwste ondersteuning in de naslaggids voor [Adobe Viewers](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/home.html).

   Dynamic Media Classic ondersteunt het afspelen van mobiele video voor MP4 H.264-video. U vindt Blackberry-apparaten die deze video-indeling ondersteunen op de volgende website:

   Zie [Ondersteunde video-indelingen op Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   U kunt de apparaten van Vensters vinden die dit videoformaat bij het volgende steunen:

   Zie [Ondersteunde video-indelingen op Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Speel de video terug gebruikend Dynamic Media Klassieke Kijker vooraf instelt, met inbegrip van het volgende:

   * Afzonderlijke videoviewers.
   * Gemengde Media-viewers die zowel video- als afbeeldingsinhoud combineren.

* Configureer videospelers om aan uw brandingbehoeften te voldoen.
* Video met een eenvoudige URL of insluitcode integreren in uw website, mobiele site of mobiele toepassing.

**Snel starten**

De volgende stapsgewijze workflowbeschrijving is ontworpen om u te helpen snel aan de slag te gaan met adaptieve videosets in Dynamic Media Classic. Na elke stap is een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

**1. Video&#39;s uploaden en coderen**

U kunt adaptieve videosets uploaden en genereren aan de hand van een van de volgende twee scenario&#39;s:

* **Upload vooraf gecodeerde video** Als uw video&#39;s reeds buiten Dynamic Media Classic werden gecodeerd, klik **Upload** op de Globale bar van de Navigatie om MP4 videodossiers direct aan het het Publiceren Scene7 Systeem te doorbladeren en te uploaden. Klik vervolgens op **Samenstellen > Adaptieve videosets**. Blader naar uw videobestanden. Sleep de gewenste videobestanden naar de tabel Adaptive Video Set en sla deze op.
* **Upload hoofdbronvideo** Als uw video&#39;s niet worden gecodeerd, klik **Upload** op de Globale bar van de Navigatie om hoofdvideobrondossiers (niet-MP4) te uploaden en Scene7 het Publiceren Systeem te hebben codeert hen aan MP4 dossiers voor u. Selecteer **Adaptieve video** onder Opties voor video uploaden.

   Met deze voorkeursoptie kunt u een adaptieve videoset maken die automatisch de juiste coderingsvoorinstelling op de video toepast, ongeacht of deze 16:9 of 4:3 is, zodat deze overeenkomt met de afmetingen van de video die u hebt geüpload. Wanneer u de uploadtaak verzendt, wordt automatisch een adaptieve videoset gemaakt die drie videocoderingen in de juiste hoogte-breedteverhouding bevat.

   Of vouw in hetzelfde dialoogvenster Taakopties onder Opties voor EVideo de voorinstellingen **voor** Single Encoding uit en selecteer de gewenste voorinstellingen voor videocodering op het **bureaublad**, **Mobiel (iPhone, iPad, Android)** en **Tablet (iPad, Android)** , zodat u de MP4-bestanden maakt.

* U kunt een hoofdvideo ook opnieuw verwerken met de functie Opnieuw verwerken. De zojuist gecodeerde video&#39;s worden toegevoegd aan de bestaande adaptieve videoset.

Zie Video&#39;s [uploaden en coderen](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optioneel**

Dynamic Media Classic biedt een groot aantal vooraf gedefinieerde voorinstellingen voor videocodering. Deze vooraf gedefinieerde voorinstellingen weerspiegelen de meest gangbare instellingen voor videocodering die vandaag worden gebruikt en zijn geoptimaliseerd voor afspelen op doelschermen.

Als verdere aanpassingen nodig zijn, kunnen beheerders echter videovoorinstellingen maken om de grootte en de afspeelervaring van Video&#39;s aan de eindgebruikers aan te passen. Beheerders kunnen voorinstellingen voor video toevoegen en beheren op de pagina Voorinstellingen video die beschikbaar is onder Instellen > Toepassing > Voorinstellingen video > Voorinstellingen voor één codering. De pagina Voorinstellingen video biedt opties voor het toevoegen, bewerken, verwijderen en activeren van videovoorinstellingen.

Zie [Werken met voorinstellingen](uploading-encoding-videos.md#working_with_video_encoding_presets)voor videocodering.

**2. Video&#39;s voorvertonen in een videoviewer**

Als u wilt zien hoe een video wordt afgespeeld voor eindgebruikers op een bureaublad, uw website of een mobiel apparaat, selecteert u de video in het deelvenster Bladeren en klikt u op **Voorvertoning**.

Zie Video&#39;s [voorvertonen in een videoviewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

U kunt de video afspelen op het voorvertoningsscherm. U kunt ook verschillende videoviewers kiezen om te zien hoe uw video er in verschillende spelers uitziet. U kunt de HTML5-videospeler het beste gebruiken voor weergave op meerdere schermen op computers, tablets en mobiele apparaten.

**Optioneel**

Aanpassing voorinstelling viewer - Dynamic Media Klassiek biedt vooraf gedefinieerde Viewer-voorinstellingen voor het afleveren van video. Deze voorinstellingen bepalen de vormgeving van de viewer en de werking van de afspeelbesturingselementen. Beheerders kunnen voorinstellingen voor viewers toevoegen en beheren via de pagina Voorinstellingen voor viewer om de videoviewer aan te passen. Om deze pagina, in de hoger-juiste hoek van het het Publiceren Scene7 Systeem te openen, klik Opstelling > de Voorinstellingen van de Kijker. De pagina Voorinstellingen viewer bevat opdrachten voor het toevoegen, bewerken, verwijderen en activeren van voorinstellingen van viewers.

Zie [Werken met voorinstellingen](previewing-videos-video-viewer.md#working_with_video_viewer_presets)voor videoviewers.

**3. Video&#39;s gebruiken voor uw websites en mobiele sites**

Als u video wilt integreren in uw website, kunt u een van de volgende handelingen uitvoeren:

* Geef de video weer in een eigen pop-upvenster of in een modaal venster. In dat geval moet u de functie URL kopiëren gebruiken.

   Als u de URL voor een video wilt opvragen, selecteert u deze in de rasterweergave of lijstweergave in het deelvenster Bladeren. Klik op Voorvertoning en klik vervolgens op URL kopiëren rechts van `Universal_HTML5_Viewer`.

   Wanneer u op URL kopiëren klikt, wordt de URL naar het klembord gekopieerd. Plaats deze code in de HTML van uw website, mobiele site of toepassing.

   >[!NOTE]
   >
   >URL&#39;s worden alleen geactiveerd nadat u de video of de adaptieve videoset hebt gepubliceerd.

* Geef de video weer die is ingesloten op de webpagina. Gebruik in dat geval de functie Code insluiten.

   Als u de insluitcode voor een video wilt verkrijgen, selecteert u de video in het deelvenster Bladeren in de rasterweergave of de lijstweergave. Klik op Voorvertoning > Viewer List. Klik in de kolom Acties van de tabel op Code insluiten rechts van `Universal_HTML5_Video`. Het bewerken van de code is niet toegestaan.

   Klik op Sluiten en plak de insluitcode in uw webpagina&#39;s.

   >[!NOTE]
   >
   >Insluitcode wordt alleen geactiveerd nadat u de video of adaptieve videoset hebt gepubliceerd.

Zie Video [distribueren naar uw websites en mobiele sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Aanbevolen procedures voor videocodering](uploading-encoding-videos.md#best_practices_for_video_encoding)

