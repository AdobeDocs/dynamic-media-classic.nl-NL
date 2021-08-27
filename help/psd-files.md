---
title: Werken met PSD-bestanden
description: Leer hoe u met PSD-bestanden werkt in Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Werken met PSD-bestanden{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (Photoshop Document files) worden meestal gebruikt in Adobe Dynamic Media Classic om sjablonen te maken. Wanneer u een PSD-bestand uploadt, kunt u automatisch een Adobe Dynamic Media Classic-sjabloon maken vanuit het bestand (selecteer de optie Sjabloon maken in het scherm Uploaden).

Adobe Dynamic Media Classic maakt meerdere afbeeldingen van een PSD-bestand met lagen als u het bestand gebruikt om een sjabloon te maken. er wordt één afbeelding voor elke laag gemaakt.

## Opties voor uploaden naar PSD {#psd-upload-options}

De opties voor het uploaden van PSD-bestanden bevinden zich onder Photoshop-opties in het dialoogvenster Opties voor uploaden. U kunt een bestand uitsnijden, een kleurprofiel kiezen, het gebruiken om een sjabloon te maken en een anker selecteren.

Deze opties zijn beschikbaar wanneer u PSD-bestanden uploadt:

* **Opties voor**  uitsnijden - bevindt zich onder  **[!UICONTROL Crop Options]**. Selecteer **[!UICONTROL Trim]** om witruimte vanaf de randen van een PSD-bestand automatisch uit te snijden. Selecteer **[!UICONTROL Manual]** om zijden van het PSD-bestand uit te snijden:

   * **[!UICONTROL Trim]** - Selecteer het  **[!UICONTROL Trim Away Based On]** menu en kies  **[!UICONTROL Color]** of  **[!UICONTROL Transparency]**.

      Als u de optie **[!UICONTROL Color]** kiest, selecteert u het menu Hoek en kiest u de hoek van het PSD-bestand met de kleur die het beste overeenkomt met de kleur voor de witruimte die u wilt uitsnijden.

      Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven. Als u wilt bijsnijden op basis van kleur, geeft u 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de PSD hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe. Als u wilt bijsnijden op basis van transparantie, geeft u 0 op om alleen pixels bij te snijden als deze transparant zijn. De cijfers dichter aan 1 staan voor meer transparantie.

   * **[!UICONTROL Manual]** - Voer het aantal pixels in dat u wilt uitsnijden vanaf elke zijde van de afbeelding. Hoeveel van de afbeelding wordt uitgesneden, is afhankelijk van de ppi-instelling (pixels per inch) in het afbeeldingsbestand. Als de afbeelding bijvoorbeeld 150 ppi weergeeft en u 75 ppi invoert in de tekstvakken Boven, Rechts, Onder en Links, wordt aan elke zijde van de afbeelding een halve inch bijgesneden.

* **Opties**  voor kleurprofiel - bevindt zich onder  **[!UICONTROL Color Profile Options]**.

   * **[!UICONTROL Default Color Preservation]**

   * **[!UICONTROL Keep Original Color Space]** - Behoudt de oorspronkelijke kleurruimte van de afbeelding.

   * **[!UICONTROL Custom From]** >  **[!UICONTROL To]** - Hiermee opent u menu&#39;s, zodat u een optie kunt kiezen voor Omzetten van en Omzetten in kleurruimte. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u hebt geüpload naar Adobe Dynamic Media Classic. Zie [ICC-profielen](/help/icc-profiles.md).

* **Photoshop-opties**

   * **[!UICONTROL Maintain Layers]** - Hiermee worden de lagen in de PSD (indien aanwezig) naar afzonderlijke elementen verplaatst. De elementlagen blijven gekoppeld aan de PSD. U kunt deze weergeven door het PSD-bestand te openen in de gedetailleerde weergave en het deelvenster Lagen te selecteren. Zie Lagen weergeven en bewerken in een PSD-bestand.

   * **[!UICONTROL Create Template]** - Hiermee maakt u een sjabloon op basis van de lagen in het PSD-bestand.

   * **[!UICONTROL Extract Text]** - Extraheert de tekst zodat gebruikers naar tekst in een viewer kunnen zoeken.

   * **[!UICONTROL Extend Layers To Background Size]** - Hiermee vergroot u de grootte van de uitgesneden afbeeldingslagen tot de grootte van de achtergrondlaag.

   * **[!UICONTROL Layer Naming]** - Lagen in het PSD-bestand worden geüpload als afzonderlijke afbeeldingen. Kies een van de volgende opties om deze afbeeldingen een naam te geven in Adobe Dynamic Media Classic:

      * **[!UICONTROL Layer Name]** - De afbeeldingen krijgen een naam na hun laagnamen in het PSD-bestand. Een laag met de naam Prijscode in het oorspronkelijke PSD-bestand wordt bijvoorbeeld een afbeelding met de naam Prijscode. Als de laagnamen in het PSD-bestand echter standaard Photoshop-laagnamen zijn (Achtergrond, Laag 1, Laag 2, enzovoort), krijgen de afbeeldingen een naam na hun laagnummers in het PSD-bestand. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop and layer number]** - De afbeeldingen krijgen een naam na hun laagnummer in het PSD-bestand, waarbij de namen van de oorspronkelijke lagen worden genegeerd. Afbeeldingen krijgen de naam Photoshop en een toegevoegd laagnummer. De tweede laag van een bestand met de naam `Spring Ad.psd` krijgt bijvoorbeeld de naam `Spring Ad_2`, zelfs als het bestand een andere naam heeft dan de standaardnaam in Photoshop.

      * **[!UICONTROL Photoshop and layer name]** - De afbeeldingen krijgen een naam na het PSD-bestand, gevolgd door de laagnaam of het laagnummer. Het laagnummer wordt gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen zijn. Een laag met de naam `Price Tag` in een PSD-bestand met de naam `SpringAd` krijgt bijvoorbeeld de naam `Spring Ad_Price Tag`. Een laag met de standaardnaam Laag 2 wordt genoemd `Spring Ad_2`.
   * **[!UICONTROL Anchor]** - Geef op hoe afbeeldingen worden verankerd in sjablonen die worden gegenereerd op basis van de laagcompositie die uit het PSD-bestand is samengesteld. Standaard is het anker het middelpunt. Met een middelste anker kunnen vervangende afbeeldingen dezelfde ruimte het beste vullen, ongeacht de hoogte-breedteverhouding van de vervangende afbeelding. Afbeeldingen met een ander aspect dat deze afbeelding vervangt, nemen bij het verwijzen naar de sjabloon en het gebruik van parametervervanging in feite dezelfde ruimte in. Schakel over naar een andere instelling als de vervangende afbeeldingen de toegewezen ruimte in de sjabloon moeten vullen.


