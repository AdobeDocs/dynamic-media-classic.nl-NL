---
title: 'Werken met PSD-bestanden '
description: Leer hoe u met PSD-bestanden werkt.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic, beheer van bedrijfsmiddelen
role: Business Practitioner
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# Werken met PSD-bestanden {#working-with-psd-files}

PSD (Photoshop Document files) worden meestal gebruikt in Dynamic Media Classic om sjablonen te maken. Wanneer u een PSD-bestand uploadt, kunt u automatisch een klassieke Dynamic Media-sjabloon maken vanuit het bestand (selecteer de optie Sjabloon maken in het scherm Uploaden).

Dynamic Media Classic maakt meerdere afbeeldingen van een PSD-bestand met lagen als u het bestand gebruikt om een sjabloon te maken. er wordt één afbeelding voor elke laag gemaakt.

## Opties voor PSD-upload {#psd-upload-options}

De opties voor het uploaden van PSD-bestanden bevinden zich onder Photoshop-opties in Opties voor uploaden. U kunt een bestand uitsnijden, een kleurprofiel kiezen, het gebruiken om een sjabloon te maken en een anker selecteren.

Deze opties zijn beschikbaar wanneer u PSD-bestanden uploadt:

**Uitsnijden**  (bevindt zich onder Opties voor uitsnijden.) Kies Bijsnijden om de witruimte aan de randen van een PSD-bestand automatisch bij te snijden. Kies Handmatig om zijden van het PSD-bestand uit te snijden:

**** BijsnijdenSelecteer het menu Wegsnijden op basis van en kies Kleur of Transparantie.

Als u de optie Kleur kiest, selecteert u het menu Hoek en kiest u de hoek van het PSD-bestand met de kleur die het beste overeenkomt met de kleur van de witruimte die u wilt uitsnijden.

Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven:

Als u wilt bijsnijden op basis van kleur, geeft u 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de PSD hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

Als u wilt bijsnijden op basis van transparantie, geeft u 0 op om alleen pixels bij te snijden als deze transparant zijn. De cijfers dichter aan 1 staan voor meer transparantie.

* **Handmatig**  - Voer het aantal pixels in dat u wilt uitsnijden vanaf een zijde of elke zijde van de afbeelding. Hoeveel van de afbeelding wordt uitgesneden, is afhankelijk van de ppi-instelling (pixels per inch) in het afbeeldingsbestand. Als de afbeelding bijvoorbeeld 150 ppi weergeeft en u 75 ppi invoert in de tekstvakken Boven, Rechts, Onder en Links, wordt aan elke zijde van de afbeelding een halve inch bijgesneden.

* **Kleurprofiel**  - (bevindt zich onder Opties kleurprofiel.) Kies een optie:

