---
title: Aanmelden bij Adobe Analytics
description: Leer hoe u zich aanmeldt bij Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---


# Aanmelden bij Adobe Analytics{#log-in-to-adobe-analytics}

Alvorens u login om de rapporten van Adobe Analytics te vormen en de rapportvariabelen van Adobe Analytics aan de Klassieke gebeurtenissen van Dynamic Media aan te passen, verifieer dat u als lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics wordt toegevoegd. De leden in deze groep kunnen tot alle rapporten in de gespecificeerde rapportreeksen door middel van de Diensten API van het Web van de Marketing Cloud ongeacht de toestemmingen toegang hebben die in de interface worden geplaatst. Als u een lid wilt toevoegen aan de groep, klikt u in Adobe Analytics op **Admin Tools** > **Gebruikersbeheer** > **Groepen bewerken**.

Als u zich aanmeldt, kunt u de Marketing Cloud-Org-id invoeren om de meest recente implementatie van videoanalyses te gebruiken. Als u ervoor kiest om uw id niet in te voeren, werkt het rapporteren van video nog steeds. De gegevens worden echter mogelijk niet correct geïntegreerd met andere gegevens voor die client van buiten Dynamic Media Classic.

>[!NOTE]
>
>Als uw Adobe Analytics-account voor aanmelding is gemigreerd naar verificatie op basis van Adobe IMS (Identity Management System), werkt het invoeren van directe referenties niet.

**Aanmelden bij Adobe Analytics**

1. Tik in de rechterbovenhoek van de klassieke Dynamic Media-pagina op **[!UICONTROL Setup > Application Setup]**.
1. Tik in het linkervenster onder **[!UICONTROL Application Setup]** op **[!UICONTROL Adobe Analytics]**.
1. Tik op **[!UICONTROL Adobe Analytics Login]** op de Adobe Analytics-configuratiepagina.
1. Voer in het dialoogvenster **[!UICONTROL Adobe Analytics Login]** uw bedrijfsnaam, Marketing Cloud-Org-id (optioneel), gebruikersnaam en de *sleutel voor gedeeld geheim* in het tekstveld **[!UICONTROL Password]** in.

   U kunt de *gedeelde geheime* sleutel van de knoop van Admin van Analytics terugwinnen. Zie [API-referenties ophalen voor gebruikersaccounts](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html).

1. Klik op **[!UICONTROL Login]**.
1. Kies in het vervolgkeuzemenu **[!UICONTROL Report Suite]** een rapportsuite en klik op **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >De eerste keer dat u zich aanmeldt bij Adobe Analytics, is de vervolgkeuzelijst Report Suite leeg. De eerste keer dat u zich aanmeldt, kiest u geen rapportsuite. Nadat u zich voor het eerst hebt aangemeld, meldt u zich af en keert u terug naar het scherm Adobe Analytics. Meld u opnieuw aan om een rapportsuite te kunnen kiezen.

>[!MORELIKETHIS]
>
>* [Adobe Analytics-rapporten configureren](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

