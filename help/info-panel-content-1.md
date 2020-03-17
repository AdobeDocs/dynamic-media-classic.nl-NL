---
title: Inhoud van deelvenster Info in afbeeldingssets beheren
seo-title: Inhoud van het deelvenster Info beheren in Afbeeldingssets
description: 'null'
seo-description: Leer hoe u de inhoud van het deelvenster Info in Afbeeldingssets beheert.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Inhoud van deelvenster Info in afbeeldingssets beheren{#managing-info-panel-content-in-image-sets}

Naast het gebruiken van de tekst van de Kaart van het Beeld voor uw omvergooien in de Reeksen van het Beeld, kunt u een informatiepaneel gebruiken om grotere hoeveelheden het omvergooientekst, met inbegrip van verbindingen toe te voegen. U kunt het InfoPanel ook beheren door getimed caching te gebruiken en inhoudsupdates te plannen.

U kunt uw opstelling InfoPanel en gegevens beheren gebruikend de volgende eigenschappen in het Publiceren Scene7 Systeem:

* In het deelvenster InfoPanel Setup kunt u de sjabloon opgeven die wordt gebruikt voor het weergeven van de tekst in het deelvenster Info, een standaardreactie voor fouten en het aantal uren dat de informatie in de cache wordt opgeslagen. Bovendien kunt u specificeren of de Reeks van het Beeld automatisch wordt gepubliceerd.
* In het deelvenster InfoPanel-gegevensinvoer kunt u een CSV-bestand opgeven met de tekst die u wilt weergeven in de rollovertekst van het deelvenster Info en kunt u tijdstippen voor het bijwerken van de gegevens opgeven.
* Met het dialoogvenster Metagegevens importeren kunt u een TXT-bestand met tabs als scheidingsteken importeren dat de gegevens over de rollover-tekst bevat. U kunt deze optie van TXT of het InfoPanel Datafeed paneel met de Csv- dossieroptie voor uw het omvergooientekst gebruiken.

## Een reactiesjabloon instellen voor afbeeldingssets {#set-up-a-response-template-for-image-sets}

U kunt een van de drie vooraf ingestelde reactiesjablonen selecteren om tekst weer te geven in een deelvenster Info. Deze vooraf ingestelde reactiesjablonen bepalen hoe uw gegevens worden weergegeven in het deelvenster Info: hoeveel kolommen en rijen, tekengrootte, lettertype enzovoort. U kunt een vooraf ingestelde reactiesjabloon selecteren of een eigen sjabloon maken.

**Een reactiesjabloon instellen**

1. Dubbelklik op de set Afbeelding om deze te openen in de gedetailleerde weergave.
1. Klik op **InfoPanel Setup** om het deelvenster te ontvouwen.
1. Voer een van de volgende handelingen uit in de vervolgkeuzelijst Antwoordsjabloon:

   * Selecteer Standaard als u het standaardantwoord wilt gebruiken. De XML voor het sjabloonontwerp wordt grijs weergegeven in het tekstvak Gebruikerssjabloon.
   * Selecteer Aangepast om uw eigen reactiesjabloon te maken. Typ de XML-definitie van de sjabloon in het tekstvak Gebruikerssjabloon. U kunt de standaardsjabloon die al in het tekstvak is gedefinieerd, gebruiken als basis voor uw eigen reactie.

1. (Optioneel) Typ in het vak Standaardreactie de tekst die u wilt weergeven als bij Dynamische media Classic een fout optreedt bij het ophalen van informatie voor een afbeeldingskaart. Als het systeem bijvoorbeeld een bedrijfsnaam en een naam van een afbeeldingsset ontvangt, maar geen rollover-id, wordt dit bericht voor de gebruiker weergegeven.
1. In het de tekstgebied van TTL van de Reactie, ga het aantal uren in dat u wilt wachten alvorens de gegevens in het voorgeheugen onder te brengen.

   * Stel een lager getal in als de gegevens regelmatig worden bijgewerkt.
   * Stel een hoger getal in als de gegevens relatief stabiel zijn en niet regelmatig hoeven te worden bijgewerkt. De standaardwaarde is tien uur.

1. Klik op **Uploaden** om de inhoud van het deelvenster Info te uploaden naar s7info op basis van de waarden rollover_key.
1. Blader in het dialoogvenster S7Info uploaden naar het bestand dat u wilt gebruiken en klik op **Uploaden**.

   Ondersteunde bestandsindelingen zijn door tabs gescheiden bestanden met UTF-16-codering en CSV-bestanden met ASCII-codering. Voor CSV-bestanden moeten niet-ASCII-tekens HTML-gecodeerd zijn.

1. Klik in het deelvenster InfoPanel Setup op **Publiceren**.

## Broninhoud importeren voor het deelvenster Info in afbeeldingssets {#import-source-content-for-the-info-panel-in-image-sets}

U kunt een CSV-bestand (door komma&#39;s gescheiden waarde) gebruiken met ASCII-codering (niet-ASCII-teken moet door HTML zijn gecodeerd) of een door tabs gescheiden bestand voor de brontekst voor een infopaneel voor een afbeeldingsset. Door tabs gescheiden bestanden moeten UTF-16 (Unicode)-codering gebruiken. U kunt de verschillende bestandstypen op verschillende manieren importeren.

Houd bij het opmaken van broninhoud rekening met de volgende richtlijnen:

* De tab- en komma-gescheiden gegevens moeten zoveel kolommen bevatten als nodig zijn voor de rollover-sjabloon.
* Het eerste item of de kolom met gegevens moet de rollover-id zijn (gekoppeld aan de waarde rollover_key van de URL&#39;s van de afbeeldingskaart).
* Zorg ervoor dat elk tab- of kommagescheiden item na de id het item is dat u wilt vervangen in de reactiesjabloon (zodat de eerste kolom wordt vervangen door $1$, de tweede kolom door $2$ enzovoort).

### CSV-inhoud importeren in afbeeldingssets vanaf een extern gehoste locatie {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Dubbelklik op de set Afbeelding om deze te openen in de gedetailleerde weergave.
1. Klik op Gegevensinvoer **InfoPanel** om het deelvenster te ontvouwen.
1. Voer in het tekstveld HTTP (External Hosted CSV file location) de URL naar het CSV-bestand in.
1. (Optioneel) Geef in de velden Update plannen een tijd op om de inhoud bij te werken en klik vervolgens op **Toevoegen**.

   U kunt meerdere malen selecteren voor bijwerken. Elke updatetijd verschijnt in het de tekstvakje van de Tijden van de Update. Als u een geplande tijd wilt verwijderen, selecteert u deze en klikt u op **Verwijderen**.

1. (Optioneel) Klik op Bijwerken **uitvoeren** om de inhoud direct bij te werken.
