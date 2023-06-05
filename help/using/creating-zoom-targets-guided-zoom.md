---
title: Zoomdoelen maken voor zoomen met instructies
description: Leer hoe u zoomdoelen maakt voor Inzoomen met instructies in Adobe Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Zoomdoelen maken voor zoomen met instructies{#creating-zoom-targets-for-guided-zoom}

Met zoomdoelen kunnen gebruikers bepaalde gedeelten van een afbeelding bekijken. Naast vrije zooming, kunnen de kijkers een duimnagel van het gezoemdoel selecteren en aan het deel van het beeld zoemen u hen wilt concentreren op. Zoomdoelen bieden u de gelegenheid om de aantrekkelijke of interessante gedeelten van een afbeelding te benadrukken.

![Zoomdoelen maken voor zoomen met instructies](/help/using/assets/zo_guided_zoom.png)

## Informatie over zoomdoelen {#about-zoom-targets}

Het maximale zoompercentage van zoomdoelen is 100 procent. Het minimale zoompercentage varieert op basis van een combinatie van de viewergrootte en de afbeeldingsgrootte, zoals in deze tabel wordt getoond:

| Afbeeldingsgrootte | Viewergrootte | Zoompercentage |
| --- | --- | --- |
| Groot | Kleiner | Kleiner minimum |
| Klein | Groter | Groter minimum |

U kunt de grootte van de zoomviewer aanpassen aan de grootte die op uw webpagina wordt gebruikt. Als u deze instelling permanent wilt wijzigen, kunt u de viewergrootte wijzigen in het scherm Setup (als u een beheerder bent). Zie [Voorinstellingen Zoomviewer instellen](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Zoomdoelen maken en bewerken {#creating-and-editing-zoom-targets}

Maak en bewerk zoomdoelen op het scherm Zoomdoeleditor. Selecteer een afbeelding en voer een van de volgende handelingen uit om dit scherm te openen:

* De rollover selecteren **[!UICONTROL Edit]** en kiest u Zoomdoelen.
* Geef de afbeelding in het deelvenster Bladeren weer in **[!UICONTROL Detail View]** selecteert u vervolgens **[!UICONTROL Zoom Targets]**.

Selecteer in het scherm Zoomdoeleditor de optie **[!UICONTROL Select Target]** (pijl) om een doel te selecteren voordat het formaat of de positie wordt gewijzigd. Selecteer **[!UICONTROL Add Targets]** (rechthoek). De pagina Zoomdoel-editor bevat ook gereedschappen voor het verwijderen, kopiëren en benoemen van zoomdoelen.

### Een zoomdoel maken {#creating-a-zoom-target}

Als u een zoomdoel wilt maken, opent u de pagina Zoomdoel-editor en gaat u als volgt te werk:

1. Selecteren **[!UICONTROL Add Targets]** (rechthoek), plaatst u de aanwijzer boven de afbeelding en selecteert u waar u het zoomdoel wilt plaatsen.

   Er wordt een miniatuurafbeelding van het zoomdoel weergegeven in het deelvenster aan de rechterkant van het scherm.

1. Selecteren **[!UICONTROL Select Target]** (pijl) en selecteer vervolgens het zoomdoel dat u hebt gemaakt en pas de grootte en positie van het doel aan.

   * **Formaat wijzigen** - Plaats de aanwijzer boven een hoek van het zoomdoel en sleep om het doel te vergroten of te verkleinen.

   * **Positie** - Plaats de aanwijzer boven het zoomdoel en sleep het naar een andere locatie.

1. Voer in het vak Naam een naam voor het zoomdoel in.

   >[!NOTE]
   >
   >Wat u in het vak Naam invoert, is meer dan een naam. Wanneer gebruikers de aanwijzer over het zoomdoel bewegen, zien ze wat u invoert in het vak Naam. Voer in het vak Naam een korte beschrijving in van het zoomdoel, zodat gebruikers weten waarop ze kunnen inzoomen.

1. Voer eventueel gebruikersgegevens in het veld Gebruikersgegevens in. In dit veld kunnen websiteontwerpers informatie toevoegen aan het zoomdoel.
1. Selecteren **[!UICONTROL Save]**.

   De coördinaten en het zoomniveau van het zoomdoel worden opgeslagen. Een miniatuur van het zoomdoel met de naam die u hebt ingevoerd, wordt aan de rechterkant van het scherm weergegeven.

>[!NOTE]
>
>Als u wilt zien hoe uw zoomdoelen er in een zoomviewer uitzien, selecteert u de optie **[!UICONTROL Preview]** in het scherm Zoomdoel-editor en kies een zoomviewer in het voorvertoningsscherm. Voor informatie over dit scherm raadpleegt u [Afbeeldingen voorvertonen met verschillende zoomweergaven](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Zoomdoelen bewerken {#editing-zoom-targets}

Als u zoomdoelen wilt bewerken, gebruikt u de volgende technieken op de pagina Zoomdoel-editor:

* **Opnieuw plaatsen** - Selecteer het doel met de knop Doel selecteren (de pijl). Sleep het doel vervolgens naar een andere locatie.

* **Formaat wijzigen** - Selecteer het doel met de knop Doel selecteren (de pijl). Als u het doel wilt vergroten of verkleinen, plaatst u de aanwijzer boven een hoek van het zoomdoel en sleept u.

* **Verwijderen** - Selecteer de miniatuurafbeelding van het doel aan de rechterkant van het scherm. Selecteer vervolgens **[!UICONTROL Delete Target]**.

* **Naam wijzigen** - Selecteer de miniatuurafbeelding van het doel aan de rechterkant van het scherm. Voer vervolgens een naam in het dialoogvenster **[!UICONTROL Name]** tekstveld en selecteer **[!UICONTROL Save]**.

### Zoomdoelen kopiëren {#copying-zoom-targets}

U kunt zoomdoelen van de ene afbeelding naar de andere kopiëren. Kopieer doelen wanneer twee afbeeldingen vergelijkbare inhoud bevatten en de zoomdoelen ervan op dezelfde locatie horen. Ga als volgt te werk om zoomdoelen naar een andere afbeelding te kopiëren:

1. Open de afbeelding met zoomdoelen die u wilt kopiëren in het scherm Zoomdoeleditor.
1. Selecteren **[!UICONTROL Copy Targets To]**.
1. Selecteer in het dialoogvenster Afbeeldingen selecteren een afbeelding en kies **[!UICONTROL Select]**.
