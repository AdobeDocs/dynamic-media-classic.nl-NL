---
title: URL's koppelen aan uw webtoepassing
description: Leer hoe u URL's aan uw webtoepassing koppelt.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: Zakelijke praktiserer
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---


# URL&#39;s koppelen aan uw webtoepassing{#linking-urls-to-your-web-application}

Uw websites en toepassingen hebben toegang tot Dynamic Media Image Server-inhoud via URL-tekenreeksen. Nadat u een afbeelding hebt gepubliceerd, activeert Dynamic Media Classic een URL-tekenreeks die verwijst naar de voorinstelling van de afbeelding op Dynamic Media Image Servers. U kunt deze URL&#39;s voor testdoeleinden in een webbrowser plakken.

Kopieer deze URL-tekenreeksen vanuit Dynamic Media Classic om deze in uw webpagina&#39;s en toepassingen te plaatsen. Als u een URL-tekenreeks wilt ophalen die is gegenereerd met een voorinstelling voor afbeelding, gaat u naar het voorvertoningsscherm of het deelvenster Bladeren (in de gedetailleerde weergave).

## Een URL voor een voorinstelling voor afbeeldingen verkrijgen {#obtaining-an-image-preset-url}

U kunt een URL-tekenreeks die is gegenereerd door een voorinstelling voor afbeelding, opvragen in de voorvertoning of in de detailweergave. Nadat u de URL hebt gekopieerd, landt deze op het Klembord, zodat u deze desgewenst kunt plakken.

***Opmerking **: De URL is pas actief als u het element publiceert.*

### Een voorinstellings-URL voor afbeeldingen verkrijgen via Voorvertoning {#obtaining-an-image-preset-url-from-preview}

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de mappen Middelen die het afbeeldingselement bevatten waarvan u een voorvertoning wilt weergeven.
1. Voer een van de volgende handelingen uit:

   * Klik rechts van de werkbalk boven het middelenvenster op Rasterweergave. Selecteer in het venster Middelen één afbeeldingselement en klik vervolgens onder de miniatuurafbeelding op Voorvertoning > Lijst met voorinstellingen afbeelding.
   * Klik rechts van de werkbalk boven het middelenvenster op Lijstweergave. Selecteer in het venster Middelen één afbeeldingselement en klik vervolgens rechts van de miniatuurafbeelding op Voorvertoning > Lijst met voorinstellingen afbeelding.
   * Klik rechts van de werkbalk boven het middelenvenster op Gedetailleerde weergave. Klik op dezelfde werkbalk op Voorvertoning > Lijst met voorinstellingen afbeelding.

1. (Optioneel) Selecteer in het venster Lijst met voorinstellingen afbeelding in de vervolgkeuzelijst URL-codering voor URL-generatie kopiëren onderaan de URL-codering die u wilt toepassen op de URL van het afbeeldingselement wanneer dit wordt gekopieerd.
1. Klik in het venster Lijst met voorinstellingen afbeelding rechtsboven in het voorvertoningsvenster op URL kopiëren voor het geselecteerde type voorinstelling.
1. Klik in de rechterbenedenhoek van het venster Lijst met voorinstellingen afbeelding op Sluiten om terug te keren naar het scherm Middelen.

### Een URL met voorinstellingen voor afbeeldingen verkrijgen in het deelvenster Bladeren {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de mappen Middelen die het afbeeldingselement bevatten waarvan u een voorvertoning wilt weergeven.
1. Klik rechts van de werkbalk boven het middelenvenster op Rasterweergave. Selecteer in het venster Middelen één afbeeldingselement.
1. Klik rechts van de werkbalk boven het middelenvenster op Gedetailleerde weergave.
1. Klik op URL&#39;s in het deelvenster aan de rechterkant van het scherm om de lijst met voorinstellingen voor afbeeldingen te ontvouwen.
1. Klik op de koppeling URL kopiëren naast de naam van de voorinstelling Afbeelding met de URL die u naar het klembord wilt kopiëren.

## Informatie over URL-tekenreeksen met voorinstellingen afbeelding {#about-image-preset-url-strings}

Een URL-aanroep naar Afbeeldingsgrootte op Dynamic Media Image Servers heeft de volgende basissyntaxis:

*pad*/*naam van afbeeldingsserver*/*accountnaam*/*afbeeldingsnaam*?*modifier1*&amp;*modifier2*&amp;..

In een URL van de Server van het Beeld van Dynamic Media, verschijnen de instructies aan de server voor het tonen van het beeld na het vraagteken (?). Deze URL-aanroep levert bijvoorbeeld een afbeelding met de naam &quot;backpack&quot; met een breedte van 250 pixels:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Een URL met voorinstellingen voor afbeeldingen bevat alle wijziginginstructies voor het weergeven van de afbeelding met de juiste grootte en opmaakspecificaties. Zonder vooraf ingesteld Beeld, merk alle bepalingsinstructies na het vraagteken (?) op in deze URL-tekenreeks:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

In een URL-tekenreeks die is gegenereerd met een voorinstelling voor afbeelding, wordt echter de naam van de voorinstelling voor afbeelding weergegeven in plaats van de instructies die zijn gedefinieerd door de voorinstelling voor afbeelding. Onder verwijzing naar de lange URL hierboven is de URL-tekenreeks bijvoorbeeld:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Namen van voorinstellingen voor afbeeldingen in URL&#39;s worden ingesloten door dollartekens ($). Wanneer een Dynamic Media Image Server het gedeelte met voorinstellingen voor afbeelding van de URL aantreft (in dit geval de `Large`), waarbij de instructies voor grootte en opmaak worden gebruikt die zijn gedefinieerd door de voorinstelling voor grote afbeeldingen.

## Dynamische afbeeldingen toevoegen aan uw webpagina {#adding-dynamic-images-to-your-web-page}

Als u dynamische afbeeldingen aan uw webpagina wilt toevoegen, wordt de `<IMG>`-tag in uw HTML-webpaginacode doorgaans gewijzigd met de klassieke URL-tekenreeks van Dynamic Media om een aanvraag in te dienen bij Dynamic Media Image Servers. Met deze tekenreeks wordt de afbeelding gemaakt met de grootte en opmaakspecificaties die zijn gedefinieerd in de voorinstelling voor afbeelding.

Bijvoorbeeld, in plaats van de typische vraag om een statische beeld zoals te openen

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

u gebruikt nu de tag `<IMG>`om de verwijzing naar een statische afbeelding te vervangen door een aanroep van een voorinstelling voor afbeeldingen naar het Dynamic Media Classic-platform. Een steekproefvraag kijkt als dit:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In dit voorbeeld &#39;zoekt&#39; een Dynamic Media Image Server de definitie van `$thumbnail$` en genereert dynamisch de juiste afbeelding met de specificaties voor grootte en opmaak die zijn gedefinieerd door de `thumbnail`Voorinstelling afbeelding. In een URL-tekenreeks worden alle items behalve de bestandsnaam van de productafbeelding ( `backpack_trns` in dit geval) doorgaans voor de paginasjabloon vastgezet. Het enige element dat automatisch in het paginasjabloon van uw handelsserver wordt opgenomen is IPS identiteitskaart of naam van het beeld.
