---
title: '"Beste praktijken: De HTML5-videoviewer gebruiken"'
seo-title: '"Beste praktijken: De HTML5-videoviewer gebruiken"'
description: 'null'
seo-description: Leer meer over de beste werkwijzen voor het gebruik van de HTML5-videoviewer.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Beste praktijken: De HTML5-videoviewer gebruiken{#best-practice-using-the-html-video-viewer}

De dynamische media Klassieke HTML5-videoviewer-voorinstellingen zijn robuuste videospelers. Aan de ontwerpkant van de speler, kunt u alle functionaliteit van de videospeler tot stand brengen gebruikend standaardhulpmiddelen van de Webontwikkeling. U kunt bijvoorbeeld de knoppen, besturingselementen en de achtergrond van een aangepaste posterafbeelding ontwerpen met HTML5 en CSS, zodat u uw klanten kunt bereiken met een aangepaste weergave.

Aan de afspeelzijde van de viewer wordt automatisch de videocapaciteit van de browser gedetecteerd. Vervolgens wordt de video afgespeeld met HLS (adaptieve videostreaming). Als deze leveringsmethode niet aanwezig is, wordt in plaats daarvan HTML5 progressief gebruikt.

Door de combinatie in één speler van de capaciteit om de playbackcomponenten te ontwerpen gebruikend HTML5 en CSS, ingebedde playback te hebben, en adaptieve en progressieve het stromen te gebruiken afhankelijk van het vermogen van browser, breidt u het bereik van uw rijke media inhoud tot zowel Desktop als mobiele gebruikers uit en verzekert een gestroomlijnde videoervaring.

Zie ook [Informatie over HTML5 Viewers](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) in de Adobe Viewers Reference Guide.

## Video afspelen op bureaubladcomputers en mobiele apparaten met gebruik van de Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Voor adaptieve videostreaming op het bureaublad en mobiele apparaten zijn de video&#39;s die worden gebruikt voor het schakelen naar een andere bitsnelheid, gebaseerd op alle MP4-video&#39;s in de adaptieve videoset.

Het afspelen van video vindt plaats met behulp van HLS of progressieve video. HLS (HTTP Live Streaming) is een Apple-standaard voor adaptieve videostreaming die het afspelen automatisch aanpast op basis van de capaciteit van de netwerkbandbreedte. Ook kan de klant naar elk punt in de video zoeken zonder dat de rest van de video hoeft te worden gedownload (zie ook Live [HTTP-streaming](#UnresolvedLink-https://developer.apple.com/streaming/)). Progressieve video wordt geleverd door de video lokaal te downloaden en op het desktopscherm of mobiele apparaat van de gebruiker op te slaan.

In de volgende tabel worden het apparaat, de browser en de afspeelmethode beschreven van video&#39;s op bureaubladcomputers en mobiele apparaten met de Dynamic Media Classic Video Viewer.

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
