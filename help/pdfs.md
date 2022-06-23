---
title: Werken met PDF
description: Leer hoe u met PDF werkt in Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Werken met PDF{#working-with-pdfs}

PDF-bestanden (Portable Document Format) worden meestal in Adobe Dynamic Media Classic gebruikt om e-catalogi te maken. Wanneer u een PDF-bestand uploadt, worden de pagina&#39;s standaard omgezet in pixels of worden de pagina&#39;s gerasterd, zodat de pagina&#39;s kunnen worden gebruikt om rich media samen te stellen.

Wanneer u een PDF uploadt voor pagina-extractie, past Adobe de volgende limiet toe:

| Type limiet | Oplegde limiet | Wijziging tot limiet op 31 december 2022 |
| --- | --- | --- |
| Maximumaantal pagina&#39;s voor een PDF dat voor extractie in aanmerking komt | 5000 (voor nieuwe uploads) | 100 (voor alle PDF) |

Zie ook [Dynamic Media-beperkingen](/help/limitations.md).

## Uploadopties voor PDF {#pdf-upload-options}

Wanneer u een PDF-bestand uploadt, kunt u het op verschillende manieren opmaken. U snijdt zijn pagina&#39;s bij, haalt zoekwoorden op, voert een pixel-per-duimresolutie in, en kiest een kleurenruimte. PDF-bestanden bevatten vaak een snijmarge, snijtekens, registratietekens en andere drukkersmarkeringen. U kunt deze markeringen vanaf de zijkanten van pagina&#39;s bijsnijden wanneer u een PDF-bestand uploadt.

U kunt PDF-bestanden uploaden via de pagina Uploaden onder PDF-opties.

### Verwerkingsopties

**[!UICONTROL Rasterize]** - (Standaard) Hiermee worden de pagina&#39;s in het PDF-bestand weggesneden en worden vectorafbeeldingen omgezet in bitmapafbeeldingen. Kies deze optie om een eCatalog te maken.

**[!UICONTROL Extract Search Words]** - Extraheert woorden uit het PDF-bestand, zodat het bestand op trefwoord kan worden doorzocht in een eCatalog-viewer.

**[!UICONTROL Extract Links]** - Extraheert koppelingen uit de PDF-bestanden en converteert deze naar Afbeeldingen met hyperlinks die worden gebruikt in een eCatalog-viewer.

**[!UICONTROL Auto-Generate eCatalog With Multi-page PDF]** - Er wordt automatisch een eCatalog gemaakt op basis van het PDF-bestand. De eCatalog wordt genoemd naar het dossier van de PDF u uploadde. (Deze optie is alleen beschikbaar als u het PDF-bestand rastert terwijl u het uploadt.)

### Resolutie

Hiermee bepaalt u de resolutie-instelling. Deze instelling bepaalt hoeveel pixels per inch in het PDF-bestand worden weergegeven. De standaardwaarde is 150.

### Opties voor kleurruimte

Selecteer het menu Kleurruimte en kies een kleurruimte voor het PDF-bestand. De meeste PDF-bestanden hebben zowel RGB- als CMYK-kleurenafbeeldingen. De kleurruimte RGB heeft de voorkeur voor onlineweergave.

* **[!UICONTROL Detect Automatically]** - Behoudt de kleurruimte van het PDF-bestand.

* **[!UICONTROL Force As RGB]** - Converteert naar de kleurruimte RGB.

* **[!UICONTROL Force As CMYK]** - Converteert naar de CMYK-kleurruimte.

* **[!UICONTROL Force As Grayscale]** - Converteert naar de grijswaardenkleurruimte.

### Opties voor kleurprofiel

* **[!UICONTROL Convert To sRGB]** - Zet om in sRGB (standaard rood-groen blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

* **[!UICONTROL Keep Original Color Space]** - Behoudt de oorspronkelijke kleurruimte.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Hiermee opent u menu&#39;s, zodat u een optie kunt kiezen voor Omzetten van en Omzetten in kleurruimte. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Adobe Dynamic Media Classic hebt geüpload.

Zie ook [ICC-profielen](/help/icc-profiles.md#icc_profiles).

## Witruimte uitsnijden vanuit een PDF-bestand {#cropping-white-space-from-a-pdf-file}

1. Als u pixels in witruimte automatisch wilt uitsnijden in een PDF-bestand terwijl u het uploadt, selecteert u het menu Uitsnijden en kiest u Bijsnijden.
1. Geef de volgende opties op:

   * **[!UICONTROL Trim Away Based On]** - Kies of u wilt uitsnijden op basis van kleur of transparantie:

      * **[!UICONTROL Color]** - Kies de optie Kleur. Selecteer vervolgens de **[!UICONTROL Corner]** en kiest u de hoek van de PDF met de kleur die het meest overeenkomt met de kleur voor de witruimte die u wilt uitsnijden.

      * **[!UICONTROL Transparency]** - Kies de optie Transparantie.
   * **[!UICONTROL Tolerance]** - Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven.

   * **[!UICONTROL Trimming based on color]** - Geef 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de PDF hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

   * **[!UICONTROL Trimming based on transparency]** - Geef 0 op om pixels alleen uit te snijden als ze transparant zijn; De cijfers dichter aan 1 staan voor meer transparantie.


## Uitsnijden vanaf de zijkanten van PDF pagina&#39;s {#cropping-from-the-sides-of-pdf-pages}

U kunt de drukkersmarkeringen handmatig van de zijkanten van de pagina&#39;s in een PDF-bestand verwijderen terwijl u het uploadt.

1. Selecteer in het menu Uitsnijden de optie **[!UICONTROL Manual]**.
1. Geef pixelinstellingen op in de tekstvakken Boven, Rechts, Onder en Links om vanaf de bovenkant, onder en zijkanten van pagina&#39;s bij te snijden.

Hoeveel van de pagina wordt bijgesneden, is afhankelijk van de resolutie PX/Inch-instelling die u voor het PDF-bestand hebt ingevoerd. Als u bijvoorbeeld 150 (de standaardinstelling) invoert als resolutie PX/Inch en 75 pixels van de zijkanten van pagina&#39;s bijsnijdt, wordt een halve inch bijgesneden. bij 150 pixels per inch is 75 pixels gelijk aan een halve inch.
