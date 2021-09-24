---
title: Aanmelden bij Adobe Analytics
description: Leer hoe u zich bij Adobe Analytics aanmeldt vanuit Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d18dbbf89a1bfe4df46cbe7d56cdf6f442595ddb
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Aanmelden bij Adobe Analytics{#log-in-to-adobe-analytics}

Alvorens u login om de rapporten van Adobe Analytics te vormen en de rapportvariabelen van Adobe Analytics aan Adobe Dynamic Media Klassieke gebeurtenissen aan te passen, verifieer dat u een lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics bent. De leden in deze groep kunnen tot alle rapporten in de gespecificeerde rapportreeksen door middel van de Diensten API van het Web van Experience Cloud toegang hebben ongeacht de toestemmingen die in de interface worden geplaatst. Als u een lid wilt toevoegen aan de groep, gaat u in Adobe Analytics naar **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Wanneer u zich aanmeldt, kunt u de Experience Cloud Org-id invoeren om de meest recente videoanalytische implementatie te gebruiken. Als u ervoor kiest om uw id niet in te voeren, werkt het rapporteren van video nog steeds. De gegevens worden echter mogelijk niet correct geïntegreerd met andere gegevens voor die client van buiten Adobe Dynamic Media Classic.

>[!NOTE]
>
>Als uw Adobe Analytics-account voor aanmelding is gemigreerd naar op Adobe IMS gebaseerde verificatie (Identity Management System), werkt het invoeren van directe referenties niet.

**U kunt zich vanuit Adobe Dynamic Media Classic aanmelden bij Adobe Analytics:**

Begin met het integreren van Dynamic Media Classic met Adobe Analytics OAuth. De Adobe Analytics OAuth-integratie met Dynamic Media Classic wordt meestal slechts één keer per gebruiker uitgevoerd.

1. Toegang [Adobe Developer Console](https://developer.adobe.com/console). Zorg ervoor dat uw account beheerdersmachtigingen heeft voor de organisatie waarvoor de integratie is vereist.
1. Selecteer in de rechterbovenhoek van de startpagina het juiste bedrijf in de vervolgkeuzelijst. (Het onderstaande screenshot is uitsluitend ter informatie; de werkelijke bedrijfsnaam die u selecteert, kan variëren.)

   ![Een nieuw project maken](assets/analytics-oauth1.png)

1. Voer een van de volgende handelingen uit:

   * Selecteer **[!UICONTROL Create new project]** op het tabblad **[!UICONTROL Home]** boven aan de pagina.
   * Bij de bovenkant van de pagina, van **[!UICONTROL Projects]** tabel. Selecteer **[!UICONTROL Create new project]** in de rechterhoek van de pagina.

1. Selecteer **[!UICONTROL Add API]** op de pagina van het project.
1. Selecteer **[!UICONTROL Adobe Analytics]** op de pagina **[!UICONTROL Add an API]**.
1. Selecteer **[!UICONTROL Next]** in de rechterbenedenhoek van de pagina.

   ![Een API toevoegen](assets/analytics-oauth2.png)

1. Selecteer **[!UICONTROL USER AUTHENTICATION OAuth]** op de pagina **[!UICONTROL Configure API]**.
1. Selecteer **[!UICONTROL Next]** in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL OAUTH 2.0 Web]** op de pagina **[!UICONTROL Configure API]**.
1. Voer in het tekstveld **[!UICONTROL Default redirect URI]** het volgende pad precies in zoals wordt weergegeven:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Voer in het tekstveld **[!UICONTROL Redirect URI pattern]** het volgende pad precies in zoals wordt weergegeven:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Selecteer **[!UICONTROL Save configured API]** in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL OAuth Web]** onder **[!UICONTROL Credentials]** in het navigatievenster, links op de Adobe Analytics-pagina.
1. Voer onder **[!UICONTROL Credential details]** de volgende handelingen uit:
   * Selecteer **[!UICONTROL Client ID]** onder **[!UICONTROL Copy]** om de waarde te kopiëren. U hebt deze waarde nodig voor de daaropvolgende configuratie Analytics in de Dynamic Media Classic-bureaubladtoepassing die moet worden gevolgd.
   * Selecteer **[!UICONTROL Client Secret]** onder **[!UICONTROL Retrieve client secret]** om de bijbehorende waarde weer te geven. Selecteer **[!UICONTROL Copy]** om de waarde te kopiëren. U hebt deze waarde nodig voor de volgende Adobe Analytics-configuratie in Dynamic Media Classic-bureaubladtoepassing die moet worden uitgevoerd.

**Adobe Analytics configureren in Dynamic Media Classic-bureaubladtoepassing**

>[!NOTE]
>
>Na de eerste configuratie van Adobe Analytics in Dynamic Media Classic kunt u de configuratie alleen in de volgende gevallen opnieuw uitvoeren:
>
>* Een nieuw rapport wordt toegevoegd in Analytics en de gebruiker wil beginnen gegevens naar dat nieuwe rapport te verzenden.
>* De trackingserver wordt bijgewerkt in Adobe Analytics.
>* Een nieuwe het volgen variabele wordt geïntroduceerd in een rapport en u wilt een specifieke variabele van de Kijker in de Klassieke gebruikersinterface van Dynamic Media met die nieuwe variabele Analytics verbinden.

>


1. Ga in de rechterbovenhoek van de Klassieke bureaubladtoepassing van Adobe Dynamic Media naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. Selecteer **[!UICONTROL Adobe Analytics]** onder **[!UICONTROL Application Setup]** in het linkerdeelvenster.
1. Selecteer **[!UICONTROL Adobe Analytics Login]** op de pagina **[!UICONTROL Adobe Analytics Configuration]**.
1. In **[!UICONTROL Adobe Analytics Login]** dialoogdoos, op het gebied van identiteitskaart van de Cliënt en het Geheime gebied van de Cliënt, kleef de respectieve waarden die u vroeger kopieerde.
1. Meld u aan bij IMS.

   Wanneer u met succes het programma wordt geopend, wordt de **[!UICONTROL COMPANIES]** drop-down lijst, die door de bedrijven in werking wordt gesteld die aan u beschikbaar zijn, zichtbaar.

1. Kies een bedrijf in de vervolgkeuzelijst **[!UICONTROL COMPANIES]**.

   Nadat u een bedrijf selecteert, wordt de **[!UICONTROL SUITES]** drop-down lijst, die door de Reeksen van het Rapport in werking wordt gesteld die voor het geselecteerde bedrijf beschikbaar zijn, zichtbaar.

1. Kies een rapportsuite in de vervolgkeuzelijst **[!UICONTROL SUITES]**.

   >[!NOTE]
   >
   >Door gebrek, moet de gebruiker zich bewust zijn van het feit dat zowel **[!UICONTROL COMPANIES]** als **[!UICONTROL SUITES]** drop-down lijsten leeg zijn. De gebruiker moet daarom in elke lijst een waarde selecteren. —>

1. Selecteer **[!UICONTROL OK]** zodat kunt u configuratie bewaren.

>[!MORELIKETHIS]
>
>* [Adobe Analytics-rapporten configureren](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