## Lagen weergeven en bewerken in een PSD-bestand {#viewing-and-editing-layers-in-a-psd-file}

Als u tijdens het uploaden van de PSD de optie Lagen behouden hebt geselecteerd, heeft Adobe Dynamic Media Classic de afzonderlijke lagen in elementen gerangschikt. U kunt de elementlagen die bij een PSD-bestand horen weergeven en bewerken door het bestand te openen in het deelvenster Bladeren in de gedetailleerde weergave.

1. Dubbelklik op het volledige PSD-bestand in het deelvenster Bladeren. Het bestand wordt geopend in de gedetailleerde weergave.

   >[!NOTE]
   >
   >Zorg ervoor dat u het volledige element opent en niet een van de PSD-lagen.

1. Selecteer **[!UICONTROL Layers]**. Alle lagen worden als afzonderlijke afbeeldingen weergegeven in het deelvenster Lagen.
1. Dubbelklik op een laag en voer een van de volgende handelingen uit:

   * Als u een afbeelding met hyperlinks op de laag wilt maken, selecteert u **[!UICONTROL Image Map]**-pictogram. (Zie [Afbeeldingskaarten maken](creating-image-maps.md#creating_image_maps).)
   * Selecteer **[!UICONTROL Zoom Targets]** pictogram om zoomdoelen op de laag te maken. (Zie [Zoomdoelen maken voor Bewerken met instructies-zoomfunctie](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Als u de laag wilt uitsnijden, selecteert u **[!UICONTROL Crop]**-pictogram. (Zie [Een afbeelding uitsnijden](cropping-image.md#cropping_an_image).)
   * Selecteer **[!UICONTROL Sharpen]** om de laag te verscherpen. (Zie [Een afbeelding verscherpen](sharpening-image.md#sharpening_an_image).)
   * Selecteer **[!UICONTROL Adjust]** om de laag aan te passen. (Zie [Een afbeelding aanpassen](adjusting-image.md#adjusting_an_image).)

1. Selecteer **[!UICONTROL Save]** of **[!UICONTROL Save As]**.
1. Als u een andere laag wilt weergeven of bewerken, selecteert u een pijl onder aan de voorvertoning van de laag.
1. Als u de weergave Laagdetails wilt afsluiten, selecteert u het pictogram **[!UICONTROL Grid View]**.
