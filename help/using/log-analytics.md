---
title: Aanmelden bij Adobe Analytics
description: Leer hoe u zich vanuit Adobe Dynamic Media Classic aanmeldt bij Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%

---

# Aanmelden bij Adobe Analytics{#log-in-to-adobe-analytics}

Verifieer dat u een lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics bent. Doe dit voordat u zich aanmeldt om Adobe Analytics-rapporten te configureren en Adobe Analytics-rapportvariabelen aan te passen aan Adobe Dynamic Media Classic-gebeurtenissen. Leden in deze groep hebben toegang tot alle rapporten in de opgegeven rapportsets. Doe dit gebruikend de Experience Cloud API van de Diensten van het Web, ongeacht de toestemmingen die in de interface worden geplaatst. Ga in Adobe Analytics naar **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]** om een lid aan de groep toe te voegen.

Wanneer u zich aanmeldt, kunt u de Experience Cloud Org-id invoeren om de meest recente implementatie van de videoanalyse te gebruiken. Als u ervoor kiest om uw id niet in te voeren, werkt het rapporteren van video nog steeds. De gegevens worden echter mogelijk niet correct geïntegreerd met andere gegevens voor die client van buiten Adobe Dynamic Media Classic.

>[!NOTE]
>
>Als uw Adobe Analytics-account voor aanmelding is gemigreerd naar op Adobe IMS gebaseerde verificatie (Identity Management System), werkt het invoeren van directe referenties niet.

## Aanmelden bij Adobe Analytics vanuit Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Begin met het integreren van Dynamic Media Classic met Adobe Analytics OAuth. De Adobe Analytics OAuth-integratie met Dynamic Media Classic wordt doorgaans slechts eenmaal per gebruiker uitgevoerd.

