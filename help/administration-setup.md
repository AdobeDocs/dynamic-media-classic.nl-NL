---
title: Instellingen voor beheer
description: Leer hoe u het beheergebied van Dynamic Media Classic instelt.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Administrator
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1814'
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

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Klik op **[!UICONTROL Add]**.
1. Voer de naam en het e-mailadres in van de gebruiker of beheerder die u wilt toevoegen en klik vervolgens op **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >Het apostrof-teken (`‘`) is niet toegestaan in e-mailadressen.

1. Als u een rol aan de gebruiker wilt toewijzen, kiest u een optie Rol.

   Zie [Dynamic Media Classic user rollen and privileges](administration-setup.md#user_administration).

1. Als u een gebruiker aan een bedrijf wilt toevoegen, selecteert u een bedrijfsnaam.
1. Als u de gebruiker aan een groep wilt toevoegen (als u een gebruiker of medewerker van het Portaal van Media toevoegt), klik **[!UICONTROL Next]** en voeg de gebruiker toe.
1. Klik **[!UICONTROL Save]** om de gebruikersinstelling te voltooien.

   Na het bewaren, vraagt een herinnering of wilt u een gebruiker aan een ander bedrijf toevoegen. Klik **[!UICONTROL Add]** als u de gebruiker aan een bedrijf wilt toevoegen.

   Alle nieuwe gebruikers krijgen een willekeurig gegenereerd wachtwoord. gebruikers moeten de wachtwoorden wijzigen wanneer zij zich voor het eerst aanmelden bij de Dynamic Media Classic-bureaubladtoepassing.

   Nieuwe gebruikers krijgen een welkomstbericht nadat u ze hebt toegevoegd. Het e-mailbericht bevat een tijdelijk wachtwoord en legt uit hoe u zich kunt aanmelden bij Dynamic Media Classic.

   Als de gebruiker het welkomstbericht niet ontvangt, meldt u hem of haar op de pagina Dynamic Media Classic aanmelden (https://s7sps1.scene7.com) en klikt u op Mijn wachtwoord vergeten. Het wachtwoord wordt opnieuw ingesteld en er wordt een nieuwe e-mail verzonden. Neem contact op met Technische ondersteuning als de gebruiker geen e-mail ontvangt en deze zich niet in de map Junk bevindt.

   Wanneer u nieuwe gebruikers van Media Portal toevoegt, kunt u ook naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL User Administration]** gaan, dan **[!UICONTROL Upload User List]** klikken en een .csv-bestand selecteren dat niet meer dan 500 gebruikers bevat.

### Een gebruiker {#deleting-a-user} verwijderen

U kunt gebruikers verwijderen uit Dynamic Media Classic door ze ongeldig te maken. Ongeldige gebruikers worden uit het systeem en alle accounts verwijderd.

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecteer een gebruiker in de lijst en klik op **[!UICONTROL Edit]**.
1. Schakel Geldig uit.
1. Klik op **[!UICONTROL Save]**.

### Gebruikers {#activating-or-deactivating-users} activeren of deactiveren

Gebruikers die zijn gedeactiveerd, hebben niet langer toestemming om de account in te voeren die boven aan het menu Selecteer accounts om toegang te krijgen wordt vermeld.

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Schakel in de gebruikerslijst de optie **[!UICONTROL Active]** naast de naam van de gebruiker in of uit.

### Gebruikersgegevens {#editing-user-information} bewerken

De gebruikersinformatie die u kunt uitgeven hangt van uw rol als beheerder en de toegewezen rol van de gebruiker af waarvan informatie u wilt uitgeven. Opties die grijs (niet beschikbaar) worden weergegeven, kunnen niet worden bewerkt.

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecteer de gebruiker en klik **[!UICONTROL Edit]**.
1. Selecteer de ingang in de lijst die het bedrijf toont u probeert om toestemmingen of toegang voor te wijzigen, dan **[!UICONTROL Manage Company]** te klikken.
1. Selecteer de gebruikersrol.
1. Als u het groepslidmaatschap van de gebruiker wilt wijzigen (als u een gebruiker of medewerker van Media Portal bewerkt of toevoegt), klikt u op **[!UICONTROL Next]** en bewerkt u het groepslidmaatschap.
1. Klik op **[!UICONTROL Save]**.

### De gebruikerslijst {#filtering-and-sorting-the-user-list} filteren en sorteren

U kunt de gebruikerslijst filteren en sorteren om van gebruikers de plaats te bepalen. Alle gebruikers in alle accounts die u beheert, worden weergegeven in de lijst Gebruikers, ongeacht de account die u hebt geselecteerd in het menu Account selecteren voor toegang.

U kunt de volgende filtertechnieken voor gebruikerslijsten gebruiken:

* **Filteren op groep**  - Selecteer het  **[!UICONTROL By Group]** menu en kies een optie om de lijst te beperken tot gebruikers in een groep.

* **Filteren op gebruikersrol**  - Selecteer het  **[!UICONTROL By User Role]** menu en kies een optie om de lijst te beperken tot gebruikers of beheerders van verschillende typen.

* **Filteren op veldnaam**  - Selecteren  **[!UICONTROL Enable Filter By Field]**. Selecteer vervolgens het menu **[!UICONTROL By Field Name]**, kies een kolom voor het filteren van de lijst, selecteer het menu Filterteken en kies een letter. De lijst wordt op een van de kolommen gefilterd met de letter die u hebt gekozen. Schakel de optie **[!UICONTROL Enable Filter By Field]** uit om de volledige lijst weer te geven.

* **Ongeldige gebruikers**  uitfilteren - Selectie opheffen  **[!UICONTROL Include Invalid]**. In de zoekresultaten worden alleen gebruikers weergegeven die zich in het systeem bevinden. Ongeldige gebruikers zijn verwijderd uit het systeem en de accounts die u beheert.

* **Sorteren op kolomkop**  - Klik op een kop om alle gebruikers te sorteren op hun status, alfabetisch op voornaam, achternaam of e-mail, op gebruikersrol of op geldige/ongeldige status.

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

De Klassieke Beheerders van Dynamic Media kunnen bandbreedte, opslag, en andere soorten rapporten voor de bedrijven produceren zij beheren. Deze rapporten zijn beschikbaar op de pagina Bandbreedte &amp; Opslag.

Klik op **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** om deze pagina te openen. Breid **[!UICONTROL Administration Setup]** uit, en klik dan **[!UICONTROL Bandwidth & Storage]**.

### Typen rapporten {#types-of-reports}

In de volgende tabel worden de rapporten beschreven die u kunt genereren op de pagina Bandbreedte en opslag:

| Rapport | Informatie | Gebruiken |
|:--- |:--- |:--- |
| Bandbreedte | Bandbreedtegebruik door bedrijf | Het bandbreedtegebruik van het spoor door bedrijf over specifieke datumwaaiers om verkeerspatronen te bepalen. |
| Opslag | Opslaggebruik | Houd de hoeveelheid gegevens bij die door het bedrijf is geüpload. |
| Afbeeldingsinhoud | Het aantal aanvragen voor afbeeldingen per type | Houd het aantal aanvragen en het volume voor verschillende afbeeldingstypen bij. |
| Domein | Het aantal URL-aanvragen per domein | Gebruik van afbeeldingen bijhouden op basis van het domein van het verzoek om een afbeelding voor een bepaald bedrijf. (Dynamic Media Classic kan meerdere domeinen per account bieden. Neem voor meer informatie contact op met de Technische ondersteuning.) |
| Videostreaming | Bandbreedtegebruik voor het streamen van video | Het stromen videogebruik van het spoor door bedrijf over specifieke datumwaaiers om verkeerspatronen te bepalen. |
| Video-inhoud | Afspeeltijd van verschillende video&#39;s | Bepaal welke de meest bekeken en minst bekeken video&#39;s zijn. |

Het rapport Inhoud afbeelding biedt informatie over verzoeken om de volgende afbeeldingstypen:

* **Afbeeldingsverzoek**  - Verzoeken om afbeeldingen.

* **Miniatuuraanvraag**  - Verzoeken om stalen of alternatieve afbeeldingen in viewers.

* **Maskeraanvraag**  - Verzoeken naar afbeeldingen die grijswaardenmaskers retourneren.

* **Tegelaanvraag**  voor viewer - Afbeeldingsverzoeken die door een viewer zijn geladen.

* **Verzoek**  om vnt-object - aanvragen voor het renderen van afbeeldingen die een afbeelding met opgegeven objecten in de gevraagde vignetten retourneren.

* **Verzoek**  om vectorgegevens - aanvragen voor het renderen van afbeeldingen die informatie over de gevraagde vignetten retourneren.

>[!NOTE]
>
>Het rapport Videostreaming is alleen van toepassing op streaming video&#39;s. De weergave van progressieve video&#39;s wordt niet bijgehouden.

### Een rapport {#generating-a-report} genereren

Een rapport over bandbreedte, opslag, afbeeldingsinhoud, domein, videostreaming of video-inhoud genereren:

1. Kies **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Breid de Opstelling van het Beleid uit, en klik dan **[!UICONTROL Bandwidth & Storage]**.
1. Klik op een tabblad: **[!UICONTROL Bandwidth]**, **[!UICONTROL Storage]**, **[!UICONTROL Image Content]**, **[!UICONTROL Domain]**, **[!UICONTROL Video Streaming]** of **[!UICONTROL Video Content]**.

   Zie [Typen rapporten](administration-setup.md#types_of_reports).

### Gegevens op verschillende manieren weergeven {#viewing-data-in-different-ways}

Nadat u een rapport hebt gegenereerd op de pagina Bandbreedte en opslag, kunt u opties kiezen voor het weergeven van informatie. U kunt kiezen hoe informatie wordt voorgesteld, informatie in een grafiek of gegevensnet bekijken, en een tijdspanne specificeren voor het vangen van informatie. In de weergave Gegevens kunt u ook gegevens sorteren en kolommen opnieuw rangschikken.

* **Gegevens weergeven in een diagram of gegevensraster** . Klik  **[!UICONTROL Chart View]** om gegevens in een grafiek weer te geven. Klik  **[!UICONTROL Data View]** om gegevens in een gegevensraster weer te geven.

* **Als u een presentatietype**  voor rapporten kiest, klikt u in het menu Type rapport  **[!UICONTROL Summary]** of  **[!UICONTROL Daily]** of  **[!UICONTROL Monthly]** ordent u de gegevens in een overzichtsvorm, op dag of op maand. Niet alle rapporten verstrekken deze optie.

* **Een tijdsperiode**  opgeven - Kies opties om een tijdsperiode voor uw rapport te definiëren en klik vervolgens  **[!UICONTROL Update]** nadat u een tijdsperiode hebt gedefinieerd:

* **Vooraf gedefinieerde tijdsperiode**  - Kies een optie in het menu Vooraf gedefinieerd rapport. Kies bijvoorbeeld Vorige maand om gegevens van de vorige maand vast te leggen.

* **Periode**  van de douane - op het Vooraf bepaalde menu van het Rapport, klik  **[!UICONTROL Custom]**. Kies vervolgens een datum in het menu **[!UICONTROL Start Month]** (of **[!UICONTROL Start Date]**) en een datum in het menu # of Months (of # of Days). Voor de Rapporten van de Inhoud van het Domein en Video, kunt u een specifieke begin en einddatum kiezen voor het vangen van rapportinformatie.

* **Gegevens sorteren (alleen in de gegevensweergave)**  - Als u gegevens in een kolom wilt sorteren, klikt u op de kop van de kolom. Klik nogmaals om in aflopende volgorde te sorteren.

* **Kolommen opnieuw rangschikken (alleen in de gegevensweergave)**  - Als u een kolom naar een andere locatie op het gegevensraster wilt verplaatsen, sleept u de kop.

### Rapporten exporteren en afdrukken {#exporting-and-printing-reports}

Nadat u een rapport hebt gegenereerd, kunt u de gegevens exporteren voor gebruik in spreadsheets en andere toepassingen. U kunt ook rapporten afdrukken.

* **Het uitvoeren van rapportgegevens**  - in de mening van Gegevens, soort, en rangschikt zonodig de gegevens. Open vervolgens het menu **[!UICONTROL Export]** en kies een indeling: **[!UICONTROL Tab Delimited]**, **[!UICONTROL Comma Separated]** of **[!UICONTROL HTML Formatted]**. De gegevens worden naar het klembord gekopieerd in de indeling die u hebt gekozen. U kunt de gegevens nu in een spreadsheet of een toepassing plakken.

* **Een rapport**  afdrukken - Klik  **[!UICONTROL Print]**, kies de gewenste opties in het dialoogvenster Afdrukken en klik op  **[!UICONTROL OK]**.

## Afbeeldingsfouten {#image-errors}

Klassieke Dynamic Media-beheerders kunnen rapporten met afbeeldingsfouten genereren. Een rapport van de Fout van het Beeld verstrekt een lijst van de 20 meest frequente beeldfouten, voor de afgelopen 24 uren, voor het bedrijf u momenteel het programma wordt geopend aan. Ga als volgt te werk om een rapport Afbeeldingsfout te genereren:

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Breid de Opstelling van het Beleid uit, en klik dan **[!UICONTROL Image Errors]**.
1. (Optioneel) Voer een van de volgende handelingen uit:

   * Als u fouten wilt sorteren op de koptekstgegevens, klikt u op een kop. Standaard worden fouten gesorteerd op aantal exemplaren, hoogste op laagste.
   * Beweeg de curseur over het gebied van de Reactie voor een fout om het specifieke foutenbericht te zien.
   * Als u de koppeling naar de webpagina van de afbeelding of referentie wilt zien, plaatst u de cursor boven het URL-veld of het veld Referenter.
   * Als u de koppeling naar de werkelijke afbeelding wilt kopiëren, klikt u op **[!UICONTROL URL Copy URL]**. U kunt deze koppeling in een browservenster plakken om naar de afbeelding te gaan en de fout te onderzoeken.
   * Klik op **[!UICONTROL Referrer Copy URL]** om de koppeling naar de verwijzende webpagina te kopiëren.

De weergegeven fouten gelden voor het bedrijf waarvoor u momenteel bent aangemeld. Elke fout bevat de volgende informatie:

* **Afbeeldings-id**  - ID voor de beledigende afbeelding.

* **Tijd**  - Het tijdbereik van de eerste keer dat de fout werd gerapporteerd tot de laatste keer dat de fout werd gemeld, binnen de laatste 24 uur.

* **Aantal** : het aantal fouten dat in de afbeelding wordt gemeld.

* **Response**  - Het specifieke foutbericht. Fouten zijn 4xx of 5xx.

* **URL&#39;s** : geeft de URL weer naar de afbeelding in Dynamic Media Classic.

* **Referrer**  - Geeft de URL op voor de website waar de oorspronkelijke aanvraag vandaan komt. De referentie kan elke website zijn die een koppeling naar de afbeelding heeft.

Aan de kolommen URL en Referrer is een kopie-URL gekoppeld om het testen te vereenvoudigen.
