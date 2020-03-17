---
title: 'Werken met PSD-bestanden '
seo-title: 'Werken met PSD-bestanden '
description: 'null'
seo-description: Leer hoe u met PSD-bestanden werkt.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Werken met PSD-bestanden {#working-with-psd-files}

PSD (Photoshop-documentbestanden) wordt meestal gebruikt in Dynamic Media Classic om sjablonen te maken. Wanneer u een PSD-bestand uploadt, kunt u automatisch vanuit het bestand een klassieke sjabloon voor dynamische media maken (selecteer de optie Sjabloon maken in het scherm Uploaden).

SPS leidt tot veelvoudige beelden van een Psd- dossier met lagen als u het dossier gebruikt om een malplaatje tot stand te brengen; er wordt één afbeelding voor elke laag gemaakt.

## Opties voor uploaden naar PSD {#psd-upload-options}

De opties voor het uploaden van PSD-bestanden bevinden zich onder Photoshop-opties in Opties voor uploaden. U kunt een bestand uitsnijden, een kleurprofiel kiezen, het gebruiken om een sjabloon te maken en een anker selecteren.

Deze opties zijn beschikbaar wanneer u PSD-bestanden uploadt:

**Uitsnijden** (bevindt zich onder Opties voor uitsnijden.) Kies Bijsnijden om de witruimte aan de randen van een PSD-bestand automatisch bij te snijden. Kies Handmatig om zijden van het PSD-bestand uit te snijden:

**Bij te snijden** selecteert u het menu Wegsnijden op basis van en kiest u Kleur of Transparantie.

Als u de optie Kleur kiest, selecteert u het menu Hoek en kiest u de hoek van het PSD-bestand met de kleur die het beste overeenkomt met de kleur van de witruimte die u wilt uitsnijden.

Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven:

Als u wilt bijsnijden op basis van kleur, geeft u 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de PSD hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

Als u wilt bijsnijden op basis van transparantie, geeft u 0 op voor het bijsnijden van pixels, alleen als deze volledig transparant zijn. De cijfers dichter aan 1 staan voor meer transparantie.

**Met Handmatig** geeft u het aantal pixels op dat u aan elke zijde van de afbeelding wilt uitsnijden. Hoeveel van de afbeelding wordt uitgesneden, is afhankelijk van de ppi-instelling (pixels per inch) in het afbeeldingsbestand. Als de afbeelding bijvoorbeeld 150 ppi weergeeft en u 75 ppi invoert in de tekstvakken Boven, Rechts, Onder en Links, wordt aan elke zijde van de afbeelding een halve inch bijgesneden.

**Kleurprofiel** (bevindt zich onder Opties voor kleurprofiel.) Kies een optie:

**Omzetten in sRGB (standaard)** Omzetten in sRGB (standaard rood-groen blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

**De oorspronkelijke kleurruimte** behouden blijft de oorspronkelijke kleurruimte van de afbeelding.

**Kies Aangepast van > naar** om de menu&#39;s te openen, zodat u de optie Omzetten van en Omzetten in kleurruimte kunt kiezen. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar SPS hebt geüpload. Zie ICC-profielen.

**Met Lagen** behouden worden de lagen in de PSD (indien aanwezig) verdeeld over afzonderlijke elementen. De elementlagen blijven gekoppeld aan de PSD. U kunt deze weergeven door het PSD-bestand te openen in de gedetailleerde weergave en het deelvenster Lagen te selecteren. Zie Lagen weergeven en bewerken in een PSD-bestand.

**Met Sjabloon** maken maakt u een sjabloon op basis van de lagen in het PSD-bestand.

**Tekst** extraheren extraheert de tekst zodat gebruikers naar tekst in een viewer kunnen zoeken.

**Lagen uitbreiden naar achtergrondgrootte** breidt de grootte van uitgesneden afbeeldingslagen uit tot de grootte van de achtergrondlaag.

**Lagen met een laagnaam** in het PSD-bestand worden geüpload als afzonderlijke afbeeldingen. Kies een optie om deze beelden in het het Publiceren Scene7 Systeem te noemen:

**De naam** van de laag noemt de beelden na hun laagnamen in het Psd- dossier. Een laag met de naam Prijscode in het oorspronkelijke PSD-bestand wordt bijvoorbeeld een afbeelding met de naam Prijscode. Als de laagnamen in het PSD-bestand echter standaardnamen van Photoshop-lagen zijn (Achtergrond, Laag 1, Laag 2, enzovoort), krijgen de afbeeldingen een naam na hun laagnummers in het PSD-bestand en niet na hun standaardlaagnamen.

**Photoshop en het Aantal** van de Laag noemen de beelden na hun laagaantallen in het Psd- dossier, negerend originele laagnamen. Afbeeldingen krijgen de naam Photoshop en een bijgevoegd laagnummer. De tweede laag van een bestand met de naam Lente-advertentie.psd krijgt bijvoorbeeld de naam Lente-advertentie_2, zelfs als deze in Photoshop een andere naam heeft dan de standaardnaam.

**Photoshop en Laagnaam** geven de afbeeldingen een naam na het PSD-bestand, gevolgd door de laagnaam of het laagnummer. Het laagnummer wordt gebruikt als de laagnamen in het PSD-bestand standaardnamen van Photoshop-lagen zijn. Een laag met de naam Prijstag in een PSD-bestand met de naam SpringAd krijgt bijvoorbeeld de naam Spring Ad_Price Tag. Een laag met de standaardnaam Laag 2 wordt genoemd Lente Ad_2.

**Anker** geeft op hoe afbeeldingen worden verankerd in sjablonen die worden gegenereerd op basis van de laagsamenstelling die uit het PSD-bestand is samengesteld. Standaard is het anker het middelpunt. Met een middelste anker kunnen vervangende afbeeldingen dezelfde ruimte het beste vullen, ongeacht de hoogte-breedteverhouding van de vervangende afbeelding. Afbeeldingen met een ander aspect dat deze afbeelding vervangt, nemen bij het verwijzen naar de sjabloon en het gebruik van parametervervanging in feite dezelfde ruimte in. Schakel over naar een andere instelling als de vervangende afbeeldingen de toegewezen ruimte in de sjabloon moeten vullen.

## Lagen weergeven en bewerken in een PSD-bestand {#viewing-and-editing-layers-in-a-psd-file}

Als u bij het uploaden van de PSD de optie Lagen behouden hebt geselecteerd, worden de afzonderlijke lagen door Dynamic Media Classic bijgesneden in elementen. U kunt de elementlagen die bij een PSD-bestand horen weergeven en bewerken door het bestand te openen in het deelvenster Bladeren in de gedetailleerde weergave.

1. Dubbelklik op het volledige PSD-bestand in het deelvenster Bladeren om het te openen in de gedetailleerde weergave.

   ***opmerking **: Zorg ervoor dat u het volledige element opent en niet een van de PSD-lagen.*

1. Klik op Lagen om het deelvenster Lagen te openen. Alle lagen worden als afzonderlijke afbeeldingen weergegeven in het deelvenster Lagen.
1. Dubbelklik op een laag om deze te openen en voer een van de volgende handelingen uit:

   * Klik op het pictogram Afbeelding met hyperlinks om een afbeelding met hyperlinks op de laag te maken. (Zie [Afbeeldingskaarten](creating-image-maps.md#creating_image_maps)maken.)
   * Klik op het pictogram Zoomdoelen om zoomdoelen op de laag te maken. (Zie Zoomdoelen [maken voor zoomen](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)met instructies.)
   * Klik op het pictogram Uitsnijden om de laag uit te snijden. (Zie Een afbeelding [](cropping-image.md#cropping_an_image)uitsnijden.)
   * Klik op Verscherpen om de laag te verscherpen. (Zie Een afbeelding [](sharpening-image.md#sharpening_an_image)verscherpen.)
   * Klik op Aanpassen om de laag aan te passen. (Zie Een afbeelding [aanpassen](adjusting-image.md#adjusting_an_image).)

1. Klik op Opslaan of Opslaan als.
1. Als u een andere laag wilt weergeven of bewerken, klikt u op een pijl onder aan de voorvertoning van de laag.
1. Klik op het pictogram van de rasterweergave om de weergave Laagdetails af te sluiten.
