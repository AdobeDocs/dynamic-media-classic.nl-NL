---
title: Metagegevens weergeven, toevoegen en exporteren
seo-title: Metagegevens weergeven, toevoegen en exporteren
description: 'null'
seo-description: Leer metagegevens weergeven, toevoegen en exporteren.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '2262'
ht-degree: 0%

---


# Metagegevens weergeven, toevoegen en exporteren{#viewing-adding-and-exporting-metadata}

U kunt informatie specifiek voor de dossiers opslaan u met in Dynamische Klassiek van Media werkt; deze informatie wordt *metagegevens* genoemd . U kunt metagegevens in Dynamic Media Classic gebruiken voor het ordenen, zoeken, filteren en sorteren van uw elementen.

Metagegevens worden in de gedetailleerde weergave weergegeven, samen met door Dynamic Media Classic gegenereerde informatie, zoals de aanmaakdatum van het bestand, de publicatiedatum en trefwoorden. Als u metagegevens wilt weergeven, opent u het element in de gedetailleerde weergave en selecteert u het deelvenster Metagegevens. U kunt metagegevens invoeren en bewerken in de gedetailleerde weergave.

Sommige metagegevens worden rechtstreeks in een bestand ingesloten. Als een bestand deze metagegevens bevat, wordt deze automatisch met het bestand geüpload via Dynamic Media Classic. U kunt metagegevens insluiten in bronelementen in Adobe Photoshop, InDesign, Illustrator en andere toepassingen. Dynamic Media Classic herkent deze metagegevens. U kunt ook metagegevens toevoegen aan afzonderlijke bestanden in het deelvenster Metagegevens in de gedetailleerde weergave. Om consistentie tussen activa te verzekeren, leiden de bedrijfbeheerders Meta-gegevensmalplaatjes die de meta-gegevensgebieden verstrekken die kunnen worden ingevuld.

Zie [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en)voor meer informatie over ingesloten metagegevens.

## Metagegevens weergeven {#view-metadata}

Als u de metagegevens van een element wilt weergeven, opent u het element in de gedetailleerde weergave en klikt u op het deelvenster Metagegevens. Kies vervolgens een optie in het menu Weergave metagegevens om een set metagegevensvelden te selecteren. Dynamic Media Classic biedt deze metagegevensweergaven:

* **Compacte weergave** Een basislijst met waarden.

* **IPTC**-waarden zoals gedefinieerd door de Internationale Raad voor de Telecommunicatie van de Pers.

* **XMP** Waarden zoals gedefinieerd door het uitbreidbare metagegevensplatform.

