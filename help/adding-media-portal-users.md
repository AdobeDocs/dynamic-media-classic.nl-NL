---
title: Gebruikers van Media Portal toevoegen en beheren
seo-title: Gebruikers van Media Portal toevoegen en beheren
description: 'null'
seo-description: Meer informatie over het toevoegen en beheren van gebruikers van Media Portal
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---


# Gebruikers van Media Portal toevoegen en beheren{#adding-and-managing-media-portal-users}

Als beheerder kunt u gebruikers toevoegen en beheren, beslissen of ze wachtwoorden kunnen wijzigen, gebruikersgegevens kunnen bewerken en gebruikerslijsten kunnen uploaden. Deze taken worden verwezenlijkt op het scherm van het Beleid van de Gebruiker. Klik op **Setup** > **Application Setup** > **Administration Setup** > **User Administration** om dit scherm te openen.

>[!NOTE]
>
>Voordat u gebruikers toevoegt, moet u groepen instellen voor het beheer ervan. Met Mediaportal kunt u geen gebruiker toevoegen zonder de gebruiker aan een of meer groepen toe te wijzen. Voor meer informatie, zie het [Creëren van en het leiden van de Poortgroepen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)van Media.

## Wachtwoorden voor Media Portal verwerken {#handling-media-portal-passwords}

De gebruikers van het Portaal van media, de medewerkers, en de medewerker-gebruikers worden verzonden een welkome e-mailbericht met een wachtwoord wanneer u hen omhoog ondertekent. Beheerders kunnen bepalen of gebruikers van Media Portal dit wachtwoord kunnen wijzigen.

1. Klik op **Instellen** > **Media Portal instellen** > **Algemene instellingen**.
1. Schakel op de pagina Algemene instellingen de optie Gebruikers van Media Portal **toestaan hun wachtwoord** te wijzigen in of uit.
1. Klik op **Opslaan**.

>[!NOTE]
>
>De gebruikers van het Portaal van media die wachtwoorden mogen veranderen kunnen dit doen door **Opstelling** > **Persoonlijke Opstelling** te klikken en wachtwoorden op het Persoonlijke scherm van de Opstelling te veranderen.

## Een gebruiker van het Media Portal toevoegen {#adding-a-media-portal-user}

