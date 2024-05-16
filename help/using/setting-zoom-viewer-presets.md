---
title: Voorinstellingen Zoomviewer instellen
description: Leer hoe u voorinstellingen voor een zoomviewer instelt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Voorinstellingen Zoomviewer instellen{#setting-up-zoom-viewer-presets}

Zoomviewervoorinstellingen bepalen de stijl, het gedrag en de vormgeving van uw zoomviewers. Adobe Dynamic Media Classic biedt veel opties voor het aanpassen en toewijzen van skins aan Viewers. Adobe Dynamic Media Classic wordt geleverd met standaard basisvoorinstellingen (snel), flyout en aangepaste voorinstellingen voor de zoomviewer. Beheerders kunnen voorinstellingen voor de zoomviewer van het bedrijf maken of een standaardvoorinstelling bewerken en deze onder een andere naam opslaan.

Alle zoomviewers beschikken over knoppen waarmee u kunt inzoomen, uitzoomen, pannen en de oorspronkelijke staat van de afbeelding kunt herstellen na het zoomen. Hoe deze knoppen eruitzien en hoe het venster zelf eruitziet, is afhankelijk van uw keuze voor Voorinstellingen van Zoomviewer. U kunt een voorinstelling voor een zoomviewer configureren met verschillende kleuren, randen, lettertypen en afbeeldingsinstellingen. Wanneer u een Viewer met instructies configureert, kunt u ook kiezen waar u de zoomdoelen wilt plaatsen. Zoomdoelen zijn de miniaturen waarop gebruikers klikken om te zoomen op de gebieden die u opgeeft.

## Voorinstellingen Zoomviewer {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic biedt de volgende voorinstellingen voor de zoomviewer:

* **Zoomviewer: standaard**: verschaft een standaardzoomfactor voor de oorspronkelijke afbeelding.

* **Zoomviewer: Uitvliegen**: geeft een tweede afbeelding van het ingezoomde gebied weer naast de oorspronkelijke afbeelding. Er zijn geen besturingselementen om te gebruiken. Gebruikers verplaatsen de selectie over het gebied dat ze willen weergeven.

Houd er bij het bepalen van het totale bandbreedtegebruik voor deze viewer rekening mee dat zowel de hoofdafbeelding als de vervolgafbeelding in de viewer worden weergegeven. De grootte van de vervolgafbeelding wordt bepaald met behulp van de hoofdafbeeldingsgrootte (breedte en hoogte van werkgebied) en de zoomfactor. Als u wilt voorkomen dat het flyout-bestand te groot wordt, brengt u de volgende twee waarden met elkaar in evenwicht: als u een grote hoofdafbeeldingsgrootte hebt, verlaagt u de waarde voor Zoomfactor. (De breedte en hoogte van de Flyout bepalen de grootte van het wegvliegvenster, maar niet de grootte van het vliegend beeld dat aan de kijker wordt gediend.)

Als de hoofdafbeelding bijvoorbeeld 350 x 350 pixels groot is, met een zoomfactor van 3, is de resulterende uitvliegafbeelding 1050 x 1050 pixels. Als de hoofdafbeeldingsgrootte 300 x 300 pixels is, met een zoomfactor van 4, is de vervolgafbeelding 1200 x 1200 pixels. Afhankelijk van de kwaliteitsinstelling JPEG (aanbevolen instellingen liggen tussen 80 en 90), kunt u de bestandsgrootte aanzienlijk verkleinen. De aanbevolen zoomfactoren zijn 2,5 tot 4, afhankelijk van de grootte van de hoofdafbeelding.

Adobe Dynamic Media Classic raadt de volgende parameters aan voor voorinstellingen van Zoom Viewer voor vlieg-uit:

* **Grotere afbeeldingsgrootte**: ongeveer 1500 x 1500 pixels, maximaal 2000 x 2000 pixels.

* **Afbeeldingsgrootte**: 100 kB of lager, maximaal 150 kB (comprimeer het bestand om het onder 150 kB te houden).

* **Zoomviewer: Aangepast**: Hiermee kunt u met of zonder instructies zoomen met afbeeldingen, afbeeldingssets met meerdere weergaven of kleurstaalsets.

## Voorinstellingen van Zoomviewer maken en bewerken {#creating-and-editing-zoom-viewer-presets}

1. Ga op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Voer een van de volgende handelingen uit:

   * **Een voorinstelling maken**: Select **[!UICONTROL Add]**. Kies in het dialoogvenster Voorinstelling viewer toevoegen een platform, kies een zoomviewer en selecteer **[!UICONTROL Add]**. Geef een naam voor de voorinstelling op in het vak Naam voorinstelling.

   * **Een voorinstelling bewerken**: Selecteer een voorinstelling voor een zoomviewer en selecteer **[!UICONTROL Edit]**.

1. Geef de gewenste instellingen op.

   Als u een beschrijving van een optie wilt weergeven, selecteert u de optie **[!UICONTROL Info Tip]** naast de optie.

   Op de pagina Voorbeeld wordt de viewer weergegeven terwijl u instellingen bijwerkt en wijzigt.

1. Selecteren **[!UICONTROL Save]** of **[!UICONTROL Save As]**.
1. Controleer op de pagina Voorinstellingen viewer de voorinstelling Zoomviewer of Voorinstelling voor Zoomen met instructies die u hebt gemaakt. Selecteer **[!UICONTROL Edit]**, wijzigt u de instellingen op de `Configure Viewer` pagina, en selecteer dan **[!UICONTROL Save]**.

Voor informatie over het beheren van Viewer-voorinstellingen op het scherm Viewer Presets raadpleegt u [Voorinstellingen viewer](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Viewer-voorinstellingen maken en bewerken](application-setup.md#adding_and_editing_viewer_presets)
