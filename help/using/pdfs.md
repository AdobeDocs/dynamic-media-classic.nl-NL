---
title: Werken met PDF's
description: Leer hoe u met PDF's werkt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Werken met PDF&#39;s{#working-with-pdfs}

PDF-bestanden (Portable Document Format) worden meestal in Adobe Dynamic Media Classic gebruikt om e-catalogi te maken. Wanneer u een PDF-bestand uploadt, worden de pagina&#39;s standaard omgezet in pixels of worden de pagina&#39;s gerasterd, zodat de pagina&#39;s kunnen worden gebruikt om rich media samen te stellen.

Wanneer u een PDF uploadt voor het uitnemen van pagina&#39;s, past Adobe de volgende limiet toe:

| Type limiet | Oplegde limiet | Wijziging tot limiet op 31 december 2022 |
| --- | --- | --- |
| Maximumaantal pagina&#39;s voor een PDF dat in aanmerking komt voor extractie | 5000 (voor nieuwe uploads) | 100 (voor alle PDF&#39;s) |

Zie ook [ Dynamische beperkingen van Media ](/help/using/limitations.md).

## Uploadopties voor PDF {#pdf-upload-options}

Wanneer u een PDF-bestand uploadt, kunt u het op verschillende manieren opmaken. U snijdt zijn pagina&#39;s bij, haalt zoekwoorden op, voert een pixel-per-duimresolutie in, en kiest een kleurenruimte. PDF-bestanden bevatten vaak een snijmarge, snijtekens, registratietekens en andere drukkersmarkeringen. U kunt deze markeringen vanaf de zijkanten van pagina&#39;s bijsnijden wanneer u een PDF-bestand uploadt.

De opties voor het uploaden van PDF-bestanden staan op de pagina Uploaden onder PDF-opties.

### Verwerkingsopties

**[!UICONTROL Rasterize]**: (Standaard) hiermee worden de pagina&#39;s in het PDF-bestand weggesneden en worden vectorafbeeldingen omgezet in bitmapafbeeldingen. Kies deze optie om een eCatalog te maken.

**[!UICONTROL Extract Search Words]**: extraheert woorden uit het PDF-bestand, zodat trefwoorden in het bestand kunnen worden doorzocht in een eCatalog-viewer.

**[!UICONTROL Extract Links]**: extraheert koppelingen uit de PDF-bestanden en converteert deze naar afbeeldingen met hyperlinks die worden gebruikt in een eCatalog-viewer.

**[!UICONTROL Auto-Generate eCatalog With Multi-page PDF]**: hiermee wordt automatisch een eCatalog gemaakt van het PDF-bestand. De eCatalog wordt genoemd naar het dossier van PDF u uploadde. (Deze optie is alleen beschikbaar als u het PDF-bestand rastert tijdens het uploaden.)

### Resolutie

Hiermee bepaalt u de resolutie-instelling. Deze instelling bepaalt hoeveel pixels per inch in het PDF-bestand worden weergegeven. De standaardwaarde is 150.

### Opties voor kleurruimte

Selecteer het menu Kleurruimte en kies een kleurruimte voor het PDF-bestand. De meeste PDF-bestanden hebben zowel RGB- als CMYK-kleurenafbeeldingen. De RGB-kleurruimte heeft de voorkeur voor onlineweergave.

* **[!UICONTROL Detect Automatically]** - Behoudt de kleurruimte van het PDF-bestand.

* **[!UICONTROL Force As RGB]** - Converteert naar de RGB-kleurruimte.

* **[!UICONTROL Force As CMYK]**: zet deze om in de CMYK-kleurruimte.

* **[!UICONTROL Force As Grayscale]** - Zet om in de grijswaardenkleurruimte.

### Opties voor kleurprofiel

* **[!UICONTROL Convert To sRGB]**: zet om in sRGB (standaard rood-groen-blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op een webpagina.

* **[!UICONTROL Keep Original Color Space]** - Behoudt de oorspronkelijke kleurruimte.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]** : opent menu&#39;s, zodat u een optie kunt kiezen voor Omzetten van en Omzetten in kleurruimte. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Adobe Dynamic Media Classic hebt geüpload.

Zie ook [ ICC profielen ](/help/using/icc-profiles.md#icc_profiles).

## Witruimte uitsnijden vanuit een PDF-bestand {#cropping-white-space-from-a-pdf-file}

U kunt pixels in witruimte automatisch uitsnijden vanuit een PDF-bestand terwijl u het uploadt.

1. Selecteer het menu Uitsnijden en kies Bijsnijden.
1. Geef de volgende opties op:

   * **[!UICONTROL Trim Away Based On]**: kies of u wilt uitsnijden op basis van kleur of transparantie:

      * **[!UICONTROL Color]**: kies de optie Kleur. Selecteer vervolgens het menu **[!UICONTROL Corner]** en kies de hoek van de PDF met de kleur die het beste overeenkomt met de kleur van de witruimte die u wilt uitsnijden.

      * **[!UICONTROL Transparency]**: kies de optie Transparantie.

   * **[!UICONTROL Tolerance]**: Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven.

   * **[!UICONTROL Trimming based on color]** - Geef 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de PDF hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

   * **[!UICONTROL Trimming based on transparency]**: geef 0 op als u pixels alleen wilt uitsnijden als ze transparant zijn; bij een waarde dichter bij 1 is meer transparantie mogelijk.

## Uitsnijden vanaf de zijkanten van PDF-pagina&#39;s {#cropping-from-the-sides-of-pdf-pages}

U kunt de drukkersmarkeringen handmatig van de zijkanten van pagina&#39;s in een PDF-bestand verwijderen terwijl u het uploadt.

1. Selecteer **[!UICONTROL Manual]** in het menu Uitsnijden.
1. Geef pixelinstellingen op in de tekstvakken Boven, Rechts, Onder en Links om vanaf de bovenkant, onder en zijkanten van pagina&#39;s bij te snijden.

Hoeveel van de pagina wordt bijgesneden, is afhankelijk van de resolutie PX/Inch-instelling die u voor het PDF-bestand hebt ingevoerd. Stel dat u 150 (de standaardinstelling) invoert als de instelling Resolutie PX/inch. Vervolgens snijdt u 75 pixels uit van de zijkanten van de pagina&#39;s. In een dergelijk geval: 0,5 inch is uitgesneden. Bij 150 pixels per inch is 75 pixels gelijk aan een halve inch.
