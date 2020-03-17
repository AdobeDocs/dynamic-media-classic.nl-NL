---
title: De PDF-bestanden uploaden
seo-title: De PDF-bestanden uploaden
description: 'null'
seo-description: Leer hoe u de PDF-bestanden uploadt die aan een eCatalog zijn gekoppeld.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# De PDF-bestanden uploaden{#uploading-the-pdf-files}

Adobe PDF-bestanden zijn doorgaans de bron voor een eCatalog; deze bestanden bevatten alle afbeeldingsgegevens , lettertypen en vectorafbeeldingen . U kunt ook een eCatalog met afbeeldingen maken. Nadat u de PDF-bestanden hebt voorbereid voor uploaden, selecteert u de knop Uploaden op de algemene navigatiebalk om de PDF&#39;s te uploaden.

## PDF-bestanden voorbereiden {#preparing-your-pdf-files}

Bereid uw Pdf- dossiers voor alvorens hen aan het het Publiceren Scene7 Systeem te uploaden:

* Plaats alle bestanden in dezelfde map op uw computer of netwerk, zodat u de bestanden gemakkelijker kunt uploaden.
* Geef de bestanden een naam in alfanumerieke volgorde op pagina. Door de pagina&#39;s te ordenen, kunt u de pagina&#39;s gemakkelijker in de juiste volgorde plaatsen nadat de bestanden zijn geüpload.
* Controleer de PDF-pagina&#39;s om te zien of deze snijtekens, registratiedoelen of kleurenbalken bevatten. Deze markeringen bepalen waar het papier moet worden geknipt wanneer documenten worden afgedrukt. deze moeten worden verwijderd voordat uw eCatalog op het web wordt geplaatst. Dynamic Media Classic biedt opties voor het uitsnijden van markeringen wanneer u PDF-bestanden uploadt.
* Als u wilt dat viewers in uw eCatalog zoeken op trefwoorden, controleert u of uw PDF-bestanden zijn samengevoegd. U kunt zoekwoorden niet extraheren uit samengevoegde PDF-bestanden. Als u wilt weten of een PDF is afgevlakt, selecteert u de tekst in de PDF. Als u geen tekst kunt selecteren, wordt de PDF afgevlakt en kunnen de gebruikers niet op sleutelwoord in uw eCatalog zoeken.
* PDF-bestanden bevatten meestal CMYK-afbeeldingen, omdat ze moeten worden afgedrukt. Standaard kunnen deze CMYK-afbeeldingen door SPS op intelligente wijze worden gedetecteerd en omgezet met een intern CMYK-kleurprofiel. Als u echter een aangepast kleurprofiel wilt gebruiken om CMYK-afbeeldingen om te zetten, kunt u dat doen.

   Zie [ICC-profielen](icc-profiles.md#icc_profiles).

## Aanbevolen opties voor uploaden naar PDF {#best-practice-pdf-upload-options}

Zie [Bestanden](uploading-files.md#uploading_your_files)uploaden voor meer informatie over de verschillende uploadmethoden.

Selecteer de bestanden die u wilt uploaden en selecteer de volgende *aanbevolen PDF-opties* :

* **Uitsnijden** Selecteer het menu Uitsnijden en kies Handmatig als de pagina&#39;s snijtekens, registratietekens of andere markeringen bevatten. Voer het aantal pixels in dat u vanaf de boven-, rechter-, onder- en linkerzijde van pagina&#39;s wilt uitsnijden. Snijtekens worden meestal ingesteld op een marge van 5 cm. Ervan uitgaande dat u 150 kiest als de resolutie per inch (aanbevolen instelling), wordt een halve inch van de marges uitgesneden door 75, 75, 75, 75 in de tekstvakken Boven, Rechts, Onder en Links in te voeren (bij 150 ppi is de helft van 1 inch gelijk aan 75 pixels).

* **Verwerken** Selecteer het menu Verwerking en kies Omzetten in pixels. Het PDF-bestand moet worden gerasterd, zodat alle pagina&#39;s en afbeeldingen in de eCatalog kunnen worden weergegeven.

* **Zoekwoorden extraheren (optioneel)** Selecteer deze optie als u wilt dat uw viewers op trefwoorden kunnen zoeken in uw eCatalog.

* **Automatisch een eCatalog genereren op basis van PDF van meerdere pagina&#39;s (optioneel)** Selecteer deze optie om automatisch een eCatalog te maken wanneer u het uploadt. U kunt rechtstreeks naar het eCatalog-scherm gaan en aan uw eCatalog beginnen te werken zonder eerst PDF- dossiers te selecteren en het bevel van de Bouwstijl te selecteren. De eCatalog wordt genoemd naar uw Pdf- dossier.

* **Resolutie** Dynamic Media Classic raadt 150 pixels per inch aan.

* **De Klassiek van de Media van de Kleurruimte** Dynamische adviseert het kiezen automatisch ontdekt. Gewoonlijk worden PDF&#39;s die voor afdrukuitvoer zijn gemaakt, in CMYK weergegeven. PDF&#39;s voor onlineweergave zijn RGB. Als een PDF beide kleurruimten gebruikt, kunt u een specifieke kleurruimte selecteren door forceren als RGB of forceren als CMYK te kiezen. PDF&#39;s gebruiken beide kleurruimten, bijvoorbeeld wanneer paginaafbeeldingen een CMYK-kleurruimte gebruiken, maar afbeeldingen RGB. Als u een ICC-profiel hebt geüpload, wordt de naam ervan weergegeven in het menu Kleurruimte en kunt u het daar kiezen.

   Zie [ICC-profielen](icc-profiles.md#icc_profiles).

* **Kleurprofiel** Kies een optie voor Kleurprofiel:

* **ConvertTo SRGB** Converts to SRGB (Standard Red Green Blue). SRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

* **De oorspronkelijke kleurruimte** behouden

* **Kies Aangepast van > naar** om de menu&#39;s te openen, zodat u de optie Omzetten van en Omzetten in kleurruimte kunt kiezen. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar SPS hebt geüpload.

Zie [ICC-profielen](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Zie Opties voor het uploaden naar [PDF voor meer informatie over alle PDF-opties](pdfs.md#pdf_upload_options).
