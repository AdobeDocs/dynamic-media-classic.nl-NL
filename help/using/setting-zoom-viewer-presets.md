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

* **Kijker van het Gezoem: Basis**: Verstrekt een basisgezoem op het originele beeld.

* **Kijker van het Gezoem: Vlucht-uit**: Toont een tweede beeld van het gezoemde gebied naast het originele beeld. Er zijn geen besturingselementen om te gebruiken. Gebruikers verplaatsen de selectie over het gebied dat ze willen weergeven.

Houd er bij het bepalen van het totale bandbreedtegebruik voor deze viewer rekening mee dat zowel de hoofdafbeelding als de vervolgafbeelding in de viewer worden weergegeven. De grootte van de vervolgafbeelding wordt bepaald met behulp van de hoofdafbeeldingsgrootte (breedte en hoogte van werkgebied) en de zoomfactor. Als u wilt voorkomen dat het flyout-bestand te groot wordt, brengt u de volgende twee waarden met elkaar in evenwicht: als u een grote hoofdafbeeldingsgrootte hebt, verlaagt u de waarde voor Zoomfactor. (De breedte en hoogte van de Flyout bepalen de grootte van het wegvliegvenster, maar niet de grootte van het vliegend beeld dat aan de kijker wordt gediend.)

Als de hoofdafbeelding bijvoorbeeld 350 x 350 pixels groot is, met een zoomfactor van 3, is de resulterende uitvliegafbeelding 1050 x 1050 pixels. Als de hoofdafbeeldingsgrootte 300 x 300 pixels is, met een zoomfactor van 4, is de vervolgafbeelding 1200 x 1200 pixels. Afhankelijk van de kwaliteitsinstelling van JPEG (aanbevolen instellingen liggen tussen 80 en 90), kunt u de bestandsgrootte aanzienlijk verkleinen. De aanbevolen zoomfactoren zijn 2,5 tot 4, afhankelijk van de grootte van de hoofdafbeelding.

Adobe Dynamic Media Classic raadt de volgende parameters aan voor voorinstellingen van Zoom Viewer voor vlieg-uit:

* **Vergrote beeldgrootte**: Ongeveer 1500 door 1500 pixel, niet om 2000 door 2000 pixel te overschrijden.

* **grootte van het Beeld**: 100 KB of onder, niet om 150 KB te overschrijden (comprimeer het dossier om het onder 150 KB te houden).

* **Kijker van het Gezoem: Douane**: verstrekt geleid of ongeleid gezoem met beelden, de Reeksen van het Beeld met veelvoudige meningen, of de Reeksen van het Monster van de Kleur.

## Voorinstellingen van Zoomviewer maken en bewerken {#creating-and-editing-zoom-viewer-presets}

1. Ga op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** .
1. Voer een van de volgende handelingen uit:

   * **creeer vooraf ingesteld**: Selecteer **[!UICONTROL Add]**. Kies een platform in het dialoogvenster Viewer-voorinstelling toevoegen, kies een zoomviewer en selecteer vervolgens **[!UICONTROL Add]** . Geef een naam voor de voorinstelling op in het vak Naam voorinstelling.

   * **geef vooraf ingesteld** uit: Selecteer een Vooraf ingestelde Kijker van het Gezoem, dan uitgezocht **[!UICONTROL Edit]**.

1. Geef de gewenste instellingen op.

   Als u een beschrijving van een optie wilt zien, selecteert u het pictogram **[!UICONTROL Info Tip]** naast de optie.

   Op de pagina Voorbeeld wordt de viewer weergegeven terwijl u instellingen bijwerkt en wijzigt.

1. Selecteer **[!UICONTROL Save]** of **[!UICONTROL Save As]** .
1. Controleer op de pagina Voorinstellingen viewer de voorinstelling Zoomviewer of Voorinstelling voor Zoomen met instructies die u hebt gemaakt. Als het moet aanpassen, selecteert u **[!UICONTROL Edit]** , wijzigt u de instellingen op de `Configure Viewer` -pagina en selecteert u vervolgens **[!UICONTROL Save]** .

Voor informatie over het beheren van Kijker stelt op de Kijker vooraf in vooraf instelt scherm, zie [&#x200B; Kijker vooraf instelt &#x200B;](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [&#x200B; creeer en geef Kijker uit vooraf instelt &#x200B;](application-setup.md#adding_and_editing_viewer_presets)
