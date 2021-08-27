---
title: Inhoud van deelvenster Info in eCatalogs beheren
description: Leer hoe u de inhoud van het deelvenster Info in eCatalogs in Adobe Dynamic Media Classic beheert.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# Inhoud van deelvenster Info in eCatalogs beheren{#managing-info-panel-content-in-ecatalogs}

Naast het gebruiken van de tekst van de Kaart van het Beeld voor uw rollovers in eCatalogs, kunt u een Comité van Info gebruiken om grotere hoeveelheden het omvergooientekst, met inbegrip van verbindingen toe te voegen. U kunt het InfoPanel ook beheren door getimed caching te gebruiken en inhoudsupdates te plannen.

U kunt de InfoPanel opstelling en gegevens beheren gebruikend de volgende eigenschappen in Adobe Dynamic Media Klassiek:

* In het deelvenster InfoPanel Setup kunt u de sjabloon opgeven die wordt gebruikt om de tekst in het deelvenster Info weer te geven, een standaardreactie voor fouten en het aantal uren dat de informatie in de cache wordt opgeslagen. Bovendien kunt u opgeven of de eCatalogs automatisch worden gepubliceerd.
* In het deelvenster InfoPanel-gegevensinvoer kunt u een CSV-bestand opgeven met de tekst die u wilt weergeven in de rollovertekst van InfoPanel en de tijdstippen voor het bijwerken van de informatie.
* Met het dialoogvenster Metagegevens importeren (dat u opent vanuit de weergave Pagina&#39;s toewijzen) kunt u een TXT-bestand met tabs als scheidingsteken importeren dat de gegevens over de rollover-tekst bevat. U kunt deze optie TXT of het paneel Datafeed met de Csv- dossieroptie voor uw het omvergooientekst gebruiken.
* In de weergave Pagina&#39;s toewijzen kunt u een voorvertoning weergeven van de xml die voor specifieke afbeeldingen met hyperlinks wordt weergegeven.

## Een reactiesjabloon voor eCatalogs instellen {#set-up-a-response-template-for-ecatalogs}

U kunt een van de drie vooraf ingestelde reactiesjablonen selecteren om tekst weer te geven in een deelvenster Info. Deze vooraf ingestelde reactiesjablonen bepalen hoe uw gegevens worden weergegeven in het deelvenster Info: hoeveel kolommen en rijen, tekengrootte, lettertype enzovoort. U kunt een vooraf ingestelde reactiesjabloon selecteren of een eigen sjabloon maken.

>[!NOTE]
>
>U kunt ook de antwoordsjabloon instellen in de voorinstelling voor de viewer. Als u in plaats daarvan de antwoordsjabloon in de voorinstelling voor de viewer wilt gebruiken, voegt u `fmt=1` toe aan het einde van de URL van de informatieserver in de voorinstelling voor de viewer.
>
>Zie [Voorinstellingen voor eCatalog-viewers instellen](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Dubbelklik op uw eCatalog zodat deze in de gedetailleerde weergave wordt geopend.
1. Selecteer het **[!UICONTROL InfoPanel Setup]** paneel.
1. Selecteer een antwoordsjabloon:

   * Selecteer een voorinstelling in het menu Reactiesjabloon. De XML voor het sjabloonontwerp wordt weergegeven in het vak Sjabloon gebruiker.
   * Als u uw eigen reactiesjabloon wilt maken, selecteert u **[!UICONTROL Custom]**. Typ de XML-definitie van de sjabloon in het vak Sjabloon gebruiker. U kunt de vooraf ingestelde malplaatjes als basis voor uw gebruiken.

1. (Optioneel) Typ in het vak Standaardreactie de tekst die u wilt weergeven als bij Adobe Dynamic Media Classic een fout optreedt bij het ophalen van informatie voor een afbeeldingskaart. Als het systeem bijvoorbeeld een bedrijfsnaam en een eCatalog-naam ontvangt, maar geen rollover-id, wordt dit bericht voor de gebruiker weergegeven.
1. Voer in het vak TTL-antwoord het aantal uren in dat u wilt wachten voordat u de gegevens in cache plaatst:

   * Stel een lager getal in als de gegevens vaak gedurende een dag worden bijgewerkt.
   * Stel een hoger getal in als de gegevens relatief stabiel zijn en niet regelmatig hoeven te worden bijgewerkt. De standaardwaarde is tien uur.

1. Selecteer **[!UICONTROL Publish]**.

## Broninhoud importeren voor het deelvenster Info in eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

U kunt een CSV-bestand (comma-separated value file) of een TXT-bestand (tab-delimited file) gebruiken voor de brontekst voor een deelvenster Info voor een eCatalog. Door tabs gescheiden bestanden moeten UTF16-codering (Unicode) gebruiken. U kunt de verschillende bestandstypen op verschillende manieren importeren.

Houd bij het opmaken van broninhoud rekening met de volgende richtlijnen:

* Zorg ervoor dat de tab- en komma-gescheiden gegevens zoveel kolommen bevatten als nodig zijn voor de rollover-sjabloon.
* Controleer of het eerste item of de kolom met gegevens de rollover-id is (gekoppeld aan de waarde rollover_key van de URL&#39;s van de afbeeldingskaart).
* Zorg ervoor dat elk tab- of kommagescheiden item na de id het item is dat u wilt vervangen in de reactiesjabloon. De eerste kolom wordt dus vervangen door $1$, de tweede kolom door $2$ enzovoort.

### CSV-inhoud vanuit een extern gehoste locatie importeren in eCatalogi {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Dubbelklik op de eCatalog zodat deze in de gedetailleerde weergave wordt geopend.
1. Selecteer het **[!UICONTROL InfoPanel Datafeed]** paneel.
1. Voer de URL voor het CSV-bestand in het vak Extern gehoste locatie voor het CSV-bestand in. U kunt de URL in dit veld plakken of rechtstreeks typen.
1. (Optioneel) Geef een tijd op om de inhoud bij te werken met de menu&#39;s Update plannen en selecteer **[!UICONTROL Add]**. U kunt meerdere malen selecteren voor bijwerken. Elke updatetijd wordt weergegeven in het vak Update Times. (Als u een tijd wilt verwijderen, selecteert u deze en selecteert u **[!UICONTROL Delete]**.)
1. (Optioneel) Selecteer **[!UICONTROL Run Update Now]** om de inhoud direct bij te werken.

### Een door tabs gescheiden of CSV-bestand importeren {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Dubbelklik op de eCatalog zodat deze in de gedetailleerde weergave wordt geopend.
1. Selecteer het **[!UICONTROL InfoPanel Setup]** paneel.
1. Selecteer **[!UICONTROL Upload S7Info Content]**.
1. Selecteer **[!UICONTROL Browse]**, selecteer het tab-delimited TXT- dossier, CSV, of Ssv- dossier u wilt gebruiken, en selecteer **[!UICONTROL Open]**.
1. Selecteer **[!UICONTROL Upload]**.

Adobe Dynamic Media Classic stuurt u een e-mailbericht met de mededeling of het uploaden is gelukt of niet.

## Voorvertoning van de rollover-sleuteltekst voor een afbeelding met hyperlinks {#preview-rollover-key-text-for-an-image-map}

Met het scherm Pagina&#39;s toewijzen kunt u de tekst in het deelvenster Info voor de afbeeldingen met hyperlinks op een specifieke pagina van uw eCatalog gemakkelijk en snel weergeven.

1. Selecteer de het omvergooienknoop **[!UICONTROL Edit]** van de Catalogus.
1. Selecteer **[!UICONTROL Map Pages]**.
1. Kies **[!UICONTROL Info Panel]** in het menu Tonen boven aan de tabel aan de rechterkant van het scherm.

   De rollover-toetstekst verschijnt naast elke afbeelding met hyperlinks die tekst van het infodeelvenster bevat.
