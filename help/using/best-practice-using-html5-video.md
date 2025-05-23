---
title: Aanbevolen procedures voor het gebruik van de HTML5-videoviewer
description: Leer meer over de beste werkwijzen voor het gebruik van de HTML5-videoviewer.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Aanbevolen procedures voor het gebruik van de HTML5-videoviewer{#best-practice-using-the-html-video-viewer}

De Adobe Dynamic Media Classic HTML5 Video Viewer-voorinstellingen zijn robuuste videospelers. Aan de ontwerpkant van de speler, kunt u de volledige functionaliteit van de videospeler tot stand brengen gebruikend de standaardhulpmiddelen van de Ontwikkeling van het Web. U kunt bijvoorbeeld de knoppen, besturingselementen en de achtergrond van een aangepaste posterafbeelding ontwerpen met behulp van HTML5 en CSS om u te helpen uw klanten te bereiken met een aangepaste weergave.

Aan de afspeelzijde van de viewer wordt automatisch de videocapaciteit van de browser gedetecteerd. Vervolgens wordt de video afgespeeld met behulp van HLS (HTTP Live Streaming), ook wel adaptieve videostreaming genoemd. Of als die leveringsmethode niet aanwezig is, wordt in plaats daarvan HTML5 progressief gebruikt.

Door de volgende mogelijkheden te combineren tot één speler:

* Afspeelcomponenten die zijn ontworpen met HTML5 en CSS
* Ingesloten afspelen
* Gebruik van adaptieve en progressieve streaming op basis van de browsermogelijkheden

U vergroot het bereik van uw rijke media-inhoud tot gebruikers op het bureaublad en mobiele apparaten. U zorgt ook voor een gestroomlijnde videobeleving.

Zie ook [Informatie over HTML5-viewers](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) in de Adobe Viewers Reference Guide.

Zie ook [Viewer-voorinstellingen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) trainingsvideo.

## Video afspelen op bureaubladcomputers en mobiele apparaten met de Adobe Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Voor adaptieve videostreaming op het bureaublad en mobiele apparaten zijn de video&#39;s die worden gebruikt voor het schakelen naar een andere bitsnelheid, gebaseerd op alle MP4-video&#39;s in de adaptieve videoset.

Het afspelen van video vindt plaats met behulp van HLS of progressieve video. HLS (HTTP Live Streaming) is een Apple-standaard voor adaptieve videostreaming die het afspelen automatisch aanpast op basis van de capaciteit van de netwerkbandbreedte. Het laat de klant ook &quot;zoeken&quot;aan om het even welk punt in de video zonder de behoefte om op de rest van de video te wachten te downloaden. Zie ook [Live HTTP-streaming](https://developer.apple.com/streaming/). Progressieve video wordt geleverd door de video lokaal te downloaden en op het desktopscherm of mobiele apparaat van de gebruiker op te slaan.

In de volgende tabel worden het apparaat, de browser en de afspeelmethode beschreven van video&#39;s op bureaubladcomputers en mobiele apparaten met de Adobe Dynamic Media Classic Video Viewer.

| Apparaat | Browser | Video-afspeelmodus |
|--- |--- |--- |
| Desktop | Internet Explorer 9 en 10 | Progressieve download. |
| Desktop | Internet Explorer 11+ | HLS-videostreaming. |
| Desktop | Firefox 23-44 | Progressieve download. |
| Desktop | Firefox 45 of hoger | HLS-videostreaming. |
| Desktop | Chroom | HLS-videostreaming. |
| Desktop | Safari (Mac) | HLS-videostreaming. |
| Mobiel | Chrome (Android™ 6 of eerder) | Progressieve download. |
| Mobiel | Chrome (Android™ 7 of hoger) | HLS-videostreaming. |
| Mobiel | Android™ (standaardbrowser) | Progressieve download. |
| Mobiel | Safari (iOS) | HLS-videostreaming. |
| Mobiel | Chrome (iOS) | HLS-videostreaming. |
| Mobiel | BlackBerry® | HLS-videostreaming. |
