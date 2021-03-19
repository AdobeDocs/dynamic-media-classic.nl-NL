---
title: Aanbevolen procedures voor het gebruik van de HTML5-videoviewer
description: Leer meer over de beste werkwijzen voor het gebruik van de HTML5-videoviewer.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Klassiek,Viewers,Video
role: Zakelijke praktiserer
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# Aanbevolen procedures voor het gebruik van de HTML5 Video-viewer{#best-practice-using-the-html-video-viewer}

De Dynamic Media Classic HTML5 Video viewer-voorinstellingen zijn robuuste videospelers. Aan de ontwerpkant van de speler, kunt u alle functionaliteit van de videospeler tot stand brengen gebruikend standaardhulpmiddelen van de Webontwikkeling. U kunt bijvoorbeeld de knoppen, besturingselementen en de achtergrond van een aangepaste posterafbeelding ontwerpen met HTML5 en CSS, zodat u uw klanten kunt bereiken met een aangepaste weergave.

Aan de afspeelzijde van de viewer wordt automatisch de videocapaciteit van de browser gedetecteerd. Vervolgens wordt de video afgespeeld met HLS (adaptieve videostreaming). Als deze leveringsmethode niet aanwezig is, wordt in plaats daarvan HTML5 progressief gebruikt.

Door de combinatie in één speler van de capaciteit om de playbackcomponenten te ontwerpen gebruikend HTML5 en CSS, ingebedde playback te hebben, en adaptieve en progressieve het stromen te gebruiken afhankelijk van het vermogen van browser, breidt u het bereik van uw rijke media inhoud tot zowel Desktop als mobiele gebruikers uit en verzekert een gestroomlijnde videoervaring.

Zie ook [Informatie over HTML5 Viewers](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) in de Gids van de Verwijzing van de Kijkers van de Adobe.

## Video afspelen op desktopcomputers en mobiele apparaten met de Klassieke Dynamic Media Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Voor adaptieve videostreaming op het bureaublad en mobiele apparaten zijn de video&#39;s die worden gebruikt voor het schakelen naar een andere bitsnelheid, gebaseerd op alle MP4-video&#39;s in de adaptieve videoset.

Het afspelen van video vindt plaats met behulp van HLS of progressieve video. HLS (HTTP Live Streaming) is een Apple-standaard voor adaptieve videostreaming die het afspelen automatisch aanpast op basis van de capaciteit van de netwerkbandbreedte. Het laat de klant ook &quot;zoeken&quot;aan om het even welk punt in de video zonder de behoefte om op de rest van de video te wachten te downloaden. Zie ook [Live HTTP-streaming](https://developer.apple.com/streaming/). Progressieve video wordt geleverd door de video lokaal te downloaden en op het desktopscherm of mobiele apparaat van de gebruiker op te slaan.

In de volgende tabel worden het apparaat, de browser en de afspeelmethode beschreven van video&#39;s op bureaubladcomputers en mobiele apparaten met de Klassieke Video Viewer van Dynamic Media.

| Apparaat | Browser | Video-afspeelmodus |
|--- |--- |--- |
| bureaublad | Internet Explorer 9 en 10 | Progressieve download. |
| Desktop | Internet Explorer 11+ | HLS-videostreaming. |
| Desktop | Firefox 23-44 | Progressieve download. |
| Desktop | Firefox 45 of hoger | HLS-videostreaming. |
| Desktop | Chroom | HLS-videostreaming. |
| Desktop | Safari (Mac) | HLS-videostreaming. |
| Mobiel | Chrome (Android 6 of eerder) | Progressieve download. |
| Mobiel | Chrome (Android 7 of hoger) | HLS-videostreaming. |
| Mobiel | Android (standaardbrowser) | Progressieve download. |
| Mobiel | Safari (iOS) | HLS-videostreaming. |
| Mobiel | Chrome (iOS) | HLS-videostreaming. |
| Mobiel | Blackberry | HLS-videostreaming. |
