---
title: Lettertypen
description: Leer hoe u lettertypen in Adobe Dynamic Media Classic kunt gebruiken.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Lettertypen{#fonts}

Soms vereist Adobe Dynamic Media Classic dat u een lettertypebestand uploadt om tekst in een bepaald lettertype in te voeren of te renderen. Als u bijvoorbeeld een bepaald lettertype voor tekst op een sjabloonlaag wilt gebruiken, uploadt u het lettertypebestand. Upload het lettertypebestand om de paginanummers van de eCatalog Viewer in een bepaald lettertype weer te geven.

Adobe Dynamic Media Classic ondersteunt de volgende lettertypen:

* Alle TrueType-fonts
* PostScript® lettertypen
* OpenType/TrueType-lettertypen
* OpenType-/PostScript-lettertypen
* PhotoFonts

Nadat een lettertypebestand is geüpload, kunt u de Adobe Dynamic Media Classic-id, de lettertypenaam en de typegegevens wijzigen in het scherm Info bewerken.

>[!NOTE]
>
>Adobe Dynamic Media Classic raadt aan alle lettertypestijlen (vet, cursief, vet/cursief en standaard) te uploaden als u lettertypen in sjabloonlagen wilt gebruiken. Adobe Dynamic Media Classic heeft deze lettertypestijlen nodig om aanvragen te verwerken. Alles uploaden `PostScript/Adobe Type1` bestanden die aan een lettertype zijn gekoppeld, worden ook aangeraden omdat sommige van deze lettertypen gedetailleerde tekenspatiëringsgegevens bevatten.

## Fontbestanden uploaden {#uploading-font-files}

Upload doopvontdossiers met de zelfde technieken u gebruikt om andere dossiers te uploaden. U kunt lettertypebestanden opslaan in elke Adobe Dynamic Media Classic-map. Zie [Bestanden uploaden](uploading-files.md#uploading_your_files).

## Informatie over lettertypebestanden bewerken {#editing-font-file-information}

U kunt de id-naam van een lettertype en de informatie over het type wijzigen. Het bewerken van een lettertypebestand kan nuttig zijn bij zoekopdrachten en het gemakkelijker maken lettertypen te identificeren.

Selecteer in het deelvenster Bladeren het lettertypebestand dat u wilt bewerken in de gedetailleerde weergave en kies Bestand > Info bewerken. Het scherm Info bewerken wordt geopend. Kies de volgende opties en selecteer **[!UICONTROL Submit]**.

* **[!UICONTROL Font Name]** - Deze naam geeft het lettertype aan wanneer het wordt gepubliceerd.

* **[!UICONTROL PostScript Name]** - Deze naam is de volledige PostScript-naam voor het lettertype. Dit geeft meestal de dikte of stijl aan.

* **[!UICONTROL RTF Name]** - Deze naam wordt weergegeven in een pop-upmenu in de RTF-editor waarin sjabloontekstlagen worden gemaakt.

* **[!UICONTROL Font Family Name]** - Deze naam geeft de fontnaam weer zonder de stijl-, dikte- of fonttypindicator.

* **[!UICONTROL Font Style]** - De opties zijn Normaal, Vet, Cursief en Vet-cursief.

* **[!UICONTROL Font Type]** - De opties zijn TrueType en Adobe Type 1. Als u deze lettertypen op een andere naam aanroept, kunt u deze naam invoeren.

* **[!UICONTROL Font Type Abbreviation]** - De opties zijn als volgt:

   * **[!UICONTROL TTF]** - TrueType-lettertypebestanden die worden gebruikt voor PDF-/PostScript-rendering en beeldweergave.

   * **[!UICONTROL AFM]** - Adobe PostScript-lettertypebestanden met Adobe Font Metrics-informatie die worden gebruikt voor beeldserving.

   * **[!UICONTROL PFM]** - Adobe PostScript-lettertypebestanden met binaire metrische informatie over lettertypen.

   * **[!UICONTROL PFB]** - Adobe PostScript-lettertypebestanden met binaire informatie over lettertypecontouren die worden gebruikt voor PDF/PostScript-rendering en beeldweergave.
