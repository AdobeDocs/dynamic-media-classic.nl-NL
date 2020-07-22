---
title: Afbeeldingskaarten maken
seo-title: Afbeeldingskaarten maken
description: 'null'
seo-description: Leer hoe u afbeeldingen met hyperlinks maakt.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '2444'
ht-degree: 0%

---


# Afbeeldingskaarten maken{#creating-image-maps}

Een afbeelding met hyperlinks is een gebied in een afbeelding, een eCatalog-pagina of een afbeelding in een SpinSet waarin een rollover-deelvenster met tekst wordt weergegeven. Wanneer de gebruiker op een afbeelding met hyperlinks klikt, wordt een handeling van een bepaalde aard geactiveerd. Er wordt bijvoorbeeld een webpagina gestart zodat de gebruiker meer over een product kan leren. Als u de aandacht wilt vestigen op Afbeeldingen met hyperlinks, verschijnt er een omtrek rond een afbeelding met hyperlinks wanneer de gebruiker de aanwijzer erboven plaatst.

Naast de mogelijkheid om een afbeelding met hyperlinks te maken in Dynamic Media Classic, kunt u ook afbeeldingen met hyperlinks maken wanneer u een catalogus ontwerpt in Adobe Acrobat of Adobe InDesign.

Wanneer u Afbeeldingen met hyperlinks maakt, kunt u een van de volgende handelingen uitvoeren:

* Voer rollovertekst in.
* Voer JavaScript en URL&#39;s in om webpagina&#39;s te starten.
* Maak URL-sjablonen voor afbeeldingen met hyperlinks.
* Kopieer Afbeeldingskaarten naar andere afbeeldingen of eCatalog-pagina&#39;s of SpinSets.
* Afbeeldingen met hyperlinks exporteren naar CSV of XML.
* Metagegevens van afbeeldingen importeren vanuit een door tabs gescheiden bestand of vanuit een XML-bestand.
* Bepaal andere acties zoals die door het Consortium van World Wide Web worden bepaald.
* Voorvertoning van afbeeldingen met hyperlinks.

## Een afbeelding met hyperlinks tekenen en aanpassen {#drawing-and-adjusting-an-image-map}

1. Voer een van de volgende handelingen uit:

   * Als u met een afbeelding werkt in de rasterweergave of lijstweergave, klikt u in de vervolgkeuzelijst Bewerken op **Afbeeldingskaart**. U kunt de afbeelding ook openen in de gedetailleerde weergave en vervolgens op **Afbeeldingskaart** boven de afbeelding klikken.
   * Als u werkt met een SpinSet in de rasterweergave of lijstweergave, klikt u op **Bewerken**. U kunt het ook openen in de gedetailleerde weergave en vervolgens op **Bewerken** klikken. Selecteer een afbeeldingselement en klik op **Afbeeldingskaart**.
   * Als u met een eCatalog, in de Mening van het Net, de Mening van de Lijst, de Mening van het Detail werkt, klik **uitgeven**. Klik op het tabblad **Pagina&#39;s** toewijzen.

   ![](assets/ma_image_map.png)

1. Teken een rechthoekige of veelhoekige (veelzijdige) afbeelding met hyperlinks:

   **Rechthoekige kaart** Selecteer het gereedschap Rechthoekafbeelding met hyperlinks en sleep op de pagina om de rechthoek te maken. Als u een punt wilt toevoegen aan een rechthoekige kaart (en het dus wilt wijzigen in een veelhoekige kaart), drukt u op Ctrl, plaatst u het invoeggereedschap op de gewenste locatie en klikt u.

   **Veelhoekkaart** Selecteer het gereedschap Veelhoekafbeelding met hyperlinks en klik op punten op de rand van het gebied van de afbeelding dat u wilt insluiten. Gebruik de schuifregelaar voor veelhoekdichtheid om de puntdichtheid in de veelhoek te variëren. De oorspronkelijke dichtheid wordt onthouden als u andere kaarten selecteert. Als een punt wordt toegevoegd, verwijderd of verplaatst in de veelhoek, gaat de oorspronkelijke dichtheid verloren en wordt de schuifregelaar ingesteld op de maximale waarde.

1. Voer desgewenst een naam voor de afbeelding met hyperlinks in de lijst Afbeeldingskaart in. Nadat u een Kaart van het Beeld tekent, wijst de Classic van Dynamic Media het een naam toe.

   Om de naam te maken, voegt de Klassieke Dynamic Media een opeenvolgend aantal aan de naam van het beeld of de eCatalogpagina toe u met werkt. U kunt een naam van uw keuze invoeren.

