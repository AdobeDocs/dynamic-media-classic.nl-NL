---
title: Lettertypen
description: Leer hoe u lettertypen kunt gebruiken in Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Lettertypen{#fonts}

Soms moet u in Dynamic Media Classic een lettertypebestand uploaden om tekst in een bepaald lettertype in te voeren of te renderen. Als u bijvoorbeeld een bepaald lettertype voor tekst op een sjabloonlaag wilt gebruiken, uploadt u het lettertypebestand. Upload het lettertypebestand om de paginanummers van de eCatalog Viewer in een bepaald lettertype weer te geven.

Dynamic Media Classic ondersteunt de volgende lettertypen:

* Alle TrueType-fonts
* PostScript® lettertypen
* OpenType/TrueType-lettertypen
* OpenType-/PostScript-lettertypen
* PhotoFonts

Nadat een lettertypebestand is geüpload, kunt u de klassieke Dynamic Media-id, de lettertypenaam en de tekstgegevens wijzigen in het scherm Info bewerken.

>[!NOTE]
>
>Dynamic Media Classic raadt aan alle lettertypestijlen (vet, cursief, vet/cursief en standaard) te uploaden als u lettertypen in sjabloonlagen wilt gebruiken. Dynamic Media Classic heeft deze lettertypestijlen nodig om aanvragen te verwerken. Het wordt ook aanbevolen alle PostScript/Adobe Type 1-bestanden te uploaden die aan een lettertype zijn gekoppeld, omdat sommige van deze lettertypen gedetailleerde tekenspatiëringsgegevens bevatten.

## Fontbestanden uploaden {#uploading-font-files}

Upload doopvontdossiers met de zelfde technieken u gebruikt om andere dossiers te uploaden. U kunt lettertypebestanden opslaan in elke Classic-map van Dynamic Media. Zie [Uw bestanden uploaden](uploading-files.md#uploading_your_files).

## Informatie over lettertypebestanden bewerken {#editing-font-file-information}

U kunt de id-naam van een lettertype en de informatie over het type wijzigen. Het bewerken van een lettertypebestand kan nuttig zijn bij zoekopdrachten en het gemakkelijker maken lettertypen te identificeren.

Selecteer in het deelvenster Bladeren het lettertypebestand dat u wilt bewerken in de gedetailleerde weergave en kies Bestand > Info bewerken. Het scherm Info bewerken wordt geopend. Kies de volgende opties en selecteer de knop Verzenden.

* **Lettertypenaam**  - Deze naam geeft het lettertype aan wanneer het wordt gepubliceerd.

* **PostScript-naam**  - Deze naam is de volledige PostScript-naam voor het lettertype. Dit geeft meestal de dikte of stijl aan.

* **RTF-naam**  - Deze naam wordt weergegeven in een pop-upmenu in de RTF-editor waarin sjabloontekstlagen worden gemaakt.

* **Naam lettertypefamilie**  - Deze naam geeft de lettertypenaam weer zonder de stijl, dikte of lettertype-indicator.

* **Lettertypestijl**  - De opties zijn Normaal, Vet, Cursief en Vet-cursief.

* **Fonttype**  - De opties zijn TrueType en Adobe Type 1. Als u deze lettertypen op een andere naam aanroept, kunt u deze naam invoeren.

* **Afkorting**  van lettertype - De opties zijn als volgt:

   * **TTFTrueType-** lettertypebestanden die worden gebruikt voor PDF/PostScript-rendering en afbeeldingsserving.

   * **** AFMAdobe PostScript-lettertypebestanden die Adobe Font Metrics-informatie bevatten en worden gebruikt voor beeldserving.

   * **** PFMAdobe PostScript-lettertypebestanden met binaire metrische informatie over lettertypen.

   * **** PFBAdobe PostScript-lettertypebestanden met binaire contourinformatie voor lettertypen die worden gebruikt voor PDF/PostScript-rendering en afbeeldingsweergave.
