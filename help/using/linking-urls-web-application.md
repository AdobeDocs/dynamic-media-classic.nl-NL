---
title: URL's koppelen aan uw webtoepassing
description: Leer hoe u URL's kunt koppelen aan uw webtoepassing vanuit Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 0%

---

# URL&#39;s koppelen aan uw webtoepassing{#linking-urls-to-your-web-application}

Uw websites en toepassingen hebben toegang tot de inhoud van Dynamic Media Image Server via URL-tekenreeksen. Nadat u een afbeelding hebt gepubliceerd, activeert Adobe Dynamic Media Classic een URL-tekenreeks die verwijst naar de voorinstelling Afbeelding op Dynamic Media Image Servers. U kunt deze URL&#39;s in een webbrowser plakken om ze te testen.

Kopieer deze URL-tekenreeksen vanuit Adobe Dynamic Media Classic om deze in uw webpagina&#39;s en toepassingen te plaatsen. Als u een URL-tekenreeks wilt ophalen die is gegenereerd met een voorinstelling voor afbeelding, gaat u naar het voorvertoningsscherm of het deelvenster Bladeren (in de gedetailleerde weergave).

## Een URL met voorinstellingen afbeelding verkrijgen {#obtaining-an-image-preset-url}

U kunt een URL-tekenreeks die is gegenereerd door een voorinstelling voor afbeelding, opvragen in de voorvertoning of in de detailweergave. Nadat u de URL hebt gekopieerd, landt deze op het Klembord, zodat u deze desgewenst kunt plakken.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

### Een vooraf ingestelde URL voor afbeeldingen verkrijgen via Voorvertoning {#obtaining-an-image-preset-url-from-preview}

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de map Asset die het afbeeldingselement bevat waarvan u een voorvertoning wilt weergeven.
1. Voer een van de volgende handelingen uit:

   * Selecteer **[!UICONTROL Grid View]** boven het Assets-venster rechts op de werkbalk. Selecteer in het venster Middelen één afbeeldingselement en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]** .
   * Selecteer **[!UICONTROL List View]** boven het Assets-venster rechts op de werkbalk. Selecteer in het venster Middelen één afbeeldingselement en ga vervolgens naar **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]** rechts van de miniatuurafbeelding.
   * Selecteer **[!UICONTROL Detail View]** boven het Assets-venster rechts op de werkbalk. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]** .

1. (Optioneel) Selecteer in de lijst Voorinstellingen afbeelding in de vervolgkeuzelijst URL-codering voor URL-generatie kopiëren de URL-codering die u op de URL van het afbeeldingselement wilt toepassen wanneer het element wordt gekopieerd.
1. Selecteer in de rechterbovenhoek van het voorvertoningsvenster van het venster Lijst met voorinstellingen afbeelding de optie **[!UICONTROL Copy URL]** voor het geselecteerde type voorinstelling.
1. Selecteer **[!UICONTROL Close]** in de rechterbenedenhoek van het venster Lijst met voorinstellingen afbeelding om terug te keren naar het Assets-scherm.

### Een vooraf ingestelde URL voor afbeeldingen verkrijgen via het deelvenster Bladeren {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de map Asset die het afbeeldingselement bevat waarvan u een voorvertoning wilt weergeven.
1. Selecteer **[!UICONTROL Grid View]** boven het Assets-venster rechts op de werkbalk. Selecteer in het venster Middelen één afbeeldingselement.
1. Selecteer **[!UICONTROL Detail View]** boven het Assets-venster rechts op de werkbalk.
1. Selecteer **[!UICONTROL URLs]** in het deelvenster aan de rechterkant van het scherm, zodat u de lijst met voorinstellingen voor afbeeldingen kunt uitvouwen.
1. Selecteer **[!UICONTROL Copy URL]** naast de naam van de voorinstelling Afbeelding met de URL die u naar het klembord wilt kopiëren.

## Over URL-tekenreeksen met voorinstellingen afbeelding {#about-image-preset-url-strings}

Een URL-aanroep voor Afbeeldingsgrootte tot Dynamische Media Image Servers heeft de volgende basissyntaxis:

*weg*/*naam van de Server van het Beeld*/ *rekeningsnaam*/ *beeldnaam*?*modifier1* &amp;*modifier2* &amp;..

In een URL van een Dynamic Media Image Server worden instructies aan de server voor het weergeven van de afbeelding weergegeven na het vraagteken (?). Deze URL-aanroep levert bijvoorbeeld een afbeelding met de naam &quot;backpack&quot; met een breedte van 250 pixels:

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

Namen van voorinstellingen voor afbeeldingen in URL&#39;s worden ingesloten door dollartekens ($). Wanneer een server van het Beeld van het Beeld van de Dynamische Media het Beeld vooraf ingestelde gedeelte van URL (`Large` in dit geval) ontmoet, gebruikend de grootte en het formatteren instructies die door de &quot;Grote&quot;Vooraf ingestelde Beeld worden bepaald.

## Dynamische afbeeldingen toevoegen aan uw webpagina {#adding-dynamic-images-to-your-web-page}

Wanneer u dynamische afbeeldingen aan uw webpagina toevoegt, wordt de tag `<IMG>` in de HTML-paginacode doorgaans gewijzigd met de Adobe Dynamic Media Classic URL-tekenreeks om een aanvraag in te dienen bij Dynamic Media Image Servers. Met deze tekenreeks wordt de afbeelding gemaakt met de grootte en opmaakspecificaties die zijn gedefinieerd in de voorinstelling voor afbeelding.

Bijvoorbeeld, in plaats van de typische vraag om een statische beeld zoals te openen

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

U gebruikt nu de `<IMG>` markering om de verwijzing naar een statisch beeld met een Beeld te vervangen vooraf ingestelde vraag aan het platform van Adobe Dynamic Media Classic. Een steekproefvraag kijkt als dit:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

In dit voorbeeld, &quot;kijkt de Dynamische Server van het Beeld van Media omhoog&quot;de definitie van `$thumbnail$` en produceert dynamisch het aangewezen beeld met het rangschikken en het formatteren specificaties die door het `thumbnail` Vooraf ingestelde Beeld worden bepaald. In een URL-tekenreeks worden alle items behalve de bestandsnaam van de productafbeelding ( `backpack_trns` in dit geval) doorgaans voor de paginasjabloon vastgezet. Het enige element dat automatisch in het paginasjabloon van uw handelsserver wordt opgenomen is IPS identiteitskaart of naam van het beeld.
