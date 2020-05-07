---
title: Persoonlijke instelling
seo-title: Persoonlijke instelling
description: 'null'
seo-description: Alle gebruikers kunnen montages op het Persoonlijke scherm van de Opstelling van Dynamische Klassieke Media veranderen.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
translation-type: tm+mt
source-git-commit: df0c2897b9fceddde648be53b23e25b13388d6b9
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 1%

---


# Persoonlijke instelling {#personal-setup}

Alle gebruikers kunnen montages op het Persoonlijke scherm van de Opstelling veranderen. Om het Persoonlijke scherm van de Opstelling te openen, klik Opstelling > Persoonlijke Opstelling.

>[!NOTE]
>
>Het Persoonlijke scherm van de Opstelling maakt een lijst van welke gebruikersrol u in het het Publiceren Scene7 Systeem hebt: Bedrijfsbeheerder, beheerder of gebruiker.

De Persoonlijke montages van de Opstelling controleren het standaardgedrag van het Browse Comité, hoe u e-mail, en wachtwoordmontages ontvangt. Vergeet niet op Opslaan te klikken nadat u deze instellingen hebt gewijzigd.

## Mijn accountgegevens

Hiermee worden uw accountnaam, naam, gebruikersnaam (e-mailadres) en toegewezen gebruikersrol geïdentificeerd.

### Desktopversie

Klik installeren nu om de Desktopversie van het Publiceren Scene7 Systeem op uw lokale harde aandrijving te installeren. U kunt ook op Nu opnieuw installeren klikken om de bureaubladversie opnieuw te installeren.

## De insteekmodule installeren op uw lokale vaste schijf

1. Voor de Persoonlijke pagina van de Opstelling in het Publiceren Scene7 Systeem, onder Insteekmodule van de Illustrator voor Web-aan-Druk, klik nu **** Download om het **Insteekmodule van de Illustrator voor Web-aan-Print.zip** dossier te downloaden.
1. Decomprimeer het ZIP-bestand naar een tijdelijke map.

   Er wordt een Lees mij-bestand opgenomen in de hoofdmap van het uitgevouwen bestand om u aanvullende informatie over de insteekmodule te geven.

1. Voer afhankelijk van het geïnstalleerde besturingssysteem een van de volgende handelingen uit:

### Windows

| Als u werkt | Doe dit |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Klik in de hoofdmap van de uitgevouwen map op CC-2014.</li><li>Afhankelijk van de bitversie van Adobe Illustrator die u gebruikt, klikt u op win32 of win64.</li><li>Klik op Bibliotheken > Naam en kopieer `aflame.dll` naar de uitvoerbare map van Adobe Illustrator. Bijvoorbeeld, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Opmerking **: Dit voorbeeldpad is voor de 64-bits locatie; De 32-bits locatie kan in plaats daarvan onder Program Files (x86) vallen.<br/><ul><li>Keer aan de zelfde bibliotheekomslag terug, klik flamingo, en kopieer dan `aflamingo.dll` aan de zelfde uitvoerbare omslag van de Illustrator van Adobe die u in de vorige stap gebruikte. </li><li>Ga terug naar de map win32 of win64 die u in stap 2 hebt geselecteerd en kopieer `AdobeS7FXGFileFormat.aip` deze naar de map met insteekmodules van Adobe Illustrator. Bijvoorbeeld, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Opmerking **: Dit voorbeeldpad is voor de 64-bits locatie; De 32-bits locatie kan in plaats daarvan onder Program Files (x86) vallen. |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Klik in de hoofdmap van de uitgevouwen map op CC. </li><li>Afhankelijk van de bitversie van Adobe Illustrator die u gebruikt, klikt u op win32 of win64.</li><li> Kopieer `AdobeS7FXGFileFormat.aip` naar de map Plug-ins van Adobe Illustrator. Bijvoorbeeld, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Opmerking **: Dit voorbeeldpad is voor de 64-bits locatie; De 32-bits locatie kan in plaats daarvan onder Program Files (x86) vallen. |
| Adobe Illustrator 16 in Adobe Creative Suite 6 | <ul><li>Klik in de hoofdmap van de uitgevouwen map op 6.0. </li><li>Afhankelijk van de bitversie van Adobe Illustrator die u gebruikt, klikt u op win32 of win64. </li><li>Kopieer AdobeS7FXGFileFormat.aip naar de map Plug-ins van Adobe Illustrator. Bijvoorbeeld, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Opmerking **: Dit voorbeeldpad is voor de 64-bits locatie; De 32-bits locatie kan in plaats daarvan onder Program Files (x86) vallen. |

