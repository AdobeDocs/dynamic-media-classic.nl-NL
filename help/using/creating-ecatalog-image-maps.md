---
title: ECatalog-afbeeldingen met hyperlinks maken
description: Leer hoe u eCatalog-afbeeldingen met hyperlinks maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 0%

---

# ECatalog-afbeeldingen met hyperlinks maken{#creating-ecatalog-image-maps}

Een afbeelding met hyperlinks is een gebied op een eCatalog-pagina waarop u met de muis kunt schuiven of waarop u een afbeelding met hyperlinks kunt selecteren om acties van verschillende soorten te activeren. Wanneer u de aanwijzer over een Afbeeldingskaart beweegt, ziet u bijvoorbeeld een beschrijving van een item met rollover-tekst. Wanneer u een afbeelding met hyperlinks selecteert, wordt een andere handeling uitgevoerd. U kunt bijvoorbeeld een webpagina openen zodat gebruikers meer kunnen weten over een item of dit kunnen kopen, of u kunt een video starten om een item in gebruik te zien.

## ECatalog-afbeeldingen met hyperlinks tekenen {#drawing-ecatalog-image-maps}

Voor eCatalogi, tekent u Kaarten van het Beeld op het lusje van de Pagina&#39;s van de Kaart van het eCatalogscherm. Dit scherm bestaat uit het gebied Afbeeldingskaart waar de eCatalog-pagina&#39;s worden weergegeven en, rechts, de lijst Afbeeldingskaart. Terwijl u Afbeeldingskaarten maakt, worden de namen ervan ingevoerd in de lijst Afbeeldingskaart.

1. Selecteer de rollover-knop van de eCatalog **[!UICONTROL Edit]** .
1. Selecteer **[!UICONTROL Map Pages]** .
1. Selecteer links in het scherm Map Pages de gewenste pagina.
1. Teken in het gebied Afbeeldingskaart een rechthoekige of veelhoekige (veelzijdige) afbeelding met hyperlinks:

   * **Rechthoekige kaart**: Selecteer het hulpmiddel van de Kaart van het Beeld van de Rechthoek en sleep op de pagina om de rechthoek tot stand te brengen.

   * **Veelhoekkaart**: Selecteer het hulpmiddel van de Kaart van het Beeld van de Veelhoek, dan selecteer zo vele tijden zonodig rond de perimeter van het beeld. Terwijl u selecteert, tekent Adobe Dynamic Media Classic de randen van de Afbeeldingskaart.

     Nadat u een afbeelding met hyperlinks hebt getekend, wijst Adobe Dynamic Media Classic er een naam aan toe in de lijst Afbeeldingskaart. Adobe Dynamic Media Classic voegt een volgnummer toe aan de naam van de eCatalog-pagina waarin u werkt.

1. (Optioneel) In de lijst Afbeeldingskaart kunt u in de kolom [!UICONTROL Name] een nieuwe naam voor de afbeelding met hyperlinks invoeren. Plaats geen lege spaties in de naam die u invoert.
1. U kunt gebruikers een nieuwe webpagina laten openen wanneer ze Afbeeldingskaart selecteren. Voer in de URL-kolom in de lijst Afbeeldingskaart de URL van de webpagina in.

   Als u het invoeren van URL&#39;s (Href-sjablonen) gemakkelijker wilt maken, selecteert u **[!UICONTROL Edit]** en voert u een sjabloon in.

Zie [ Gebruik een malplaatje om JavaScript en URLs ](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls) in te gaan.

