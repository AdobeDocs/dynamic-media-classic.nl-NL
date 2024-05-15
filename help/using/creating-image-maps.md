---
title: Afbeeldingen met hyperlinks maken
description: Leer hoe u afbeeldingen met hyperlinks maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 0%

---

# Afbeeldingen met hyperlinks maken {#creating-image-maps}

Een afbeelding met hyperlinks is een gebied op een afbeelding, een eCatalog-pagina of een afbeelding in een SpinSet waarin een rollover-deelvenster met tekst wordt weergegeven. Wanneer de gebruiker een Kaart van het Beeld selecteert, wordt een actie van één of andere soort teweeggebracht. Er wordt bijvoorbeeld een webpagina gestart zodat de gebruiker meer over een product kan leren. Er verschijnt een omtrek rond een afbeelding met hyperlinks wanneer de gebruiker de aanwijzer erboven plaatst.

Naast de mogelijkheid om afbeeldingen met hyperlinks te maken in Adobe Dynamic Media Classic, kunt u ook afbeeldingen met hyperlinks maken wanneer u een catalogus ontwerpt in Adobe Acrobat of Adobe InDesign.

Wanneer u Afbeeldingskaarten maakt, kunt u het volgende doen:

* Voer rollovertekst in.
* Voer JavaScript en URL&#39;s in om webpagina&#39;s te starten.
* Maak URL-sjablonen voor afbeeldingen met hyperlinks.
* Kopieer Afbeeldingskaarten naar andere afbeeldingen of eCatalog-pagina&#39;s of SpinSets.
* Afbeeldingen met hyperlinks exporteren naar CSV of XML.
* Importeer metagegevens van een afbeelding uit een door tabs gescheiden bestand of uit een XML-bestand.
* Bepaal Andere Acties zoals die door het Consortium van World Wide Web worden bepaald.
* Afbeeldingen met hyperlinks voorvertonen.

## Een afbeelding met hyperlinks tekenen en aanpassen {#drawing-and-adjusting-an-image-map}

1. Voer een van de volgende handelingen uit:

   * Als u met een afbeelding werkt in de rasterweergave of lijstweergave, selecteert u in de vervolgkeuzelijst Bewerken de optie **[!UICONTROL Image Map]**. Of open het in de Gedetailleerde Mening, en selecteer dan **[!UICONTROL Image Map]** boven de afbeelding.
   * Als u met een SpinSet werkt in de rasterweergave of lijstweergave, selecteert u **[!UICONTROL Edit]**. Of open het in de Gedetailleerde Mening, en selecteer dan **[!UICONTROL Edit]**. Selecteer een afbeeldingselement en selecteer vervolgens **[!UICONTROL Image Map]**.
   * Als u met een eCatalog werkt, in de Mening van het Net, de Mening van de Lijst, de Mening van het Detail, selecteert **[!UICONTROL Edit]**. Selecteer de **[!UICONTROL Map Pages]** tab.

   ![Afbeelding met hyperlinks illustratie](assets/ma_image_map.png)

1. Teken een rechthoekige of veelhoekige (veelzijdige) afbeelding met hyperlinks:

   * **Rechthoekige kaart**: Selecteer het gereedschap Afbeeldingskaart rechthoek en sleep op de pagina om de rechthoek te maken. Als u een punt wilt toevoegen aan een rechthoekige kaart (en het dus wilt wijzigen in een veelhoekige kaart), drukt u op Ctrl en plaatst u het invoeggereedschap op de gewenste locatie en selecteert u.

   * **Veelhoekige kaart**: Selecteer het gereedschap Veelhoekafbeelding met hyperlinks en selecteer punten op de rand van het gebied van de afbeelding dat u wilt insluiten. Gebruik de schuifregelaar voor veelhoekdichtheid om de puntdichtheid in de veelhoek te variëren. De oorspronkelijke dichtheid wordt onthouden als u andere kaarten selecteert. Als een punt wordt toegevoegd, verwijderd of verplaatst in de veelhoek, gaat de oorspronkelijke dichtheid verloren. De schuifregelaar wordt teruggezet op de maximale waarde.

1. Voer desgewenst een naam voor de afbeelding met hyperlinks in de lijst Afbeeldingskaart in. Nadat u een afbeelding met hyperlinks hebt getekend, wijst Adobe Dynamic Media Classic er een naam aan toe.

   Om de naam te maken, voegt Adobe Dynamic Media Classic een volgnummer toe aan de naam van de afbeelding of de eCatalog-pagina waarmee u werkt. U kunt een naam van uw keuze invoeren.