1. Als u wilt dat gebruikers een nieuwe webpagina openen wanneer zij op Afbeeldingskaart klikken, voert u de URL in de lijst Afbeeldingskaart in.

   Zie JavaScript en URL&#39;s [invoeren](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Als u rollovertekst wilt weergeven wanneer gebruikers de aanwijzer over de Afbeeldingskaart bewegen, voert u de tekst in de lijst Afbeeldingskaart in. Selecteer in de lijst Afbeeldingskaart het menu Tonen en kies Rollover-tekst. Voer vervolgens de tekst in die gebruikers op het scherm moeten zien. U kunt de tekst in een tekstverwerker schrijven en het kopiëren in het de tekstgebied van het Omvergooien.
1. Als u een ander actieeffect wilt voorkomen wanneer de gebruikers de muis over een Kaart van het Beeld bewegen, bepaal de actie. Klik in de vervolgkeuzelijst Tonen op Overige handelingen. Voer de kenmerken van de handeling in. (Klik op Tonen > Beide om rollovertekst en een handeling voor een afbeelding met hyperlinks te maken.)

   Zie Andere handelingen [definiëren voor afbeeldingen met hyperlinks](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Optioneel) Voer een van de volgende handelingen uit:

   * Klik op Voorvertoning om een voorvertoning van afbeeldingen met hyperlinks weer te geven.
   * Als u een afbeelding met hyperlinks of een veelhoekpunt wilt verwijderen, selecteert u een vorm in de afbeelding en klikt u op Verwijderen. Of klik voor een eCatalog op het tabblad Order Pages op Kaarten wissen om de afbeeldingen met hyperlinks van alle pagina&#39;s te verwijderen.
   * Als u een afbeelding met hyperlinks tijdelijk uit een afbeelding, een afbeelding in een SpinSet of een eCatalog-pagina wilt verwijderen zonder deze te verwijderen, schakelt u de desbetreffende optie Op in de lijst Afbeeldingskaart uit.

1. Klik op Opslaan.

### De positie, vorm en grootte van afbeeldingskaarten aanpassen {#adjusting-the-position-shape-and-size-of-image-maps}

Als u de positie, vorm en grootte van een afbeelding met hyperlinks wilt wijzigen, selecteert u de knop Afbeelding met hyperlinks. Selecteer vervolgens het gereedschap Pannen en volg de volgende instructies:

**Wijzigende positie** Verplaats de aanwijzer naar de rand van de afbeelding met hyperlinks, maar niet naar de rand van de afbeelding met hyperlinks. Als u het pictogram met de vier pijlpunten ziet, sleept u de kaart naar een nieuwe locatie.

**Het wijzigen van de grootte en de vorm** Hoe u de vorm en de grootte van een Afbeeldingskaart wijzigt, hangt af van het feit of u met een rechthoekige of veelhoekige afbeelding met hyperlinks werkt:

***Tip **: U kunt de schuifregelaar Grootte onder aan het scherm verslepen om de weergave te wijzigen en uw afbeelding met hyperlinks beter te bekijken.*

**Rechthoekige afbeelding met hyperlinks** Plaats de aanwijzer boven een zijde of hoek van de afbeelding met hyperlinks. Wanneer u het pictogram met de dubbele pijl ziet, begint u te slepen. Houd Shift ingedrukt terwijl u sleept om de grootte te wijzigen, maar de hoogte-breedteverhouding (de vorm) te behouden.

**Veelhoekige afbeelding met hyperlinks** Sleep een vierkante selectiegreep. Als u een selectiegreep wilt maken, klikt u op de rand van de afbeelding met hyperlinks en begint u te slepen.

### Overlappende afbeeldingen met hyperlinks verwerken {#handling-overlapping-image-maps}

Als uw afbeelding of eCatalog-pagina meer dan één afbeelding met hyperlinks bevat en de afbeeldingen overlappen, kunt u bepalen hoe de afbeeldingen overlappen. Wijzig hiertoe de volgorde van de afbeeldingen in de lijst Afbeeldingskaart. Sleep hun namen hoger of lager in de lijst. Hoe hoog een naam op de lijst is bepaalt of zijn Kaart van het Beeld andere Kaarten van het Beeld overlapt.