* **Omzetten in sRGB (standaard)**  - Omzetten in sRGB (standaard rood-groen blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

* **Oorspronkelijke kleurruimte**  behouden - Behoudt de oorspronkelijke kleurruimte van de afbeelding.

* **Aangepast van > naar**  - opent menu&#39;s zodat u een Omzetten van en Omzetten in kleurenruimte kunt kiezen. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Dynamic Media Classic hebt geüpload. Zie ICC-profielen.

* **Lagen**  behouden - Hiermee worden de lagen in de PSD (indien aanwezig) in afzonderlijke elementen geplaatst. De elementlagen blijven gekoppeld aan de PSD. U kunt deze weergeven door het PSD-bestand te openen in de gedetailleerde weergave en het deelvenster Lagen te selecteren. Zie Lagen weergeven en bewerken in een PSD-bestand.

* **Sjabloon**  maken - hiermee maakt u een sjabloon op basis van de lagen in het PSD-bestand.

* **Tekst**  uitnemen - extraheert de tekst zodat gebruikers naar tekst in een viewer kunnen zoeken.

* **Lagen uitbreiden naar achtergrondgrootte**  - hiermee wordt de grootte van de uitgesneden afbeeldingslagen uitgebreid tot de grootte van de achtergrondlaag.

* **Laagnaamgeving**  - Lagen in het PSD-bestand worden geüpload als afzonderlijke afbeeldingen. Kies een van de volgende opties om deze afbeeldingen een naam te geven in Dynamic Media Classic:

* **Laagnaam**  - De afbeeldingen krijgen een naam achter de laagnamen in het PSD-bestand. Een laag met de naam Prijscode in het oorspronkelijke PSD-bestand wordt bijvoorbeeld een afbeelding met de naam Prijscode. Als de laagnamen in het PSD-bestand echter standaard Photoshop-laagnamen zijn (Achtergrond, Laag 1, Laag 2, enzovoort), krijgen de afbeeldingen een naam na hun laagnummers in het PSD-bestand, niet na hun standaardlaagnamen.

* **Photoshop en Laagnummer**  - De afbeeldingen krijgen een naam na hun laagnummers in het PSD-bestand, waarbij de oorspronkelijke laagnamen worden genegeerd. Afbeeldingen krijgen de naam Photoshop en een toegevoegd laagnummer. De tweede laag van een bestand met de naam Voorjaar-Ad.psd krijgt bijvoorbeeld de naam Voorjaar-Ad_2, zelfs als deze in Photoshop een andere naam heeft dan de standaardnaam.

* **Photoshop en Laagnaam**  - De afbeeldingen krijgen een naam na het PSD-bestand, gevolgd door de laagnaam of het laagnummer. Het laagnummer wordt gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen zijn. Een laag met de naam Prijstag in een PSD-bestand met de naam SpringAd krijgt bijvoorbeeld de naam Spring Ad_Price Tag. Een laag met de standaardnaam Laag 2 wordt genoemd Lente Ad_2.

* **Anker**  - Geef op hoe afbeeldingen worden verankerd in sjablonen die worden gegenereerd op basis van de laagsamenstelling die uit het PSD-bestand is samengesteld. Standaard is het anker het middelpunt. Met een middelste anker kunnen vervangende afbeeldingen dezelfde ruimte het beste vullen, ongeacht de hoogte-breedteverhouding van de vervangende afbeelding. Afbeeldingen met een ander aspect dat deze afbeelding vervangt, nemen bij het verwijzen naar de sjabloon en het gebruik van parametervervanging in feite dezelfde ruimte in. Schakel over naar een andere instelling als de vervangende afbeeldingen de toegewezen ruimte in de sjabloon moeten vullen.

## Lagen weergeven en bewerken in een PSD-bestand {#viewing-and-editing-layers-in-a-psd-file}

Als u bij het uploaden van de PSD de optie Lagen behouden hebt geselecteerd, heeft Dynamic Media Classic de afzonderlijke lagen in elementen bijgesneden. U kunt de elementlagen die bij een PSD-bestand horen weergeven en bewerken door het bestand te openen in het deelvenster Bladeren in de gedetailleerde weergave.

1. Dubbelklik op het volledige PSD-bestand in het deelvenster Bladeren om het te openen in de gedetailleerde weergave.

   >[!NOTE]
   >
   >Zorg ervoor dat u het volledige element opent en niet een van de PSD-lagen.

1. Klik op **[!UICONTROL Layers]**. Alle lagen worden als afzonderlijke afbeeldingen weergegeven in het deelvenster Lagen.
1. Dubbelklik op een laag om deze te openen en voer een van de volgende handelingen uit:

   * Als u een afbeelding met hyperlinks op de laag wilt maken, klikt u op het pictogram **[!UICONTROL Image Map]**. (Zie [Afbeeldingskaarten maken](creating-image-maps.md#creating_image_maps).)
   * Als u zoomdoelen op de laag wilt maken, klikt u op het pictogram **[!UICONTROL Zoom Targets]**. (Zie [Zoomdoelen maken voor Bewerken met instructies-zoomfunctie](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Als u de laag wilt uitsnijden, klikt u op het pictogram **[!UICONTROL Crop]**. (Zie [Een afbeelding uitsnijden](cropping-image.md#cropping_an_image).)
   * Klik op **[!UICONTROL Sharpen]** om de laag te verscherpen. (Zie [Een afbeelding verscherpen](sharpening-image.md#sharpening_an_image).)
   * Klik op **[!UICONTROL Adjust]** om de laag aan te passen. (Zie [Een afbeelding aanpassen](adjusting-image.md#adjusting_an_image).)

1. Klik op **[!UICONTROL Save]** of **[!UICONTROL Save As]**.
1. Als u een andere laag wilt weergeven of bewerken, klikt u op een pijl onder aan de voorvertoning van de laag.
1. Klik op het pictogram van de rasterweergave om de weergave Laagdetails af te sluiten.
