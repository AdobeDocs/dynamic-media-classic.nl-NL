---
title: Zoomdoelen maken voor zoomen met instructies
description: Leer hoe u zoomdoelen maakt voor Inzoomen met instructies in Adobe Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Zoomdoelen maken voor zoomen met instructies{#creating-zoom-targets-for-guided-zoom}

Met zoomdoelen kunnen gebruikers bepaalde gedeelten van een afbeelding bekijken. Naast vrije zooming, kunnen de kijkers een duimnagel van het gezoemdoel selecteren en aan het deel van het beeld zoemen u hen wilt concentreren op. Zoomdoelen bieden u de gelegenheid om de aantrekkelijke of interessante gedeelten van een afbeelding te benadrukken.

![Zoomdoelen maken voor zoomen met instructies](/help/assets/zo_guided_zoom.png)

## Informatie over zoomdoelen {#about-zoom-targets}

Het maximale zoompercentage van zoomdoelen is 100 procent. Het minimale zoompercentage varieert op basis van een combinatie van de viewergrootte en de afbeeldingsgrootte, zoals in deze tabel wordt getoond:

| Afbeeldingsgrootte | Viewergrootte | Zoompercentage |
| --- | --- | --- |
| Groot | Kleiner | Kleiner minimum |
| Klein | Groter | Groter minimum |

U kunt de grootte van de zoomviewer aanpassen aan de grootte die op uw webpagina wordt gebruikt. Als u deze instelling permanent wilt wijzigen, kunt u de viewergrootte wijzigen in het scherm Setup (als u een beheerder bent). Zie [Voorinstellingen van zoomviewer instellen](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Zoomdoelen maken en bewerken {#creating-and-editing-zoom-targets}

Maak en bewerk zoomdoelen op het scherm Zoomdoeleditor. Selecteer een afbeelding en voer een van de volgende handelingen uit om dit scherm te openen:

* Selecteer de rollover **[!UICONTROL Edit]** knop en kies Zoomdoelen.
* Geef in het deelvenster Bladeren de afbeelding weer in **[!UICONTROL Detail View]** en selecteer **[!UICONTROL Zoom Targets]**.

Selecteer **[!UICONTROL Select Target]** (pijl) in het scherm Zoomdoeleditor om een doel te selecteren voordat u de grootte of positie wijzigt. Selecteer **[!UICONTROL Add Targets]** (rechthoek) om een zoomdoel op de afbeelding te maken. De pagina Zoomdoel-editor bevat ook gereedschappen voor het verwijderen, kopiëren en benoemen van zoomdoelen.

### Een zoomdoel maken {#creating-a-zoom-target}

Als u een zoomdoel wilt maken, opent u de pagina Zoomdoel-editor en gaat u als volgt te werk:

1. Selecteer **[!UICONTROL Add Targets]** (rechthoek), verplaats de aanwijzer boven de afbeelding en selecteer waar u het zoomdoel wilt plaatsen.

   Er wordt een miniatuurafbeelding van het zoomdoel weergegeven in het deelvenster aan de rechterkant van het scherm.

1. Kies **[!UICONTROL Select Target]** (pijl) en selecteer het zoomdoel dat u hebt gemaakt en pas de grootte en positie van het doel aan.

   * **Grootte wijzigen**  - Plaats de aanwijzer boven een hoek van het zoomdoel en sleep om het doel te vergroten of te verkleinen.

   * **Positie**  - Plaats de aanwijzer boven het zoomdoel en sleep deze naar een andere locatie.

1. Voer in het vak Naam een naam voor het zoomdoel in.

   >[!NOTE]
   >
   >Wat u in het vak Naam invoert, is meer dan een naam. Wanneer gebruikers de aanwijzer over het zoomdoel bewegen, zien ze wat u invoert in het vak Naam. Voer in het vak Naam een korte beschrijving in van het zoomdoel, zodat gebruikers weten waarop ze kunnen inzoomen.

1. Voer eventueel gebruikersgegevens in het veld Gebruikersgegevens in. In dit veld kunnen websiteontwerpers informatie toevoegen aan het zoomdoel.
1. Selecteer **[!UICONTROL Save]**.

   De coördinaten en het zoomniveau van het zoomdoel worden opgeslagen. Een miniatuur van het zoomdoel met de naam die u hebt ingevoerd, wordt aan de rechterkant van het scherm weergegeven.

>[!NOTE]
>
>Als u wilt zien hoe de zoomdoelen er in een zoomviewer uitzien, selecteert u de knop **[!UICONTROL Preview]** in het scherm Zoomdoeleditor en kiest u een zoomviewer in het voorvertoningsscherm. Zie [Afbeeldingen voorvertonen met verschillende zoomviewers](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers) voor informatie over dit scherm.

### Zoomdoelen bewerken {#editing-zoom-targets}

Als u zoomdoelen wilt bewerken, gebruikt u de volgende technieken op de pagina Zoomdoel-editor:

* **Positie wijzigen**  - Selecteer het doel met de knop Doel selecteren (de pijl). Sleep het doel vervolgens naar een andere locatie.

* **Formaat wijzigen**  - Selecteer het doel met de knop Doel selecteren (de pijl). Als u het doel wilt vergroten of verkleinen, plaatst u de aanwijzer boven een hoek van het zoomdoel en sleept u.

* **Verwijderen**  - Selecteer de miniatuurafbeelding van het doel aan de rechterkant van het scherm. Selecteer vervolgens **[!UICONTROL Delete Target]**.

* **Naam wijzigen**  - Selecteer de miniatuurafbeelding van het doel aan de rechterkant van het scherm. Voer vervolgens een naam in het tekstveld **[!UICONTROL Name]** in en selecteer **[!UICONTROL Save]**.

### Zoomdoelen kopiëren {#copying-zoom-targets}

U kunt zoomdoelen van de ene afbeelding naar de andere kopiëren. Kopieer doelen wanneer twee afbeeldingen vergelijkbare inhoud bevatten en de zoomdoelen ervan op dezelfde locatie horen. Ga als volgt te werk om zoomdoelen naar een andere afbeelding te kopiëren:

1. Open de afbeelding met zoomdoelen die u wilt kopiëren in het scherm Zoomdoeleditor.
1. Selecteer **[!UICONTROL Copy Targets To]**.
1. Selecteer in het dialoogvenster Afbeeldingen selecteren een afbeelding en kies **[!UICONTROL Select]**.
