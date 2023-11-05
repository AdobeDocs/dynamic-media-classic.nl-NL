---
title: Hoofdstukmarkeringen aan video toevoegen
description: Leer hoe u hoofdstukmarkeringen aan een video in Adobe Dynamic Media Classic kunt toevoegen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Hoofdstukmarkeringen aan video toevoegen {#adding-chapter-markers-to-video}

U kunt lange-vormvideo&#39;s gemakkelijker bekijken en navigeren door hoofdstukmarkeringen toe te voegen aan enkele video&#39;s of aan Adaptieve videosets. Wanneer een gebruiker de video afspeelt, kunnen deze de hoofdstukmarkeringen op de videotijdlijn selecteren (ook wel de videoscrubber genoemd). Als u dit doet, kunnen ze gemakkelijk naar hun interesse gaan of direct naar nieuwe inhoud, demonstraties, zelfstudies, enzovoort gaan.

>[!NOTE]
>
>De videospeler die wordt gebruikt moet het gebruik van hoofdstukmarkeringen steunen.

Zie [Een voorinstelling voor een videoviewer toevoegen of bewerken](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) als u de hoofdstuknavigatie actiepunten en de hoofdstuktitel pop-uptekst voor de `Universal_HTML5_Video` viewer (HTML5).

Zie ook [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).

U maakt een hoofdstuklijst voor uw video op ongeveer dezelfde manier als u bijschriften maakt. U maakt dus een WebVTT-bestand. Dit bestand moet echter gescheiden zijn van elk WebVTT-bijschriftbestand dat u ook kunt gebruiken. U kunt bijschriften en hoofdstukken niet combineren tot één WebVTT-bestand.

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

In het bovenstaande voorbeeld: `Chapter 1` is de cue-id en is optioneel. De actieduur van `00:00:000 --> 01:04:364` geeft de begin- en eindtijd van het hoofdstuk aan, in 00:00:000-indeling. Deze laatste drie cijfers zijn milliseconden en kunnen desgewenst worden ingesteld op 000. De titel van het hoofdstuk `The bicycle store behind it all` Dit is de feitelijke beschrijving van de inhoud van het hoofdstuk. De actidentificator, de begintijd en de hoofdstuktitel worden allemaal in een pop-up in de videospeler weergegeven wanneer de aanwijzer op een visueel actiepunt in de tijdlijn van de video wordt geplaatst.

Omdat u een HTML5-videoviewer gebruikt, moet u ervoor zorgen dat het hoofdstukbestand dat u maakt, voldoet aan de WebVTT-standaard (Web Video Text Tracks). De bestandsextensie van het hoofdstuk is .VTT. U kunt meer informatie over de WebVTT ondertitelingsnorm leren.

Zie [WebVTT: De indeling Web Video Text Tracks](https://w3c.github.io/webvtt/).

**Hoofdstukmarkeringen aan video toevoegen:**

1. Maak met een eenvoudige teksteditor buiten Adobe Dynamic Media Classic een hoofdbestand voor de video.

   >[!NOTE]
   >
   >Voor wereldwijde ondersteuning van videohoofdstukken in andere talen dan Engels, vereist de WebVTT-standaard dat u afzonderlijke .vtt-bestanden maakt en dat u elke taal die u wilt ondersteunen, aanroept.

1. Sla het VTT-bestand op in UTF8-codering, zodat u problemen kunt voorkomen met de uitvoering van tekens in de tekst van de hoofdstuktitel.

   Over het algemeen wilt u het hoofdstuk VTT-bestand dezelfde naam geven als het videobestand en het toevoegen aan het bestand `chapters`. Op deze manier kunt u het genereren van video-URL&#39;s automatiseren met behulp van uw bestaande systeem voor webcontentbeheer.

1. Upload in Adobe Dynamic Media Classic uw WebVTT-hoofdstukbestand.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die het videobestand bevat dat u wilt koppelen aan het hoofdstukbestand dat u hebt geüpload.
1. Selecteer in het deelvenster Asset Browse één video-element en selecteer vervolgens onder de miniatuurafbeelding van het element **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Zoek in de tabel Viewer List naar de HTML5-viewer met de naam **Univeral_HTML5_Video** en voer vervolgens een van de volgende handelingen uit:

   * Voor een pop-upviewerervaring voor video selecteert u **[!UICONTROL Copy URL]** helemaal rechts van de naam.

     Voeg de gekopieerde URL van de video toe aan de volgende syntaxis, zodat u deze kunt koppelen aan de gekopieerde URL naar het bijschriftbestand:

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Voor een ingesloten videoviewerervaring selecteert u **[!UICONTROL Embed Code]** helemaal rechts van de naam.

     Selecteer in het dialoogvenster Code insluiten **[!UICONTROL Copy to Clipboard]**.

     Voor de HTML5 `Universal_HTML5_Video` voegt u de gekopieerde insluitcode als volgt toe aan de viewer:

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
