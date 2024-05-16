---
title: Beheerinstellingen
description: Leer hoe u het beheergebied van Adobe Dynamic Media Classic instelt.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Instellingen voor beheer{#administration-setup}

De schermen van de Opstelling van het Beleid zijn voor het beheren van de gebruikers van Adobe Dynamic Media Classic. Gebruik deze schermen om gebruikers in staat te stellen in Adobe Dynamic Media Classic te werken en via e-mail met andere gebruikers te communiceren.

1. Ga naar **Instellen** > **Persoonlijke instelling** > **Instellingen voor beheer**.

## Gebruikersbeheer {#user-administration}

Alle Adobe Dynamic Media Classic-gebruikers krijgen een rol toegewezen die hun rechten en toegangsrechten voor functies in Adobe Dynamic Media Classic bepaalt. De beheerders bepalen de verschillende rollen en verantwoordelijkheden voor de bedrijven waaraan zij worden toegewezen.

Typisch, vormt Adobe Dynamic Media Classic de eerste reeks bedrijven en wijst een Beheerder van het Onderneming toe. De beheerder van het Bedrijf plaatst dan opstelling en beheert de gebruikers van Adobe Dynamic Media Classic.

Adobe Dynamic Media Classic ondersteunt verschillende gebruikersrollen. Deze rollen kunnen tot bedrijven toegang hebben die voor Adobe Dynamic Media Classic worden gevestigd:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic-gebruiker** Kan toegang krijgen tot de ondernemingen waaraan zij zijn toegewezen; kan geen administratieve taken uitvoeren.

**Adobe Dynamic Media Classic Company Admin** Alleen hun eigen bedrijven kunnen weergeven en beheren. Een beheerder van het Bedrijf kan alle beleidsfuncties ook uitvoeren, met inbegrip van het toevoegen van beheerders en gebruikers. Een bedrijfsbeheerder kan een gebruiker toevoegen aan de DMC-bedrijfsbeheeraccounts. (Deze rol is de standaardgebruikersrol.)

Nadat u een gebruiker hebt toegevoegd, stuurt Adobe Dynamic Media Classic de gebruiker een welkomstbericht per e-mail. Het bericht bevat een wachtwoord en de Adobe Dynamic Media Classic-URL.

### Een gebruiker of beheerder toevoegen {#adding-a-user-or-administrator}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecteren **[!UICONTROL Add]**.
1. Voer de naam en het e-mailadres in van de gebruiker of beheerder die u wilt toevoegen en selecteer **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >Het apostrof-teken (`'`) is niet toegestaan in e-mailadressen.

1. Als u een rol aan de gebruiker wilt toewijzen, kiest u een optie Rol.

   Zie [Adobe Dynamic Media Classic-gebruikersrollen en -rechten](administration-setup.md#user_administration).

1. Als u een gebruiker aan een bedrijf wilt toevoegen, selecteert u een bedrijfsnaam.
1. Als u de gebruiker aan een groep wilt toevoegen (als u een gebruiker of medewerker van het Portaal van Media toevoegt), uitgezocht **[!UICONTROL Next]** en voeg de gebruiker toe.
1. Selecteren **[!UICONTROL Save]** om de gebruikersinstellingen te voltooien.

   Na het bewaren, vraagt een herinnering of wilt u een gebruiker aan een ander bedrijf toevoegen. Selecteren **[!UICONTROL Add]** als u de gebruiker aan een bedrijf wilt toevoegen.

   Alle nieuwe gebruikers krijgen een willekeurig gegenereerd wachtwoord. Gebruikers moeten de wachtwoorden wijzigen wanneer zij zich voor het eerst aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing.

   Nieuwe gebruikers krijgen een welkomstbericht nadat u ze hebt toegevoegd. Het e-mailbericht bevat een tijdelijk wachtwoord en legt uit hoe u zich bij Adobe Dynamic Media Classic kunt aanmelden.

   Als de gebruiker het welkomstbericht niet ontvangt, moet hij of zij op de pagina Adobe Dynamic Media Classic aanmelden (https://s7sps1.scene7.com) en **[!UICONTROL Forgot My Password]**. Het wachtwoord wordt opnieuw ingesteld en er wordt een nieuwe e-mail verzonden. Neem contact op met Technische ondersteuning als de gebruiker geen e-mail ontvangt en deze zich niet in de map Junk bevindt.

   Wanneer het toevoegen van nieuwe gebruikers van het Portaal van Media, kunt u ook naar gaan **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL User Administration]** selecteert u vervolgens **[!UICONTROL Upload User List]** en selecteert u een CSV-bestand dat maximaal 500 gebruikers bevat.

### Een gebruiker verwijderen {#delet-a-user}

U kunt gebruikers uit Adobe Dynamic Media Classic verwijderen door ze ongeldig te maken. Ongeldige gebruikers worden uit het systeem en alle accounts verwijderd.

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecteer een gebruiker in de lijst en selecteer vervolgens **[!UICONTROL Edit]**.
1. Schakel Geldig uit.
1. Selecteren **[!UICONTROL Save]**.

### Gebruikers activeren of deactiveren {#activating-or-deactivating-users}

Gebruikers die zijn gedeactiveerd, hebben niet langer toestemming om de account in te voeren die boven aan het menu Selecteer accounts om toegang te krijgen wordt vermeld.

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Schakel in de gebruikerslijst de optie **[!UICONTROL Active]** naast de gebruikersnaam.

### Gebruikersgegevens bewerken {#editing-user-information}

De gebruikersinformatie die u kunt uitgeven hangt van uw rol als beheerder en de toegewezen rol van de gebruiker af waarvan informatie u wilt uitgeven. Opties die grijs (niet beschikbaar) worden weergegeven, kunnen niet worden bewerkt.

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecteer een gebruiker in de lijst en selecteer vervolgens **[!UICONTROL Edit]**.
1. Selecteer de ingang in de lijst die het bedrijf toont u toestemmingen of toegang voor probeert te wijzigen, dan selecteren **[!UICONTROL Manage Company]**.
1. Selecteer de gebruikersrol.
1. Als u het groepslidmaatschap van de gebruiker wilt wijzigen (als u een gebruiker of medewerker van Media Portal bewerkt of toevoegt), selecteert u **[!UICONTROL Next]** en bewerk het groepslidmaatschap.
1. Selecteren **[!UICONTROL Save]**.

### De gebruikerslijst filteren en sorteren {#filtering-and-sorting-the-user-list}

U kunt de gebruikerslijst filteren en sorteren om van gebruikers de plaats te bepalen. Alle gebruikers in alle accounts die u beheert, worden weergegeven in de lijst Gebruikers, ongeacht de account die u hebt geselecteerd in het menu Account selecteren voor toegang.

U kunt de volgende gebruikerslijst-filtrerende technieken gebruiken:

* **Filteren op groep**: Selecteer de **[!UICONTROL By Group]** en kiest u een optie om de lijst te beperken tot gebruikers in een groep.

* **Filteren op gebruikersrol**: Selecteer de **[!UICONTROL By User Role]** en kiest u een optie om de lijst te beperken tot gebruikers of beheerders van verschillende typen.

* **Filteren op veldnaam**: Select **[!UICONTROL Enable Filter By Field]**. Selecteer vervolgens de optie **[!UICONTROL By Field Name]** kiest u een kolom voor het filteren van de lijst, selecteert u het menu Filterteken en kiest u een letter. De lijst wordt op een van de kolommen gefilterd met de letter die u hebt gekozen. Als u de volledige lijst wilt weergeven, schakelt u de optie **[!UICONTROL Enable Filter By Field]** -optie.

* **Ongeldige gebruikers filteren**: Deselecteren **[!UICONTROL Include Invalid]**. In de zoekresultaten worden alleen gebruikers weergegeven die zich in het systeem bevinden. Ongeldige gebruikers zijn verwijderd uit het systeem en de accounts die u beheert.

* **Sorteren op kolomkop**: Selecteer een kop om alle gebruikers te sorteren op hun status, alfabetisch op voornaam, achternaam of e-mail. Of sorteren op gebruikersrol of op geldige/ongeldige status.

Als u veel gebruikers hebt, kunt u de grootte van de lijst beperken door het menu Maximale lijstgrootte te selecteren en een aantal te kiezen.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bandbreedte en opslag {#bandwidth-storage}

Adobe Dynamic Media Classic-beheerders kunnen bandbreedte, opslag en andere typen rapporten genereren voor de bedrijven die ze beheren. Deze rapporten zijn beschikbaar op de pagina Bandbreedte &amp; Opslag.

Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**. Uitbreiden **[!UICONTROL Administration Setup]** en selecteer vervolgens **[!UICONTROL Bandwidth & Storage]**.

### Typen rapporten {#types-of-reports}

In de volgende tabel worden de rapporten beschreven die u kunt genereren op de pagina Bandbreedte en opslag:

| Rapport | Informatie | Gebruiken |
|:--- |:--- |:--- |
| Bandbreedte | Bandbreedtegebruik door bedrijf | Het bandbreedtegebruik van het spoor door bedrijf over specifieke datumwaaiers om verkeerspatronen te bepalen. |
| Opslag | Opslaggebruik | Houd de hoeveelheid gegevens bij die door het bedrijf is geüpload. |
| Afbeeldingsinhoud | Het aantal aanvragen voor afbeeldingen per type | Houd het aantal aanvragen en het volume voor verschillende afbeeldingstypen bij. |
| Domein | Het aantal URL-aanvragen per domein | Gebruik van afbeeldingen bijhouden op basis van het domein van het verzoek om een afbeelding voor een bepaald bedrijf. (Adobe Dynamic Media Classic kan meer dan één domein per account opgeven. Neem voor meer informatie contact op met de Technische ondersteuning.) |
| Videostreaming | Bandbreedtegebruik voor het streamen van video | Het stromen videogebruik van het spoor door bedrijf over specifieke datumwaaiers om verkeerspatronen te bepalen. |
| Video-inhoud | Afspeeltijd van verschillende video&#39;s | Bepaal welke de meest bekeken en minst bekeken video&#39;s zijn. |

Het rapport Inhoud afbeelding biedt informatie over verzoeken om de volgende afbeeldingstypen:

* **Verzoek om afbeelding**: Verzoeken om afbeeldingen.

* **Aanvraag miniatuur**: Verzoeken om stalen of alternatieve afbeeldingen in viewers.

* **Maskeraanvraag**: Verzoeken om afbeeldingen die grijswaardenmaskers retourneren.

* **Tegelaanvraag viewer**: Afbeeldingsverzoeken die door een viewer zijn geladen.

* **VNT-objectaanvraag**: Bij het renderen van afbeeldingen wordt een afbeelding met opgegeven objecten in de gevraagde vignetten geretourneerd.

* **Verzoek om informatie over VNT**: Voor het renderen van afbeeldingen wordt informatie over de gevraagde vignetten geretourneerd.

>[!NOTE]
>
>Het rapport Videostreaming is alleen van toepassing op streaming video&#39;s. De weergave van progressieve video&#39;s wordt niet bijgehouden.

### Een rapport genereren {#generating-a-report}

Een rapport over bandbreedte, opslag, afbeeldingsinhoud, domein, videostreaming of video-inhoud genereren:

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Breid de Opstelling van het Beleid uit, en selecteer dan **[!UICONTROL Bandwidth & Storage]**.
1. Selecteer een tabblad: **[!UICONTROL Bandwidth]**, **[!UICONTROL Storage]**, **[!UICONTROL Image Content]**, **[!UICONTROL Domain]**, **[!UICONTROL Video Streaming]**, of **[!UICONTROL Video Content]**.

   Zie [Typen rapporten](administration-setup.md#types_of_reports).

### Gegevens op verschillende manieren weergeven {#viewing-data-in-different-ways}

Nadat u een rapport hebt gegenereerd op de pagina Bandbreedte en opslag, kunt u opties kiezen voor het weergeven van informatie. U kunt kiezen hoe informatie wordt voorgesteld, informatie in een grafiek of gegevensnet bekijken, en een tijdspanne specificeren voor het vangen van informatie. In de weergave Gegevens kunt u ook gegevens sorteren en kolommen opnieuw rangschikken.

* **Gegevens weergeven in een diagram of gegevensraster**: Select **[!UICONTROL Chart View]** om gegevens in een grafiek te zien; selecteer **[!UICONTROL Data View]** om gegevens in een gegevensraster weer te geven.

* **Kies een presentatietype voor een rapport**: Selecteer in het menu Type rapport de optie **[!UICONTROL Summary]**, **[!UICONTROL Daily]**, of **[!UICONTROL Monthly]** om gegevens in summiere vorm, door dag, of door maand te organiseren. Niet alle rapporten verstrekken deze optie.

* **Een tijdsperiode opgeven**: Kies opties om een tijdsperiode voor uw rapport te definiëren en selecteer **[!UICONTROL Update]** nadat u een tijdsperiode hebt gedefinieerd:

* **Vooraf gedefinieerde tijdsperiode**: Kies een optie in het menu Vooraf gedefinieerd rapport. Kies bijvoorbeeld Vorige maand om gegevens van de vorige maand vast te leggen.

* **Aangepaste tijdsperiode**: Selecteer in het menu Vooraf gedefinieerd rapport de optie **[!UICONTROL Custom]**. Kies vervolgens een datum op het tabblad **[!UICONTROL Start Month]** (of **[!UICONTROL Start Date]**) en een datum in het menu # van maanden (of # of dagen). Voor de Rapporten van de Inhoud van het Domein en Video, kunt u een specifieke begin en einddatum kiezen voor het vangen van rapportinformatie.

* **Gegevens sorteren (alleen in de weergave Gegevens)**: Sorteer gegevens in een kolom. Selecteer de kop van de kolom. Selecteer nogmaals om in aflopende volgorde te sorteren.

* **Kolommen opnieuw rangschikken (alleen in de gegevensweergave)**: Als u een kolom naar een andere locatie op het gegevensraster wilt verplaatsen, sleept u de kop.

### Rapporten exporteren en afdrukken {#exporting-and-printing-reports}

Nadat u een rapport hebt gegenereerd, kunt u de gegevens exporteren voor gebruik in spreadsheets en andere toepassingen. U kunt ook rapporten afdrukken.

* **Rapportgegevens exporteren**: In de weergave Gegevens sorteert u de gegevens en rangschikt u deze zo nodig. Open vervolgens het dialoogvenster **[!UICONTROL Export]** en kiest u een indeling: **[!UICONTROL Tab Delimited]**, **[!UICONTROL Comma Separated]**, of **[!UICONTROL HTML Formatted]**. De gegevens worden naar het klembord gekopieerd in de indeling die u hebt gekozen. U kunt de gegevens nu in een spreadsheet of een toepassing plakken.

* **Een rapport afdrukken**: Select **[!UICONTROL Print]** kiest u de gewenste opties in het dialoogvenster Afdrukken en selecteert u vervolgens **[!UICONTROL OK]**.

## Afbeeldingsfouten {#image-errors}

Adobe Dynamic Media Classic-beheerders kunnen rapporten met afbeeldingsfouten genereren. Een rapport van de Fout van het Beeld verstrekt een lijst van de 20 meest frequente beeldfouten, voor de afgelopen 24 uren, voor het bedrijf u momenteel het programma wordt geopend aan. Ga als volgt te werk om een rapport Afbeeldingsfout te genereren:

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Breid de Opstelling van het Beleid uit, en selecteer dan **[!UICONTROL Image Errors]**.
1. (Optioneel) Voer een van de volgende handelingen uit:

   * Als u fouten wilt sorteren op de koptekstgegevens, selecteert u een kop. Standaard worden fouten gesorteerd op aantal exemplaren, hoogste op laagste.
   * Beweeg de curseur over het gebied van de Reactie voor een fout om het specifieke foutenbericht te zien.
   * Als u de koppeling naar de afbeelding of de verwijzende webpagina wilt zien, plaatst u de cursor boven het URL-veld of het veld Referenter.
   * Selecteer **[!UICONTROL URL Copy URL]**. U kunt deze koppeling in een browservenster plakken om naar de afbeelding te gaan en de fout te onderzoeken.
   * Als u de koppeling naar de verwijzende webpagina wilt kopiëren, selecteert u **[!UICONTROL Referrer Copy URL]**.

De getoonde fouten zijn voor het bedrijf u momenteel het programma wordt geopend aan. Elke fout bevat de volgende informatie:

* **Afbeelding-id**: ID voor de desbetreffende afbeelding.

* **Tijd**: Het tijdbereik van de eerste keer dat de fout werd gerapporteerd tot de laatste keer dat de fout werd gemeld, binnen de laatste 24 uur.

* **Aantal**: Het aantal fouten dat in de afbeelding wordt gerapporteerd.

* **Antwoord**: Het specifieke foutbericht. Fouten zijn 4xx of 5xx.

* **URL&#39;s**: geeft de URL weer naar de afbeelding op Adobe Dynamic Media Classic.

* **Referenter**: Hiermee geeft u de URL op voor de website waar de oorspronkelijke aanvraag vandaan komt. De verwijzer kan om het even welke Website zijn die een verbinding aan het beeld heeft.

Aan de kolommen URL en Referrer is een kopie-URL gekoppeld om het testen te vereenvoudigen.
