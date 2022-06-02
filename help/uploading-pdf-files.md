---
title: De PDF-bestanden uploaden
description: Leer hoe u de PDF-bestanden die aan een eCatalog zijn gekoppeld, uploadt naar Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: ac9cba2c33fb1df65e64746dea2557632b7b2903
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# De PDF-bestanden uploaden{#uploading-the-pdf-files}

Adobe PDF-bestanden zijn doorgaans de bron voor een eCatalog. Deze bestanden bevatten alle afbeeldingsgegevens, lettertypen en vectorafbeeldingen. U kunt ook een eCatalog met afbeeldingen maken. Nadat u de PDF-bestanden hebt voorbereid voor uploaden, selecteert u op de algemene navigatiebalk de optie **[!UICONTROL Upload]** om te beginnen met het uploaden van de PDF.

>[!NOTE]
>
>Wanneer u een PDF uploadt voor het uitnemen van pagina&#39;s, stelt Adobe de volgende richtlijnen voor best practices en een afgedwongen limiet op.
>
>* Maximumaantal pagina&#39;s per PDF dat wordt gebruikt voor extractie
   >   * Beste praktijken: 100
   >   * Afgedwongen limiet: 1000 (voor uploads vernieuwen)


## PDF-bestanden voorbereiden {#preparing-your-pdf-files}

PDF-bestanden voorbereiden voordat u ze uploadt naar Adobe Dynamic Media Classic:

* Als u het uploaden van de bestanden gemakkelijker wilt maken, plaatst u alle bestanden in dezelfde map op uw computer of netwerk.
* Geef de bestanden een naam in alfanumerieke volgorde op pagina. Door de pagina&#39;s te ordenen, kunt u de pagina&#39;s gemakkelijker in de juiste volgorde plaatsen nadat de bestanden zijn geüpload.
* Bekijk de pagina&#39;s om te zien of PDF-pagina&#39;s snijtekens, registratiedoelen of kleurenbalken bevatten. Deze markeringen bepalen waar het papier moet worden geknipt wanneer documenten worden afgedrukt. deze moeten worden verwijderd voordat uw eCatalog op het web wordt geplaatst. Adobe Dynamic Media Classic biedt opties voor snijtekens wanneer u PDF-bestanden uploadt.
* Als u wilt dat de kijkers uw eCatalog door sleutelwoord zoeken, kom te weten of uw dossiers van de PDF &quot;afgevlakt.&quot; zijn U kunt zoekwoorden niet extraheren uit samengevoegde PDF-bestanden. Als u wilt weten of een PDF is afgevlakt, selecteert u de tekst in de afbeelding. Als u geen tekst kunt selecteren, wordt de PDF afgevlakt en kunnen de kijkers niet op sleutelwoord in uw eCatalog zoeken.
* PDF-bestanden bevatten meestal CMYK-afbeeldingen, omdat ze moeten worden afgedrukt. Adobe Dynamic Media Classic kan deze CMYK-afbeeldingen standaard op intelligente wijze detecteren en converteren met een intern CMYK-kleurprofiel. Als u echter een aangepast kleurprofiel wilt gebruiken om CMYK-afbeeldingen om te zetten, kunt u dat doen.

   Zie [ICC-profielen (International Color Consortium)](icc-profiles.md#icc_profiles).

## Beste praktijken PDF uploadopties {#best-practice-pdf-upload-options}

Voor gedetailleerde informatie over de verschillende uploadmethoden raadpleegt u [Bestanden uploaden](uploading-files.md#uploading_your_files).

Selecteer de bestanden die u wilt uploaden en selecteer deze *beste praktijken* PDF-opties:

* **Opties voor uitsnijden** - Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL Crop Options]**. Als de PDF-pagina&#39;s snijtekens, registratietekens of andere markeringen bevatten in het dialoogvenster **[!UICONTROL Crop]** vervolgkeuzelijst kiest u **[!UICONTROL Manual]**. Voer het aantal pixels in dat u vanaf de boven-, rechter-, onder- en linkerzijde van pagina&#39;s wilt uitsnijden. Snijtekens worden vaak ingesteld op een marge van 5 cm. Stel dat u **[!UICONTROL 150]** (aanbevolen) als de resolutie per pixel en voer 75, 75, 75, 75, 75 in de tekstvakken Boven, Rechts, Onder en Links in. In dat geval wordt een halve inch van de marges geoogst (bij 150 ppi is de helft van 1 gelijk aan 75 pixels).

* **Verwerking** - Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL PDF Options]**. In de **[!UICONTROL Processing]** vervolgkeuzelijst kiest u **[!UICONTROL Rasterize]**. Het PDF-bestand moet worden omgezet in pixels, zodat alle pagina&#39;s en afbeeldingen in de eCatalog kunnen worden weergegeven.

* **Zoekwoorden extraheren (optioneel)** - Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL PDF Options]**. Kies in de vervolgkeuzelijst Extraheren de optie **[!UICONTROL Search words]** als u wilt dat uw viewers op trefwoorden kunnen zoeken in uw eCatalog.

* **E-catalogus automatisch genereren op basis van PDF van meerdere pagina&#39;s (optioneel)** - Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL PDF Options]**. Selecteren **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** om automatisch een eCatalog tot stand te brengen wanneer u uploadt. U kunt direct naar het eCatalog scherm gaan en beginnen werkend aan uw eCatalog zonder het moeten eerst PDF dossiers selecteren en het bevel van de Bouwstijl selecteren. De eCatalog wordt genoemd naar uw PDF dossier.

* **Resolutie** - Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL PDF Options]**. In de **[!UICONTROL Resolution]** Voer een waarde in voor het tekstveld. Adobe Dynamic Media Classic raadt 150 pixels per inch aan.

* **Kleurruimte** - Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL PDF Options]**. Kies in de vervolgkeuzelijst Kleurruimte de optie **[!UICONTROL Detect automatically]**. Gewoonlijk zijn PDF die voor afdrukuitvoer zijn gemaakt, in CMYK; PDF voor online weergave zijn RGB. Als een PDF beide kleurruimten gebruikt, kunt u een specifieke kleurruimte selecteren door Forceren als RGB of Forceren als CMYK te kiezen. PDF gebruiken beide kleurruimten, bijvoorbeeld wanneer paginaafbeeldingen een CMYK-kleurruimte gebruiken, maar afbeeldingen RGB gebruiken. Als u een ICC-profiel hebt geüpload, wordt de naam ervan weergegeven in het menu Kleurruimte en kunt u het daar kiezen.

   Zie [ICC-profielen (International Color Consortium)](/help/icc-profiles.md).

* **Opties voor kleurprofiel** - Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL Color Profile Options]** en kies vervolgens een optie voor Kleurprofiel:

   * **Oorspronkelijke kleurruimte behouden** - Behoudt de oorspronkelijke kleurruimte.

   * **Aangepast van > tot** - Hiermee opent u submenu&#39;s, zodat u een **[!UICONTROL Convert From]** en **[!UICONTROL Convert To]** kleurruimte. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Adobe Dynamic Media Classic hebt geüpload.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Zie [ICC-profielen (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Voor meer informatie over alle PDF-opties raadpleegt u [Uploadopties voor PDF](pdfs.md#pdf_upload_options).
