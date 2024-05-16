---
title: Metagegevens weergeven, toevoegen en exporteren
description: Leer metagegevens weergeven, toevoegen en exporteren in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2154'
ht-degree: 0%

---

# Metagegevens weergeven, toevoegen en exporteren{#viewing-adding-and-exporting-metadata}

U kunt gegevens opslaan die specifiek zijn voor de bestanden waarmee u werkt in Adobe Dynamic Media Classic. Deze gegevens worden *metagegevens*. U kunt metagegevens in Adobe Dynamic Media Classic gebruiken voor het ordenen, zoeken, filteren en sorteren van uw elementen.

Metagegevens worden weergegeven in de gedetailleerde weergave. Deze wordt samen met door Adobe Dynamic Media Classic gegenereerde informatie weergegeven. Bijvoorbeeld de aanmaakdatum van het bestand, de publicatiedatum en trefwoorden. Als u metagegevens wilt weergeven, opent u het element in de gedetailleerde weergave en selecteert u het deelvenster Metagegevens. U kunt metagegevens invoeren en bewerken in de gedetailleerde weergave.

Sommige metagegevens worden rechtstreeks in een bestand ingesloten. Als een bestand deze metagegevens bevat, wordt deze automatisch door Adobe Dynamic Media Classic met het bestand geüpload. U kunt metagegevens insluiten in bronelementen in Adobe Photoshop, InDesign, Illustrator en andere toepassingen. Deze metagegevens worden door Adobe Dynamic Media Classic herkend. U kunt ook metagegevens toevoegen aan afzonderlijke bestanden in het deelvenster Metagegevens in de gedetailleerde weergave. Om consistentie tussen activa te verzekeren, leiden de bedrijfbeheerders Meta-gegevensmalplaatjes die de meta-gegevensgebieden verstrekken die kunnen worden ingevuld.