### Afbeeldingskaartgegevens importeren {#importing-image-map-data}

In plaats van de gegevens van de Kaart van het Beeld op elke pagina in te gaan, kunt u de gegevens voor uw beeld, de Reeks van de Rotatie, of eCatalog in het Summiere scherm van de Kaart invoeren. U importeert de gegevens van de Kaart van het Beeld in de vorm van een lusje-afgebakend dossier of van XML DTD. De velden in het bestand moeten in de volgorde staan die wordt weergegeven in het scherm Kaartoverzicht: Naam, labels voor inhoudsopgave, Kaarten, URL&#39;s, Rollover-tekst, Overige handelingen en Zoeken. Door de gegevens van de Kaart van het Beeld in te voeren bespaart u het probleem om de gegevens in de Lijst van de Kaart van het Beeld in te gaan aangezien u elke Kaart van het Beeld creeert.

**Afbeeldingskaartgegevens importeren**

1. Ga naar de de redacteurspagina van de Kaart van het Beeld (voor beelden of beelden in SpinSets) of het lusje van de Pagina&#39;s van de Kaart van het eCatalog het uitgeven scherm.
1. Klik op Metagegevens importeren.
1. Klik in het dialoogvenster Metagegevens uploaden op Afbeelding of Afbeeldingskaart om de metagegevens van het gewenste type elementeigenschap te uploaden.
1. Selecteer in de vervolgkeuzelijst Bestand genereren het type bestand dat u wilt maken.
1. (Optioneel) Klik op Genereren om een voorvertoning van de resulterende gegevens weer te geven op basis van het type bestand dat u wilt maken. Klik op Sluiten om terug te keren naar het dialoogvenster Metagegevens uploaden.
1. Blader naar het bestand dat u wilt uploaden. Geef in het tekstveld Bestandsnaam de naam van het gegenereerde bestand op.
1. (Optioneel) Geef in het veld Taaknaam een naam op voor de uploadtaak voor metagegevens.
1. Klik op Uploaden.

### Afbeeldingen met hyperlinks kopiëren {#copying-image-maps}

U kunt afbeeldingen met hyperlinks kopiëren van een afbeelding of van een eCatalog-pagina naar een andere. Gebruik Afbeeldingskaart kopiëren om een head start met het maken ervan. U kunt Afbeeldingskaarten ook kopiëren en opnieuw maken in afbeeldingen of pagina&#39;s met dezelfde layout- of toewijzingsstructuur.

Het kopiëren van afbeeldingen met hyperlinks in een eCatalog is bijvoorbeeld een handige manier om alle afbeeldingen met hyperlinks te kopiëren naar andere versies in dezelfde eCatalog. Voor de beste resultaten is kopiëren het meest succesvol als u kopieert tussen eCatalogi met hetzelfde aantal pagina&#39;s en dezelfde afbeeldingen. Als de eCatalog waarnaar u kopieert reeds Kaarten van het Beeld bevat, me ervan bewust ben dat die Kaarten van het Beeld worden geschrapt wanneer het exemplaar wordt gemaakt.

**Afbeeldingen met hyperlinks kopiëren**

1. Ga naar de de redacteurspagina van de Kaart van het Beeld (voor beelden of beelden in SpinSets) of het lusje van de Pagina&#39;s van de Kaart van het eCatalog het uitgeven scherm.
1. Klik op Kaarten kopiëren naar.
1. Voer een van de volgende handelingen uit op basis van het feit of u afbeeldingen met hyperlinks kopieert of afbeeldingen met hyperlinks kopieert uit een eCatalog:

   * (Afbeeldingen) Selecteer in het scherm Afbeeldingen selecteren de afbeeldingen waarnaar u de Afbeeldingen met hyperlinks wilt kopiëren.
   * (eCatalog) Selecteer in het scherm Select Asset de afbeeldingen of eCatalog-pagina&#39;s waarnaar u de Afbeeldingen met hyperlinks wilt kopiëren.

1. Klik op Selecteren.

## Een sjabloon gebruiken om JavaScript en URL&#39;s in te voeren {#using-a-template-to-enter-javascript-and-urls}