1. Toegang [ Adobe Developer Console ](https://developer.adobe.com/console). Zorg ervoor dat uw account beheerdersmachtigingen heeft voor de organisatie waarvoor de integratie is vereist.
1. Selecteer in de rechterbovenhoek van de startpagina het juiste bedrijf in de vervolgkeuzelijst. (Het onderstaande screenshot is alleen ter informatie. De werkelijke bedrijfsnaam die u selecteert, kan variëren.)

   ![ creeer een nieuw project ](assets/analytics-oauth1.png)

1. Voer een van de volgende handelingen uit:

   * Selecteer boven aan de pagina op het tabblad **[!UICONTROL Home]** de optie **[!UICONTROL Create a new project]** .
   * Boven aan de pagina bevindt zich de tab **[!UICONTROL Projects]** . Selecteer **[!UICONTROL Create a new project]** in de rechterhoek van de pagina.

1. Selecteer **[!UICONTROL Add API]** op de pagina van het project.
1. Selecteer op de pagina **[!UICONTROL Add an API]** de optie **[!UICONTROL Adobe Analytics]** .
1. Selecteer **[!UICONTROL Next]** in de rechterbenedenhoek van de pagina.

   ![ voeg API ](assets/analytics-oauth2.png) toe

1. Selecteer op de pagina **[!UICONTROL `Configure API`]** de optie **[!UICONTROL USER AUTHENTICATION OAuth]** .
1. Selecteer **[!UICONTROL Next]** in de rechterbenedenhoek van de pagina.
1. Selecteer op de pagina **[!UICONTROL `Configure API`]** de optie **[!UICONTROL OAUTH 2.0 Web]** .
1. Voer in het tekstveld **[!UICONTROL Default redirect URI]** het volgende pad in zoals wordt weergegeven:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Voer in het tekstveld **[!UICONTROL Redirect URI pattern]** het volgende pad in zoals wordt weergegeven:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Selecteer **[!UICONTROL Save configured API]** rechtsonder op de pagina.
1. Selecteer in het navigatievenster links van de Adobe Analytics-pagina onder **[!UICONTROL Credentials]** de optie **[!UICONTROL OAuth Web]** .
1. Voer onder **[!UICONTROL Credential details]** de volgende handelingen uit:
   * Selecteer onder **[!UICONTROL Client ID]** de optie **[!UICONTROL Copy]** om de waarde te kopiëren. U hebt deze waarde nodig voor de daaropvolgende configuratie Analytics in de Dynamic Media Classic-bureaubladtoepassing die moet worden uitgevoerd.
   * Selecteer onder **[!UICONTROL Client Secret]** de optie **[!UICONTROL Retrieve client secret]** om de bijbehorende waarde weer te geven. Selecteer **[!UICONTROL Copy]** om de waarde te kopiëren. U hebt deze waarde nodig voor de volgende Adobe Analytics-configuratie in de Dynamic Media Classic-bureaubladtoepassing die moet worden uitgevoerd.

## Adobe Analytics configureren in Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Na uw eerste configuratie van Adobe Analytics in Dynamic Media Classic kunt u de configuratie alleen in de volgende gevallen opnieuw uitvoeren:
>
>* Een nieuw rapport wordt toegevoegd in Analytics en de gebruiker wil beginnen gegevens naar dat nieuwe rapport te verzenden.
>* De trackingserver wordt bijgewerkt in Adobe Analytics.
>* Een nieuwe volgvariabele wordt geïntroduceerd in een rapport en u wilt een specifieke variabele van de Kijker in het gebruikersinterface van Dynamic Media Classic met die nieuwe variabele van de Analytics verbinden.
>

1. Ga in de rechterbovenhoek van de Adobe Dynamic Media Classic-bureaubladtoepassing naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** .
1. Selecteer in het linkerdeelvenster onder **[!UICONTROL Application Setup]** de optie **[!UICONTROL Adobe Analytics]** .
1. Selecteer op de pagina **[!UICONTROL Adobe Analytics Configuration]** de optie **[!UICONTROL Adobe Analytics Login]** .
1. Plak in het dialoogvenster **[!UICONTROL Adobe Analytics Login]** in het veld **[!UICONTROL CLIENT ID]** en **[!UICONTROL CLIENT SECRET]** de respectievelijke waarden die u eerder hebt gekopieerd.
1. Selecteer in de rechterbenedenhoek van het dialoogvenster **[!UICONTROL Login]** de Adobe IMS-aanmelding (Identity Management Services) en voer deze uit.

   Wanneer u zich met succes hebt aangemeld, wordt het dialoogvenster Adobe Analytics-aanmelding weer weergegeven, samen met de vervolgkeuzelijst **[!UICONTROL COMPANIES]** , die wordt gestart door de bedrijven die u ter beschikking staan.

1. Kies een bedrijf in de vervolgkeuzelijst **[!UICONTROL COMPANIES]** .

   Nadat u een bedrijf hebt geselecteerd, wordt de vervolgkeuzelijst **[!UICONTROL SUITES]** die wordt gestart door de rapportsets die beschikbaar zijn voor het geselecteerde bedrijf, weergegeven.

1. Kies een rapportsuite in de vervolgkeuzelijst **[!UICONTROL SUITES]** .

   >[!NOTE]
   >
   >Standaard moet de gebruiker weten dat zowel de vervolgkeuzelijsten **[!UICONTROL COMPANIES]** als **[!UICONTROL SUITES]** leeg zijn. De gebruiker moet daarom in elke lijst een waarde selecteren.

1. Selecteer **[!UICONTROL OK]** zodat u de configuratie kunt opslaan.

   >[!NOTE]
   >
   >Het veld **[!UICONTROL Adobe Analytics Server]** wordt gevuld met een voorgestelde externe traceringsserver die overeenkomt met de naamruimte voor analysemogelijkheden wanneer u **[!UICONTROL OK]** selecteert. Als u een andere trackingserver gebruikt, werkt u deze in dit veld bij om gegevensverlies te voorkomen.

1. Selecteer **[!UICONTROL Save]** in de linkerbenedenhoek van de Adobe Analytics-configuratiepagina om ervoor te zorgen dat de configuratie van uw Adobe Analytics-account wordt bijgewerkt.

>[!MORELIKETHIS]
>
>* [ vorm de rapporten van Adobe Analytics ](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