Zie voor meer informatie over ingesloten metagegevens [Extensible Metadata Platform](https://www.adobe.com/products/xmp.html).

## Metagegevens weergeven {#view-metadata}

Als u de metagegevens van een element wilt weergeven, opent u het element in de gedetailleerde weergave en tikt u op het deelvenster Metagegevens. Als u een set metagegevensvelden wilt selecteren, kiest u een optie in het menu Weergave metagegevens. Adobe Dynamic Media Classic biedt de volgende weergaven van metagegevens:

* **Compacte weergave**: Een basislijst met waarden.

* **IPTC**: Waarden zoals gedefinieerd door de Internationale Raad voor de Telecommunicatie van de Pers.

* **XMP**: Waarden zoals gedefinieerd door het uitbreidbare metagegevensprogramma.

Beheerders kunnen weergaven van metagegevens maken. Deze weergaven worden ook weergegeven in het menu Weergaven metagegevens.

Zie [Weergaven metagegevens](application-setup.md#metadata_views) voor informatie over het maken van weergaven van metagegevens.

## Metagegevens voor een element handmatig invoeren {#manually-enter-metadata-for-an-asset}

1. Open het element in de gedetailleerde weergave.
1. Open het deelvenster Metagegevens en voer een of beide van de volgende handelingen uit:

   * Kies een metagegevensweergave om te bepalen welke metagegevensvelden in het deelvenster worden weergegeven.
   * Kies een vooraf ingestelde waarde en selecteer **[!UICONTROL Apply]** om metagegevensvelden te vullen met vooraf ingestelde waarden. Bedrijfsbeheerders maken deze vooraf ingestelde waarden.

1. Voer de waarden in het deelvenster Metagegevens in.

>[!NOTE]
>
>Als u de metagegevens van verschillende elementen tegelijk wilt bewerken, selecteert u de elementen en gaat u naar **[!UICONTROL File]** > **[!UICONTROL Edit Info]**. De bewerkingen die u hebt aangebracht in metagegevens in het venster Info bewerken, worden toegepast op alle elementen die u hebt geselecteerd.

## Trefwoorden toevoegen of bewerken {#add-or-edit-keywords}

Naast metagegevens kunt u ook trefwoorden gebruiken voor het zoeken en beheren van uw elementen.

Als u tijdens deze sessie trefwoorden hebt toegevoegd aan andere bestanden of als u trefwoorden uit de lijst hebt verwijderd, worden deze weergegeven in de tabel Suggesties voor trefwoorden.

1. Open het bestand in de gedetailleerde weergave.
1. Selecteren **[!UICONTROL Keywords]**.
1. Voer een van de volgende handelingen uit om trefwoorden toe te voegen:

   * Typ een trefwoord in het tekstvak en selecteer **[!UICONTROL Add]**.
   * Selecteer een trefwoord in het dialoogvenster **[!UICONTROL Keyword Suggestions]** tabel.

1. Als u een trefwoord wilt verwijderen, selecteert u het en selecteert u het **[!UICONTROL Remove]**. Het beweegt zich aan de lijst van Suggesties van het Sleutelwoord.

>[!NOTE]
>
>U kunt trefwoorden aan bestanden toevoegen terwijl u deze uploadt naar Adobe Dynamic Media Classic. Kies in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL More Metadata]** en voer trefwoorden in.
>Zie [Uploadopties](uploading-files.md#upload_options).

## Metagegevens importeren {#import-metadata}

In plaats van handmatig metagegevens één element tegelijk in te voeren, kunt u metagegevens voor veel verschillende elementen importeren uit een door tabs gescheiden of XML-bestand. Het invoeren van de metagegevens in een door tabs gescheiden of XML-bestand en het importeren van het bestand neemt minder tijd in beslag dan het invoeren van metagegevens in afzonderlijke elementen. Voer in de eerste rij van het door tabs gescheiden bestand de id in en de namen van velden waarvoor u metagegevens wilt opnemen. Voer in elke volgende rij de naam van een element-id in, gevolgd door metagegevenswaarden. Velden die niet zijn opgenomen in het door tabs gescheiden of XML-bestand, worden niet gewijzigd. Als u metagegevens uit een XML-bestand wilt importeren, moet u controleren of u voldoet aan de DTD.

>[!NOTE]
>
>U kunt een sjabloon maken voor het invoeren van metagegevens, zodat deze op de juiste manier naar Adobe Dynamic Media Classic kunnen worden geïmporteerd. Nadat u de sjabloon hebt gemaakt, kunt u deze gebruiken om de metagegevens in te voeren.
>Zie [Een sjabloon maken voor het invoeren van te uploaden metagegevens](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Meer informatie over gestandaardiseerde eigenschappen vindt u op het tabblad [Adobe XMP Ontwikkelaarscentrum](https://www.adobe.com/devnet/xmp.html).

1. Selecteer in het deelvenster Bladeren de afbeeldingen waaraan u metagegevens wilt toevoegen uit het XML- of tabgescheiden bestand.
1. Ga naar **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. In de **[!UICONTROL Upload Metadata]** dialoogvenster selecteert u **[!UICONTROL Browse]**.
1. In de **[!UICONTROL Select files to upload]** selecteert u het door tabs gescheiden of XML-bestand met de metagegevens.
1. Voer een taaknaam in.
1. Selecteren **[!UICONTROL Upload]**.

### Verschillende typen metagegevens tijdens het importeren identificeren

Houd rekening met het volgende wanneer u verschillende typen metagegevens identificeert die u wilt importeren:

* De namen van door de gebruiker gedefinieerde velden worden geïdentificeerd als gemaakt in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined fields]**. Gebruik de `Generate file` om een lijst met alle gedefinieerde UDF&#39;s in de juiste importindeling op te halen.
* XMP eigenschappen van metagegevens moeten het gerelateerde XMP-voorvoegsel vóór de naam (eigenschap-) hebben. Een dubbele punt scheidt het voorvoegsel en de naam. Het XMP voorvoegsel vindt u in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]** editor. De technische namen zijn te vinden in documentatie van verwant XMP schema. XMP eigenschapsnamen worden niet weergegeven in het dialoogvenster `Generate file` gebruiken.
* Eigenschappen van Metagegevensschema moeten het verwante voorvoegsel vóór de naam (eigenschap-) hebben. Een dubbele punt scheidt het voorvoegsel en de naam. Het voorvoegsel en de eigenschapnamen worden gedefinieerd in de Metadata Schema Editor. Namen van metagegevensschema-eigenschappen worden niet weergegeven in het dialoogvenster `Generate file` gebruiken.

Bijvoorbeeld, is het XMP bezit voor sleutelwoorden het XMP schema &quot;Dublin Core&quot;met het prefix `dc` en `subject` is de technische XMP. Het voorvoegsel en de technische XMP worden gecombineerd in de `dc:subject` volledige eigenschapsnaam. In de indeling voor het importeren van XML-metagegevens `dc.subject` moet de eigenschapsnaam zijn. In de door tabs gescheiden importindeling moet dit de kolomkop zijn.

### Trefwoorden importeren

Trefwoorden kunnen worden geïmporteerd als een lijst met door komma&#39;s gescheiden waarden. Als een komma in een van de afzonderlijke waarden voorkomt, kunt u dit omzeilen door een backslash (\) te gebruiken. Een letterlijke backslash is de gebruikelijke dubbele backslash (\\).

Bijvoorbeeld een bestand met metagegevens die de waarde bevatten `Hello\, World!,back\\slash,foo` for `dc:subject` stelt drie XMP trefwoorden in op het element: `Hello, World!,` `back\slash,` en `foo`.

### XMP- en metagegevensschema-XMP importeren

De XML-import accepteert alleen geldige XML. Bij het importeren van XMP- of metagegevensschemavelden wordt het naamruimtevoorvoegsel toegevoegd en gedraagt het zich hier als een XMP-naamruimte. Deze naamruimte moet worden gedeclareerd. Bijvoorbeeld in de tag op hoofdniveau.

Bijvoorbeeld:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Door tabs gescheiden bestanden voor XMP- en metagegevensschema&#39;s importeren

Het voorvoegsel moet worden toegevoegd aan de gerelateerde kolomkop van het importveld.

## Metagegevens importeren (via FTP) {#import-metadata-via-ftp}

U kunt metagegevens voor meerdere bestanden importeren. U voert de metagegevens in een door tabs gescheiden of XML-bestand in. Selecteer vervolgens **[!UICONTROL Process metadata files]** op de pagina Upload Job Options (Via FTP tab).

Zorg ervoor dat de gegevens in het door tabs gescheiden of XML-bestand de juiste indeling hebben. Voer in de eerste rij het veld Id in, gevolgd door de namen van de metagegevensvelden die moeten worden gewijzigd. Voer in elke volgende rij de naam van een element-id in, gevolgd door metagegevenswaarden. Velden die niet zijn opgenomen in het door tabs gescheiden of XML-bestand, worden niet gewijzigd.

Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Upload]**. Als u de metagegevens wilt importeren, selecteert u op de pagina Uploaden de optie **[!UICONTROL Via FTP]** tab, dan selecteren **[!UICONTROL Job Options]**. Selecteer in het dialoogvenster Opties voor uploaden de optie **[!UICONTROL Job]** en selecteert u vervolgens de **[!UICONTROL Process metadata files]** selectievakje.

## Naam-id&#39;s wijzigen in batch met metagegevens {#batch-rename-ids-using-metadata}

U kunt de naam van Adobe Dynamic Media Classic-id&#39;s wijzigen door metagegevens te importeren uit een door tabs gescheiden bestand of XML-bestand. De geïmporteerde metagegevens worden alleen toegepast op de afbeeldingen die in het metagegevensbestand zelf zijn opgegeven. Het maakt niet uit of afbeeldingen zijn geselecteerd in het deelvenster Bladeren.

Als u de naam van de Adobe Dynamic Media Classic-id van een afbeelding wilt wijzigen, voegt u een kolom met het label *newipsid* aan het lusje-afgebakende dossier, of voeg een genoemd gebied toe `new_vc_objectname` op de XML-gegevens.

Bijvoorbeeld:

| | newipsid |
| --- | --- |
| testjasje_1 | Jasje_test_1 |
| testvest_blue | Jasje_test_2 |

In het taaklogboek voor de metagegevenstaak wordt aangegeven welke id&#39;s zijn hernoemd en welke niet.

## Een sjabloon maken voor het invoeren van te uploaden metagegevens {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic biedt een opdracht voor het maken van een sjabloon voor het opnemen van metagegevens. Met de sjabloon zorgt u ervoor dat de metagegevens in de juiste indeling worden ingevoerd, zodat deze correct naar Adobe Dynamic Media Classic kunnen worden geüpload. Voer de volgende stappen uit om een sjabloon te maken voor het opnemen en importeren van metagegevens naar Adobe Dynamic Media Classic:

1. Selecteer afbeeldingselementen met metagegevensvelden die u voor de sjabloon wilt gebruiken.
1. Ga naar **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. Voor de **[!UICONTROL Asset Properties Type]**, selecteert u **[!UICONTROL Image]**.
1. Van de **[!UICONTROL `Generate File`]** vervolgkeuzelijst kiest u **[!UICONTROL Tab-delimited Template]**, **[!UICONTROL Asset's XML Metadata]**, of **[!UICONTROL XML DTD]**.
1. Selecteren **[!UICONTROL Generate]**.
1. Kopieer de gegevens in het dialoogvenster dat wordt weergegeven. Gebruik deze gegevens om de sjabloon samen te stellen.

## Werken met metagegevensschema&#39;s {#working-with-metadata-schemas}

Een beheerder van het Bedrijf kan een lijst van alle beschikbare schema&#39;s bekijken. Ga op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]**.

In eerste instantie is de lijst met algemene standaardschema&#39;s, zoals XMP, verborgen. Ze kunnen worden weergegeven met het selectievakje onder aan de lijst.

De Beheerder van het Bedrijf kan een douaneschema tot stand brengen, of een bestaand douaneschema uitgeven.

U kunt de Editor Metagegevensschema gebruiken om de volgende handelingen uit te voeren:

| Handeling | Beschrijving |
| --- | --- |
| Toevoegen | Voegt een eigenschap toe aan het schema. Een modaal dialoogvenster verzamelt de informatie: ID, Label, Structuur en Gegevenstype. |
| Keuzevrijheid toevoegen | Voegt een nieuwe selecteerbare keus aan een bezit met structuur Open Keus of Gesloten Keuze toe. Alle keuzevelden hebben hetzelfde type. Selecteer de eigenschap zelf om de knop in te schakelen. |
| Bewerken | Bewerk het label van een eigenschap of keuzevrijheid. U kunt het label, de id en de typegegevens alleen wijzigen als dit niet mogelijk is. |
| Omhoog/Omlaag | De orde in het schema wordt weerspiegeld in UI. Als u de volgorde wilt wijzigen, selecteert u een eigenschap of keuzevrijheid en verplaatst u deze met de knoppen. Slepen en neerzetten wordt momenteel niet ondersteund. |
| Verwijderen | Hiermee verwijdert u een eigenschap of keuzevrijheid uit het schema. Waarden worden niet verwijderd uit het XMP of de database. De eigenschap is niet meer beschikbaar voor weergaven van metagegevens en wordt verwijderd uit de weergave Details van element. Als het bezit aan de Server van Meta-gegevens werd gepubliceerd, voer een kracht uit publiceert om de gegevens uit de openbaar-onder ogen ziet Server van Meta-gegevens te verwijderen. |

Het systeem genereert automatisch een aangepast schema voor door de gebruiker gedefinieerde velden met het voorvoegsel `s7udf`. Het schema bestaat uit bestaande Gebruiker-bepaalde gebieden die in hun eigen sectie van de Opstelling worden uitgegeven.

>[!NOTE]
>
>Door wijzigingen in het schema veranderen de metagegevens van de elementen zelf nooit. Ze zijn echter niet zichtbaar voor alle Adobe Dynamic Media Classic- en Metadata Server-functionaliteit en kunnen niet worden geopend nadat ze zijn gewijzigd. Op dezelfde manier geldt dat als er metagegevens voor een element bestaan, het bijbehorende schema de metagegevens bruikbaar maakt in Adobe Dynamic Media Classic en de Metadata Server.

De redacteur van het Schema van Meta-gegevens biedt een grafische manier aan om een douaneschema binnen Adobe Dynamic Media Classic toe te voegen of uit te geven. Een voorvoegsel, een naamruimte en een lijst met eigenschappen definiëren een schema.

* **[!UICONTROL Name]**: UI-naam voor het schema. Hiermee identificeert u de eigenschappen in Metagegevensweergaven en Geavanceerd zoeken. Vergelijkbaar met XMP secties zoals Standaard, IPTC, PDF.

* **[!UICONTROL Prefix]**: Technische unieke id voor het schema. Beperkt tot de letters a-z en A-Z. Het voorvoegsel is niet zichtbaar in de gebruikersinterface van Adobe Dynamic Media Classic, maar wordt gebruikt wanneer metagegevens voor een element worden opgeslagen in het XMP en de database. Het voorvoegsel identificeert uniek meta-gegevensgebieden in meta-gegevensonderzoek vragen op de Server of de invoer van Meta-gegevens.

* **[!UICONTROL Namespace]**: Technische unieke id voor het schema, doorgaans een URL in het formulier `https://your.company.com/name/version/`. Zie de lijst met standaardschema&#39;s voor voorbeelden. De naamruimte is niet zichtbaar in de gebruikersinterface van Adobe Dynamic Media Classic, maar wordt gebruikt om metagegevens op te slaan in het XMP.

* **[!UICONTROL Description]**: Vrije-vormbeschrijving van het schema.

>[!NOTE]
>
>Het voorvoegsel en de naamruimte kunnen niet worden bewerkt. Als u deze eigenschappen wilt wijzigen, moet u het schema verwijderen en opnieuw maken.

De eigenschappen beschrijven de meta-gegevens die met dit schema in het XMP blok kunnen worden opgeslagen. Een eigenschap bestaat uit:

| Eigenschap | Beschrijving |
| --- | --- |
| ID | Technische id voor deze eigenschap. De id is niet zichtbaar in de gebruikersinterface van Adobe Dynamic Media Classic, maar wordt gebruikt wanneer metagegevens voor een element zijn opgeslagen in het XMP en de database. De id wordt gebruikt om zoekopdrachten te maken op de Metagegevensserver. De id heeft een aantal beperkingen, zoals: `<ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul>` <br>Nadat de id is gemaakt, kan deze niet worden gewijzigd. |
| Label | UI-naam voor deze eigenschap. |
| Structuur | Bepaalt het type van het bezit samen met het Type van Gegevens. Structuur kan een van de volgende zijn:<ul><li>Eenvoudig type: enkele waarde van gegevenstype</li><li>Reeks: een lijst met waarden van hetzelfde gegevenstype</li><li>Open Keuze: selecteer een item in een lijst met vooraf gedefinieerde waarden of voer tekst in. Dit kan alleen van het gegevenstype String of Integer zijn</li><li>Gesloten keuze: selecteer een item uit een lijst met vooraf gedefinieerde waarden (een keuzelijst of keuzelijst met invoervak)</li></ul> |
| Gegevenstype | Maak een keuze uit de volgende beschikbare typen: <ul><li>String</li><li>Geheel</li><li>Float</li><li>Ja/Nee (Boolean)</li><li>Datum</li></ul> |

Wanneer de eigenschap de structuur Open Keuze of Gesloten keuze heeft, moet u ten minste één keuzevrijheid opgeven. De optie Open Keuze kan worden gewijzigd. Gesloten keuze kan niet worden gewijzigd. Alle keuzevelden hebben het gegevenstype van de eigenschap.

| Eigenschap | Beschrijving |
| --- | --- |
| ID | Technische identificatie voor deze waarde. De id is niet zichtbaar in de gebruikersinterface van Adobe Dynamic Media Classic, maar wordt gebruikt wanneer metagegevens voor een element zijn opgeslagen in het XMP en de database. De id wordt gebruikt in zoekopdrachten op de Metagegevensserver. De id mag geen spaties bevatten. Nadat de id is gemaakt, kan deze niet worden gewijzigd. |
| Label | UI-naam voor deze waarde. |

>[!MORELIKETHIS]
>
>* [Voorinstellingen viewer](application-setup.md#viewer_presets)
>* [Voorinstellingen metagegevens](application-setup.md#metadata_presets)
