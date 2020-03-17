---
title: Voorinstellingen Zoomviewer instellen
seo-title: Voorinstellingen Zoomviewer instellen
description: 'null'
seo-description: Leer hoe u voorinstellingen voor de zoomviewer instelt.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Voorinstellingen Zoomviewer instellen{#setting-up-zoom-viewer-presets}

Voorinstellingen voor zoomviewer bepalen de stijl, het gedrag en de vormgeving van uw zoomviewers. Dynamic Media Classic biedt veel opties voor het aanpassen en toewijzen van viewers. Dynamische media Klassiek wordt geleverd met standaard basisvoorinstellingen (snel), flyout en aangepaste voorinstellingen voor de zoomviewer. Beheerders kunnen nieuwe voorinstellingen voor de zoomviewer van het bedrijf maken of een standaardvoorinstelling bewerken en deze onder een andere naam opslaan.

Alle zoomviewers beschikken over knoppen waarmee u kunt inzoomen, uitzoomen, pannen en de oorspronkelijke staat van de afbeelding kunt herstellen nadat u hebt ingezoomd. Hoe deze knoppen er uitzien en hoe het venster er zelf uitziet, is afhankelijk van uw keuze voor Voorinstellingen van Zoomviewer. U kunt een voorinstelling voor een zoomviewer configureren met verschillende kleuren, randen, lettertypen en afbeeldingsinstellingen. Wanneer u een Viewer met instructies voor zoomen configureert, kunt u ook kiezen waar u de zoomdoelen wilt plaatsen. Zoomdoelen zijn de miniaturen waarop gebruikers klikken om te zoomen op de gebieden die u opgeeft.

## Voorinstellingen Zoomviewer {#about-zoom-viewer-presets}

Dynamische media Klassiek biedt de volgende voorinstellingen voor de zoomviewer:

* **Zoomviewer: Met Standaard** kunt u eenvoudig inzoomen op de oorspronkelijke afbeelding.

* **Zoomviewer: Uitvliegen** geeft een tweede afbeelding weer van het ingezoomde gebied naast de oorspronkelijke afbeelding. Er zijn geen besturingselementen om te gebruiken. Gebruikers verplaatsen de selectie over het gebied dat ze willen weergeven.

Houd er bij het bepalen van het totale bandbreedtegebruik voor deze viewer rekening mee dat zowel de hoofdafbeelding als de vervolgafbeelding in de viewer worden weergegeven. De grootte van de vervolgafbeelding wordt bepaald door de hoofdafbeeldingsgrootte (breedte en hoogte van werkgebied) en de zoomfactor. Als u wilt voorkomen dat de flyout-bestandsgrootte te groot wordt, brengt u de volgende twee waarden met elkaar in evenwicht: Als u een grote hoofdafbeeldingsgrootte hebt, verlaagt u de waarde voor Zoomfactor. (De breedte en hoogte van de Flyout bepalen de grootte van het wegvliegvenster, maar niet de grootte van het vliegend beeld dat aan de kijker wordt gediend.)

Als de hoofdafbeelding bijvoorbeeld 350 x 350 pixels groot is, met een zoomfactor van 3, is de resulterende uitvliegafbeelding 1050 x 1050 pixels. Als de hoofdafbeeldingsgrootte 300 x 300 pixels is, met een zoomfactor van 4, is de vervolgafbeelding 1200 x 1200 pixels. Afhankelijk van de kwaliteitsinstelling voor JPEG (de aanbevolen instellingen liggen tussen 80 en 90), kunt u de bestandsgrootte aanzienlijk verkleinen. De aanbevolen zoomfactoren zijn 2,5 tot 4, afhankelijk van de grootte van de hoofdafbeelding.

Dynamic Media Classic raadt deze parameters aan voor voorinstellingen van de uitgevouwen zoomviewer:

* **Vergrote afbeeldingsgrootte**: ongeveer 1500 x 1500 pixels, maximaal 2000 x 2000 pixels.

* **Afbeeldingsgrootte** 100 kB of lager, niet groter dan 150 kB (comprimeer het bestand om het onder 150 kB te houden).

* **Zoomviewer: Met Aangepast** kunt u met of zonder instructies zoomen op afbeeldingen, Afbeeldingssets met meerdere weergaven of Kleurstaalsets.

## Voorinstellingen van Zoomviewer maken en bewerken {#creating-and-editing-zoom-viewer-presets}

Ga als volgt te werk om een voorinstelling voor een zoomviewer te maken of te bewerken:

1. Klik op **Instellen** > Voorinstellingen **van viewer**.
1. Voer een van de volgende handelingen uit:

   * **Een voorinstelling** maken Klik op Toevoegen. Kies een platform in het dialoogvenster Viewer-voorinstelling toevoegen, kies een zoomviewer en klik op Toevoegen. Geef een naam voor de voorinstelling op in het vak Naam voorinstelling.

   * **Als u een voorinstelling** bewerkt, selecteert u een voorinstelling voor een zoomviewer en klikt u op **Bewerken**.

1. Geef de gewenste instellingen op.

   Als u een beschrijving van een optie wilt zien, klikt u op het pictogram Info Tip naast de optie.

   In het voorvertoningsscherm wordt de viewer weergegeven terwijl u instellingen bijwerkt en wijzigt.

1. Klik op **Opslaan** of **Opslaan als**.
1. Bekijk in het scherm Voorinstellingen viewer de voorinstelling van de Zoomviewer of de voorinstelling van de Zoomviewer met instructies die u hebt gemaakt. Als het moet aanpassen, **geeft de klik uit**, verandert montages op het Configure scherm van de Kijker, en klikt **sparen**.

Zie Voorinstellingen voor [viewers voor informatie over het beheren van voorinstellingen voor viewers in het scherm Viewer Presets](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Viewer-voorinstellingen maken en bewerken](application-setup.md#adding_and_editing_viewer_presets)

