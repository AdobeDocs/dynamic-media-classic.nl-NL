---
title: Werken met PDF's
seo-title: Werken met PDF's
description: 'null'
seo-description: Leer hoe u met PDF's werkt in Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# Werken met PDF&#39;s{#working-with-pdfs}

PDF-bestanden (Portable Document Format) worden meestal gebruikt in Dynamic Media Classic voor het maken van e-catalogi. Wanneer u een PDF-bestand uploadt, worden de pagina&#39;s standaard gerasterd in Dynamic Media (Klassiek), zodat de pagina&#39;s kunnen worden gebruikt om rich media te maken.

## Opties voor uploaden naar PDF {#pdf-upload-options}

Wanneer u een PDF-bestand uploadt, kunt u het op verschillende manieren opmaken. U snijdt zijn pagina&#39;s bij, haalt zoekwoorden op, voert een pixel-per-dun resolutie in, en kiest een kleurenruimte. PDF-bestanden bevatten vaak een snijmarge, snijtekens, registratietekens en andere drukkersmarkeringen. U kunt deze markeringen vanaf de zijkanten van pagina&#39;s bijsnijden terwijl u een PDF-bestand uploadt.

De opties voor het uploaden van PDF-bestanden staan in het scherm Uploaden onder PDF-opties.

**Verwerking**

De verwerkingsopties zijn als volgt:

**Met de optie Rasteren** (standaard) worden de pagina&#39;s in het PDF-bestand gewist en worden vectorafbeeldingen naar bitmapafbeeldingen geconverteerd. Kies deze optie om een eCatalog te maken.

**Met Woorden** zoeken extraheren worden woorden uit het PDF-bestand geëxtraheerd, zodat het bestand op trefwoord in een eCatalog-viewer kan worden doorzocht.

**Koppelingen** extraheren extraheert koppelingen uit de PDF-bestanden en converteert deze naar Afbeeldingen met hyperlinks die worden gebruikt in een eCatalog-viewer.

**Met Automatisch een eCatalog genereren met PDF** -bestand met meerdere pagina&#39;s wordt automatisch een eCatalog gemaakt van het PDF-bestand. De eCatalog wordt genoemd naar het Pdf- dossier u uploadde. (Deze optie is alleen beschikbaar als u het PDF-bestand rastert terwijl u het uploadt.)

**Resolutie**

Hiermee bepaalt u de resolutie-instelling. Deze instelling bepaalt hoeveel pixels per inch in het PDF-bestand worden weergegeven. De standaardwaarde is 150.

**Kleurruimte**

Selecteer het menu Kleurruimte en kies een kleurruimte voor het PDF-bestand. De meeste PDF-bestanden hebben zowel RGB- als CMYK-kleurenafbeeldingen. De RGB-kleurruimte heeft de voorkeur voor onlineweergave.

**Met Automatisch** detecteren blijft de kleurruimte van het PDF-bestand behouden.

**Omzetten in de RGB-kleurruimte door forceren als RGB** .

**Als CMYK** afdwingen wordt omgezet in de CMYK-kleurruimte.

**Omzetten in grijswaarden** in grijswaardenkleurruimte.

**Kleurprofiel**

Kies een optie voor Kleurprofiel:

**Omzetten in sRGB** converteert naar sRGB (standaard rood-groen blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

**De oorspronkelijke kleurruimte** behouden

**Kies Aangepast van > naar** om de menu&#39;s te openen, zodat u de optie Omzetten van en Omzetten in kleurruimte kunt kiezen. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Dynamic Media Classic hebt geüpload.

Zie [ICC-profielen](icc-profiles.md#icc_profiles).

## Witruimte uitsnijden vanuit een PDF-bestand {#cropping-white-space-from-a-pdf-file}

1. Als u pixels in witruimte automatisch wilt uitsnijden in een PDF-bestand terwijl u het uploadt, selecteert u het menu Uitsnijden en kiest u Bijsnijden.
1. Geef de volgende opties op:

   **Wegsnijden op basis van** kiezen of u wilt uitsnijden op basis van kleur of transparantie:

   **De optie Kleur** kiezen. Selecteer vervolgens het menu Hoek en kies de hoek van de PDF met de kleur die het beste overeenkomt met de kleur voor de witruimte die u wilt uitsnijden.

   **Transparantie** Kies de optie Transparantie.

   **Tolerantie** Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven:

   **Bijsnijden op basis van kleur** Geef 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de PDF hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

   **Bijsnijden op basis van transparantie** Geef 0 op om alleen pixels bij te snijden als deze volledig transparant zijn. De cijfers dichter aan 1 staan voor meer transparantie.

## Uitsnijden vanaf de zijkanten van PDF-pagina&#39;s {#cropping-from-the-sides-of-pdf-pages}

U kunt de drukkersmarkeringen handmatig van de zijkanten van de pagina&#39;s in een PDF-bestand verwijderen terwijl u het uploadt.

1. Selecteer het menu Uitsnijden en kies Handmatig.
1. Geef pixelinstellingen op in de tekstvakken Boven, Rechts, Onder en Links om vanaf de bovenkant, onder en zijkanten van pagina&#39;s bij te snijden.

Hoeveel van de pagina wordt bijgesneden, is afhankelijk van de resolutie PX/Inch-instelling die u voor het PDF-bestand hebt ingevoerd. Als u bijvoorbeeld 150 invoert (de standaardinstelling) als resolutie PX/Inch en u 75 pixels uitsnijdt vanaf de zijkanten van pagina&#39;s, wordt een halve inch bijgesneden, omdat 75 pixels bij 150 pixels per inch gelijk zijn aan een halve inch.
