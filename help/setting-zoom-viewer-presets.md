---
title: Voorinstellingen Zoomviewer instellen
description: Leer hoe u voorinstellingen voor de zoomviewer instelt.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Klassiek,Viewers,Zoomen
role: Business Practitioner
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
translation-type: tm+mt
source-git-commit: 9d73e74ffc4a1e7e31c84720a9bae105b6afb1ae
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Voorinstellingen Zoomviewer instellen{#setting-up-zoom-viewer-presets}

Voorinstellingen voor zoomviewer bepalen de stijl, het gedrag en de vormgeving van uw zoomviewers. Dynamic Media Classic biedt veel opties voor het aanpassen en toewijzen van weergaven. Dynamic Media Classic wordt geleverd met standaard basisvoorinstellingen (snel), flyout en aangepaste voorinstellingen voor de zoomviewer. Beheerders kunnen voorinstellingen voor de zoomviewer van het bedrijf maken of een standaardvoorinstelling bewerken en deze onder een andere naam opslaan.

Alle zoomviewers beschikken over knoppen waarmee u kunt inzoomen, uitzoomen, pannen en de oorspronkelijke staat van de afbeelding kunt herstellen nadat u hebt ingezoomd. Hoe deze knoppen eruitzien en hoe het venster zelf eruitziet, is afhankelijk van uw keuze voor Voorinstellingen van Zoomviewer. U kunt een voorinstelling voor een zoomviewer configureren met verschillende kleuren, randen, lettertypen en afbeeldingsinstellingen. Wanneer u een Viewer met instructies voor zoomen configureert, kunt u ook kiezen waar u de zoomdoelen wilt plaatsen. Zoomdoelen zijn de miniaturen waarop gebruikers klikken om te zoomen op de gebieden die u opgeeft.

## Info over Voorinstellingen van zoomviewer {#about-zoom-viewer-presets}

Dynamic Media Classic bevat de volgende voorinstellingen voor de zoomviewer:

* **Zoomviewer: Standaard**  - Hiermee kunt u eenvoudig inzoomen op de oorspronkelijke afbeelding.

* **Zoomviewer: Uitvliegen**  - Geeft een tweede afbeelding weer van het ingezoomde gebied naast de oorspronkelijke afbeelding. Er zijn geen besturingselementen om te gebruiken. Gebruikers verplaatsen de selectie over het gebied dat ze willen weergeven.

Houd er bij het bepalen van het totale bandbreedtegebruik voor deze viewer rekening mee dat zowel de hoofdafbeelding als de vervolgafbeelding in de viewer worden weergegeven. De grootte van de vervolgafbeelding wordt bepaald door de hoofdafbeeldingsgrootte (breedte en hoogte van werkgebied) en de zoomfactor. Als u wilt voorkomen dat de flyout-bestandsgrootte te groot wordt, brengt u de volgende twee waarden met elkaar in evenwicht: Als u een grote hoofdafbeeldingsgrootte hebt, verlaagt u de waarde voor Zoomfactor. (De breedte en hoogte van de Flyout bepalen de grootte van het wegvliegvenster, maar niet de grootte van het vliegend beeld dat aan de kijker wordt gediend.)

Als de hoofdafbeelding bijvoorbeeld 350 x 350 pixels groot is, met een zoomfactor van 3, is de resulterende uitvliegafbeelding 1050 x 1050 pixels. Als de hoofdafbeeldingsgrootte 300 x 300 pixels is, met een zoomfactor van 4, is de vervolgafbeelding 1200 x 1200 pixels. Afhankelijk van de kwaliteitsinstelling voor JPEG (de aanbevolen instellingen liggen tussen 80 en 90), kunt u de bestandsgrootte aanzienlijk verkleinen. De aanbevolen zoomfactoren zijn 2,5 tot 4, afhankelijk van de grootte van de hoofdafbeelding.

Dynamic Media Classic raadt de volgende parameters aan voor voorinstellingen van een uitgevouwen zoomviewer:

* **Grotere afbeeldingsgrootte** : ongeveer 1500 x 1500 pixels, maximaal 2000 x 2000 pixels.

* **Afbeeldingsgrootte** : 100 kB of lager, maximaal 150 kB (comprimeer het bestand om het onder 150 kB te houden).

* **Zoomviewer: Aangepast**  - Zoom met instructies of zonder instructies met afbeeldingen, Afbeeldingssets met meerdere weergaven of Kleurstaalsets.

## Voorinstellingen voor zoomviewers maken en bewerken {#creating-and-editing-zoom-viewer-presets}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** op de algemene navigatiebalk.
1. Voer een van de volgende handelingen uit:

   * **Een voorinstelling**  maken. Klik  **[!UICONTROL Add]**. Kies een platform in het dialoogvenster Viewer-voorinstelling toevoegen, kies een zoomviewer en klik op **[!UICONTROL Add]**. Geef een naam voor de voorinstelling op in het vak Naam voorinstelling.

   * **Een voorinstelling**  bewerken - Selecteer een voorinstelling voor een zoomviewer en klik op  **[!UICONTROL Edit]**.

1. Geef de gewenste instellingen op.

   Als u een beschrijving van een optie wilt zien, klikt u op het pictogram **[!UICONTROL Info Tip]** naast de optie.

   Op de pagina Voorbeeld wordt de viewer weergegeven terwijl u instellingen bijwerkt en wijzigt.

1. Klik op **[!UICONTROL Save]** of **[!UICONTROL Save As]**.
1. Controleer op de pagina Voorinstellingen viewer de voorinstelling Zoomviewer of Voorinstelling voor Zoomen met instructies die u hebt gemaakt. Als het moet aanpassen, klik **[!UICONTROL Edit]**, verander montages op de Configure pagina van de Kijker, en klik ****[!UICONTROL Save]****.

Zie [Viewer Presets](application-setup.md#viewer_presets) voor informatie over het beheren van Viewer-voorinstellingen op het scherm Viewer Presets.

>[!MORELIKETHIS]
>
>* [Viewer-voorinstellingen maken en bewerken](application-setup.md#adding_and_editing_viewer_presets)

