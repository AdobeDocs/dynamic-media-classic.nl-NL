---
title: URL's koppelen aan uw webtoepassing
description: Leer hoe u URL's vanuit Adobe Dynamic Media Classic aan uw webtoepassing koppelt.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# URL&#39;s koppelen aan uw webtoepassing{#linking-urls-to-your-web-application}

Uw websites en toepassingen hebben toegang tot Dynamic Media Image Server-inhoud via URL-tekenreeksen. Nadat u een afbeelding hebt gepubliceerd, activeert Adobe Dynamic Media Classic een URL-tekenreeks die verwijst naar de voorinstelling Afbeelding op Dynamic Media Image Servers. U kunt deze URL&#39;s voor testdoeleinden in een webbrowser plakken.

Als u deze URL-tekenreeksen wilt plaatsen in uw webpagina&#39;s en toepassingen, kopieert u ze van Adobe Dynamic Media Classic. Als u een URL-tekenreeks wilt ophalen die is gegenereerd met een voorinstelling voor afbeelding, gaat u naar het voorvertoningsscherm of het deelvenster Bladeren (in de gedetailleerde weergave).

## Een URL met voorinstellingen afbeelding verkrijgen {#obtaining-an-image-preset-url}

U kunt een URL-tekenreeks die is gegenereerd door een voorinstelling voor afbeelding, opvragen in de voorvertoning of in de detailweergave. Nadat u de URL hebt gekopieerd, landt deze op het Klembord, zodat u deze desgewenst kunt plakken.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

### Een vooraf ingestelde URL voor afbeeldingen verkrijgen via Voorvertoning {#obtaining-an-image-preset-url-from-preview}

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de mappen Middelen die het afbeeldingselement bevatten waarvan u een voorvertoning wilt weergeven.
1. Voer een van de volgende handelingen uit:

   * Selecteer **[!UICONTROL Grid View]** rechts van de werkbalk boven het middelenvenster. Selecteer in het venster Middelen één afbeeldingselement en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Selecteer **[!UICONTROL List View]** rechts van de werkbalk boven het middelenvenster. Selecteer in het venster Middelen één afbeeldingselement en ga vervolgens rechts van de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Selecteer **[!UICONTROL Detail View]** rechts van de werkbalk boven het middelenvenster. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.

1. (Optioneel) Selecteer in de lijst Voorinstellingen afbeelding in de vervolgkeuzelijst URL-codering voor URL-generatie kopiëren de URL-codering die u wilt toepassen op de URL van het afbeeldingselement wanneer dit wordt gekopieerd.
1. Selecteer **[!UICONTROL Copy URL]** voor het geselecteerde type voorinstelling in het venster Lijst met voorinstellingen afbeelding rechtsboven in het voorvertoningsvenster.
1. Selecteer **[!UICONTROL Close]** in de rechterbenedenhoek van het venster Lijst met voorinstellingen afbeelding om terug te keren naar het scherm Middelen.

### Een vooraf ingestelde URL voor afbeeldingen verkrijgen via het deelvenster Bladeren {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de mappen Middelen die het afbeeldingselement bevatten waarvan u een voorvertoning wilt weergeven.
1. Selecteer **[!UICONTROL Grid View]** rechts van de werkbalk boven het middelenvenster. Selecteer in het venster Middelen één afbeeldingselement.
1. Selecteer **[!UICONTROL Detail View]** rechts van de werkbalk boven het middelenvenster.
1. Selecteer **[!UICONTROL URLs]** op het paneel op de rechterkant van het scherm zodat kunt u de lijst van vooraf ingestelde Beeld ontvouwen.
1. Selecteer **[!UICONTROL Copy URL]** koppeling naast de naam van de voorinstelling Afbeelding met de URL die u naar het klembord wilt kopiëren.

## Over URL-tekenreeksen met voorinstellingen afbeelding {#about-image-preset-url-strings}

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

## Dynamische afbeeldingen aan uw webpagina toevoegen {#adding-dynamic-images-to-your-web-page}

Als u dynamische afbeeldingen aan uw webpagina wilt toevoegen, wordt de `<IMG>`-tag in de HTML-webpaginacode doorgaans gewijzigd met de Klassieke URL-tekenreeks van Adobe Dynamic Media om een aanvraag in te dienen bij Dynamic Media Image Servers. Met deze tekenreeks wordt de afbeelding gemaakt met de grootte en opmaakspecificaties die zijn gedefinieerd in de voorinstelling voor afbeelding.

Bijvoorbeeld, in plaats van de typische vraag om een statische beeld zoals te openen

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

U gebruikt nu de tag `<IMG>`om de verwijzing naar een statische afbeelding te vervangen door een aanroep van Voorinstellingen afbeelding naar het Klassieke platform van Adobe Dynamic Media. Een steekproefvraag kijkt als dit:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In dit voorbeeld &#39;zoekt&#39; een Dynamic Media Image Server de definitie van `$thumbnail$` en genereert dynamisch de juiste afbeelding met de specificaties voor grootte en opmaak die zijn gedefinieerd door de `thumbnail`Voorinstelling afbeelding. In een URL-tekenreeks worden alle items behalve de bestandsnaam van de productafbeelding ( `backpack_trns` in dit geval) doorgaans voor de paginasjabloon vastgezet. Het enige element dat automatisch in het paginasjabloon van uw handelsserver wordt opgenomen is IPS identiteitskaart of naam van het beeld.
