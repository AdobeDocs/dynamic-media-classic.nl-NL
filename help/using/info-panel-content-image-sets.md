---
title: Inhoud in deelvenster Info beheren in afbeeldingssets
description: Leer hoe u de inhoud van het deelvenster Info in Afbeeldingssets in Adobe Dynamic Media Classic beheert.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 0%

---

# Inhoud in deelvenster Info beheren in afbeeldingssets{#managing-info-panel-content-in-image-sets}

Naast het gebruiken van de tekst van de Kaart van het Beeld voor uw omvergooien in de Reeksen van het Beeld, kunt u een informatiepaneel gebruiken om grotere hoeveelheden het omvergooientekst, met inbegrip van verbindingen toe te voegen. U kunt het InfoPanel ook beheren door getimed caching te gebruiken en inhoudsupdates te plannen.

U kunt de InfoPanel-instellingen en -gegevens beheren met de volgende functies in Adobe Dynamic Media Classic:

* In het deelvenster InfoPanel Setup kunt u de sjabloon opgeven die wordt gebruikt voor het weergeven van de tekst in het deelvenster Info, een standaardreactie voor fouten en het aantal uren dat de informatie in de cache wordt opgeslagen. Bovendien kunt u specificeren of de Reeks van het Beeld automatisch wordt gepubliceerd.
* In het venster InfoPanel Data feed kunt u een CSV-bestand opgeven met de tekst die u wilt weergeven in de rollovertekst van het deelvenster Info en de tijdstippen voor het bijwerken van de informatie.
* Met het dialoogvenster Metagegevens importeren kunt u een TXT-bestand met tabs als scheidingsteken importeren dat de gegevens over de rollover-tekst bevat. U kunt deze optie TXT of het de voederpaneel van Gegevens InfoPanel met de Csv- dossieroptie voor uw het omvergooientekst gebruiken.

## Een reactiesjabloon instellen voor afbeeldingssets {#set-up-a-response-template-for-image-sets}

U kunt een van de drie vooraf ingestelde reactiesjablonen selecteren om tekst weer te geven in een deelvenster Info. Deze vooraf ingestelde reactiesjablonen bepalen hoe uw informatie wordt weergegeven in het deelvenster Info: hoeveel kolommen en rijen, tekengrootte, lettertype, enzovoort. U kunt een vooraf ingestelde reactiesjabloon selecteren of een eigen sjabloon maken.

**Een reactiesjabloon instellen voor Afbeeldingssets:**

1. Dubbelklik op de afbeeldingsset zodat deze in de gedetailleerde weergave wordt geopend.
1. Selecteren **[!UICONTROL InfoPanel Setup]**.
1. Voer een van de volgende handelingen uit in de vervolgkeuzelijst Antwoordsjabloon:

   * Als u de standaardreactie wilt gebruiken, selecteert u **[!UICONTROL Default]**. De XML voor het sjabloonontwerp wordt grijs weergegeven in het tekstvak Gebruikerssjabloon.
   * Als u uw eigen reactiesjabloon wilt maken, selecteert u **[!UICONTROL Custom]**. Typ de XML-definitie van de sjabloon in het tekstvak Gebruikerssjabloon. U kunt de standaardsjabloon die al in het tekstvak is gedefinieerd, gebruiken als basis voor uw eigen reactie.

1. (Optioneel) Typ in het vak Standaardreactie de tekst die u wilt weergeven als er in Adobe Dynamic Media Classic een fout optreedt bij het ophalen van informatie voor een afbeeldingskaart. Als het systeem bijvoorbeeld een bedrijfsnaam en een naam van een afbeeldingsset ontvangt, maar geen rollover-id, wordt dit bericht voor de gebruiker weergegeven.
1. In het de tekstgebied van TTL van de Reactie, ga het aantal uren in dat u wilt wachten alvorens de gegevens in cache te plaatsen.

   * Stel een lager getal in als de gegevens regelmatig worden bijgewerkt.
   * Stel een hoger getal in als de gegevens relatief stabiel zijn en niet regelmatig hoeven te worden bijgewerkt. De standaardwaarde is tien uur.

1. Selecteren **[!UICONTROL Upload]** om de inhoud van het informatiepaneel, op basis van de waarden rollover_key, te uploaden naar s7info.
1. Blader in het dialoogvenster S7Info uploaden naar het bestand dat u wilt gebruiken en selecteer vervolgens **[!UICONTROL Upload]**.

   Ondersteunde bestandsindelingen zijn door tabs gescheiden bestanden met UTF-16-codering en CSV-bestanden met ASCII-codering. Voor CSV-bestanden moeten niet-ASCII-tekens worden gecodeerd als HTML.

1. Selecteer in het deelvenster InfoPanel Setup de optie **[!UICONTROL Publish]**.

## Broninhoud importeren voor het deelvenster Info in afbeeldingssets {#import-source-content-for-the-info-panel-in-image-sets}

U kunt een CSV-bestand (door komma&#39;s gescheiden waarde) gebruiken met ASCII-codering (niet-ASCII-teken moet zijn gecodeerd als HTML) of een door tabs gescheiden bestand voor de brontekst voor een infopaneel voor een afbeeldingsset. Door tabs gescheiden bestanden moeten UTF-16 (Unicode)-codering gebruiken. U kunt de verschillende bestandstypen op verschillende manieren importeren.

Houd bij het opmaken van broninhoud rekening met de volgende richtlijnen:

* De tab- en komma-gescheiden gegevens kunnen zoveel kolommen bevatten als nodig zijn voor de rollover-sjabloon.
* Het eerste item of de kolom met gegevens is de rollover-id (gekoppeld aan de waarde rollover_key van de URL&#39;s van de afbeeldingskaart).
* Zorg ervoor dat elk tab- of kommagescheiden item na de id het item is dat u wilt vervangen in de reactiesjabloon. De eerste kolom wordt dus vervangen door $1$, de tweede kolom door $2$ enzovoort).

### CSV-inhoud importeren in afbeeldingssets vanaf een extern gehoste locatie {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Dubbelklik op de Afbeeldingsset zodat deze in de gedetailleerde weergave wordt geopend.
1. Selecteren **[!UICONTROL InfoPanel Data feed]**.
1. Voer in het tekstveld HTTP (External Hosted CSV file location) de URL naar het CSV-bestand in.
1. (Optioneel) Geef in de velden Update plannen een tijd op om de inhoud bij te werken en selecteer vervolgens **[!UICONTROL Add]**.

   U kunt meerdere malen selecteren voor bijwerken. Elke updatetijd verschijnt in het de tekstvakje van de Tijden van de Update. Als u een geplande tijd wilt verwijderen, selecteert u deze en selecteert u vervolgens **[!UICONTROL Delete]**.

1. (Optioneel) Selecteer **[!UICONTROL Run Update]** om de inhoud onmiddellijk bij te werken.
