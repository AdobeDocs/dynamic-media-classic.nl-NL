---
title: De PDF-bestanden uploaden
description: Leer hoe u de PDF-bestanden die aan een eCatalog zijn gekoppeld, uploadt naar Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# De PDF-bestanden uploaden{#uploading-the-pdf-files}

Adobe PDF-bestanden zijn doorgaans de bron voor een eCatalog. Deze bestanden bevatten alle afbeeldingsgegevens, lettertypen en vectorafbeeldingen. U kunt ook een eCatalog met afbeeldingen maken. Nadat u de PDF-bestanden hebt voorbereid voor uploaden, selecteert u op de algemene navigatiebalk de optie **[!UICONTROL Upload]** om te beginnen met het uploaden van de PDF.

Wanneer u een PDF uploadt voor pagina-extractie, wordt de volgende limiet aangehouden door de Adobe:

| Type PDF-limiet | Oplegde limiet | Wijziging tot limiet op 31 december 2022 |
| --- | --- | --- |
| Maximumaantal pagina&#39;s voor een PDF dat voor extractie in aanmerking komt | 5000 (voor nieuwe uploads) | 100 (voor alle PDF) |

Zie ook [Dynamic Media-beperkingen](/help/using/limitations.md).

## PDF-bestanden voorbereiden

Bereid uw PDF-bestanden voor voordat u ze uploadt naar Adobe Dynamic Media Classic:

* Als u het uploaden van de bestanden gemakkelijker wilt maken, plaatst u alle bestanden in dezelfde map op uw computer of netwerk.
* Geef de bestanden een naam in alfanumerieke volgorde op pagina. Door de pagina&#39;s te ordenen, kunt u de pagina&#39;s gemakkelijker in de juiste volgorde plaatsen nadat de bestanden zijn geüpload.
* Bekijk de pagina&#39;s om te zien of PDF-pagina&#39;s snijtekens, registratiedoelen of kleurenbalken bevatten. Deze markeringen bepalen waar het papier moet worden geknipt als documenten worden afgedrukt. Deze markeringen moeten worden verwijderd voordat uw eCatalog op het web wordt geplaatst. Adobe Dynamic Media Classic biedt opties voor snijtekens wanneer u PDF-bestanden uploadt.
* Als u wilt dat de kijkers uw eCatalog door sleutelwoord zoeken, kom te weten of uw dossiers van de PDF &quot;afgevlakt.&quot; zijn U kunt zoekwoorden niet extraheren uit samengevoegde PDF-bestanden. Als u wilt weten of een PDF is afgevlakt, selecteert u de tekst in de afbeelding. Als u geen tekst kunt selecteren, wordt de PDF afgevlakt en kunnen de kijkers niet op sleutelwoord in uw eCatalog zoeken.
* PDF-bestanden bevatten meestal CMYK-afbeeldingen, omdat ze moeten worden afgedrukt. Adobe Dynamic Media Classic kan deze CMYK-afbeeldingen standaard op intelligente wijze detecteren en converteren met een intern CMYK-kleurprofiel. Als u echter een aangepast kleurprofiel wilt gebruiken om CMYK-afbeeldingen om te zetten, kunt u dat doen.

  Zie [ICC-profielen (International Color Consortium)](icc-profiles.md#icc_profiles).

## Beste praktijken PDF uploadopties {#best-practice-pdf-upload-options}

Zie voor meer informatie over de verschillende uploadmethoden [Bestanden uploaden](uploading-files.md#uploading_your_files).

Selecteer de bestanden die u wilt uploaden en selecteer deze *beste praktijken* PDF-opties:

* **Opties voor uitsnijden** - Selecteer in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL Crop Options]**. Als de PDF-pagina&#39;s snijtekens, registratietekens of andere markeringen bevatten in het dialoogvenster **[!UICONTROL Crop]** vervolgkeuzelijst kiest u **[!UICONTROL Manual]**. Voer het aantal pixels in dat u vanaf de boven-, rechter-, onder- en linkerzijde van pagina&#39;s wilt uitsnijden. Snijtekens worden vaak ingesteld op een marge van 5 cm. Stel dat u **[!UICONTROL 150]** (aanbevolen) als de resolutie per pixel en voer 75, 75, 75, 75, 75 in de tekstvakken Boven, Rechts, Onder en Links in. In dat geval wordt een halve inch van de marges geoogst (bij 150 ppi is de helft van 1 gelijk aan 75 pixels).

* **Verwerking** - Selecteer in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL PDF Options]**. In de **[!UICONTROL Processing]** vervolgkeuzelijst kiest u **[!UICONTROL Rasterize]**. Het PDF-bestand moet worden omgezet in pixels, zodat alle pagina&#39;s en afbeeldingen in de eCatalog kunnen worden weergegeven.

* **Zoekwoorden extraheren (optioneel)** - Selecteer in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL PDF Options]**. Kies in de vervolgkeuzelijst Extraheren de optie **[!UICONTROL Search words]** als u wilt dat uw viewers op trefwoorden kunnen zoeken in uw eCatalog.

* **E-catalogus automatisch genereren op basis van PDF van meerdere pagina&#39;s (optioneel)** - Selecteer in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL PDF Options]**. Selecteren **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** om automatisch een eCatalog tot stand te brengen wanneer u uploadt. U kunt direct naar het eCatalog scherm gaan en beginnen werkend aan uw eCatalog zonder het moeten eerst PDF dossiers selecteren en het bevel van de Bouwstijl selecteren. De eCatalog wordt genoemd naar uw PDF dossier.

* **Resolutie** - Selecteer in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL PDF Options]**. In de **[!UICONTROL Resolution]** Voer een waarde in voor het tekstveld. Adobe Dynamic Media Classic raadt 150 pixels per inch aan.

* **Kleurruimte** - Selecteer in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL PDF Options]**. Kies in de vervolgkeuzelijst Kleurruimte de optie **[!UICONTROL Detect automatically]**. Gewoonlijk worden PDF die voor afdrukuitvoer zijn gemaakt, weergegeven in CMYK. PDF voor onlineweergave zijn RGB. Als een PDF beide kleurruimten gebruikt, kunt u een specifieke kleurruimte selecteren door Forceren als RGB of Forceren als CMYK te kiezen. PDF gebruiken beide kleurruimten, bijvoorbeeld wanneer paginaafbeeldingen een CMYK-kleurruimte gebruiken, maar afbeeldingen RGB gebruiken. Als u een ICC-profiel hebt geüpload, wordt de naam ervan weergegeven in het menu Kleurruimte en kunt u het daar kiezen.

  Zie [ICC-profielen (International Color Consortium)](/help/using/icc-profiles.md).

* **Opties voor kleurprofiel** - Selecteer in het dialoogvenster Taakopties uploaden de optie **[!UICONTROL Color Profile Options]** en kies vervolgens een optie voor Kleurprofiel:

   * **Oorspronkelijke kleurruimte behouden** - Behoudt de oorspronkelijke kleurruimte.

   * **Aangepast van > tot** - Opent submenu&#39;s zodat u een **[!UICONTROL Convert From]** en **[!UICONTROL Convert To]** kleurruimte. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Adobe Dynamic Media Classic hebt geüpload.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Zie [ICC-profielen (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Zie voor meer informatie over alle PDF-opties [Uploadopties voor PDF](pdfs.md#pdf_upload_options).
