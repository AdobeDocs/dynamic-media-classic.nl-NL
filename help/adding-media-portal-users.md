---
title: Gebruikers van Media Portal toevoegen en beheren
description: Leer hoe u gebruikers van Media Portal in Adobe Dynamic Media Classic kunt toevoegen en beheren.
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

# Gebruikers van Media Portal toevoegen en beheren{#adding-and-managing-media-portal-users}

Als beheerder kunt u gebruikers toevoegen en beheren, beslissen of ze wachtwoorden kunnen wijzigen, gebruikersgegevens kunnen bewerken en gebruikerslijsten kunnen uploaden. Deze taken worden verwezenlijkt op het scherm van het Beleid van de Gebruiker. Navigeer naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.

>[!NOTE]
>
>Voordat u gebruikers toevoegt, moet u groepen instellen voor het beheer ervan. Met Mediaportal kunt u geen gebruiker toevoegen zonder de gebruiker aan een of meer groepen toe te wijzen. Zie voor meer informatie [Mediaportaalgroepen maken en beheren](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Beheer van wachtwoorden voor mediaportaal {#handling-media-portal-passwords}

De gebruikers van het Portaal van media, de medewerkers, en de medewerker-gebruikers worden verzonden een welkome e-mailbericht met een wachtwoord wanneer u hen omhoog ondertekent. Beheerders kunnen bepalen of gebruikers van Media Portal dit wachtwoord kunnen wijzigen.

1. Navigeren naar **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL General Settings]**.
1. Schakel op de pagina Algemene instellingen de optie **[!UICONTROL Allow Media Portal user to change Password]**.
1. Selecteren **[!UICONTROL Save]**.

>[!NOTE]
>
>Gebruikers van Media Portal die wachtwoorden mogen wijzigen, kunnen dit doen door **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** en veranderende wachtwoorden op het Persoonlijke scherm van de Opstelling.

## Gebruikers van een mediaportaal toevoegen {#adding-a-media-portal-user}

1. Navigeren naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecteer op de pagina Gebruikersbeheer de optie **Toevoegen**.
1. Voer in het dialoogvenster Gebruiker toevoegen in het deelvenster Gebruikersinfo de voornaam, achternaam en e-mailadres van de gebruiker in en selecteer vervolgens **[!UICONTROL Next]**.
1. Selecteer in het deelvenster Bedrijf/Rol in de vervolgkeuzelijst Bedrijven een bedrijf of bedrijven voor de gebruiker.
1. Selecteer in de lijst Rol een rol voor Media Portal en selecteer vervolgens **[!UICONTROL Next]**.

   Zie [Gebruikersrollen van Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. Selecteer een of meer groepen in het deelvenster Toegangsgroepen.

   Zie [Mediaportaalgroepen maken en beheren](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Optioneel) Selecteer **[!UICONTROL Email Settings]** om andere e-mailinstellingen te kiezen dan de standaardinstellingen.

   Zie [Het welkomstbericht voor gebruikers van het Media Portal instellen](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Selecteren **[!UICONTROL Add User]**.

Nadat u een gebruiker hebt toegevoegd, verzendt het Portaal van Media de gebruiker een Welkome e-mailbericht. Het bericht bevat een tijdelijk wachtwoord en de URL van het Media Portal.

## Een gebruikerslijst voor een Media Portal uploaden {#uploading-a-media-portal-user-list}

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
| Prairie | Kat | `prairiek@company.com` | welkom | MediaPortalAdmin | PortalCo/IT, PortalCo/Admin |
| Rick | Bout | `rickb@myco.com` | welkom | MediaPortalUser | PortalCo/MktgGroup, PortalCo/test |

### Het CSV-bestand uploaden {#uploading-the-csv-file}

1. Open het scherm van de Opstelling van het Beleid van de Gebruiker.
1. Selecteren **[!UICONTROL Upload User List]**.
1. Selecteer in het dialoogvenster Bestand selecteren om te uploaden het CSV-bestand en selecteer vervolgens **[!UICONTROL Open]**.

Elke gebruiker in de lijst wordt automatisch toegevoegd aan de opgegeven groepen. Er wordt een welkomstbericht per e-mail naar beide verzonden.

>[!NOTE]
>
>Als het CSV-bestand niet correct is opgemaakt, wordt het volgende foutbericht weergegeven: &quot;Er is een fout opgetreden tijdens het verwerken van het geüploade CSV-bestand. Controleer de inhoud van het bestand op geldige gegevens.&quot; Bovendien als CSV bestaande IP of IPS gebruiker bevat, wordt de gebruiker niet toegevoegd aan de Lijst van de Gebruiker.

## Genereer een selecteerbare lijst van gebruikers van het Portaal van Media {#generating-a-selectable-list-of-media-portal-users}

U kunt de namen en e-mailadressen van gebruikers van het Portaal van Media in een pop-up venster tonen. Deze lijst is nuttig als u gebruikersnamen en adressen voor gebruik buiten het Portaal van Media wilt knippen en kleven.

1. Navigeren naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. In de **[!UICONTROL By User Role]** drop-down lijst, kies de naam van een Poortgebruikersrol van Media, en selecteer **[!UICONTROL Refresh]** om de namen van één klasse van de gebruiker van het Portaal van Media te tonen.
1. Selecteren **[!UICONTROL Popup List]**. Kopieer en plak deze lijst.

## Het welkomstbericht voor gebruikers van het Media Portal instellen {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

U kunt een welkome e-mail verzenden wanneer u nieuwe gebruikers van het Portaal van Media, medewerkers, en medewerker-gebruikers toevoegt. U kunt dit e-mailbericht configureren of Adobe Dynamic Media Classic vertellen het niet te verzenden.

1. Navigeren naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. In het scherm van de Opstelling van het Beleid van de Gebruiker, selecteer **[!UICONTROL Email Settings]**.
1. Geef in het dialoogvenster E-mailinstellingen een of meer van de volgende instellingen op:

   * **[!UICONTROL Send Email]** - Schakel deze optie uit als u nieuwe gebruikers niet via e-mail wilt laten weten dat u hen hebt aangemeld.

   * **[!UICONTROL Default Password]** - Voer een tijdelijk wachtwoord in voor nieuwe gebruikers of laat het veld leeg om Adobe Dynamic Media Classic willekeurige wachtwoorden te laten genereren. Gebruikers wordt gevraagd wachtwoorden te wijzigen wanneer zij zich voor het eerst aanmelden.

   * **[!UICONTROL Replacement URL]** - Voer een andere URL in dan de standaardURL als uw gebruikers Adobe Dynamic Media Classic openen via een andere URL.

## Andere taken voor gebruikersbeheer {#other-user-management-tasks}

Beginnend op het scherm van de Opstelling van het Beleid van de Gebruiker, kunt u deze taken ook doen:

* **[!UICONTROL Filter and sort the user list]** - Filter de lijst met gebruikers van Media Portal om gebruikers te zoeken.

* **[!UICONTROL Delete users]** - Verwijder een gebruiker uit de lijst.

* **[!UICONTROL Activate and deactivate users]** - Een gebruiker de toegang tot mappen opschorten.

* **[!UICONTROL Edit user information]** - Voer actuele informatie in over een gebruiker.

* **[!UICONTROL Create user-defined fields]** - Maak aangepaste, door de gebruiker gedefinieerde metagegevensvelden zodat u elementen in de Adobe Dynamic Media Classic kunt ordenen. De velden kunnen desgewenst ook worden geactiveerd of gedeactiveerd.

Zie [Door gebruiker gedefinieerde velden](application-setup.md#user_defined_fields).
