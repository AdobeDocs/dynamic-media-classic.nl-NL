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
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 0%

---

# ECatalog-afbeeldingen met hyperlinks maken{#creating-ecatalog-image-maps}

Een afbeelding met hyperlinks is een gebied op een eCatalog-pagina waarop u met de muis kunt schuiven of waarop u een afbeelding met hyperlinks kunt selecteren om acties van verschillende soorten te activeren. Wanneer u de aanwijzer over een Afbeeldingskaart beweegt, ziet u bijvoorbeeld een beschrijving van een item met rollover-tekst. Wanneer u een afbeelding met hyperlinks selecteert, wordt een andere handeling uitgevoerd. U kunt bijvoorbeeld een webpagina openen zodat gebruikers meer kunnen weten over een item of dit kunnen kopen, of u kunt een video starten om een item in gebruik te zien.

## ECatalog-afbeeldingen met hyperlinks tekenen {#drawing-ecatalog-image-maps}

Voor eCatalogi, tekent u Kaarten van het Beeld op het lusje van de Pagina&#39;s van de Kaart van het eCatalogscherm. Dit scherm bestaat uit het gebied Afbeeldingskaart waar de eCatalog-pagina&#39;s worden weergegeven en, rechts, de lijst Afbeeldingskaart. Terwijl u Afbeeldingskaarten maakt, worden de namen ervan ingevoerd in de lijst Afbeeldingskaart.

1. De rollover van de eCatalog selecteren **[!UICONTROL Edit]** knop.
1. Selecteren **[!UICONTROL Map Pages]**.
1. Selecteer links in het scherm Map Pages de gewenste pagina.
1. Teken in het gebied Afbeeldingskaart een rechthoekige of veelhoekige (veelzijdige) afbeelding met hyperlinks:

   * **Rechthoekige kaart** - Selecteer het gereedschap Afbeeldingskaart rechthoek en sleep op de pagina om de rechthoek te maken.

   * **Veelhoekige kaart** - Selecteer het gereedschap Veelhoekafbeelding met hyperlinks en selecteer vervolgens zo vaak als nodig is rond de omtrek van de afbeelding. Terwijl u selecteert, tekent Adobe Dynamic Media Classic de randen van de Afbeeldingskaart.

     Nadat u een afbeelding met hyperlinks hebt getekend, wijst Adobe Dynamic Media Classic er een naam aan toe in de lijst Afbeeldingskaart. Adobe Dynamic Media Classic voegt een volgnummer toe aan de naam van de eCatalog-pagina waarin u werkt.

1. (Optioneel) Kies in de lijst Afbeeldingskaart de optie [!UICONTROL Name] kunt u een nieuwe naam voor de Afbeeldingskaart invoeren. Plaats geen lege spaties in de naam die u invoert.
1. U kunt gebruikers een nieuwe webpagina laten openen wanneer ze de Afbeeldingskaart selecteren. Voer in de URL-kolom in de lijst Afbeeldingskaart de URL van de webpagina in.

   Selecteer **[!UICONTROL Edit]** en voert u een sjabloon in.

