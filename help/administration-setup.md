---
title: Instellingen voor beheer
seo-title: Instellingen voor beheer
description: 'null'
seo-description: Leer hoe u het beheergebied van Dynamic Media Classic instelt.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Instellingen voor beheer{#administration-setup}

De schermen van de Opstelling van het Beleid zijn voor het beheren van Dynamic Media Klassieke gebruikers. Gebruik deze schermen om gebruikers in Dynamic Media Klassiek te laten werken en door e-mail met gebruikers te communiceren.

1. Om tot de opties van de Opstelling van het Beleid toegang te hebben, klik **Opstelling** > **Persoonlijke Opstelling** > de Opstelling **van het** Beleid.

## Gebruikersbeheer {#user-administration}

Alle Dynamic Media Klassieke gebruikers worden toegewezen een rol die hun voorrechten en toegangsrechten op eigenschappen in Dynamic Media Klassiek bepaalt. De beheerders bepalen de verschillende rollen en verantwoordelijkheden voor de bedrijven waaraan zij worden toegewezen.

Typisch, vormt de Klassieke Dynamic Media de eerste reeks bedrijven en wijst een bedrijfbeheerder toe. De bedrijfbeheerder plaatst dan opstelling en beheert Dynamic Media Klassieke gebruikers.

Classic van Dynamic Media steunt verscheidene gebruikersrollen. Deze rollen kunnen tot bedrijven toegang hebben die voor de Klassieke Dynamic Media worden gevestigd:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**De Klassieke Gebruiker** van Adobe Dynamic Media kan tot bedrijven toegang hebben waaraan zij zijn toegewezen; geen administratieve taken kan vervullen.

**Adobe Dynamic Media Classic Company Admin** kan alleen hun eigen bedrijven weergeven en beheren. Een beheerder van het Bedrijf kan alle beleidsfuncties ook uitvoeren, met inbegrip van het toevoegen van beheerders en gebruikers. Een bedrijfsbeheerder kan een gebruiker toevoegen aan de DMC-bedrijfsbeheeraccounts. (Deze rol is de standaardgebruikersrol.)

Nadat u een gebruiker hebt toegevoegd, stuurt Dynamic Media Classic de gebruiker een welkomste-mailbericht. Het bericht bevat een wachtwoord en de Klassieke URL van Dynamic Media.

### Een gebruiker of beheerder toevoegen {#adding-a-user-or-administrator}

1. Klik op Setup > Application Setup > Administration Setup > User Administration.
1. Klik op Toevoegen.
1. Voer de naam en het e-mailadres in van de gebruiker of beheerder die u wilt toevoegen en klik op Volgende.

   >[!NOTE]
   >
   >Het apostrof-teken (&#39;) is niet toegestaan in e-mailadressen.

1. Kies een optie Rol om een rol toe te wijzen aan de gebruiker.

   Zie [Dynamic Media Klassieke gebruikersrollen en voorrechten](administration-setup.md#user_administration).

1. Selecteer een bedrijfsnaam om een gebruiker aan een bedrijf toe te voegen.
1. Als u de gebruiker aan een groep wilt toevoegen (als u een gebruiker of een medewerker van het Portaal van Media toevoegt), daarna klikken en de gebruiker toevoegen.
1. Klik op Opslaan om de gebruikersinstellingen te voltooien.

   Na het bewaren, vraagt een herinnering of wilt u een gebruiker aan een ander bedrijf toevoegen. Klik toevoegen als u de gebruiker aan een bedrijf wilt toevoegen.

   Alle nieuwe gebruikers krijgen een willekeurig gegenereerd wachtwoord. gebruikers moeten wachtwoorden wijzigen wanneer zij zich voor het eerst aanmelden bij Dynamic Media Classic.

   Nieuwe gebruikers krijgen een welkomstbericht nadat u ze hebt toegevoegd. E-mail verstrekt een tijdelijk wachtwoord en verklaart hoe te login aan Scene 7 het Publiceren Systeem.

   Als de gebruiker de welkomste-mail niet ontvangt, moet hij of zij op de pagina Dynamic Media Classic aanmelden (https://s7sps1.scene7.com) en op Mijn wachtwoord vergeten klikken. Het wachtwoord wordt opnieuw ingesteld en er wordt een nieuwe e-mail verzonden. Neem contact op met Technische ondersteuning als de gebruiker geen e-mail ontvangt en deze zich niet in de map Junk bevindt.

   Wanneer u nieuwe gebruikers van Media Portal toevoegt, kunt u ook naar Setup > Toepassingsinstellingen > Gebruikersbeheer gaan en vervolgens op Gebruikerslijst uploaden klikken en een .csv-bestand selecteren dat maximaal 500 gebruikers bevat.

### Een gebruiker verwijderen {#deleting-a-user}

U kunt gebruikers uit Dynamic Media Klassiek schrappen door hen ongeldig te maken. Ongeldige gebruikers worden uit het systeem en alle accounts verwijderd.

1. Klik **Opstelling** > **Opstelling** van de Toepassing >**Opstelling** van het Beleid > **Gebruikersbeleid**.
1. Selecteer een gebruiker in de lijst en klik op **Bewerken**.
1. Schakel Geldig uit.
1. Klik op **Opslaan**.

### Gebruikers activeren of deactiveren {#activating-or-deactivating-users}

Gebruikers die zijn gedeactiveerd, hebben niet langer toestemming om de account in te voeren die boven aan het menu Selecteer accounts om toegang te krijgen wordt vermeld.

1. Klik **Opstelling** > **Opstelling** van de Toepassing >**Opstelling** van het Beleid > **Gebruikersbeleid**.
1. Schakel in de gebruikerslijst de optie Actief naast de naam van de gebruiker in of uit.

### Gebruikersgegevens bewerken {#editing-user-information}

De gebruikersinformatie die u kunt uitgeven hangt van uw rol als beheerder en de toegewezen rol van de gebruiker af waarvan informatie u wilt uitgeven. Opties die grijs (niet beschikbaar) worden weergegeven, kunnen niet worden bewerkt.

1. Ga naar **Setup** > **Application Setup**>**Administration Setup** > **User Administration**.
1. Selecteer de gebruiker en klik op **Bewerken**.
1. Selecteer de ingang in de lijst die het bedrijf toont u probeert om toestemmingen of toegang voor te wijzigen, dan de Manage verbinding van het Bedrijf te klikken.
1. Selecteer de gebruikersrol.
1. Als u het groepslidmaatschap van de gebruiker wilt wijzigen (als u een gebruiker of medewerker van Media Portal bewerkt of toevoegt), klikt u op Volgende en bewerkt u het groepslidmaatschap.
1. Klik op **Opslaan**.

### De gebruikerslijst filteren en sorteren {#filtering-and-sorting-the-user-list}

U kunt de gebruikerslijst filteren en sorteren om van gebruikers de plaats te bepalen. Alle gebruikers in alle accounts die u beheert, worden weergegeven in de lijst Gebruikers, ongeacht de account die u hebt geselecteerd in het menu Account selecteren voor toegang.

U kunt de volgende filtertechnieken voor gebruikerslijsten gebruiken:

**Filteren op groep** Selecteer het menu Op groep en kies een optie om de lijst te beperken tot gebruikers in een groep.

**Filteren op gebruikersrol** Selecteer het menu Op gebruikersrol en kies een optie om de lijst te beperken tot gebruikers of beheerders van verschillende typen.

**Filteren op veldnaam** Selecteer de optie Filteren op veld inschakelen. Selecteer vervolgens het menu Op veldnaam, kies een kolom voor het filteren van de lijst, selecteer het menu Filterteken en kies een letter. De lijst wordt op een van de kolommen gefilterd met de letter die u hebt gekozen. Schakel de optie Filteren op veld inschakelen uit om de volledige lijst weer te geven.

**Ongeldige gebruikers** uitfilteren Schakel de optie Inclusief ongeldig uit. In de zoekresultaten worden alleen gebruikers weergegeven die zich in het systeem bevinden. Ongeldige gebruikers zijn verwijderd uit het systeem en de accounts die u beheert.

**Sorteren op kolomkop** Klik op een kop om alle gebruikers te sorteren op hun status, alfabetisch op voornaam, achternaam of e-mail, op gebruikersrol of op geldige/ongeldige status.

Als u veel gebruikers hebt, kunt u de grootte van de lijst beperken door het menu Maximale lijstgrootte te selecteren en een aantal te kiezen.

### Een IMS-gebruikersidentiteit koppelen aan een Classic IPS-gebruikersaccount voor Dynamic Media {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

U kunt een Adobe IMS gebruikersidentiteit met een Dynamic Media Klassieke IPS gebruikersrekening verbinden zodat kunt u SSO (Enige Sign On) gebruiken om het Publiceren Scene7 Systeem van binnen Adobe Marketing Cloud aan te melden en te lanceren.

1. Adobe zou al opstelling uw rekening met een organisatie van de Adobe Marketing Cloud moeten hebben en het aan uw Scene7 het Publiceren van het Systeem productcontext koppelde. Neem contact op met de klantenservice van Adobe als deze installatie nog niet is uitgevoerd of als u niet zeker weet of deze is uitgevoerd.

   Wanneer de opstelling volledig is, kunt u login aan Adobe Marketing Cloud en uw identiteit van de Adobe Marketing Cloud met uw Dynamic Media Klassieke gebruikersrekening verbinden door het volgende te doen.

1. Navigeer in Adobe Marketing Cloud naar de accountinstellingen.
1. Klik op **Organisaties** beheren.
1. Klik op **Koppelingsaccount** of **Toegang** ophalen.
1. Selecteer **Experience Manager** en typ uw referenties.

   Uw geloofsbrieven omvatten uw IPS bedrijfgebied, e-mailadres, en wachtwoord.

1. Klik op **Koppeling**.
1. Wanneer de verbinding wordt geplaatst, kunt u het Publiceren Scene7 Systeem van binnen Adobe Marketing Cloud lanceren, of u kunt het direct lanceren.

   Voer een van de volgende handelingen uit:

   * Als u Dynamic Media Classic vanuit de Adobe Marketing Cloud wilt starten, klikt u in de linkerrails van de Adobe Marketing Cloud op **Oplossingen** > **Experience Manager**. Klik op **Starten onder Klassieke kaart van Dynamic Media**.
   * Om aan het Publiceren Scene7 Systeem direct het programma te openen gebruikend uw geloofsbrieven IMS, gebruik de volgende website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Vervang &quot;N&quot;in de bovengenoemde weg met het aantal voor uw IPS bedrijfgebied. Dat wil zeggen: N = 1 voor Noord-Amerika; 3 voor EMEA; of 5 voor JAPAC.

## Bandbreedte en opslag {#bandwidth-storage}

De Klassieke Beheerders van Dynamic Media kunnen bandbreedte, opslag, en andere soorten rapporten voor de bedrijven produceren zij beheren. Deze rapporten zijn beschikbaar op het scherm Bandbreedte en opslag.

Klik op Instellen > Persoonlijke instellingen om dit scherm te openen. Breid de Opstelling van het Beleid uit, en klik dan Bandbreedte &amp; Opslag.

### Typen rapporten {#types-of-reports}

In de volgende tabel worden de rapporten beschreven die u kunt genereren op het scherm Bandbreedte en opslag:

| Rapport | Informatie | Gebruiken |
|:--- |:--- |:--- |
| Bandbreedte | Bandbreedtegebruik door bedrijf | Het bandbreedtegebruik van het spoor door bedrijf over specifieke datumwaaiers om verkeerspatronen te bepalen. |
| Opslag | Opslaggebruik | Houd de hoeveelheid gegevens bij die door het bedrijf is geüpload. |
| Afbeeldingsinhoud | Het aantal aanvragen voor afbeeldingen per type | Houd het aantal aanvragen en het volume voor verschillende afbeeldingstypen bij. |
| Domein | Het aantal URL-aanvragen per domein | Gebruik van afbeeldingen bijhouden op basis van het domein van het verzoek om een afbeelding voor een bepaald bedrijf. (Dynamic Media Klassiek kan meer dan één domein per rekening verstrekken. Neem voor meer informatie contact op met de Technische ondersteuning.) |
| Videostreaming | Bandbreedtegebruik voor het streamen van video | Het stromen videogebruik van het spoor door bedrijf over specifieke datumwaaiers om verkeerspatronen te bepalen. |
| Video-inhoud | Afspeeltijd van verschillende video&#39;s | Bepaal welke de meest bekeken en minst bekeken video&#39;s zijn. |


Het rapport Inhoud afbeelding biedt informatie over verzoeken om de volgende afbeeldingstypen:

**Aanvragen** om afbeeldingen.

**Aanvragen** voor miniatuuraanvraag voor stalen of alternatieve afbeeldingen in viewers.

**Aanvragen** voor maskers voor afbeeldingen waarbij grijswaardenmaskers worden geretourneerd.

**Aanvragen voor** afbeelding voor viewertegel worden door een viewer geladen.

**Voor het renderen van een** vnt-object-afbeelding wordt een afbeelding met opgegeven objecten in de gevraagde vignetten geretourneerd.

**Voor het renderen van** vlakinfo-aanvragen voor afbeeldingen wordt informatie over de gevraagde vignetten geretourneerd.

>[!NOTE]
>
>Het rapport Videostreaming is alleen van toepassing op streaming video&#39;s. De weergave van progressieve video&#39;s wordt niet bijgehouden.

### Een rapport genereren {#generating-a-report}

Een rapport over bandbreedte, opslag, afbeeldingsinhoud, domein, videostreaming of video-inhoud genereren:

1. Kies Instellen > Persoonlijke instellingen.
1. Breid de Opstelling van het Beleid uit, en klik dan Bandbreedte &amp; Opslag.
1. Klik op een tabblad: Bandbreedte, opslag, afbeeldingsinhoud, domein, videostreaming of video-inhoud.

   Zie [Typen rapporten](administration-setup.md#types_of_reports).

### Gegevens op verschillende manieren weergeven {#viewing-data-in-different-ways}

Nadat u een rapport hebt gegenereerd op de pagina Bandbreedte en opslag, kunt u opties kiezen voor het weergeven van informatie. U kunt kiezen hoe informatie wordt voorgesteld, informatie in een grafiek of gegevensnet bekijken, en een tijdspanne specificeren voor het vangen van informatie. In de weergave Gegevens kunt u ook gegevens sorteren en kolommen opnieuw rangschikken.

**Het bekijken gegevens in een grafiek of gegevensnet** klikken de optie van de Mening van de Grafiek om gegevens in een grafiek te bekijken; Klik op de optie Gegevens weergeven om gegevens in een gegevensraster weer te geven.

**Kies een presentatietype** Rapport Op het menu Type rapport en kies Samenvatting, Dagelijks of Maandelijks om gegevens in een samenvattende vorm, op dag of op maand te ordenen. Niet alle rapporten verstrekken deze optie.

**Een tijdsperiode** opgeven Kies opties om een tijdsperiode voor uw rapport te definiëren en klik vervolgens op Bijwerken nadat u een tijdsperiode hebt gedefinieerd:

**Vooraf gedefinieerde tijdsperiode** Kies een optie in het menu Vooraf gedefinieerd rapport. Kies bijvoorbeeld Vorige maand om gegevens van de vorige maand vast te leggen.

**Kies Aangepaste tijdsperiode** in het menu Vooraf gedefinieerd rapport. Kies vervolgens een datum in het menu Beginmaand (of Begindatum) en een datum in het menu # of # of Days). Voor de Rapporten van de Inhoud van het Domein en Video, kunt u een specifieke begin en einddatum kiezen voor het vangen van rapportinformatie.

**Gegevens sorteren (alleen in de gegevensweergave)** Als u gegevens in een kolom wilt sorteren, klikt u op de kop van de kolom. Klik nogmaals om in aflopende volgorde te sorteren.

**Kolommen opnieuw rangschikken (alleen in de gegevensweergave)** Als u een kolom naar een andere locatie op het gegevensraster wilt verplaatsen, sleept u de kop.

### Rapporten exporteren en afdrukken {#exporting-and-printing-reports}

Nadat u een rapport hebt gegenereerd, kunt u de gegevens exporteren voor gebruik in spreadsheets en andere toepassingen. U kunt ook rapporten afdrukken.

**Het uitvoeren van rapportgegevens** in de mening van Gegevens, sorteer en rangschikt zonodig de gegevens. Open vervolgens het menu Exporteren en kies een indeling: Door tabs gescheiden, door komma&#39;s gescheiden of HTML-opmaak. De gegevens worden naar het klembord gekopieerd in de indeling die u hebt gekozen. U kunt de gegevens nu in een spreadsheet of een toepassing plakken.

**Het drukken van een rapport** klikt Druk, kiest de opties u in de de dialoogdoos van de Druk wilt, en dan O.K. klikken.

## Afbeeldingsfouten {#image-errors}

Klassieke Dynamic Media-beheerders kunnen rapporten met afbeeldingsfouten genereren. Een rapport van de Fout van het Beeld verstrekt een lijst van de 20 meest frequente beeldfouten, voor de afgelopen 24 uren, voor het bedrijf u momenteel het programma wordt geopend aan. Ga als volgt te werk om een rapport Afbeeldingsfout te genereren:

1. Klik Opstelling > Persoonlijke Opstelling.
1. Breid de Opstelling van het Beleid uit, en klik dan de Fouten van het Beeld.
1. (Optioneel) Voer een van de volgende handelingen uit:

   * Klik op een kop om fouten te sorteren op koptekstgegevens. Standaard worden fouten gesorteerd op aantal exemplaren, hoogste op laagste.
   * Beweeg de curseur over het gebied van de Reactie voor een fout om het specifieke foutenbericht te zien.
   * Plaats de cursor boven het URL-veld of het verwijzingsveld om de koppeling naar de afbeelding of verwijzende webpagina weer te geven.
   * Klik URL van het Exemplaar URL om de verbinding aan het daadwerkelijke beeld te kopiëren. U kunt deze koppeling in een browservenster plakken om naar de afbeelding te gaan en de fout te onderzoeken.
   * Klik op URL van verwijzingskopie om de koppeling naar de verwijzingswebpagina te kopiëren.

De weergegeven fouten gelden voor het bedrijf waarvoor u momenteel bent aangemeld. Elke fout bevat de volgende informatie:

**Id** van afbeelding voor de desbetreffende afbeelding.

**Tijd** Het tijdbereik van de eerste keer dat de fout werd gerapporteerd tot de laatste keer dat de fout werd gemeld, binnen de laatste 24 uur.

**Aantal** het aantal fouten dat in de afbeelding is gemeld.

**Reactie** op het specifieke foutbericht. Fouten zijn 4xx of 5xx.

**URLs** maakt een lijst van URL aan het beeld op Scène 7.

**Referrer** geeft de URL op voor de website waar de oorspronkelijke aanvraag vandaan komt. De referentie kan elke website zijn die een koppeling naar de afbeelding heeft.

Aan de kolommen URL en Referrer is een kopie-URL gekoppeld om het testen te vereenvoudigen.
