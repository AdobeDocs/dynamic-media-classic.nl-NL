---
title: Hoofdstukmarkeringen aan video toevoegen
seo-title: Hoofdstukmarkeringen aan video toevoegen
description: 'null'
seo-description: Leer hoe u hoofdstukmarkeringen aan een video kunt toevoegen.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# Hoofdstukmarkeringen aan video toevoegen{#adding-chapter-markers-to-video}

U kunt uw lange formuliervideo&#39;s beter weergeven en navigeren door hoofdstukmarkeringen toe te voegen aan enkele video&#39;s of aan Adaptieve videosets. Wanneer een gebruiker de video afspeelt, kunnen zij de hoofdstuktellers op de videochronologie (die ook als videoscrubber wordt bekend) klikken om aan hun aandachtspunt gemakkelijk te navigeren, of onmiddellijk aan nieuwe inhoud, demonstraties, leerprogramma&#39;s, etc. springen.

>[!NOTE]
>
>De videospeler die wordt gebruikt moet het gebruik van hoofdstukmarkeringen steunen.

Zie Een voorinstelling [voor](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) een videoviewer toevoegen of bewerken om de actiepunten voor hoofdstuknavigatie en de pop-uptekst voor hoofdstuktitels voor de `Universal_HTML5_Video` viewer te configureren (HTML5).

Zie ook Voorinstellingen [voor viewers](application-setup.md#adding_and_editing_viewer_presets)toevoegen en bewerken.

U maakt een hoofdstuklijst voor uw video op ongeveer dezelfde manier als u bijschriften maakt. U maakt dus een WebVTT-bestand. Merk op, echter, dat dit dossier van om het even welk WebVTT titeldossier moet gescheiden zijn dat u ook kunt gebruiken; u kunt geen titels en hoofdstukken in één dossier combineren WebVTT.

U kunt het volgende voorbeeld als voorbeeld van het formaat gebruiken u gebruikt om een dossier WebVTT met hoofdstuknavigatie tot stand te brengen:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

In het bovenstaande voorbeeld `Chapter 1` is dit de actidentificator en is deze optioneel. De actieduur van `00:00:000 --> 01:04:364` geeft de begin- en eindtijd van het hoofdstuk op in de notatie 00:00:000. Deze laatste drie cijfers zijn milliseconden en kunnen desgewenst worden ingesteld op 000. De hoofdstuktitel van `The bicycle store behind it all` is de daadwerkelijke beschrijving van de inhoud van het hoofdstuk. De actidentificator, de begintijd en de hoofdstuktitel worden allemaal weergegeven in een pop-up in de videospeler wanneer een gebruiker de muisaanwijzer boven een visueel actiepunt in de tijdlijn van de video houdt.

Omdat u een HTML5-videoviewer gebruikt, moet u ervoor zorgen dat het hoofdstukbestand dat u maakt, voldoet aan de WebVTT-standaard (Web Video Text Tracks). De bestandsextensie van het hoofdstuk is .vtt. U kunt meer informatie over de WebVTT ondertitelingsnorm leren.

Zie [WebVTT: De indeling](https://dev.w3.org/html5/webvtt/)Webvideoteksttracks.

**Hoofdstukmarkeringen aan video toevoegen**

1. Maak met een eenvoudige teksteditor buiten Dynamic Media Classic een hoofdbestand voor de video.

   >[!NOTE]
   >
   >Voor wereldwijde ondersteuning van videohoofdstukken in andere talen dan het Engels, dient u er rekening mee te houden dat de WebVTT-standaard vereist dat u afzonderlijke .vtt-bestanden maakt en dat u elke taal die u wilt ondersteunen, aanroept.

1. Sla het .vtt-bestand op in UTF8-codering om problemen met tekenuitvoering in de hoofdstuktiteltekst te voorkomen.

   Over het algemeen wilt u het hoofdstuk VTT-bestand dezelfde naam geven als het videobestand en dit bestand toevoegen met `chapters`. Hierdoor kunt u het genereren van video-URL&#39;s automatiseren met behulp van uw bestaande systeem voor webcontentbeheer.

1. Upload het WebVTT-hoofdstukbestand in Dynamic Media Classic.

   Zie Bestanden [uploaden](uploading-files.md#uploading_files).

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die het videobestand bevat dat u wilt koppelen aan het hoofdstukbestand dat u hebt geüpload.
1. Selecteer in het deelvenster Asset Browse één video-element en klik vervolgens onder de miniatuurafbeelding van het element op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Zoek in de Viewer List-tabel naar de HTML5-viewer **Univeral_HTML5_Video** en voer een van de volgende handelingen uit:

   * Klik uiterst rechts van de naam voor een video-viewerbeleving **[!UICONTROL Copy URL]** in een pop-up.

      Voeg de gekopieerde URL van de video toe aan de volgende syntaxis om deze te koppelen aan de gekopieerde URL naar het bijschriftbestand:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Voor een ingesloten video-viewerbeleving klikt u uiterst rechts op **[!UICONTROL Embed Code]** de naam.

      Klik in het dialoogvenster Code insluiten op **[!UICONTROL Copy to Clipboard]**.

      Voor de HTML5- `Universal_HTML5_Video` viewer voegt u de gekopieerde insluitcode als volgt toe:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

