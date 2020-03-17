---
title: DOM-manipulatie
seo-title: DOM-manipulatie
description: 'null'
seo-description: Meer informatie over DOM-manipulatie.
uuid: 275cd49d-2a55-41f9-80b0-e147d0cd2907
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 890ca93e-3146-4347-864b-bd5e94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# DOM-manipulatie{#dom-manipulation}

manipulatie met DOM (Document Object Model) is een techniek voor het bewerken van een ontwerpbestand door de XML-code ervan rechtstreeks te bewerken. Met DOM-manipulatie hebt u meer controle over elementen die variabel ontwerp bevatten, zoals het wijzigen van de inhoud en de weergave ervan. u kunt zelfs nieuwe elementen op een zonodig basis tot stand brengen.

Met Dynamic Media Classic kunt u het DOM van een Dynamic Media Classic FXG-sjabloon manipuleren met behulp van URL-opdrachten nadat de sjabloon is gepubliceerd. De elementen van het ontwerp in het malplaatje FXG worden gemanipuleerd door bevelen door URL over te gaan. Op deze manier kunt u op dynamische wijze kenmerken bewerken en toevoegen aan afbeeldingen.

Als u DOM-manipulatie wilt gebruiken, maakt u s7:elementID&#39;s in uw Illustrator-bestand voordat u het omzet in een Dynamic Media Classic FXG-bestand en uploadt u het bestand naar SPS.

>[!NOTE]
>
>Als u DOM-manipulatieopdrachten gebruikt, moeten alle doorgegeven waarden URL-gecodeerd zijn.

>[!NOTE]
>
>Illustrator-plug-in voor web-to-print (voor het converteren van Illustrator-bestanden) wordt omgezet in FXG 2.0. Zie [www.adobe.com/go/learn_s7_fxg2_en voor meer informatie over deze specificatie](https://www.adobe.com/go/learn_s7_fxg2_en).

## s7 maken:elementID&#39;s in Illustrator-bestanden {#creating-s-elementids-in-illustrator-files}

Als u DOM-manipulatie wilt gebruiken met een ontwerp dat in Illustrator is gemaakt, maakt u s7:elementID&#39;s in uw Illustrator-ontwerp. Als u s7:elementID&#39;s maakt, kunnen ontwerpelementen worden gewijzigd met URL-opdrachten nadat de sjabloon is gepubliceerd.

### s7 maken:elementID&#39;s voor DOM-bewerking van tekst {#creating-s-elementids-for-dom-manipulation-of-text}

Als u een s7:elementID voor DOM-bewerking van een tekstobject wilt maken, opent u het deelvenster Lagen in Illustrator. Geef vervolgens op de tekstlaag die variabele tekst bevat, de laag een naam met s7:elementID. Voer daartoe de letters `id` (ter identificatie), een dubbele punt ( `:`) en een naam in. Hier volgen voorbeelden van namen van tekstlagen s7:elementID:

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### s7 maken:elementID&#39;s voor DOM-bewerking van objecten {#creating-s-elementids-for-dom-manipulation-of-objects}

Maak s7:elementIDs voor objecten wanneer u wilt dat eindgebruikers de kenmerken van objecten kunnen wijzigen. Objecten kunnen hele tekstkaders, afbeeldingen en afbeeldingen zijn. Een kleurenachtergrond is een voorbeeld van een object-element-id. Naarmate de seizoenen veranderen, kan de eindgebruiker de achtergrondkleur van een poster omwisselen om de poster passend te maken voor het seizoen.

Maak een aparte laag voor het object voordat u een s7:element-id maakt voor een object in Illustrator.

Ga als volgt te werk om een s7:elementID voor een object in Illustrator te maken:

1. Selecteer het object.
1. Klik op **Venster** > **Lagen**.
1. Geef in het deelvenster Lagen de objectlaag een naam met een s7:elementID. Voer daartoe de letters `id` (ter identificatie), een dubbele punt ( `:`) en een beschrijving in om het element te identificeren. Hier volgen voorbeelden van namen van s7:elementID-objectlagen:

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## FXG-sjablonen publiceren {#publish-fxg-templates}

Als u uw FXG-sjabloon publiceert, wordt deze op de Dynamic Media Classic-servers geplaatst, waar deze beschikbaar zijn voor uw website en toepassing. Tijdens het het publiceren proces, activeert het het Publiceren Scene7 Systeem URLs u voor uw website of toepassing nodig hebt.

>[!NOTE]
>
>Als u uw FXG-sjabloon wilt gebruiken, publiceert u alle inhoud die u eraan hebt toegevoegd, inclusief lettertypen en afbeeldingen. Als u niet alle vereiste bestanden opneemt, verschijnt er een foutbericht wanneer u publiceert.

### FXG-sjablonen markeren voor publicatie {#mark-fxg-templates-for-publish}

Sjablonen en alle bijbehorende ondersteuningsbestanden moeten zijn gemarkeerd voor publicatie zodat ze op Dynamic Media Image Servers kunnen worden geplaatst.

1. Selecteer in het deelvenster Bladeren de FXG-sjabloon samen met de gebruikte afbeeldingen, afbeeldingen en lettertypen.
1. Klik op **Markeren voor publiceren**.

### Uw FXG-sjabloon publiceren {#publish-your-fxg-template}

1. Klik op **Publiceren** op de algemene navigatiebalk.
1. Selecteer een optie bij en voer desgewenst een naam voor de publicatietaak in.
1. Klik op Publiceren **starten**.

### Weergave overloopindicator tekst {#text-overflow-indicator-display}

Een *indicator* voor tekstoverloop geeft aan wanneer de tekst de ruimte overschrijdt die voor de tekst is toegewezen in een tekstkader (of in het laatste tekstkader bij verbonden tekst). De indicator is een rood vak met daarin een plusteken. De indicatoren van de tekstoverloop op SPS worden altijd toegelaten.

De indicatoren van de tekstoverloop worden gecontroleerd met de `markOverflowingTextFrame` bepaling. Gebruik de optie als volgt:

| Modifier/Values | Beschrijving |
|--- |--- |
| markOverflowTextFrame=0,1 | Met de waarde 1 worden tekstflowindicatoren weergegeven. De standaardwaarde is 0. (Hoewel het gebrek 0 is, worden de indicatoren van de tekstoverloop in SPS altijd toegelaten.) Merk op dat de markOverflowsTextFrame bepaling case-sensitive is. |

>[!MORELIKETHIS]
>
>* [Variabiliteit definiëren: Parameterization versus DOM manipulatie](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publiceren](publishing-files.md#publishing_files)