1. (Optioneel) Selecteer **[!UICONTROL Rollover Text]** in de vervolgkeuzelijst Tonen en voer vervolgens de tekst in die gebruikers op het scherm moeten zien wanneer zij hun aanwijzers over de Afbeeldingskaart bewegen.
1. (Optioneel) Selecteer **[!UICONTROL Other Actions]** in de vervolgkeuzelijst Tonen en voer een kenmerk in om een vervaging- of focusactie te activeren wanneer gebruikers hun aanwijzers over een Afbeeldingskaart bewegen.

   Zie [ andere acties voor de Kaarten van het Beeld ](creating-image-maps.md#defining_other_actions_for_image_maps) bepalen.

1. Selecteer **[!UICONTROL Save]** .
1. (Optioneel) Selecteer **[!UICONTROL Preview]** om de eCatalog weer te geven met de standaard eCatalog Viewer-voorinstelling.

Als u een afbeelding met hyperlinks wilt verwijderen, selecteert u de naam in de lijst Afbeeldingskaart en selecteert u **[!UICONTROL Delete]** . U kunt een afbeelding met hyperlinks tijdelijk uitschakelen zonder de afbeelding met hyperlinks te verwijderen. Selecteer de optie Afbeeldingen met hyperlinks op in de lijst Afbeelding met hyperlinks.

## Veelzijdige media insluiten in een eCatalog {#embedding-rich-media-in-an-ecatalog}

U kunt de rijke optie van Media van eCatalog gebruiken om video&#39;s in formaat MP4 of de Reeksen van de Draai aan de Kaarten van het Beeld toe te voegen die u aan een eCatalog hebt toegevoegd. Wanneer een gebruiker het gebied Afbeeldingskaart in de eCatalog selecteert, wordt de bijbehorende Spin-set of video weergegeven. Deze functionaliteit is vooral handig als u wilt dat klanten een onderdeel in gebruik zien of een onderdeel vanuit verschillende invalshoeken en perspectieven bekijken.

U kunt knopinfo ook weergeven wanneer klanten hun aanwijzers over de Afbeeldingskaart bewegen, zodat ze weten wat ze selecteren.

**om rijke media in een eCatalog in te bedden:**

1. Teken een eCatalog-afbeelding met hyperlinks.

   Zie [ de Kaarten van het Beeld van de Catalogus trekken ](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Selecteer **[!UICONTROL Rich Media]** in de vervolgkeuzelijst Tonen.
1. Navigeer in het deelvenster Assets toevoegen aan de linkerkant naar een map die de centrifugeset of het videoelement (MP4-indeling) bevat die u wilt insluiten.
1. Sleep het element naar de afbeelding met hyperlinks.
1. (Optioneel) Typ in het lijstdeelvenster Afbeeldingskaart onder de kolomkop **[!UICONTROL Tool Tip]** de tekst die gebruikers op het scherm moeten zien wanneer ze de aanwijzer op de Afbeeldingskaart plaatsen.
1. Selecteer **[!UICONTROL Save]** .

## Afbeeldingen met hyperlinks bewerken in eCatalog {#editing-ecatalog-image-maps}

Ga als volgt te werk om eCatalog Image Maps te bewerken, beginnend op het tabblad Kaartpagina&#39;s van het eCatalog-scherm:

* **pas de positie** aan: Selecteer het hulpmiddel van het Pannen en beweeg de wijzer dichtbij maar niet over de grens van de kaart. Wanneer de aanwijzer een pijl met vier punten ziet, sleept u de hele afbeelding met hyperlinks naar een nieuwe locatie.

  Zie [ de positie, de vorm, en de grootte van Kaarten van het Beeld aanpassen ](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **verander de vorm en de grootte**: Om een rechthoekige Kaart van het Beeld te resize, selecteer het hulpmiddel van de Pannen. Plaats de aanwijzer vervolgens boven een rand of een hoek en sleep wanneer u het pictogram met de dubbele pijl ziet. Als u de grootte van een veelhoekige afbeelding met hyperlinks wilt wijzigen, sleept u een vierkante selectiegreep. Als u een selectiegreep wilt maken, selecteert u de rand van de Afbeeldingskaart en sleept u.

  Zie [ de positie, de vorm, en de grootte van Kaarten van het Beeld aanpassen ](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **het Schrappen van de Kaarten van het Beeld**: Selecteer het hulpmiddel van het Pannen, selecteer de Kaart van het Beeld om het te selecteren, en selecteer dan **[!UICONTROL Delete]**.

  Als u alle afbeeldingen met hyperlinks uit een eCatalog wilt verwijderen, selecteert u het tabblad **[!UICONTROL Order Pages]** en selecteert u vervolgens **[!UICONTROL Clear Maps]** .

* **Behandelend overlappende Kaarten van het Beeld**: Sleep om de orde van Kaarten van het Beeld op de Lijst van de Kaart van het Beeld te veranderen.

  Zie [ handvat overlappende Kaarten van het Beeld ](creating-image-maps.md#handling_overlapping_image_maps).

* **het Kopiëren Afbeeldingskaarten aan andere pagina&#39;s**: Selecteer **[!UICONTROL Copy Maps To]** (zorg ervoor u op het lusje van de Pagina&#39;s van de Kaart bent). Selecteer in het scherm Afbeeldingen selecteren de pagina of pagina&#39;s waarop u de Afbeeldingen met hyperlinks wilt kopiëren en selecteer **[!UICONTROL Select]** .

  Zie [ Kaarten van het Beeld van het Exemplaar aan andere beelden ](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Wanneer u Afbeeldingen met hyperlinks kopieert naar verschillende pagina&#39;s in een eCatalog, kunt u alle afbeeldingen met hyperlinks in een eCatalog kopiëren naar een andere eCatalog. Zie [ Kaarten van het Beeld van het Exemplaar onder andere eCatalogs ](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Afbeeldingskaartgegevens controleren en importeren {#reviewing-and-importing-image-map-data}

Het scherm Kaartoverzicht biedt metagegevens over uw eCatalog. U kunt de gegevens van de Kaart van het Beeld van het Beeld voor uw eCatalog ook groeperen die op het scherm van de Samenvatting van de Kaart beginnen. Door op deze manier gegevens met afbeeldingen met hyperlinks te importeren, kunt u gemakkelijker URL&#39;s met afbeeldingskaart en rollovertekst invoeren.

Selecteer **[!UICONTROL Summary]** om het scherm Kaartoverzicht weer te geven op het tabblad Kaartpagina&#39;s van het eCatalog-scherm.

### Overzicht van de gegevens van Image Map controleren {#review-image-map-data-summary}

1. Selecteer **[!UICONTROL Summary]** in het scherm Map Pages.

   In het scherm Kaartoverzicht ziet u hoeveel Afbeeldingen met hyperlinks, URL&#39;s, beschrijvingen van rollover-tekst en andere handelingen zich in uw eCatalog bevinden.

1. Als er fouten met de rollover-toets optreden, selecteert u de fout in de kolom **[!UICONTROL Rollover_Key Error]** om te zien wat er in het spreadsheet moet veranderen om de fout te corrigeren. U kunt de tekst van dit bericht selecteren en kopiëren en deze in uw werkblad plakken.
1. Selecteer **[!UICONTROL Preview]** zodat u een pagina in de eCatalog Viewer kunt bekijken. Selecteer X om het Summiere scherm te sluiten en aan het scherm van de Pagina&#39;s van de Kaart terug te keren, of **[!UICONTROL Close]** te selecteren om terug te keren naar Browse.

### Afbeeldingskaartgegevens importeren {#import-image-map-data}

In plaats van de gegevens van de Kaart van het Beeld op elke pagina in te gaan, kunt u de gegevens voor uw volledige eCatalog in het Summiere scherm van de Kaart invoeren. U importeert de gegevens van de Kaart van het Beeld in de vorm van een lusje-afgebakend dossier of van XML DTD. De velden in het bestand moeten in de volgorde staan die wordt weergegeven in het scherm Kaartoverzicht: Naam, inhoudsopgavelabels, Kaarten, URL&#39;s, Rollover-tekst, Overige handelingen en Zoeken. Door de gegevens van de Kaart van het Beeld in te voeren bespaart u het probleem om de gegevens in de lijst van de Kaart van het Beeld in te gaan aangezien u elke Kaart van het Beeld creeert.

>[!NOTE]
>
>Voordat u de gegevens van de Kaart van het Beeld invoert, moet u reeds de Kaarten van het Beeld hebben gecreeerd.

Ga als volgt te werk om Image Map-gegevens voor door u gemaakte afbeeldingen met hyperlinks te importeren en te beginnen in het scherm Map Summary:

1. Selecteer **[!UICONTROL Import Map Data]** .
1. Selecteer **[!UICONTROL Browse]** in het dialoogvenster Metagegevens importeren en selecteer vervolgens het door tabs gescheiden of XML DTD-bestand.
1. Typ in het veld Taaknaam een naam voor het bestand (zorg ervoor dat u de extensie behoudt).
1. Selecteer **[!UICONTROL Upload]** .

## Afbeeldingen met hyperlinks kopiëren naar andere eCatalogi {#copying-image-maps-between-ecatalogs}

U kunt alle afbeeldingen met hyperlinks in een eCatalog kopiëren naar een andere eCatalog. Het kopiëren van Afbeeldingen met hyperlinks op deze manier is een handige methode voor het kopiëren van afbeeldingen met hyperlinks tussen vertalingen in vreemde talen van dezelfde eCatalog. Adobe Dynamic Media Classic raadt aan om eCatalogi te kopiëren met hetzelfde aantal pagina&#39;s en dezelfde afbeeldingen, zodat het kopiëren lukt.

>[!NOTE]
>
>Als de eCatalog waarnaar u Afbeeldingen met hyperlinks kopieert al Afbeeldingen met hyperlinks bevat, worden deze Afbeeldingen met hyperlinks verwijderd wanneer de kopie wordt gemaakt.

Ga als volgt te werk om alle afbeeldingen met hyperlinks in een eCatalog te kopiëren naar een andere eCatalog:

1. Selecteer de eCatalog met de Kaarten van het Beeld u wilt kopiëren, en de het omvergooienknoop van de eCatalog **[!UICONTROL Edit]** selecteren.
1. Selecteer op het tabblad Order Pages de optie **[!UICONTROL Copy Maps]** .
1. Selecteer in het dialoogvenster Element selecteren de eCatalog waar u de Afbeeldingskaarten wilt kopiëren en selecteer vervolgens **[!UICONTROL Select]** .

Adobe Dynamic Media Classic geeft een waarschuwingsbericht weer als de eCatalog waarvan u afbeeldingen met hyperlinks kopieert, een ander aantal pagina&#39;s of afbeeldingen heeft die een andere grootte hebben. Selecteer **[!UICONTROL Continue]** om de Afbeeldingskaarten ondanks de waarschuwing te kopiëren.