1. Als u wilt dat gebruikers een nieuwe webpagina openen wanneer zij Afbeeldingskaart selecteren, voert u de URL in de lijst Afbeeldingskaart in.

   Zie [JavaScript en URL&#39;s invoeren](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Als u rollovertekst wilt weergeven wanneer gebruikers de aanwijzer over de Afbeeldingskaart bewegen, voert u de tekst in de lijst Afbeeldingskaart in. Selecteer in de lijst Afbeeldingskaart de optie **[!UICONTROL Show]** en selecteert u **[!UICONTROL Rollover Text]**. Voer vervolgens de tekst in die gebruikers op het scherm moeten zien. U kunt de tekst in een tekstverwerker schrijven en het kopiëren in het de tekstgebied van het Omvergooien.

1. Als u een ander actieeffect wilt voorkomen wanneer de gebruikers de muis over een Kaart van het Beeld bewegen, bepaal de actie. In de **[!UICONTROL Show]** vervolgkeuzelijst, selecteert u **[!UICONTROL Other Actions]**. Voer de kenmerken van de handeling in. (Ga naar **[!UICONTROL Show]** > **[!UICONTROL Both]** om rollover-tekst en een handeling voor een afbeelding met hyperlinks te maken.)

   Zie [Andere handelingen voor afbeeldingen met hyperlinks definiëren](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Optioneel) Voer een van de volgende handelingen uit:

   * Selecteer **[!UICONTROL Preview]**.
   * Als u een afbeelding met hyperlinks of veelhoekpunt wilt verwijderen, selecteert u een vorm in de afbeelding en selecteert u vervolgens **[!UICONTROL Delete]**. Of selecteer voor een eCatalog op het tabblad Order Pages de optie **[!UICONTROL Clear Maps]** om afbeeldingen met hyperlinks van alle pagina&#39;s te verwijderen.
   * Een afbeelding verwijderen:
      * Afbeeldingskaart van een afbeelding
      * een afbeelding in een SpinSet
      * of, een eCatalog-pagina

     Schakel tijdelijk, zonder deze te verwijderen, de desbetreffende optie Op uit in de lijst Afbeeldingskaart.

1. Selecteren **[!UICONTROL Save]**.

### De positie, vorm en grootte van afbeeldingskaarten aanpassen {#adjusting-the-position-shape-and-size-of-image-maps}

Als u de positie, vorm en grootte van een afbeelding met hyperlinks wilt wijzigen, selecteert u de knop Afbeelding met hyperlinks. Selecteer vervolgens de **[!UICONTROL Pan]** en volg deze instructies:

* **Positie wijzigen**: Verplaats de aanwijzer naar de rand van de afbeelding met hyperlinks, maar niet naar de rand van de afbeelding. Als u het pictogram met de vier pijlpunten ziet, sleept u de kaart naar een nieuwe locatie.

* **Grootte en vorm wijzigen**: Hoe u de vorm en grootte van een afbeelding met hyperlinks wijzigt, hangt af van het feit of u met een rechthoekige of veelhoekige afbeelding met hyperlinks werkt:

>[!TIP]
>
>U kunt de schuifregelaar Grootte onder aan het scherm verslepen om de weergave te wijzigen en uw afbeelding met hyperlinks beter te bekijken.

* **Rechthoekige afbeelding met hyperlinks**: Plaats de aanwijzer boven een zijde of hoek van de Afbeeldingskaart. Wanneer u het pictogram met de dubbele pijl ziet, begint u te slepen. Houd Shift ingedrukt terwijl u sleept om de grootte te wijzigen, maar de hoogte-breedteverhouding (de vorm) te behouden.

* **Veelhoekige afbeelding met hyperlinks**: Sleep een vierkante selectiegreep. Als u een selectiegreep wilt maken, selecteert u de rand van de Afbeeldingskaart en begint u te slepen.

### Overlappende afbeeldingen met hyperlinks verwerken {#handling-overlapping-image-maps}

Als uw afbeelding of eCatalog-pagina meer dan één afbeelding met hyperlinks bevat en de afbeeldingen overlappen, kunt u bepalen hoe de afbeeldingen overlappen. Wijzig hiertoe de volgorde van de afbeeldingen in de lijst Afbeeldingskaart. Sleep hun namen hoger of lager in de lijst. Hoe hoog een naam op de lijst is bepaalt of zijn Kaart van het Beeld andere Kaarten van het Beeld overlapt.

### Afbeeldingskaartgegevens importeren {#importing-image-map-data}

In plaats van de gegevens van de Kaart van het Beeld op elke pagina in te gaan, kunt u de gegevens voor uw beeld, de Reeks van de Rotatie, of eCatalog in het Summiere scherm van de Kaart invoeren. U importeert de gegevens van de Kaart van het Beeld in de vorm van een lusje-afgebakend dossier of van XML DTD. De velden in het bestand moeten in de volgorde staan die wordt weergegeven in het scherm Kaartoverzicht: Naam, inhoudsopgavelabels, Kaarten, URL&#39;s, Rollover-tekst, Overige handelingen en Zoeken. Door de gegevens van de Kaart van het Beeld in te voeren bespaart u het probleem om de gegevens in de lijst van de Kaart van het Beeld in te gaan aangezien u elke Kaart van het Beeld creeert.

**Afbeeldingskaartgegevens importeren:**

1. Ga naar de de redacteurspagina van de Kaart van het Beeld (voor beelden of beelden in SpinSets) of het lusje van de Pagina&#39;s van de Kaart van het eCatalog het uitgeven scherm.
1. Selecteren **[!UICONTROL Import Metadata]**.
1. Selecteer Afbeelding of Afbeeldingskaart in het dialoogvenster Metagegevens uploaden om de metagegevens van het gewenste type elementeigenschap te uploaden.
1. In de `Generate File` selecteert u het type bestand dat u wilt maken.
1. (Optioneel) Selecteer **[!UICONTROL Generate]** om een voorvertoning van de resulterende gegevens weer te geven op basis van het type bestand dat u wilt maken. Selecteren **[!UICONTROL Close]** om terug te keren naar het dialoogvenster Metagegevens uploaden.
1. Blader naar het bestand dat u wilt uploaden. Geef in het tekstveld Bestandsnaam de naam van het gegenereerde bestand op.
1. (Optioneel) Geef in het veld Taaknaam een naam op voor de uploadtaak voor metagegevens.
1. Selecteren **[!UICONTROL Upload]**.

### Afbeeldingen met hyperlinks kopiëren {#copying-image-maps}

U kunt afbeeldingen met hyperlinks kopiëren van een afbeelding of van een eCatalog-pagina naar een andere. Gebruiken **[!UICONTROL Copy Image Map]** om een begin te maken met het maken ervan. U kunt Afbeeldingskaarten ook kopiëren en opnieuw maken in afbeeldingen of pagina&#39;s met dezelfde layout- of toewijzingsstructuur.

Het kopiëren van afbeeldingen met hyperlinks in een eCatalog is bijvoorbeeld een handige manier om alle afbeeldingen met hyperlinks te kopiëren naar een andere taalversie van dezelfde eCatalog. Voor de beste resultaten is kopiëren het meest succesvol als u kopieert tussen eCatalogi met hetzelfde aantal pagina&#39;s en dezelfde afbeeldingen. Als de eCatalog waarnaar u kopieert reeds Kaarten van het Beeld bevat, worden die Kaarten van Beeld geschrapt wanneer het exemplaar wordt gemaakt.

**Afbeeldingskaarten kopiëren:**

1. Ga naar de de redacteurspagina van de Kaart van het Beeld (voor beelden of beelden in SpinSets) of het lusje van de Pagina&#39;s van de Kaart van het eCatalog het uitgeven scherm.
1. Selecteren **[!UICONTROL Copy Maps to]**.
1. Voer een van de volgende handelingen uit op basis van het feit of u afbeeldingen met hyperlinks kopieert of afbeeldingen met hyperlinks kopieert uit een eCatalog:

   * (Afbeeldingen) Selecteer in het scherm Afbeeldingen selecteren de afbeeldingen waarnaar u de afbeeldingen met hyperlinks wilt kopiëren.
   * (eCatalog) Selecteer in het scherm Select Asset de afbeeldingen of eCatalog-pagina&#39;s waarnaar u de Afbeeldingen met hyperlinks wilt kopiëren.

1. Kies **[!UICONTROL Select]**.

## Een sjabloon gebruiken om JavaScript en URL&#39;s in te voeren {#using-a-template-to-enter-javascript-and-urls}

U kunt een URL-sjabloon (ook wel een Href-sjabloon genoemd) definiëren om het invoeren van URL&#39;s voor afbeeldingen met hyperlinks eenvoudiger en efficiënter te maken. Definieer een URL-sjabloon als de meeste URL&#39;s van de Afbeeldingskaart een gemeenschappelijke, vaste indeling hebben. Door het gedeelte van URL in te voeren dat als malplaatje URL vast is, moet u niet dit gedeelte van URL ingaan telkens als u een Kaart van het Beeld creeert. Uw URL-sjabloon kan ook JavaScript-opdrachten, -padnamen en -parameters bevatten. Standaard bevat de URL-sjabloon een eigen Adobe Dynamic Media Classic JavaScript-handler, genaamd `loadProduct` Hiermee opent u de afbeelding in een nieuw venster.

>[!NOTE]
>
>Wanneer u de JavaScript-code toevoegt aan het HREF-kenmerk van de Afbeeldingskaart, wordt de code uitgevoerd op de computer van de client. Controleer daarom of de JavaScript-code veilig is.

### Informatie over URL-sjablonen {#about-url-templates}

De URL-sjabloon vervangt de inhoud van de URL-kolom in de lijst Afbeelding met hyperlinks. Deze vervangt deze door de dubbele dollartekens (&#39;$$&#39;) in de sjabloon:

```as3
Javascript:loadProduct('$$');void(0);
```

U plaatst alle waarden die niet tussen Afbeeldingen met hyperlinks veranderen in het malplaatje URL. Voeg alleen de waarden toe die wel veranderen in de URL-kolom in de lijst Afbeelding met hyperlinks. Bijvoorbeeld:

* URL-sjabloon - `javascript:loadProduct('https://www.examplesitehere.com/$$');void(0);`
* URL-waarde - `product.htm`
* Werkelijke URL gegenereerd - `javascript:loadProduct('https://www.examplesitehere.com/product.html);void(0);`

Standaard bevat de URL-sjabloon een eigen Adobe Dynamic Media Classic JavaScript-handler, genaamd `loadProduct` dat een nieuw venster met de bestemming URL opent. U kunt echter elke JavaScript-code gebruiken om deze JavaScript-handler te vervangen of een van de volgende Adobe Dynamic Media Classic-handlers gebruiken:

* `loadProductCW`: Hiermee geeft u het URL-doel weer dat is opgegeven in de kolom URL in het huidige venster. Deze handler is vooral bedoeld voor eCatalogi die zijn geïntegreerd in een pagina binnen een website.

* `loadProductPW`: Hiermee geeft u het URL-doel weer dat is opgegeven in de URL-kolom in het bovenliggende venster (de pagina die het huidige venster heeft geopend). Het huidige venster blijft geopend, maar het bovenliggende venster verandert om het URL-doel weer te geven.

  >[!NOTE]
  >
  >De handler `loadProductPW` biedt geen ondersteuning voor DHTML- en HTML5-viewers.

### Een URL-sjabloon maken {#creating-a-url-template}

1. Selecteer Bewerken naast de sjabloonoptie URL in het scherm Kaarteditor (afbeeldingen of SpinSets) of op het tabblad Kaartpagina&#39;s van het eCatalog-scherm (eCatalogs). Het dialoogvenster Kaartsjabloon bewerken wordt geopend.
1. Voer de JavaScript-code en de volledige URL in (waarbij het gedeelte van de variabele wordt vervangen door dollartekens) [$$]). U kunt de code plakken door met de rechtermuisknop te klikken en te kiezen **[!UICONTROL Paste]**.
1. Selecteren **[!UICONTROL Save]**.

### URL-sjablonen afhandelen {#handling-url-templates}

De pagina Kaarteditor (afbeeldingen en SpinSets) en het tabblad Kaartpagina&#39;s van het eCatalog-scherm (eCatalogs) bieden de volgende opdrachten voor de verwerking van URL-sjablonen:

* **URL-sjabloon, optie**: Selecteer de sjabloonoptie URL om uw URL-sjabloon toe te passen op alle afbeeldingen met hyperlinks op een afbeelding of een eCatalog-pagina.

* **Sjabloon, optie**: Schakel een sjabloonoptie uit in de lijst URL-afbeeldingskaart als u niet wilt dat een afzonderlijke afbeelding met hyperlinks de URL-sjabloon gebruikt.

## Andere handelingen voor afbeeldingen met hyperlinks definiëren {#defining-other-actions-for-image-maps}

U kunt de **[!UICONTROL Show]** en kiest u **[!UICONTROL Other Actions]** om andere handelingen dan rollover-tekst en het starten van een webpagina te activeren. Wanneer de gebruiker de aanwijzer boven een Afbeeldingskaart plaatst, kunt u een handeling starten. Deze acties zijn attributen die voor cliënt-kant de Kaarten van het Beeld door de specificaties van HTML van het Consortium van World Wide Web worden bepaald. Deze omvatten:

* **`accesskey`**: Triggert een actie wanneer de gebruiker op een bepaalde toets op het toetsenbord drukt.

* **`onfocus`**: Triggert een gebeurtenis wanneer de Kaart van het Beeld nadruk-door de curseur, door met de Tab-toets, of door een toegangssleutel te drukken ontvangt. U kunt bijvoorbeeld een webpagina starten wanneer de afbeelding met hyperlinks de focus krijgt en sluiten wanneer de afbeelding met hyperlinks de focus verliest.

* **`onblur`**: Triggert een gebeurtenis wanneer de Kaart van het Beeld nadruk verliest, of door curseur of door lusjes.

**Andere handelingen voor afbeeldingen met hyperlinks definiëren:**

1. Selecteer in het scherm Kaarteditor (afbeeldingen en SpinSets) of op het tabblad Kaartpagina&#39;s van het eCatalog-scherm (eCatalogs) de optie **[!UICONTROL Show]** en selecteert u **[!UICONTROL Other Actions]**.
1. Gebruikend de syntaxis die door de HTML specificaties van het Consortium van World Wide Web wordt gespecificeerd, voeg de gesteunde attributen in de Andere kolom van Acties van de Lijst van de Kaart van het Beeld toe.
1. Selecteren **[!UICONTROL Save]**.

Selecteer de **[!UICONTROL Show]** en selecteert u **[!UICONTROL Both]** als u een afbeelding met hyperlinks wilt weergeven met rollovertekst en een handeling.

## Afbeeldingen met hyperlinks maken in Adobe Acrobat of Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

U kunt afbeeldingen met hyperlinks maken terwijl u uw eCatalog ontwerpt in Adobe Acrobat of Adobe InDesign.

Maak in Adobe Acrobat of Adobe InDesign hyperlinkverwijzingen naar de plaats waar de afbeeldingen met hyperlinks moeten worden weergegeven, en geef URL-locaties op voor de afbeelding met hyperlinks. Als u de optie Koppelingen extraheren selecteert wanneer u het PDF-bestand uploadt naar Adobe Dynamic Media Classic, worden de koppelingen automatisch omgezet naar Afbeeldingskaarten.

Raadpleeg de Help bij Adobe InDesign of Adobe Acrobat voor meer informatie.

### Afbeeldingen toewijzen in Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. Ga in Adobe InDesign naar **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hyperlinks]**.
1. Selecteer in het deelvenster Hyperlinks de tekst, het kader of de afbeelding die u wilt omzetten in een afbeelding met hyperlinks.
1. Selecteren **[!UICONTROL New Hyperlink]** in het deelvenstermenu.
1. Kies in het dialoogvenster Nieuwe hyperlink de optie **[!UICONTROL Link To]** kiest u de optie **[!UICONTROL URL]**.
1. Typ of plak de product-id in het vak URL.
1. Selecteren **[!UICONTROL OK]**. (Adobe Dynamic Media Classic voltooit de URL met behulp van de sjabloon URL afbeeldingskaart.)

   >[!NOTE]
   >
   >U hoeft geen weergaveopties in te stellen in Adobe InDesign. U kunt de weergave in Adobe Dynamic Media Classic opgeven.

1. Herhaal stap 2 tot en met 6 voor alle afbeeldingen met hyperlinks die u wilt maken.
1. Exporteer het bestand als een PDF.
1. Upload de PDF naar Adobe Dynamic Media Classic.
1. In **[!UICONTROL PDF Options]**, selecteert u **[!UICONTROL Extract Links]**.

### Afbeeldingen toewijzen in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Ga in Adobe Acrobat naar **[!UICONTROL Tools]** > **[!UICONTROL Advanced Editing]** > **[!UICONTROL Link Tool]**.
1. Sleep om de afbeelding met hyperlinks te maken.
1. Selecteer in het vak Koppeling maken de optie **[!UICONTROL Custom Link]** en selecteert u **[!UICONTROL Next]**.

>[!NOTE]
>
>U hoeft geen weergaveopties in te stellen in Adobe Acrobat. U kunt de weergave in Adobe Dynamic Media Classic opgeven.

1. Selecteer in het vak Koppelingseigenschappen de optie **[!UICONTROL Actions]**.
1. Selecteren **[!UICONTROL Open A Web Link]** in het menu Handeling selecteren en selecteer vervolgens **[!UICONTROL Add]**.
1. Typ de product-id voor de afbeelding met hyperlinks in het vak URL bewerken en selecteer **[!UICONTROL OK]**. (Adobe Dynamic Media Classic voltooit de URL met behulp van de sjabloon URL afbeeldingskaart.)
1. Herhaal stap 1 tot en met 7 voor alle afbeeldingen met hyperlinks die u wilt maken.
1. Sla het bestand op.
1. Upload de PDF naar Adobe Dynamic Media Classic en selecteer Koppelingen extraheren in de PDF-opties.
