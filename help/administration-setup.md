---
title: Instellingen voor beheer
description: Leer hoe u het beheergebied van Dynamic Media Classic instelt.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1944'
ht-degree: 0%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Beheerinstellingen{#administration-setup}

De schermen van de Opstelling van het Beleid zijn voor het beheren van de Klassieke gebruikers van Dynamic Media. Gebruik deze schermen om gebruikers in Dynamic Media Classic te laten werken en via e-mail met gebruikers te communiceren.

1. Om tot de opties van de Opstelling van het Beleid toegang te hebben, klik **Opstelling** > **Persoonlijke Opstelling** > **Opstelling van het Beleid**.

## Gebruikersbeheer {#user-administration}

Alle Dynamic Media Classic-gebruikers krijgen een rol toegewezen die hun rechten en toegangsrechten voor functies in Dynamic Media Classic bepaalt. De beheerders bepalen de verschillende rollen en verantwoordelijkheden voor de bedrijven waaraan zij worden toegewezen.

Dynamic Media Classic configureert doorgaans de eerste reeks bedrijven en wijst een bedrijfsbeheerder toe. De bedrijfbeheerder plaatst dan opstelling en beheert de Klassieke gebruikers van Dynamic Media.

Dynamic Media Classic ondersteunt verschillende gebruikersrollen. Deze rollen kunnen tot bedrijven toegang hebben die voor Dynamic Media Classic worden gevestigd:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic** UserCan heeft toegang tot bedrijven waaraan zij zijn toegewezen; geen administratieve taken kan vervullen.

**Adobe Dynamic Media Classic Company** AdminCan bekijkt en beheert alleen hun eigen bedrijven. Een beheerder van het Bedrijf kan alle beleidsfuncties ook uitvoeren, met inbegrip van het toevoegen van beheerders en gebruikers. Een bedrijfsbeheerder kan een gebruiker toevoegen aan de DMC-bedrijfsbeheeraccounts. (Deze rol is de standaardgebruikersrol.)

Nadat u een gebruiker hebt toegevoegd, stuurt Dynamic Media Classic een welkomstbericht naar de gebruiker. Het bericht bevat een wachtwoord en de Klassieke URL van Dynamic Media.

### Een gebruiker of beheerder {#adding-a-user-or-administrator} toevoegen

1. Klik op Setup > Application Setup > Administration Setup > User Administration.
1. Klik op Toevoegen.
1. Voer de naam en het e-mailadres in van de gebruiker of beheerder die u wilt toevoegen en klik op Volgende.

   >[!NOTE]
   >
   >Het apostrof-teken (&#39;) is niet toegestaan in e-mailadressen.

1. Kies een optie Rol om een rol toe te wijzen aan de gebruiker.

   Zie [Dynamic Media Classic user rollen and privileges](administration-setup.md#user_administration).

1. Selecteer een bedrijfsnaam om een gebruiker aan een bedrijf toe te voegen.
1. Als u de gebruiker aan een groep wilt toevoegen (als u een gebruiker of een medewerker van het Portaal van Media toevoegt), daarna klikken en de gebruiker toevoegen.
1. Klik op Opslaan om de gebruikersinstellingen te voltooien.

   Na het bewaren, vraagt een herinnering of wilt u een gebruiker aan een ander bedrijf toevoegen. Klik toevoegen als u de gebruiker aan een bedrijf wilt toevoegen.

   Alle nieuwe gebruikers krijgen een willekeurig gegenereerd wachtwoord. gebruikers moeten de wachtwoorden wijzigen wanneer zij zich voor het eerst aanmelden bij de Dynamic Media Classic-bureaubladtoepassing.

   Nieuwe gebruikers krijgen een welkomstbericht nadat u ze hebt toegevoegd. Het e-mailbericht bevat een tijdelijk wachtwoord en legt uit hoe u zich kunt aanmelden bij Dynamic Media Classic.

   Als de gebruiker het welkomstbericht niet ontvangt, meldt u hem of haar op de pagina Dynamic Media Classic aanmelden (https://s7sps1.scene7.com) en klikt u op Mijn wachtwoord vergeten. Het wachtwoord wordt opnieuw ingesteld en er wordt een nieuwe e-mail verzonden. Neem contact op met Technische ondersteuning als de gebruiker geen e-mail ontvangt en deze zich niet in de map Junk bevindt.

   Wanneer u nieuwe gebruikers van Media Portal toevoegt, kunt u ook naar Setup > Toepassingsinstellingen > Gebruikersbeheer gaan en vervolgens op Gebruikerslijst uploaden klikken en een .csv-bestand selecteren dat maximaal 500 gebruikers bevat.

### Een gebruiker {#deleting-a-user} verwijderen

U kunt gebruikers verwijderen uit Dynamic Media Classic door ze ongeldig te maken. Ongeldige gebruikers worden uit het systeem en alle accounts verwijderd.

1. Klik **Setup** > **Toepassingsinstelling** > A **Beheerinstellingen** > **Gebruikersbeheer**.
1. Selecteer een gebruiker in de lijst en klik op **Bewerken**.
1. Schakel Geldig uit.
1. Klik **Opslaan**.

### Gebruikers {#activating-or-deactivating-users} activeren of deactiveren

Gebruikers die zijn gedeactiveerd, hebben niet langer toestemming om de account in te voeren die boven aan het menu Selecteer accounts om toegang te krijgen wordt vermeld.

1. Klik **Setup** > **Toepassingsinstelling** > A **Beheerinstellingen** > **Gebruikersbeheer**.
1. Schakel in de gebruikerslijst de optie Actief naast de naam van de gebruiker in of uit.

### Gebruikersgegevens {#editing-user-information} bewerken

De gebruikersinformatie die u kunt uitgeven hangt van uw rol als beheerder en de toegewezen rol van de gebruiker af waarvan informatie u wilt uitgeven. Opties die grijs (niet beschikbaar) worden weergegeven, kunnen niet worden bewerkt.

1. Ga naar **Setup** > **Toepassingsinstellingen**> A **Beheerinstellingen** > **Gebruikersbeheer**.
1. Selecteer de gebruiker en klik **Edit**.
1. Selecteer de ingang in de lijst die het bedrijf toont u probeert om toestemmingen of toegang voor te wijzigen, dan de Manage verbinding van het Bedrijf te klikken.
1. Selecteer de gebruikersrol.
1. Als u het groepslidmaatschap van de gebruiker wilt wijzigen (als u een gebruiker of medewerker van Media Portal bewerkt of toevoegt), klikt u op Volgende en bewerkt u het groepslidmaatschap.
1. Klik **Opslaan**.

### De gebruikerslijst {#filtering-and-sorting-the-user-list} filteren en sorteren

U kunt de gebruikerslijst filteren en sorteren om van gebruikers de plaats te bepalen. Alle gebruikers in alle accounts die u beheert, worden weergegeven in de lijst Gebruikers, ongeacht de account die u hebt geselecteerd in het menu Account selecteren voor toegang.

U kunt de volgende filtertechnieken voor gebruikerslijsten gebruiken:

**Filteren op** groepSelecteer het menu Op groep en kies een optie om de lijst te beperken tot gebruikers in een groep.

**Filteren op** gebruikersrolSelecteer het menu Op gebruikersrol en kies een optie om de lijst te beperken tot gebruikers of beheerders van verschillende typen.

**Filteren op** veldnaamSelecteer de optie Filteren op veld inschakelen. Selecteer vervolgens het menu Op veldnaam, kies een kolom voor het filteren van de lijst, selecteer het menu Filterteken en kies een letter. De lijst wordt op een van de kolommen gefilterd met de letter die u hebt gekozen. Schakel de optie Filteren op veld inschakelen uit om de volledige lijst weer te geven.

**Ongeldige** gebruikers uitfilterenSchakel de optie Inclusief ongeldig uit. In de zoekresultaten worden alleen gebruikers weergegeven die zich in het systeem bevinden. Ongeldige gebruikers zijn verwijderd uit het systeem en de accounts die u beheert.

**Sorteren op** kolomkopKlik op een kop om alle gebruikers te sorteren op hun status, alfabetisch op voornaam, achternaam of e-mail, op gebruikersrol of op geldige/ongeldige status.

Als u veel gebruikers hebt, kunt u de grootte van de lijst beperken door het menu Maximale lijstgrootte te selecteren en een aantal te kiezen.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** > **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

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
| Domein | Het aantal URL-aanvragen per domein | Gebruik van afbeeldingen bijhouden op basis van het domein van het verzoek om een afbeelding voor een bepaald bedrijf. (Dynamic Media Classic kan meerdere domeinen per account bieden. Neem voor meer informatie contact op met de Technische ondersteuning.) |
| Videostreaming | Bandbreedtegebruik voor het streamen van video | Het stromen videogebruik van het spoor door bedrijf over specifieke datumwaaiers om verkeerspatronen te bepalen. |
| Video-inhoud | Afspeeltijd van verschillende video&#39;s | Bepaal welke de meest bekeken en minst bekeken video&#39;s zijn. |


Het rapport Inhoud afbeelding biedt informatie over verzoeken om de volgende afbeeldingstypen:

**Image** RequestRequests for images.

**Miniatuur** RequestRequests voor stalen of alternatieve afbeeldingen in viewers.

**Masker** RequestRequests aan afbeeldingen die grijswaardenmaskers retourneren.

**Aanvragen** voor Viewer Tile RequestImage die door een viewer zijn geladen.

**Voor het renderen van Vnt Object** RequestImage moet een afbeelding met opgegeven objecten in de gevraagde vignetten worden geretourneerd.

**Voor het renderen van Vnt Info** RequestImage moet informatie over de gevraagde vignetten worden geretourneerd.

>[!NOTE]
>
>Het rapport Videostreaming is alleen van toepassing op streaming video&#39;s. De weergave van progressieve video&#39;s wordt niet bijgehouden.

### Een rapport {#generating-a-report} genereren

Een rapport over bandbreedte, opslag, afbeeldingsinhoud, domein, videostreaming of video-inhoud genereren:

1. Kies Instellen > Persoonlijke instellingen.
1. Breid de Opstelling van het Beleid uit, en klik dan Bandbreedte &amp; Opslag.
1. Klik op een tabblad: Bandbreedte, opslag, afbeeldingsinhoud, domein, videostreaming of video-inhoud.

   Zie [Typen rapporten](administration-setup.md#types_of_reports).

### Gegevens op verschillende manieren weergeven {#viewing-data-in-different-ways}

Nadat u een rapport hebt gegenereerd op de pagina Bandbreedte en opslag, kunt u opties kiezen voor het weergeven van informatie. U kunt kiezen hoe informatie wordt voorgesteld, informatie in een grafiek of gegevensnet bekijken, en een tijdspanne specificeren voor het vangen van informatie. In de weergave Gegevens kunt u ook gegevens sorteren en kolommen opnieuw rangschikken.

**Het bekijken van gegevens in een grafiek of** gegevensnetKlik de optie van de Mening van de Grafiek om gegevens in een grafiek te bekijken; Klik op de optie Gegevens weergeven om gegevens in een gegevensraster weer te geven.

**Kies een rapportpresentatietype** In het menu Type rapport kiest u Samenvatting, Dagelijks of Maandelijks om gegevens in een samenvattende vorm te ordenen, op dag of op maand. Niet alle rapporten verstrekken deze optie.

**Het specificeren van een** tijdperiodeKies opties om een tijdsperiode voor uw rapport te bepalen, en klik dan Update nadat u een tijdspanne bepaalt:

**Vooraf gedefinieerde** periodeKies een optie in het menu Vooraf gedefinieerd rapport. Kies bijvoorbeeld Vorige maand om gegevens van de vorige maand vast te leggen.

**Aangepaste tijdsperiodeKies Aangepast in het menu Vooraf gedefinieerd rapport.** Kies vervolgens een datum in het menu Beginmaand (of Begindatum) en een datum in het menu # of # of Days). Voor de Rapporten van de Inhoud van het Domein en Video, kunt u een specifieke begin en einddatum kiezen voor het vangen van rapportinformatie.

**Gegevens sorteren (alleen in de gegevensweergave)** Als u gegevens in een kolom wilt sorteren, klikt u op de kop van de kolom. Klik nogmaals om in aflopende volgorde te sorteren.

**Kolommen opnieuw rangschikken (alleen in de weergave Gegevens)** Als u een kolom naar een andere locatie op het gegevensraster wilt verplaatsen, sleept u de kop.

### Rapporten exporteren en afdrukken {#exporting-and-printing-reports}

Nadat u een rapport hebt gegenereerd, kunt u de gegevens exporteren voor gebruik in spreadsheets en andere toepassingen. U kunt ook rapporten afdrukken.

**Het uitvoeren van rapportgegevens** in de mening van Gegevens, sorteer en rangschikt zonodig de gegevens. Open vervolgens het menu Exporteren en kies een indeling: Door tabs gescheiden, door komma&#39;s gescheiden of HTML-opmaak. De gegevens worden naar het klembord gekopieerd in de indeling die u hebt gekozen. U kunt de gegevens nu in een spreadsheet of een toepassing plakken.

**Een** rapport afdrukkenKlik op Afdrukken, kies de gewenste opties in het dialoogvenster Afdrukken en klik op OK.

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

**Id van afbeelding** voor de desbetreffende afbeelding.

**** TimeHet tijdbereik van de eerste keer dat de fout werd gerapporteerd tot de laatste keer dat de fout werd gemeld, binnen de laatste 24 uur.

**** AantalHet aantal fouten dat in de afbeelding wordt gerapporteerd.

**** ResponseThe specific error message. Fouten zijn 4xx of 5xx.

**URL&#39;** sHiermee geeft u de URL weer naar de afbeelding in scène 7.

**** ReferrerHiermee geeft u de URL op voor de website waar de oorspronkelijke aanvraag vandaan komt. De referentie kan elke website zijn die een koppeling naar de afbeelding heeft.

Aan de kolommen URL en Referrer is een kopie-URL gekoppeld om het testen te vereenvoudigen.
