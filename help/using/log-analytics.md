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

Verifieer dat u een lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics bent. Doe dit voordat u zich aanmeldt om Adobe Analytics-rapporten te configureren en Adobe Analytics-rapportvariabelen aan te passen aan Adobe Dynamic Media Classic-gebeurtenissen. Leden in deze groep hebben toegang tot alle rapporten in de opgegeven rapportsets. Doe dit gebruikend de Diensten API van het Web van het Experience Cloud, ongeacht de toestemmingen die in de interface worden geplaatst. Ga in Adobe Analytics naar **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Wanneer u zich aanmeldt, kunt u de Experience Cloud-Org-id invoeren om de meest recente videoanalytische implementatie te gebruiken. Als u ervoor kiest om uw id niet in te voeren, werkt het rapporteren van video nog steeds. De gegevens worden echter mogelijk niet correct geïntegreerd met andere gegevens voor die client van buiten Adobe Dynamic Media Classic.

>[!NOTE]
>
>Als uw Adobe Analytics-account voor aanmelding is gemigreerd naar op Adobe IMS gebaseerde verificatie (Identity Management System), werkt het invoeren van directe referenties niet.

## Aanmelden bij Adobe Analytics vanuit Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Begin met het integreren van Dynamic Media Classic met Adobe Analytics OAuth. De Adobe Analytics OAuth-integratie met Dynamic Media Classic wordt doorgaans slechts eenmaal per gebruiker uitgevoerd.