Beheerders kunnen weergaven van metagegevens maken. Deze weergaven worden ook weergegeven in het menu Weergaven metagegevens. Zie Weergaven [metagegevens voor informatie over het maken van weergaven](application-setup.md#metadata_views)van metagegevens.

## Metagegevens voor een element handmatig invoeren {#manually-enter-metadata-for-an-asset}

1. Open het element in de gedetailleerde weergave.
1. Open het deelvenster Metagegevens en voer een of beide van de volgende handelingen uit:

   * Kies een metagegevensweergave om te bepalen welke metagegevensvelden in het deelvenster worden weergegeven.
   * Kies een vooraf ingestelde waarde en klik op Toepassen om metagegevensvelden te vullen met vooraf ingestelde waarden. Bedrijfsbeheerders maken deze vooraf ingestelde waarden.

1. Geef waarden op in het deelvenster Metagegevens.

>[!NOTE]
>
>Als u de metagegevens van meerdere elementen tegelijk wilt bewerken, selecteert u de elementen en kiest u Bestand > Info bewerken. Wijzigingen die u aanbrengt in metagegevens in het venster Info bewerken, worden toegepast op alle elementen die u hebt geselecteerd.

## Trefwoorden toevoegen of bewerken {#add-or-edit-keywords}

Naast metagegevens kunt u ook trefwoorden gebruiken als hulp bij het zoeken en beheren van uw elementen.

Als u tijdens deze sessie trefwoorden hebt toegevoegd aan andere bestanden of als u trefwoorden uit de lijst hebt verwijderd, worden deze weergegeven in de tabel Suggesties voor trefwoorden.

1. Open het bestand in de gedetailleerde weergave.
1. Klik op Trefwoorden.
1. Voer een van de volgende handelingen uit om trefwoorden toe te voegen:

   * Typ een trefwoord in het tekstvak en klik op Toevoegen.
   * Klik op een trefwoord in de tabel Suggesties voor trefwoorden.

1. Als u een trefwoord wilt verwijderen, selecteert u het en klikt u op Verwijderen. De tabel gaat naar de tabel Suggesties voor trefwoorden.

>[!NOTE]
>
>U kunt trefwoorden aan bestanden toevoegen terwijl u deze uploadt naar Dynamic Media Classic. Kies Extra metagegevens in het dialoogvenster Taakopties uploaden en voer trefwoorden in. Zie [Uploadopties](uploading-files.md#upload_options).

## Metagegevens importeren {#import-metadata}

In plaats van handmatig metagegevens één element tegelijk in te voeren, kunt u metagegevens voor veel verschillende elementen importeren uit een door tabs gescheiden of XML-bestand. Het invoeren van de metagegevens in een door tabs gescheiden of XML-bestand en het importeren van het bestand neemt minder tijd in beslag dan het invoeren van metagegevens in afzonderlijke elementen. Voer in de eerste rij van het door tabs gescheiden bestand de id in en de namen van velden waarvoor u metagegevens wilt opnemen. Voer in elke volgende rij de naam van een element-id in, gevolgd door metagegevenswaarden. Velden die niet zijn opgenomen in het door tabs gescheiden of XML-bestand, worden niet gewijzigd. Als u metagegevens uit een XML-bestand wilt importeren, moet u controleren of u voldoet aan de DTD.

>[!NOTE]
>
>U kunt een sjabloon maken voor het invoeren van metagegevens, zodat deze op de juiste wijze kunnen worden geïmporteerd in Dynamic Media Classic. Nadat u de sjabloon hebt gemaakt, kunt u deze gebruiken om de metagegevens in te voeren. Zie Een sjabloon [maken voor het invoeren van te uploaden](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)metagegevens.

Meer informatie over gestandaardiseerde eigenschappen vindt u op: https://www.adobe.com/devnet/xmp.html

1. Selecteer in het deelvenster Bladeren de afbeeldingen waaraan u metagegevens wilt toevoegen uit het bestand met tabs of XML.
1. Klik op **Bestand** > Metagegevens **** importeren.
1. Klik in het dialoogvenster Metagegevens **** uploaden op **Bladeren**.
1. Selecteer in het dialoogvenster Bestanden **selecteren om te uploaden** het door tabs gescheiden of XML-bestand met de metagegevens.
1. Voer een taaknaam in.
1. Klik op **Uploaden**.

**Verschillende typen metagegevens tijdens het importeren identificeren**

Houd rekening met het volgende wanneer u verschillende typen metagegevens identificeert die u wilt importeren:

* Door de gebruiker gedefinieerde velden worden aangeduid met hun naam, zoals deze zijn gemaakt in Setup > Setup > Metagegevens > Door de gebruiker gedefinieerde velden. Gebruik de functie Bestanden genereren om een lijst met alle gedefinieerde PDF&#39;s in de juiste importindeling op te halen.
* XMP eigenschappen van metagegevens moeten het gerelateerde XMP-voorvoegsel vóór de naam (eigenschap-) hebben. Een dubbele punt scheidt het voorvoegsel en de naam. U vindt het XMP voorvoegsel in Setup > Application Setup > Metadata > Metadata Schema editor. De technische namen zijn te vinden in documentatie van verwant XMP schema. Namen van XMP eigenschappen worden niet weergegeven in de functie Bestand genereren.
* Eigenschappen van Metagegevensschema moeten het verwante voorvoegsel vóór de naam (eigenschap-) hebben. Een dubbele punt scheidt het voorvoegsel en de naam. Het voorvoegsel en de eigenschapnamen worden gedefinieerd in de editor voor het metagegevensschema. Namen van eigenschappen van het metagegevensschema worden niet weergegeven in de functie Bestand genereren.

Bijvoorbeeld: De XMP eigenschap voor trefwoorden is het XMP schema &quot;Dublin Core&quot; met het voorvoegsel &quot;dc&quot; en &quot;subject&quot; is de technische XMP naam. Het voorvoegsel en de technische XMP worden gecombineerd in de volledige eigenschapnaam &quot;dc:subject&quot;. In de indeling voor het importeren van XML-metagegevens moet &quot;dc.subject&quot; de naam van de eigenschap zijn. In de door tabs gescheiden importindeling moet dit de kolomkop zijn.

**Trefwoorden importeren**

Trefwoorden kunnen worden geïmporteerd als door komma&#39;s gescheiden lijsten. Als een komma in een van de afzonderlijke waarden voorkomt, moet deze worden beschermd door een backslash (\). Een letterlijke backslash is de gebruikelijke dubbele backslash (\\).

Met een bestand voor het importeren van metagegevens met de waarde &quot;Hello\, World!,back\\slash,foo&quot; voor &quot;dc:subject&quot; worden bijvoorbeeld drie XMP trefwoorden voor het element ingesteld: &quot;Hello, World!&quot;, &quot;back\slash&quot; en &quot;foo.&quot;

**XMP- en metagegevensschema-XMP importeren**

De XML-import accepteert alleen geldige XML. Bij het importeren van XMP- of metagegevensschemavelden wordt het naamruimtevoorvoegsel toegevoegd en gedraagt dit zich als een XMP-naamruimte. Deze naamruimte moet bijvoorbeeld in de tag op hoofdniveau worden gedeclareerd.

Bijvoorbeeld:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Door tabs gescheiden bestanden voor het importeren van XMP- en metagegevensschema**

Het voorvoegsel moet worden toegevoegd aan de gerelateerde kolomkop van het importveld.

## Metagegevens importeren (via FTP) {#import-metadata-via-ftp}

U kunt metagegevens voor meerdere bestanden importeren door de metagegevens in te voeren in een door tabs gescheiden of XML-bestand en de optie Metagegevensbestanden verwerken te selecteren in het scherm Uploaden (via FTP).

Zorg ervoor dat de gegevens in het door tabs gescheiden of XML-bestand de juiste indeling hebben. Voer in de eerste rij het veld Id in, gevolgd door de namen van de metagegevensvelden die moeten worden gewijzigd. Voer in elke volgende rij de naam van een element-id in, gevolgd door metagegevenswaarden. Velden die niet zijn opgenomen in het door tabs gescheiden of XML-bestand, worden niet gewijzigd.

Klik op de knop Uploaden op de algemene navigatiebalk en selecteer in het scherm Taken het tabblad Via FTP om de metagegevens te importeren. Klik vervolgens op Taakopties. Kies in het dialoogvenster Taakopties uploaden de optie Metagegevensbestanden verwerken.

## Naam-id&#39;s wijzigen in batch met metagegevens {#batch-rename-ids-using-metadata}

Met behulp van metagegevens die zijn geïmporteerd uit een door tabs gescheiden bestand of XML-bestand, kunt u de naam van dynamische media klassieke id&#39;s wijzigen. De geïmporteerde metagegevens worden alleen toegepast op de afbeeldingen die in het metagegevensbestand zelf zijn opgegeven. Het maakt niet uit of afbeeldingen zijn geselecteerd in het deelvenster Bladeren.

Als u de naam van de dynamische media-klassieke id van een afbeelding wilt wijzigen, voegt u een kolom met het label *Net* toe aan het door tabs gescheiden bestand of voegt u een veld met de naam* new_vc_objectname* toe aan de XML-gegevens.

Bijvoorbeeld:

| ipsid | newipsid |
|--- |--- |
| testjasje_1 | Jasje_test_1 |
| testjasje_blauw | Jasje_test_2 |


In het taaklogboek voor de metagegevenstaak wordt aangegeven welke id&#39;s zijn hernoemd en welke niet.

## Een sjabloon maken voor het invoeren van te uploaden metagegevens {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic biedt een opdracht voor het maken van een sjabloon voor het opnemen van metagegevens. Met behulp van de sjabloon zorgt u ervoor dat de metagegevens in de juiste indeling worden ingevoerd, zodat deze op de juiste wijze kunnen worden geüpload naar Dynamic Media Classic. Ga als volgt te werk om een sjabloon te maken voor het opnemen en importeren van metagegevens naar Dynamic Media Classic:

1. Selecteer afbeeldingselementen met de metagegevensvelden die u voor de sjabloon wilt gebruiken.
1. Kies Bestand > Metagegevens importeren.
1. Selecteer Afbeelding voor het type elementeigenschappen.
1. Selecteer Door tabs gescheiden sjabloon, XML-metagegevens van element of XML DTD in het menu Bestand genereren.
1. Klik op Genereren.
1. Kopieer de gegevens in het dialoogvenster dat wordt weergegeven. Gebruik deze gegevens om de sjabloon samen te stellen.

## Werken met metagegevensschema&#39;s {#working-with-metadata-schemas}

Een bedrijfbeheerder kan een lijst van alle beschikbare schema&#39;s bekijken. Open Application Setup -> Metadata -> Metadata Schema.

In eerste instantie is de lijst met algemene standaardschema&#39;s zoals XMP verborgen. Ze kunnen worden weergegeven met het selectievakje onder aan de lijst.

De bedrijfbeheerder kan een nieuw douaneschema tot stand brengen, of een bestaand douaneschema uitgeven.

U kunt de Editor Metagegevensschema gebruiken om de volgende handelingen uit te voeren:

| Handeling | Beschrijving |
|--- |--- |
| Toevoegen | Voegt een nieuwe eigenschap toe aan het schema. Een modaal dialoogvenster verzamelt de informatie: ID, Label, Structuur en Gegevenstype. |
| Keuzevrijheid toevoegen | Voegt een nieuwe selecteerbare keus aan een bezit met structuur Open Keus of Gesloten Keuze toe. Alle keuzevelden hebben hetzelfde type. U moet de eigenschap zelf selecteren om de knop in te schakelen. |
| Bewerken | Bewerk het label van een eigenschap of keuzevrijheid. U kunt het label, de id en de typegegevens alleen wijzigen als dit niet mogelijk is. |
| Omhoog/Omlaag | De orde in het schema wordt weerspiegeld in UI. Als u de volgorde wilt wijzigen, selecteert u een eigenschap of keuzevrijheid en verplaatst u deze met de knoppen. Slepen en neerzetten wordt momenteel niet ondersteund. |
| Verwijderen | Hiermee verwijdert u een eigenschap of keuzevrijheid uit het schema. Hiermee verwijdert u geen waarden uit het XMP of de database. De eigenschap is niet meer beschikbaar voor weergaven van metagegevens en wordt verwijderd uit de weergave Details van element. Als de eigenschap is gepubliceerd naar de server met metagegevens, voert u een kracht uit die publiceert om de gegevens te verwijderen uit de openbare metagegevensserver. |

Het systeem genereert automatisch een aangepast schema voor door de gebruiker gedefinieerde velden met het voorvoegsel &#39;s7udf&#39;. Dit zijn de bestaande user-defined Gebieden en in hun eigen sectie van de Opstelling uitgegeven.

>[!NOTE]
>
>Door wijzigingen in het schema veranderen de metagegevens van de elementen zelf nooit. Nochtans, zijn zij niet zichtbaar voor alle Dynamische Media Klassieke en functionaliteit van de Server van Meta-gegevens en kunnen niet na worden veranderd worden betreden. Op dezelfde manier, als de meta-gegevens voor een activa bestaan, maakt de verwezenlijking van het passende schema de meta-gegevens bruikbaar in Dynamische Media Klassiek en de Server van Meta-gegevens.

De redacteur van het Schema van Meta-gegevens biedt een grafische manier aan om een douaneschema binnen Dynamische Klassiek van Media toe te voegen of uit te geven. Een schema wordt gedefinieerd door een voorvoegsel, een naamruimte en een lijst met eigenschappen.

* Naam

   UI-naam voor het schema. Hiermee identificeert u de eigenschappen in Metagegevensweergaven en Geavanceerd zoeken. Vergelijkbaar met XMP secties zoals Standaard, IPTC en PDF.

* Voorvoegsel

   Technische unieke id voor het schema. Beperkt tot de letters a-z en A-Z. Het voorvoegsel is niet zichtbaar in de Klassieke UI van de Dynamische Media, maar gebruikt, wanneer de meta-gegevens voor een element in het XMP en onze gegevensbestand worden opgeslagen. Het voorvoegsel wordt gebruikt om metagegevensvelden op unieke wijze te identificeren in zoekquery&#39;s voor metagegevens op de Metagegevensserver of het importeren.

* Naamruimte

   Technische unieke id voor het schema, doorgaans een URL in het formulier `https://your.company.com/name/version/`. Zie de lijst met standaardschema&#39;s voor voorbeelden. De naamruimte is niet zichtbaar in de klassieke gebruikersinterface van Dynamic Media, maar wordt gebruikt om metagegevens in het XMP op te slaan.

* Beschrijving

   Vrije-vormbeschrijving van het schema.

>[!NOTE]
>
>Het voorvoegsel en de naamruimte kunnen niet worden bewerkt. Als u deze eigenschappen wilt wijzigen, moet u het schema verwijderen en opnieuw maken.

De eigenschappen beschrijven de meta-gegevens die met dit schema in het XMP blok kunnen worden opgeslagen. Een eigenschap bestaat uit:

| Eigenschap | Beschrijving |
|--- |--- |
| ID | Technische id voor deze eigenschap. De id is niet zichtbaar in de Klassieke UI van de Dynamische Media, maar gebruikt, wanneer de meta-gegevens voor een element in het XMP en onze gegevensbestand worden opgeslagen. De id wordt gebruikt om zoekopdrachten te maken op de Metagegevensserver. De id heeft een aantal beperkingen, zoals: <ul><li>Geen spaties</li><li>Geen &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Geen getal als eerste teken</li><li>De beste manier is om a-z of A-Z als eerste teken te gebruiken</li></ul> <br>Nadat de id is gemaakt, kan deze niet worden gewijzigd. |
| Label | UI-naam voor deze eigenschap. |
| Structuur | Bepaalt het type van het bezit samen met het Type van Gegevens. Structuur kan een van de volgende zijn:<ul><li>Eenvoudig type: enkele waarde van gegevenstype</li><li>Volgorde: een lijst met waarden van hetzelfde gegevenstype</li><li>Open keuze: Selecteer een item in een lijst met vooraf gedefinieerde waarden of voer vrije tekst in. Kan alleen van het gegevenstype String of Integer zijn</li><li>Gesloten keuze: selecteert u een item in een lijst met vooraf gedefinieerde waarden (een pop-up- of keuzelijst met invoervak)</li></ul> |
| Gegevenstype | Maak een keuze uit de volgende beschikbare typen: <ul><li>String</li><li>Geheel</li><li>Float</li><li>Ja/Nee (Boolean)</li><li>Datum</li></ul> |


Wanneer de eigenschap de structuur Open Keuze of Gesloten Keuze heeft, moet u ten minste één Keuzewaarde opgeven. De optie Open Keuze kan worden gewijzigd. Gesloten keuze kan niet worden gewijzigd. Alle Keuzevelden hebben het gegevenstype van de eigenschap.

| Eigenschap | Beschrijving |
|--- |--- |
| ID | Technische identificatie voor deze waarde. De id is niet zichtbaar in de Klassieke UI van de Dynamische Media, maar wordt gebruikt wanneer de meta-gegevens voor een element in het XMP en het gegevensbestand worden opgeslagen. De id wordt gebruikt in zoekopdrachten op de Metagegevensserver. De id mag geen spaties bevatten. Nadat de id is gemaakt, kan deze niet worden gewijzigd. |
| Label | UI-naam voor deze waarde. |

>[!MORELIKETHIS]
>
>* [Voorinstellingen viewer](application-setup.md#viewer_presets)
>* [Voorinstellingen metagegevens](application-setup.md#metadata_presets)

