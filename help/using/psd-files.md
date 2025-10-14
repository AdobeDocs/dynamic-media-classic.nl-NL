---
title: Werken met PSD-bestanden
description: Leer hoe u met PSD-bestanden werkt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Werken met PSD-bestanden{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

PSD (Photoshop-documentbestanden) worden meestal in Adobe Dynamic Media Classic gebruikt om sjablonen te maken. Wanneer u een PSD-bestand uploadt, kunt u automatisch een Adobe Dynamic Media Classic-sjabloon maken vanuit het bestand (selecteer de optie Sjabloon maken in het scherm Uploaden).

Adobe Dynamic Media Classic maakt meerdere afbeeldingen van een PSD-bestand met lagen als u het bestand gebruikt om een sjabloon te maken. Voor elke laag wordt één afbeelding gemaakt.

## Uploadopties voor PSD {#psd-upload-options}

U vindt opties voor het uploaden van PSD-bestanden onder Photoshop-opties in het dialoogvenster Taakopties uploaden. U kunt een bestand uitsnijden, een kleurprofiel kiezen, het gebruiken om een sjabloon te maken en een anker selecteren.

Deze opties zijn beschikbaar wanneer u PSD-bestanden uploadt:

* **Opties van het Gewas**: Vergrendeld onder **[!UICONTROL Crop Options]**. Selecteer **[!UICONTROL Trim]** , zodat u witruimte automatisch kunt laten doorlopen vanaf de randen van een PSD-bestand. Selecteer **[!UICONTROL Manual]** om de zijden van het PSD-bestand uit te snijden:

   * **[!UICONTROL Trim]**: selecteer het menu **[!UICONTROL Trim Away Based On]** en kies **[!UICONTROL Color]** of **[!UICONTROL Transparency]** .

  Als u de optie **[!UICONTROL Color]** kiest, selecteert u het menu Hoek en kiest u de hoek van de PSD met de kleur die het beste overeenkomt met de kleur van de witruimte die u wilt uitsnijden.

  Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven. Als u wilt bijsnijden op basis van kleur, geeft u 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de PSD hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe. Als u wilt bijsnijden op basis van transparantie, geeft u 0 op voor het bijsnijden van pixels alleen als deze transparant zijn. Bij nummers die dichter bij 1 liggen, is meer transparantie mogelijk.

   * **[!UICONTROL Manual]** - Voer het aantal pixels in dat u wilt uitsnijden vanaf een zijde of elke zijde van de afbeelding. Hoeveel van de afbeelding wordt uitgesneden, is afhankelijk van de ppi-instelling (pixels per inch) in het afbeeldingsbestand. Stel dat de afbeelding 150 ppi weergeeft. Vervolgens voert u 75 in de tekstvakken Boven, Rechts, Onder en Links in. Elke zijde van de afbeelding wordt bijgesneden (0,5 inch).

* **de Opties van het Profiel van de Kleur**: Vergrendeld onder **[!UICONTROL Color Profile Options]**.

   * **[!UICONTROL Default Color Preservation]**

   * **[!UICONTROL Keep Original Color Space]** - Behoudt de oorspronkelijke kleurruimte van de afbeelding.

   * **[!UICONTROL Custom From]** > **[!UICONTROL To]** : opent menu&#39;s, zodat u een optie kunt kiezen voor Omzetten van en Omzetten in kleurruimte. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Adobe Dynamic Media Classic hebt geüpload. Zie [&#x200B; ICC profielen &#x200B;](/help/using/icc-profiles.md).

* **de Opties van Photoshop**

   * **[!UICONTROL Maintain Layers]**: hiermee worden de lagen in de PSD, indien aanwezig, uitgelijnd op afzonderlijke elementen. De elementlagen blijven gekoppeld aan de PSD. U kunt ze weergeven door het PSD-bestand te openen in de Gedetailleerde weergave en het deelvenster Lagen te selecteren. Zie Lagen weergeven en bewerken in een PSD-bestand.

   * **[!UICONTROL Create Template]**: maakt een sjabloon op basis van de lagen in het PSD-bestand.

   * **[!UICONTROL Extract Text]**: extraheert de tekst zodat gebruikers naar tekst in een viewer kunnen zoeken.

   * **[!UICONTROL Extend Layers To Background Size]** - Hiermee vergroot u de grootte van de aan elkaar geknipte afbeeldingslagen tot de grootte van de achtergrondlaag.

   * **[!UICONTROL Layer Naming]**: Lagen in het PSD-bestand worden geüpload als afzonderlijke afbeeldingen. Kies een van de volgende opties om deze afbeeldingen een naam te geven in Adobe Dynamic Media Classic:

      * **[!UICONTROL Layer Name]** : de afbeeldingen krijgen een naam na de laagnamen in het PSD-bestand. Een laag met de naam Prijscode in het oorspronkelijke PSD-bestand wordt bijvoorbeeld een afbeelding met de naam Prijscode. Als de laagnamen in het PSD-bestand echter standaard Photoshop-laagnamen zijn (Achtergrond, Laag 1, Laag 2, enzovoort), krijgen de afbeeldingen een naam na hun laagnummers in het PSD-bestand. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop and layer number]**: de afbeeldingen krijgen een naam na hun laagnummer in het PSD-bestand, waarbij de oorspronkelijke laagnamen worden genegeerd. Afbeeldingen krijgen de naam Photoshop en een toegevoegd laagnummer. De tweede laag van een bestand met de naam `Spring Ad.psd` krijgt bijvoorbeeld de naam `Spring Ad_2` , zelfs als het bestand een andere naam heeft dan de standaardnaam in Photoshop.

      * **[!UICONTROL Photoshop and layer name]** : geeft de afbeeldingen een naam na het PSD-bestand, gevolgd door de laagnaam of het laagnummer. Het laagnummer wordt gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen zijn. Een laag met de naam `Price Tag` in een PSD-bestand met de naam `SpringAd` krijgt bijvoorbeeld de naam `Spring Ad_Price Tag` . Een laag met de standaardnaam Laag 2 wordt genoemd `Spring Ad_2`.

   * **[!UICONTROL Anchor]**: geef op hoe afbeeldingen worden verankerd in sjablonen die worden gegenereerd op basis van de laagsamenstelling die uit het PSD-bestand is samengesteld. Standaard is het anker het middelpunt. Met een middelste anker kunt u afbeeldingen vervangen die het beste dezelfde ruimte kunnen vullen, ongeacht de hoogte-breedteverhouding van de vervangende afbeelding. Afbeeldingen met een ander aspect dat deze afbeelding vervangt, nemen bij het verwijzen naar de sjabloon en het gebruik van parametervervanging in feite dezelfde ruimte in. Schakel over naar een andere instelling als de vervangende afbeeldingen de toegewezen ruimte in de sjabloon moeten vullen.