1. Toegang [Adobe Developer Console](https://developer.adobe.com/console). Zorg ervoor dat uw account beheerdersmachtigingen heeft voor de organisatie waarvoor de integratie is vereist.
1. Selecteer in de rechterbovenhoek van de startpagina het juiste bedrijf in de vervolgkeuzelijst. (Het onderstaande screenshot is alleen ter informatie. De werkelijke bedrijfsnaam die u selecteert, kan variëren.)

   ![Een nieuw project maken](assets/analytics-oauth1.png)

1. Voer een van de volgende handelingen uit:

   * Boven aan de pagina, vanaf de **[!UICONTROL Home]** tab, selecteert u **[!UICONTROL Create a new project]**.
   * Boven aan de pagina, vanaf de **[!UICONTROL Projects]** tab. Selecteer in de rechterhoek van de pagina de optie **[!UICONTROL Create a new project]**.

1. Selecteer op de projectpagina de optie **[!UICONTROL Add API]**.
1. Op de **[!UICONTROL Add an API]** pagina, selecteert u **[!UICONTROL Adobe Analytics]**.
1. Selecteer in de rechterbenedenhoek van de pagina de optie **[!UICONTROL Next]**.

   ![Een API toevoegen](assets/analytics-oauth2.png)

1. Op de **[!UICONTROL `Configure API`]** pagina, selecteert u **[!UICONTROL USER AUTHENTICATION OAuth]**.
1. Selecteer in de rechterbenedenhoek van de pagina de optie **[!UICONTROL Next]**.
1. Op de **[!UICONTROL `Configure API`]** pagina, selecteert u **[!UICONTROL OAUTH 2.0 Web]**.
1. In de **[!UICONTROL Default redirect URI]** Typ het volgende pad precies zoals wordt weergegeven in het tekstveld:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. In de **[!UICONTROL Redirect URI pattern]** Typ het volgende pad precies zoals wordt weergegeven in het tekstveld:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Selecteer in de rechterbenedenhoek van de pagina de optie **[!UICONTROL Save configured API]**.
1. In het navigatievenster, links op de Adobe Analytics-pagina, onder **[!UICONTROL Credentials]**, selecteert u **[!UICONTROL OAuth Web]**.
1. Onder **[!UICONTROL Credential details]** Ga als volgt te werk:
   * Onder **[!UICONTROL Client ID]**, selecteert u **[!UICONTROL Copy]** de waarde kopiëren. U hebt deze waarde nodig voor de daaropvolgende configuratie Analytics in de Dynamic Media Classic-bureaubladtoepassing die moet worden uitgevoerd.
   * Onder **[!UICONTROL Client Secret]**, selecteert u **[!UICONTROL Retrieve client secret]** om de bijbehorende waarde weer te geven. Selecteren **[!UICONTROL Copy]** de waarde kopiëren. U hebt deze waarde nodig voor de volgende Adobe Analytics-configuratie in de Dynamic Media Classic-bureaubladtoepassing die moet worden uitgevoerd.

## Adobe Analytics configureren in Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Na uw eerste configuratie van Adobe Analytics in Dynamic Media Classic kunt u de configuratie alleen in de volgende gevallen opnieuw uitvoeren:
>
>* Een nieuw rapport wordt toegevoegd in Analytics en de gebruiker wil beginnen gegevens naar dat nieuwe rapport te verzenden.
>* De trackingserver wordt bijgewerkt in Adobe Analytics.
>* Een nieuwe volgvariabele wordt geïntroduceerd in een rapport en u wilt een specifieke variabele van de Kijker in het gebruikersinterface van Dynamic Media Classic met die nieuwe variabele van de Analytics verbinden.
>

1. Ga in de rechterbovenhoek van de Adobe Dynamic Media Classic-bureaubladtoepassing naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. In het linkerdeelvenster, onder **[!UICONTROL Application Setup]**, selecteert u **[!UICONTROL Adobe Analytics]**.
1. Op de **[!UICONTROL Adobe Analytics Configuration]** pagina, selecteert u **[!UICONTROL Adobe Analytics Login]**.
1. In de **[!UICONTROL Adobe Analytics Login]** in het dialoogvenster **[!UICONTROL CLIENT ID]** en de **[!UICONTROL CLIENT SECRET]** plakken de waarden die u eerder hebt gekopieerd.
1. Selecteer rechtsonder in het dialoogvenster de optie **[!UICONTROL Login]** en voer uw Adobe IMS-aanmelding (Identity Management Services) uit.

   Wanneer u zich met succes hebt aangemeld, verschijnt het dialoogvenster Adobe Analytics-aanmelding opnieuw samen met het dialoogvenster **[!UICONTROL COMPANIES]** vervolgkeuzelijst, geopend door de bedrijven die u ter beschikking staan.

1. Van de **[!UICONTROL COMPANIES]** kiest u een bedrijf.

   Nadat u een bedrijf hebt geselecteerd, **[!UICONTROL SUITES]** de drop-down lijst, die door de Reeksen van het Rapport in werking wordt gesteld die voor het geselecteerde bedrijf beschikbaar zijn, wordt zichtbaar.

1. Van de **[!UICONTROL SUITES]** kiest u een rapportsuite.

   >[!NOTE]
   >
   >Standaard moet de gebruiker weten dat beide **[!UICONTROL COMPANIES]** en **[!UICONTROL SUITES]** vervolgkeuzelijsten zijn leeg. De gebruiker moet daarom in elke lijst een waarde selecteren.

1. Selecteren **[!UICONTROL OK]** zodat kunt u de configuratie opslaan.

   >[!NOTE]
   >
   >De **[!UICONTROL Adobe Analytics Server]** veld wordt gevuld met een voorgestelde externe traceringsserver die overeenkomt met de naamruimte voor analysemogelijkheden wanneer u **[!UICONTROL OK]**. Als u een andere trackingserver gebruikt, werkt u deze in dit veld bij om gegevensverlies te voorkomen.

1. Selecteer in de linkerbenedenhoek van de Adobe Analytics-configuratiepagina de optie **[!UICONTROL Save]** om ervoor te zorgen dat de configuratie van uw Adobe Analytics-account wordt bijgewerkt.

>[!MORELIKETHIS]
>
>* [Adobe Analytics-rapporten configureren](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