U kunt een URL-sjabloon (ook wel een Href-sjabloon genoemd) definiëren om het invoeren van URL&#39;s voor afbeeldingen met hyperlinks eenvoudiger en efficiënter te maken. Definieer een URL-sjabloon als de meeste URL&#39;s van de Afbeeldingskaart een gemeenschappelijke, vaste indeling hebben. Door het gedeelte van URL in te voeren dat als malplaatje URL vast is, moet u niet dit gedeelte van URL ingaan telkens als u een Kaart van het Beeld creeert. Uw URL-sjabloon kan ook JavaScript-opdrachten, -padnamen en -parameters bevatten. Standaard bevat de URL-sjabloon een merkgebonden Dynamic Media Classic JavaScript-handler met de naam `loadProduct` waarmee de afbeelding in een nieuw venster wordt geopend.

>[!NOTE]
>
>Houd er rekening mee dat wanneer u de Javascript-code toevoegt aan het HREF-kenmerk van de afbeeldingskaart, de code wordt uitgevoerd op de computer van de client. Zorg daarom dat de JavaScript-code veilig is.

### Over URL-sjablonen {#about-url-templates}

De URL-sjabloon werkt door de inhoud van de URL-kolom in de lijst Afbeeldingskaart te vervangen door de dubbele dollartekens (&#39;$$&#39;) in de sjabloon:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

U plaatst alle waarden die niet tussen Afbeeldingen met hyperlinks veranderen in het malplaatje URL. Voeg alleen de waarden toe die wel veranderen in de URL-kolom in de lijst Afbeelding met hyperlinks. Bijvoorbeeld:

* URL-sjabloon: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL-waarde: `product.htm`
* Werkelijke URL gegenereerd: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Standaard bevat de URL-sjabloon een merkgebonden Dynamic Media Classic JavaScript-handler met de naam `loadProduct` waarmee een nieuw venster met de URL-bestemming wordt geopend. U kunt echter elke JavaScript-code gebruiken om deze JavaScript-handler te vervangen of een van de volgende klassieke Dynamic Media-handlers gebruiken:

* `loadProductCW`

   Hiermee geeft u het URL-doel weer dat is opgegeven in de kolom URL in het huidige venster. Deze handler is vooral bedoeld voor eCatalogi die zijn geïntegreerd in een pagina binnen een website.

* `loadProductPW`

   Hiermee geeft u het URL-doel weer dat is opgegeven in de URL-kolom in het bovenliggende venster (de pagina die de huidige URL heeft geopend). Het huidige venster blijft geopend, maar het bovenliggende venster verandert om het URL-doel weer te geven.

   ***opmerking **: De handler biedt`loadProductPW`geen ondersteuning voor DHTML- en HTML5-viewers.*

### Creating a URL template {#creating-a-url-template}

Een URL-sjabloon maken:

1. Selecteer Bewerken naast de optie URL-sjabloon in het scherm Kaarteditor (afbeeldingen of SpinSets) of op het tabblad Kaartpagina&#39;s van het eCatalog-scherm (eCatalogs). Het dialoogvenster Kaartsjabloon bewerken wordt geopend.
1. Voer de JavaScript-code en de volledige URL in (waarbij het gedeelte van de variabele wordt vervangen door het dollarteken [$$]). U kunt de code plakken door met de rechtermuisknop te klikken en Plakken te kiezen.
1. Selecteer de knop Opslaan.

### URL-sjablonen afhandelen {#handling-url-templates}

De pagina Kaarteditor (afbeeldingen en SpinSets) en het tabblad Kaartpagina&#39;s van het eCatalog-scherm (eCatalogs) bieden de volgende opdrachten voor de verwerking van URL-sjablonen:

**Met de optie** URL-sjabloon selecteert u de optie URL-sjabloon om uw URL-sjabloon toe te passen op alle afbeeldingen met hyperlinks op een afbeelding of een eCatalog-pagina.

**Sjabloonoptie** Schakel een sjabloonoptie uit in de lijst URL-afbeeldingskaart als u niet wilt dat een afzonderlijke afbeelding met hyperlinks de URL-sjabloon gebruikt.

## Andere handelingen voor afbeeldingen met hyperlinks definiëren {#defining-other-actions-for-image-maps}

U kunt het menu Tonen selecteren en Andere handelingen kiezen om andere handelingen dan rollovertekst en het starten van een webpagina te activeren. Wanneer de gebruiker de aanwijzer boven een Afbeeldingskaart plaatst, kunt u een handeling starten. Deze acties zijn attributen die voor cliënt-kant de Kaarten van het Beeld door de specificaties van HTML van het Consortium van World Wide Web worden bepaald. Deze omvatten:

**Toegangssleutel** activeert een actie wanneer de gebruiker op een bepaalde toets op het toetsenbord drukt.

**onfocus** activeert een gebeurtenis wanneer de Kaart van het Beeld nadruk-door de curseur, door met de Tab-toets, of door een toegangssleutel te drukken ontvangt. U kunt bijvoorbeeld een webpagina starten wanneer de afbeelding met hyperlinks de focus krijgt en sluiten wanneer de afbeelding met hyperlinks de focus verliest.

**Bij onvervagen** wordt een gebeurtenis geactiveerd wanneer de afbeelding met hyperlinks de focus verliest. Dit kan door de cursor of door een Tab-toets te gebruiken.

**Andere handelingen voor afbeeldingen met hyperlinks definiëren**

1. Selecteer in het scherm Kaarteditor (afbeeldingen en SpinSets) of het tabblad Kaartpagina&#39;s van het eCatalog-scherm (eCatalogs) het menu Tonen en kies Overige handelingen.
1. Gebruikend de syntaxis die door de specificaties van HTML van het Consortium van World Wide Web wordt gespecificeerd, voeg de gesteunde attributen in de Andere kolom van Acties van de Lijst van de Kaart van het Beeld toe.
1. Klik op **Opslaan**.

Selecteer het menu Tonen en kies Beide als u een afbeelding met hyperlinks en een handeling wilt weergeven.

## Afbeeldingskaarten maken in Adobe Acrobat of Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

U kunt afbeeldingen met hyperlinks maken terwijl u uw eCatalog ontwerpt in Adobe Acrobat of Adobe InDesign.

Maak in Acrobat of InDesign hyperlinkverwijzingen waar u de afbeeldingen met hyperlinks wilt weergeven en geef de URL-locaties op voor de afbeelding met hyperlinks. Als u de optie Koppelingen extraheren selecteert wanneer u het PDF-bestand uploadt naar Dynamic Media Classic, worden de koppelingen naar afbeeldingen met hyperlinks automatisch geconverteerd.

Raadpleeg de Help bij InDesign of Acrobat voor meer informatie.

### Afbeeldingskaarten maken in Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. Klik in InDesign op Venster > Interactief > Hyperlinks om het deelvenster Hyperlinks te openen.
1. Selecteer de tekst, het kader of de afbeelding die u in de Afbeeldingskaart wilt maken.
1. Klik in het deelvenster Hyperlinks op Nieuwe hyperlink in het deelvenstermenu.
1. Kies in het dialoogvenster Nieuwe hyperlink de optie URL in het menu Koppelen naar.
1. Typ of plak de product-id in het vak URL en klik op OK. (Met Dynamic Media Klassiek wordt de URL voltooid met de sjabloon URL van afbeelding met hyperlinks.)

   >[!NOTE]
   >
   >U hoeft geen weergaveopties in te stellen in InDesign. U kunt vormgeving opgeven in Dynamic Media Classic.

1. Herhaal stap 2 tot en met 5 voor alle afbeeldingen met hyperlinks die u wilt maken.
1. Exporteer het bestand als een PDF-bestand.
1. Upload de PDF naar Dynamic Media Classic en selecteer Koppelingen extraheren uit de PDF-opties.

### Afbeeldingen met hyperlinks maken in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Kies in Acrobat Gereedschappen > Geavanceerd bewerken > Koppeling.
1. Sleep om de afbeelding met hyperlinks te maken. Het vak Koppeling maken wordt geopend.
1. Selecteer Eigen koppeling en klik op Volgende.

   ***opmerking **: U hoeft geen weergaveopties in te stellen in Acrobat. U kunt vormgeving opgeven in Dynamic Media Classic.*

1. Klik in het vak Koppelingseigenschappen op Handelingen.
1. Selecteer Een webkoppeling openen in het menu Handeling selecteren en klik op Toevoegen.
1. Typ de product-id voor de afbeelding met hyperlinks in het vak URL bewerken en klik op OK. (Met Dynamic Media Classic wordt de URL voltooid met de URL-sjabloon voor de afbeeldingskaart.)
1. Herhaal stap 1 tot en met 7 voor alle afbeeldingen met hyperlinks die u wilt maken.
1. Sla het bestand op.
1. Upload de PDF naar Dynamic Media Classic en selecteer Koppelingen extraheren uit de PDF-opties.