1. Klik op **Instellen** > **Toepassingsinstelling** > **Beheerinstellingen** > **Gebruikersbeheer**.
1. Klik op de pagina Gebruikersbeheer op **Toevoegen**.
1. Voer in het dialoogvenster Gebruiker toevoegen in het deelvenster Gebruikersinfo de voornaam, achternaam en e-mailadres van de gebruiker in en klik op **Volgende**.
1. Selecteer in het deelvenster Bedrijf/Rol in de vervolgkeuzelijst Bedrijven een bedrijf of bedrijven voor de gebruiker.
1. Selecteer in de lijst Rol een rol voor Media Portal en klik op **Volgende**.

   Zie Gebruikersrollen [van](media-portal-user-roles.md#media_portal_user_roles)Media Portal.

1. Selecteer een of meer groepen in het deelvenster Toegangsgroepen.

   Zie [Mediaportaalgroepen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)maken en beheren.

1. (Optioneel) Klik op **E-mailinstellingen** om andere e-mailinstellingen te kiezen dan de standaardinstellingen.

   Zie [Opstelling het Welkome e-mailbericht voor gebruikers](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)van het Portaal van Media.

1. Klik op Gebruiker **** toevoegen.

Nadat u een gebruiker hebt toegevoegd, verzendt het Portaal van Media de gebruiker een Welkome e-mailbericht. Het bericht bevat een tijdelijk wachtwoord en de URL van het Media Portal.

## Een gebruikerslijst voor een mediaportaal uploaden {#uploading-a-media-portal-user-list}

Als u meerdere gebruikers wilt toevoegen, kunt u een gebruikerslijst uploaden. De gebruikers worden automatisch toegevoegd aan het geselecteerde account.

Maak de gebruikerslijst als een CSV-bestand (met door komma&#39;s gescheiden waarden) dat de gebruikersgegevens bevat. Nadat de lijst is geüpload, worden de gebruikers in de lijst automatisch toegevoegd aan de account met hun opgegeven groepstoewijzingen. Een welkomste-mail wordt verzonden naar elke nieuwe gebruiker, met inbegrip van een verbinding aan het Portaal van Media en een tijdelijk wachtwoord.

### Het CSV-bestand maken {#creating-the-csv-file}

Maak een CSV-bestand (filename.csv) dat voldoet aan de volgende indeling en velden. De eerste rij van het bestand moet de kolomkoppen bevatten die in deze tabel staan. U kunt deze kolommen naar wens ordenen. Alle kolommen zijn vereist.

| Kolomnaam | Beschrijving |
|--- |--- |
| Voornaam | De voornaam. |
| Achternaam | De achternaam. |
| E-mail | Een geldig e-mailadres. |
| Wachtwoord | Een hoofdlettergevoelige wachtwoordtekenreeks. |
| Gebruikersrol | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| Groepen | Lijst met een of meer toewijzingen voor accountgroepen voor elke gebruiker, gescheiden door komma&#39;s. U geeft de groep op door de accountnaam vooraf in te stellen, gescheiden door een slash (/). Zo is PortalCo/IT, waar PortalCo de account is en IT de groep binnen de PortalCo-account. |

In het volgende voorbeeldwerkblad ziet u hoe u een CSV-bestand indeelt:

| Voornaam | Achternaam | E-mail | Wachtwoord | Gebruikersrol | Groepen |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | welkom | MediaPortalAdmin | PortalCo/IT,PortalCo/Admin |
| Kevin | Markeringen | `kevinm@myco.com` | welkom | MediaPortalUser | PortalCo/MktgGroup, PortalCo/test |


### Het CSV-bestand uploaden {#uploading-the-csv-file}

1. Open het scherm van de Opstelling van het Beleid van de Gebruiker.
1. Klik op Gebruikerslijst **** uploaden.
1. Selecteer in het dialoogvenster Bestand selecteren om te uploaden het CSV-bestand en klik op **Openen**.

Elke gebruiker in de lijst wordt automatisch toegevoegd aan de opgegeven groepen. Er wordt een welkomstbericht per e-mail naar beide verzonden.

>[!NOTE]
Als het CSV-bestand niet correct is opgemaakt, wordt het volgende foutbericht weergegeven: &quot;Er is een fout opgetreden tijdens het verwerken van het geüploade CSV-bestand. Controleer de inhoud van het bestand op geldige gegevens.&quot; Bovendien als CSV bestaande IP of IPS gebruiker bevat, wordt de gebruiker niet toegevoegd aan de Lijst van de Gebruiker.

## Het produceren van een selecteerbare lijst van gebruikers van het Portaal van Media {#generating-a-selectable-list-of-media-portal-users}

U kunt de namen en e-mailadressen van gebruikers van het Portaal van Media in een pop-up venster tonen. Deze lijst is nuttig als u gebruikersnamen en adressen voor gebruik buiten het Portaal van Media wilt knippen en kleven.

1. Klik **Opstelling** > **Opstelling** van de Toepassing > **Opstelling** van het Beleid > **Gebruikersbeleid**.
1. Kies in de vervolgkeuzelijst **Op gebruikersrol** de naam van een gebruikersrol van een mediaportaal en klik op **Vernieuwen** om de namen van één klasse van een gebruiker van het mediaportaal weer te geven.
1. Klik op **Pop-uplijst** om het pop-upvenster te openen. U kunt deze lijst kopiëren en plakken.

## Het welkome e-mailbericht voor gebruikers van Media Portal instellen {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

U kunt een welkome e-mail verzenden wanneer u nieuwe gebruikers van het Portaal van Media, medewerkers, en medewerker-gebruikers toevoegt. U kunt dit e-mailbericht vormen of Dynamic Media Klassiek vertellen om het niet te verzenden.

1. Kies **Setup** > **Application Setup** > **Administration Setup** > **User Administration**.
1. Klik in het scherm Gebruikersbeheerinstellingen op **E-mailinstellingen**.
1. Geef in het dialoogvenster E-mailinstellingen een of meer van de volgende instellingen op:

   **Schakel deze optie uit als u nieuwe gebruikers niet per e-mail wilt laten weten dat u hen hebt aangemeld.**

   **Het standaardwachtwoord** gaat een tijdelijk wachtwoord voor nieuwe gebruikers in, of laat het gebied leeg om Dynamic Media te hebben Klassiek willekeurige wachtwoorden produceren. Gebruikers wordt gevraagd wachtwoorden te wijzigen wanneer zij zich voor het eerst aanmelden.

   **Vervangings-URL** Voer een andere URL in dan de standaard als uw gebruikers Dynamic Media Klassiek benaderen via een andere URL.

## Andere taken voor gebruikersbeheer {#other-user-management-tasks}

Beginnend op het scherm van de Opstelling van het Beleid van de Gebruiker, kunt u deze taken ook doen:

**Filter en sorteer de gebruikerslijst** Filter de lijst met gebruikers van Media Portal om gebruikers te zoeken. Zie Filter en sorteer de gebruikerslijst.

**Gebruikers** verwijderen Een gebruiker uit de lijst verwijderen. Zie Een gebruiker verwijderen.

**Activeer en deactiveer gebruikers** Suspend een gebruiker van de toegang tot omslagen. Zie Gebruikers activeren en deactiveren.

**Gebruikersgegevens** bewerken Voer actuele informatie over een gebruiker in. Zie Gebruikersgegevens bewerken.

**Maak door de gebruiker gedefinieerde velden** Maak aangepaste, door de gebruiker gedefinieerde metagegevensvelden voor het ordenen van elementen in de Dynamic Media Klassiek. De velden kunnen desgewenst ook worden geactiveerd of gedeactiveerd.

Zie Door [de gebruiker gedefinieerde velden](application-setup.md#user_defined_fields).