Zie [Een sjabloon gebruiken om JavaScript en URL&#39;s in te voeren](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Optioneel) Selecteer in de vervolgkeuzelijst Tonen de optie **[!UICONTROL Rollover Text]** en voer vervolgens de tekst in die gebruikers op het scherm moeten zien wanneer zij hun aanwijzers over de Afbeeldingskaart bewegen.
1. (Optioneel) Selecteer in de vervolgkeuzelijst Tonen de optie **[!UICONTROL Other Actions]** en voer een kenmerk in om een vervaging- of focusactie te activeren wanneer gebruikers hun aanwijzers over een afbeelding met hyperlinks bewegen.

   Zie [Andere handelingen voor afbeeldingen met hyperlinks definiëren](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Selecteren **[!UICONTROL Save]**.
1. (Optioneel) Selecteer **[!UICONTROL Preview]** om de eCatalog met de standaard vooraf ingestelde eCatalogKijker te bekijken.

Als u een afbeelding met hyperlinks wilt verwijderen, selecteert u de naam in de lijst Afbeeldingskaart en selecteert u **[!UICONTROL Delete]**. U kunt een afbeelding met hyperlinks tijdelijk uitschakelen zonder de afbeelding met hyperlinks te verwijderen. Selecteer de optie Afbeeldingen met hyperlinks op in de lijst Afbeelding met hyperlinks.

## Veelzijdige media insluiten in een eCatalog {#embedding-rich-media-in-an-ecatalog}

Met de optie Rijke media van eCatalog kunt u video&#39;s in MP4-indeling toevoegen of sets met afbeeldingen die u aan een eCatalog hebt toegevoegd. Wanneer een gebruiker het gebied Afbeelding met hyperlinks in de eCatalog selecteert, wordt de bijbehorende spelset of video weergegeven. Deze functionaliteit is vooral handig als u wilt dat klanten een onderdeel in gebruik zien of een onderdeel vanuit verschillende invalshoeken en perspectieven bekijken.

U kunt knopinfo ook weergeven wanneer klanten hun aanwijzers over de Afbeeldingskaart bewegen, zodat ze weten wat ze selecteren.

**Veelzijdige media insluiten in een eCatalog:**

1. Teken een eCatalog-afbeelding met hyperlinks.

   Zie [ECatalog-afbeeldingen met hyperlinks tekenen](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Selecteer in de vervolgkeuzelijst Tonen de optie **[!UICONTROL Rich Media]**.
1. Navigeer in het paneel Middelen toevoegen aan de linkerkant naar een map met de centrifugeset of het videoelement (MP4-indeling) dat u wilt insluiten.
1. Sleep het element naar de afbeelding met hyperlinks.
1. (Optioneel) Kies in de lijst Afbeelding met hyperlinks onder **[!UICONTROL Tool Tip]** Voer de tekst in die gebruikers op het scherm moeten zien wanneer ze de muisaanwijzer op de Afbeeldingskaart plaatsen.
1. Selecteren **[!UICONTROL Save]**.

## Afbeeldingen met hyperlinks bewerken in eCatalog {#editing-ecatalog-image-maps}

Ga als volgt te werk om eCatalog Image Maps te bewerken, beginnend op het tabblad Kaartpagina&#39;s van het eCatalog-scherm:

* **De positie aanpassen** - Selecteer het gereedschap Pannen en verplaats de aanwijzer in de buurt maar niet boven de rand van de kaart. Wanneer de aanwijzer een pijl met vier punten ziet, sleept u de hele afbeelding met hyperlinks naar een nieuwe locatie.

  Zie [De positie, vorm en grootte van afbeeldingskaarten aanpassen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Vorm en grootte wijzigen** - Als u het formaat van een rechthoekige afbeelding met hyperlinks wilt wijzigen, selecteert u het gereedschap Pannen. Plaats de aanwijzer vervolgens boven een rand of een hoek en sleep wanneer u het pictogram met de dubbele pijl ziet. Als u de grootte van een veelhoekige afbeelding met hyperlinks wilt wijzigen, sleept u een vierkante selectiegreep. Als u een selectiegreep wilt maken, selecteert u de rand van de Afbeeldingskaart en sleept u.

  Zie [De positie, vorm en grootte van afbeeldingskaarten aanpassen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Afbeeldingen met hyperlinks verwijderen** - Selecteer het gereedschap Pannen, selecteer de afbeelding met hyperlinks om deze te selecteren en selecteer vervolgens **[!UICONTROL Delete]**.

  Als u alle afbeeldingen met hyperlinks uit een eCatalog wilt verwijderen, selecteert u de optie **[!UICONTROL Order Pages]** en selecteert u vervolgens **[!UICONTROL Clear Maps]**.

* **Overlappende afbeeldingen met hyperlinks verwerken** - Sleep om de volgorde van Afbeeldingskaarten in de lijst Afbeeldingskaart te wijzigen.

  Zie [Overlappende afbeeldingen met hyperlinks verwerken](creating-image-maps.md#handling_overlapping_image_maps).

* **Afbeeldingen met hyperlinks kopiëren naar andere pagina&#39;s** - Selecteer **[!UICONTROL Copy Maps To]** (Controleer of u zich op het tabblad Kaartpagina&#39;s bevindt). Selecteer in het scherm Afbeeldingen selecteren de pagina of pagina&#39;s waarop u de afbeeldingen met hyperlinks wilt kopiëren en selecteer **[!UICONTROL Select]**.

  Zie [Afbeeldingen met hyperlinks kopiëren naar andere afbeeldingen](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Wanneer u Afbeeldingen met hyperlinks kopieert naar verschillende pagina&#39;s in een eCatalog, kunt u alle afbeeldingen met hyperlinks in een eCatalog kopiëren naar een andere eCatalog. Zie [Afbeeldingen met hyperlinks kopiëren naar andere eCatalogi](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Afbeeldingskaartgegevens controleren en importeren {#reviewing-and-importing-image-map-data}

Het scherm Kaartoverzicht biedt metagegevens over uw eCatalog. U kunt de gegevens van de Kaart van het Beeld van het Beeld voor uw eCatalog ook groeperen die op het scherm van de Samenvatting van de Kaart beginnen. Door op deze manier gegevens met afbeeldingen met hyperlinks te importeren, kunt u gemakkelijker URL&#39;s met afbeeldingskaart en rollovertekst invoeren.

Als u het scherm Kaartoverzicht wilt weergeven, selecteert u op het tabblad Kaartpagina&#39;s van het eCatalog-scherm de optie **[!UICONTROL Summary]**.

### Overzicht van de gegevens van Image Map controleren {#review-image-map-data-summary}

1. Selecteer in het scherm Map Pages de optie **[!UICONTROL Summary]**.

   In het scherm Kaartoverzicht ziet u hoeveel Afbeeldingen met hyperlinks, URL&#39;s, beschrijvingen van rollover-tekst en andere handelingen zich in uw eCatalog bevinden.

1. Als er fouten met de rollover-toets optreden, selecteert u de fout in het dialoogvenster **[!UICONTROL Rollover_Key Error]** om te zien wat in uw spreadsheet moet veranderen om de fout te verbeteren. U kunt de tekst van dit bericht selecteren en kopiëren en deze in uw werkblad plakken.
1. Selecteren **[!UICONTROL Preview]** zodat u een pagina kunt bekijken in de eCatalog Viewer. Selecteer X om het Summiere scherm te sluiten en aan het scherm van de Pagina&#39;s van de Kaart terug te keren, of selecteer **[!UICONTROL Close]** om terug te keren naar Bladeren.

### Afbeeldingskaartgegevens importeren {#import-image-map-data}

In plaats van de gegevens van de Kaart van het Beeld op elke pagina in te gaan, kunt u de gegevens voor uw volledige eCatalog in het Summiere scherm van de Kaart invoeren. U importeert de gegevens van de Kaart van het Beeld in de vorm van een lusje-afgebakend dossier of van XML DTD. De velden in het bestand moeten in de volgorde staan die wordt weergegeven in het scherm Kaartoverzicht: Naam, inhoudsopgavelabels, Kaarten, URL&#39;s, Rollover-tekst, Overige handelingen en Zoeken. Door de gegevens van de Kaart van het Beeld in te voeren bespaart u het probleem om de gegevens in de lijst van de Kaart van het Beeld in te gaan aangezien u elke Kaart van het Beeld creeert.

>[!NOTE]
>
>Voordat u de gegevens van de Kaart van het Beeld invoert, moet u reeds de Kaarten van het Beeld hebben gecreeerd.

Ga als volgt te werk om Image Map-gegevens voor door u gemaakte afbeeldingen met hyperlinks te importeren en te beginnen in het scherm Map Summary:

1. Selecteren **[!UICONTROL Import Map Data]**.
1. Selecteer in het dialoogvenster Metagegevens importeren de optie **[!UICONTROL Browse]** en selecteer vervolgens het door tabs gescheiden of XML DTD-bestand.
1. Typ in het veld Taaknaam een naam voor het bestand (zorg ervoor dat u de extensie behoudt).
1. Selecteren **[!UICONTROL Upload]**.

## Afbeeldingen met hyperlinks kopiëren naar andere eCatalogi {#copying-image-maps-between-ecatalogs}

U kunt alle afbeeldingen met hyperlinks in een eCatalog kopiëren naar een andere eCatalog. Het kopiëren van Afbeeldingen met hyperlinks op deze manier is een handige methode voor het kopiëren van afbeeldingen met hyperlinks tussen vertalingen in vreemde talen van dezelfde eCatalog. Adobe Dynamic Media Classic raadt aan om eCatalogi te kopiëren met hetzelfde aantal pagina&#39;s en dezelfde afbeeldingen, zodat het kopiëren lukt.

>[!NOTE]
>
>Als de eCatalog waarnaar u Afbeeldingen met hyperlinks kopieert al Afbeeldingen met hyperlinks bevat, worden deze Afbeeldingen met hyperlinks verwijderd wanneer de kopie wordt gemaakt.

Ga als volgt te werk om alle afbeeldingen met hyperlinks in een eCatalog te kopiëren naar een andere eCatalog:

1. Selecteer de eCatalog met de Kaarten van het Beeld u wilt kopiëren, en de het omvergooien van eCatalog selecteren **[!UICONTROL Edit]** knop.
1. Selecteer op het tabblad Order Pages de optie **[!UICONTROL Copy Maps]**.
1. Selecteer in het dialoogvenster Element selecteren de eCatalog waar u de Afbeeldingskaarten wilt kopiëren en selecteer vervolgens **[!UICONTROL Select]**.

Adobe Dynamic Media Classic geeft een waarschuwingsbericht weer als de eCatalog waarvan u afbeeldingen met hyperlinks kopieert, een ander aantal pagina&#39;s of afbeeldingen heeft die een andere grootte hebben. Selecteren **[!UICONTROL Continue]** om de afbeeldingen met hyperlinks te kopiëren, ondanks de waarschuwing.