## Lagen weergeven en bewerken in een PSD-bestand {#viewing-and-editing-layers-in-a-psd-file}

Als u de optie **[!UICONTROL Maintain Layers]** hebt geselecteerd bij het uploaden van uw PSD, heeft Adobe Dynamic Media Classic de afzonderlijke lagen omgezet in elementen. U kunt de elementlagen die bij een PSD-bestand horen weergeven en bewerken door het bestand te openen in het deelvenster Bladeren in de gedetailleerde weergave.

>[!NOTE]
>
>Adobe Dynamic Media Classic ondersteunt maximaal vijf niveaus in een geneste laaggroep.

1. Dubbelklik op het volledige PSD-bestand in het deelvenster Bladeren. Het bestand wordt geopend in de gedetailleerde weergave.

   >[!NOTE]
   >
   >Open het volledige element en niet een van de PSD-lagen.

1. Selecteer **[!UICONTROL Layers]** . Alle lagen worden als afzonderlijke afbeeldingen weergegeven in het deelvenster Lagen.
1. Dubbelklik op een laag en voer een van de volgende handelingen uit:

   * Als u een afbeelding met hyperlinks op de laag wilt maken, selecteert u het pictogram **[!UICONTROL Image Map]** . (Zie [&#x200B; de Kaarten van het Beeld creëren &#x200B;](creating-image-maps.md#creating_image_maps).)
   * Als u zoomdoelen op de laag wilt maken, selecteert u het pictogram **[!UICONTROL Zoom Targets]** . (Zie [&#x200B; Doelen van het Gezoem voor Geleide Gezoem &#x200B;](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom) creëren.)
   * Als u de laag wilt uitsnijden, selecteert u het pictogram **[!UICONTROL Crop]** . (Zie [&#x200B; uitsnijden een beeld &#x200B;](cropping-image.md#cropping_an_image).)
   * Selecteer **[!UICONTROL Sharpen]** als u de laag wilt verscherpen. (Zie [&#x200B; een beeld &#x200B;](sharpening-image.md#sharpening_an_image) verscherpen.)
   * Selecteer **[!UICONTROL Adjust]** als u de laag wilt aanpassen. (Zie [&#x200B; een beeld &#x200B;](adjusting-image.md#adjusting_an_image) aanpassen.)

1. Selecteer **[!UICONTROL Save]** of **[!UICONTROL Save As]** .
1. Als u een andere laag wilt weergeven of bewerken, selecteert u een pijl onder aan de voorvertoning van de laag.
1. Als u de weergave Laagdetails wilt afsluiten, selecteert u het pictogram **[!UICONTROL Grid View]** .
