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
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Aanmelden bij Adobe Analytics{#log-in-to-adobe-analytics}

Alvorens u login om de rapporten van Adobe Analytics te vormen en de rapportvariabelen van Adobe Analytics aan Adobe Dynamic Media Klassieke gebeurtenissen aan te passen, verifieer dat u een lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics bent. De leden in deze groep kunnen tot alle rapporten in de gespecificeerde rapportreeksen door middel van de Diensten API van het Web van Experience Cloud toegang hebben ongeacht de toestemmingen die in de interface worden geplaatst. Als u een lid wilt toevoegen aan de groep, gaat u in Adobe Analytics naar **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Wanneer u zich aanmeldt, kunt u de Experience Cloud Org-id invoeren om de meest recente videoanalytische implementatie te gebruiken. Als u ervoor kiest om uw id niet in te voeren, werkt het rapporteren van video nog steeds. De gegevens worden echter mogelijk niet correct geïntegreerd met andere gegevens voor die client van buiten Adobe Dynamic Media Classic.

>[!NOTE]
>
>Als uw Adobe Analytics-account voor aanmelding is gemigreerd naar op Adobe IMS gebaseerde verificatie (Identity Management System), werkt het invoeren van directe referenties niet.

**Aanmelden bij Adobe Analytics:**

1. Ga in de rechterbovenhoek van de Klassieke pagina van Adobe Dynamic Media naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. Tik in het linkervenster onder **[!UICONTROL Application Setup]** op **[!UICONTROL Adobe Analytics]**.
1. Tik op **[!UICONTROL Adobe Analytics Login]** op de Adobe Analytics-configuratiepagina.
1. Voer in het dialoogvenster **[!UICONTROL Adobe Analytics Login]** de bedrijfsnaam, de Experience Cloud Org-id (optioneel), de gebruikersnaam en de *gedeelde geheime sleutel* in het tekstveld **[!UICONTROL Password]** in.

   U kunt de *gedeelde geheime* sleutel van de Admin Console van Analytics terugwinnen. Zie [API-referenties ophalen voor gebruikersaccounts](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Selecteer **[!UICONTROL Login]**.
1. Kies in het vervolgkeuzemenu **[!UICONTROL Report Suite]** een rapportsuite en selecteer **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >De eerste keer dat u zich aanmeldt bij Adobe Analytics, is de vervolgkeuzelijst Report Suite leeg. De eerste keer dat u zich aanmeldt, kiest u geen rapportsuite. Nadat u zich voor het eerst hebt aangemeld, meldt u zich af en keert u terug naar het scherm Adobe Analytics. Meld u opnieuw aan om een rapportsuite te kunnen kiezen.

>[!MORELIKETHIS]
>
>* [Adobe Analytics-rapporten configureren](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