### Mac

| Als u werkt | Doe dit |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Klik in de hoofdmap van de uitgevouwen map op CC-2014 > mac64.</li><li>Klik op Bibliotheken > Naam vlammen en kopieer de `aflame.framework` map naar de pakketinhoudsmap van Adobe Illustrator. Bijvoorbeeld, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Als u de pakketinhoudsmap van Adobe Illustrator wilt openen, klikt u met de rechtermuisknop op het pictogram van Adobe Illustrator CC 2014 en klikt u op Toon pakketinhoud in het contextmenu.)</li><li>Ga terug naar dezelfde bibliotheekmap, klik `flamingo`en kopieer de `aflamingo.framework` map naar dezelfde Adobe Illustrator-pakketinhoudsmap die u in de vorige stap hebt gebruikt.</li><li>Ga terug naar de map mac64 die u in stap 1 hebt geselecteerd en kopieer de `AdobeS7FXGFileFormat.aip` map naar de plug-in van Adobe Illustrator. Bijvoorbeeld, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Klik in de hoofdmap van de uitgevouwen map op CC > mac64</li><li>Kopieer de `AdobeS7FXGFileFormat.aip` map naar de plug-inmap van Adobe Illustrator. Bijvoorbeeld, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 in Adobe Creative Suite 6 | <ul><li>Klik in de hoofdmap van de uitgevouwen map op 6.0 > mac64</li><li>Kopieer de `AdobeS7FXGFileFormat.aip` map naar de plug-inmap van Adobe Illustrator. Bijvoorbeeld, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

U kunt de plug-in nu gebruiken in Adobe Illustrator.

### Browser

* **Miniatuurgrootte**
   * Bepaalt de standaardgrootte van duimnagelbeelden in de mening van het Net in het Browse Comité.
* **Standaardweergave van middelenbibliotheek**
   * Hiermee bepaalt u of de elementen in de elementenbibliotheek voor samenstellen als miniaturen of op naam worden weergegeven. Als u met grote hoeveelheden elementen werkt in de Asset Library, kunt u de elementen op naam bekijken. Als u bijvoorbeeld een grote eCatalog maakt met veel PDF-bestanden, kunt u de elementen op naam weergeven om de lijst korter te maken.
* **Standaard bladersorteervolgorde**
   * Bepaalt de orde waarin de activa door gebrek in het Browse Comité verschijnen. Kies een sorteercriterium in het menu en bepaal of u oplopende of aflopende sortering wilt.
* **Standaardlocatie voor bladeren**
   * Hiermee kunt u de bladerlocatie instellen op de standaardlocatie, de laatste bladermap of een specifieke locatie waarnaar u navigeert en die u herkent. U kunt ook de locatie van de browsers instellen om de bestanden en mappen in oplopende of aflopende volgorde te sorteren.
* **Standaardweergave Bladeren**
   * Hiermee bepaalt u of de rasterweergave of lijstweergave de standaardweergave is die u ziet wanneer u het deelvenster Bladeren voor het eerst opent.
* **Welkomstscherm**
   * Hiermee bepaalt u of er welkomstschermen worden weergegeven, inclusief het welkomstwelkomstscherm.
