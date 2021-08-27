---
title: De PDF-bestanden uploaden
description: Leer hoe u de PDF-bestanden uploadt die aan een eCatalog zijn gekoppeld.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# De PDF-bestanden uploaden{#uploading-the-pdf-files}

Adobe PDF-bestanden zijn doorgaans de bron voor een eCatalog. Deze bestanden bevatten alle afbeeldingsgegevens, lettertypen en vectorafbeeldingen. U kunt ook een eCatalog met afbeeldingen maken. Nadat u de PDF-bestanden voor uploaden hebt voorbereid, klikt u op **[!UICONTROL Upload]** op de algemene navigatiebalk om de PDF&#39;s te uploaden.

## PDF-bestanden voorbereiden {#preparing-your-pdf-files}

PDF-bestanden voorbereiden voordat u ze uploadt naar Adobe Dynamic Media Classic:

* Als u het uploaden van de bestanden gemakkelijker wilt maken, plaatst u alle bestanden in dezelfde map op uw computer of netwerk.
* Geef de bestanden een naam in alfanumerieke volgorde op pagina. Door de pagina&#39;s te ordenen, kunt u de pagina&#39;s gemakkelijker in de juiste volgorde plaatsen nadat de bestanden zijn geüpload.
* Bekijk de pagina&#39;s om te zien of PDF-pagina&#39;s snijtekens, registratiedoelen of kleurenbalken bevatten. Deze markeringen bepalen waar het papier moet worden geknipt wanneer documenten worden afgedrukt. deze moeten worden verwijderd voordat uw eCatalog op het web wordt geplaatst. Adobe Dynamic Media Classic biedt opties voor het uitsnijden van markeringen wanneer u PDF-bestanden uploadt.
* Als u wilt dat viewers in uw eCatalog zoeken op trefwoorden, controleert u of uw PDF-bestanden zijn samengevoegd. U kunt zoekwoorden niet extraheren uit samengevoegde PDF-bestanden. Als u wilt weten of een PDF is afgevlakt, selecteert u de tekst in de PDF. Als u geen tekst kunt selecteren, wordt de PDF afgevlakt en kunnen de gebruikers niet op sleutelwoord in uw eCatalog zoeken.
* PDF-bestanden bevatten meestal CMYK-afbeeldingen, omdat ze moeten worden afgedrukt. Standaard kan Adobe Dynamic Media Classic deze CMYK-afbeeldingen op intelligente wijze detecteren en omzetten met een intern CMYK-kleurprofiel. Als u echter een aangepast kleurprofiel wilt gebruiken om CMYK-afbeeldingen om te zetten, kunt u dat doen.

   Zie [ICC-profielen](icc-profiles.md#icc_profiles).

## Aanbevolen opties voor uploaden naar PDF {#best-practice-pdf-upload-options}

Zie [Uw bestanden uploaden](uploading-files.md#uploading_your_files) voor gedetailleerde informatie over de verschillende uploadmethoden.

Selecteer de bestanden die u wilt uploaden en selecteer vervolgens de volgende *aanbevolen PDF-opties:*

* **Opties voor**  uitsnijden - Klik in het dialoogvenster Opties voor uploaden taak op  **[!UICONTROL Crop Options]**. Als de PDF-pagina&#39;s snijtekens, registratietekens of andere markeringen bevatten, kiest u **[!UICONTROL Manual]** in de vervolgkeuzelijst **[!UICONTROL Crop]**. Voer het aantal pixels in dat u vanaf de boven-, rechter-, onder- en linkerzijde van pagina&#39;s wilt uitsnijden. Snijtekens worden vaak ingesteld op een marge van 5 cm. Stel dat u **[!UICONTROL 150]** (aanbevolen) kiest als resolutie per pixel en 75, 75, 75, 75, 75 in de tekstvakken Boven, Rechts, Onder en Links. In dat geval wordt een halve inch van de marges geoogst (bij 150 ppi is de helft van 1 gelijk aan 75 pixels).

* **Verwerken**  - Klik op het dialoogvenster Taakopties uploaden  **[!UICONTROL PDF Options]**. Kies **[!UICONTROL Rasterize]** in de vervolgkeuzelijst **[!UICONTROL Processing]**. Het PDF-bestand moet worden gerasterd, zodat alle pagina&#39;s en afbeeldingen in de eCatalog kunnen worden weergegeven.

* **Zoekwoorden extraheren (optioneel)** - Klik in het dialoogvenster Taakopties uploaden op  **[!UICONTROL PDF Options]**. Kies **[!UICONTROL Search words]** in de vervolgkeuzelijst Extraheren als u wilt dat uw viewers op trefwoorden kunnen zoeken in uw eCatalog.

* **Automatisch een eCatalog genereren op basis van PDF van meerdere pagina&#39;s (optioneel)**  - Klik in het dialoogvenster Taakopties uploaden op  **[!UICONTROL PDF Options]**. Selecteer **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** om automatisch een eCatalog tot stand te brengen wanneer u uploadt. U kunt rechtstreeks naar het eCatalog-scherm gaan en aan uw eCatalog beginnen te werken zonder eerst PDF- dossiers te selecteren en het bevel van de Bouwstijl te selecteren. De eCatalog wordt genoemd naar uw Pdf- dossier.

* **Resolutie**  - Klik in het dialoogvenster Taakopties uploaden op  **[!UICONTROL PDF Options]**. Voer in het tekstveld **[!UICONTROL Resolution]** een waarde in. Adobe Dynamic Media Classic raadt 150 pixels per inch aan.

* **Kleurruimte** - Klik op het dialoogvenster Taakopties uploaden  **[!UICONTROL PDF Options]**. Kies **[!UICONTROL Detect automatically]** in de vervolgkeuzelijst Kleurruimte. Gewoonlijk worden PDF&#39;s die voor afdrukuitvoer zijn gemaakt, in CMYK weergegeven. PDF&#39;s voor onlineweergave zijn RGB. Als een PDF beide kleurruimten gebruikt, kunt u een specifieke kleurruimte selecteren door forceren als RGB of forceren als CMYK te kiezen. PDF&#39;s gebruiken beide kleurruimten, bijvoorbeeld wanneer paginaafbeeldingen een CMYK-kleurruimte gebruiken, maar afbeeldingen RGB. Als u een ICC-profiel hebt geüpload, wordt de naam ervan weergegeven in het menu Kleurruimte en kunt u het daar kiezen.

   Zie [ICC-profielen](/help/icc-profiles.md).

* **Opties**  voor kleurprofiel - Klik in het dialoogvenster Taakopties uploaden op  **[!UICONTROL Color Profile Options]** en kies een optie voor het kleurprofiel:

   * **Oorspronkelijke kleurruimte**  behouden - Behoudt de oorspronkelijke kleurruimte.

   * **Aangepast van > tot**  - Hiermee opent u submenu&#39;s, zodat u een  **[!UICONTROL Convert From]** en  **[!UICONTROL Convert To]** kleurruimte kunt kiezen. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u hebt geüpload naar Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Zie [ICC-profielen](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Zie [Opties voor het uploaden naar PDF](pdfs.md#pdf_upload_options) voor meer informatie over alle PDF-opties.