* **Knopinfo tonen**
   * Hiermee bepaalt u of knopinfo wordt weergegeven wanneer u de aanwijzer over knoppen, menu&#39;s en navigatiekoppelingen beweegt. Knopinfo beschrijft items op het scherm.
* **Achtergrond klembord**
   * Hiermee geeft u een laag met een schaakbordpatroon achter afbeeldingen weer, zodat u de transparante gebieden van een afbeelding met een alfakanaal gemakkelijk kunt zien.
* **Bestandsgrootte tonen**
   * Hiermee geeft u de bestandsgrootte van een element weer wanneer u bladert.
* **Bevestigen bij verlaten van SPS**
   * Toont een bevestigingsvenster alvorens u het Publiceren Scene7 Systeem weggaat.
* **UDF&#39;s opnemen in zoekopdracht**
   * Deze optie is uitgeschakeld (standaard) om de systeemprestaties te verbeteren voor de meeste metagegevenszoekopdrachten die u uitvoert.

Als de meeste zoekopdrachten in metagegevens van nut zijn wanneer u door de gebruiker gedefinieerde velden opneemt, kunt u deze optie selecteren en inschakelen. U kunt ook Geavanceerd zoeken gebruiken om u een gerichtere en snellere zoekervaring te bieden dan het opnemen van door de gebruiker gedefinieerde velden.

Zie [Een geavanceerde zoekopdracht](searching-assets.md#conducting_an_advanced_search)uitvoeren.

Zie ook Door [de gebruiker gedefinieerde velden](application-setup.md#user_defined_fields).

* **Standaardzoektype**
   * Kies een standaardtype zoekopdracht, Bevat of Begint met.
* **Functies van mediaportal tonen**
   * Selecteer deze optie om toegang te krijgen tot functies van Media Portal, zoals Media Cart.
* **Feedback opdracht tonen**
   * Opdrachtaanvragen aan de server tonen.
* **Dialoogvenster tonen tijdens exporteren**
   * Hiermee wordt een dialoogvenster weergegeven wanneer u een exportbewerking uitvoert. Als u deze optie uitschakelt, kunt u nog steeds naar de pagina Taken gaan om de resultaten van uw export op te halen.

## E-mail

* **E-mailopties**
   * Kies hoe u via Dynamic Media Classic via e-mail op de hoogte moet worden gebracht wanneer het uploaden en publiceren van taken is voltooid. U kunt berichten voor het voltooien van een taak alleen ontvangen als er waarschuwingen of fouten zijn opgetreden.
* **E-mailbereik**
   * Hiermee bepaalt u of u alle taken per e-mail voor uw bedrijf ontvangt of alleen e-mail over uploads en publicatietaken die u hebt gestart.
* **E-mailtypen**
   * Hiermee bepaalt u of u op de hoogte wordt gesteld wanneer het uploaden van taken en het publiceren van taken zijn voltooid.
* **Taal**
* **Voorkeurstaal**
   * Bepaalt de taal voor de interface.
* **Wachtwoord**
* **Nieuw wachtwoord**
   * Voer een nieuw, geldig wachtwoord in. Uw wachtwoord moet aan de volgende vereisten voldoen:
      * Tussen 8 en 25 tekens lang zijn
      * Bevat ten minste één kleine letter
      * Bevat ten minste één hoofdletter
      * Bevat minstens één getal
      * Bevat ten minste een van de volgende speciale tekens: #$&amp;-_:{}
* **Wachtwoord opnieuw typen**
   * Voer het nieuwe wachtwoord opnieuw in om te bevestigen dat u het correct invoert.
* **Wachtwoordvervaldatum**
   * Hiermee bepaalt u of uw wachtwoord na 72 dagen verloopt als beveiligingsmaatregel. Als u Ja selecteert, wordt u gevraagd na 72 dagen een nieuw wachtwoord te maken.
