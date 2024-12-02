---
title: 'Snel starten: Adobe Dynamic Media Classic en Adobe Analytics integreren'
description: Een introductie en Snel aan de slag om Adobe Dynamic Media Classic en Adobe Analytics te integreren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Snel starten: Adobe Dynamic Media Classic en Adobe Analytics integreren {#quick-start-integrating-dmc-analytics}

Adobe Analytics is het toonaangevende product dat marketers één plek biedt waar ze geïntegreerde gegevens van alle online initiatieven via meerdere marketingkanalen kunnen meten, analyseren en optimaliseren.

Nadat u Adobe Analytics hebt geïntegreerd met Adobe Dynamic Media Classic, kunt u meldingen krijgen over het gedrag van websitebezoekers die Adobe Dynamic Media Classic-viewers gebruiken op uw website. Wanneer een websitebezoeker bijvoorbeeld een zoomdoel selecteert in een Adobe Dynamic Media Classic Zoom Viewer, neemt Adobe Analytics deze handeling op. Adobe Analytics-rapporten kunnen cumulatieve informatie verzamelen over gebruikersactiviteiten in Adobe Dynamic Media Classic-viewers.

Met Adobe Analytics-rapporten krijgt u een duidelijk beeld van de activiteiten van klanten op uw website. U kunt bepalen welke productpresentaties tot conversie leiden en welke niet de interesse van de klant wekken.

Zie ook [ Video van de Maatregel in Adobe Analytics ](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Er is een geldig Adobe Analytics-account vereist om Analytics te integreren met Adobe Dynamic Media Classic en analyserapporten te genereren.

Deze snelle start is ontworpen om u snel aan de slag te krijgen met de Adobe Analytics Instrumentation Kit.

## 1. Meld u via Adobe Dynamic Media Classic aan bij Adobe Analytics en download de Adobe Analytics-rapportvariabelen

>[!NOTE]
>
>Verifieer dat u als lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics wordt toegevoegd. Voer deze verificatie uit voordat u Adobe Analytics-rapporten configureert. En voordat je Adobe Analytics-rapportvariabelen koppelt aan Adobe Dynamic Media Classic-gebeurtenissen. Leden in deze groep hebben toegang tot alle rapporten in de opgegeven rapportaereeksen. U kunt dit doen gebruikend de API van de Diensten van het Web van het Experience Cloud ongeacht de toestemmingen die in de interface worden geplaatst. Ga in Adobe Analytics naar **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]** om een lid aan de groep toe te voegen.

Nadat u hebt gecontroleerd dat u lid bent van de groep Webservice Access, gaat u in Adobe Dynamic Media Classic naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]** . Selecteer **[!UICONTROL Adobe Analytics Login]** op de Adobe Analytics Configuration-pagina.

Zie [ Logon aan Adobe Analytics ](log-analytics.md#log_in_to_adobe_analytics).

Typ in het dialoogvenster Adobe Analytics-aanmelding uw Experience Cloud-Org-id (optioneel) en uw volledige referenties en selecteer vervolgens **[!UICONTROL Login]** . Selecteer in het keuzemenu Rapportsuite de naam van de rapportsuite die u wilt gebruiken.

## 2. Adobe Analytics-rapportvariabelen toewijzen aan Adobe Dynamic Media Classic-viewergebeurtenissen en Adobe Dynamic Media Classic-variabelen

Geef op de Adobe Analytics Configuration-pagina de gewenste informatie op in Adobe Analytics-rapporten. Voor elke Adobe Dynamic Media Classic-viewergebeurtenis waarover u informatie wilt, kiest u een Adobe Analytics-variabele (uit uw rapportsuite) en een Adobe Dynamic Media Classic-variabele.

* Viewergebeurtenissen beschrijven de gebruikersactiviteit die u wilt meten in rapporten.
* Adobe Dynamic Media Classic-variabelen beschrijven de gegevens over gebruikersgebeurtenissen die de rapporten moeten leveren.

De configuratie van Adobe Analytics biedt ook hulpmiddelen voor het activeren, het uitgeven, en het schrappen van kijkergebeurtenissen.

Nadat u **[!UICONTROL Save]** op de Adobe Analytics-configuratiepagina hebt geselecteerd, wordt een aangepaste trackingcode voor het meten van gebruikersactiviteit ingevoegd in Adobe Dynamic Media Classic-viewers. Met deze functionaliteit kunt u gebruikersactiviteiten bijhouden in Adobe Analytics-rapporten.

Zie [ de rapporten van Adobe Analytics ](configuring-analytics-reports.md#configuring_adobe_analytics_reports) vormen.

## 3. Publish uw Adobe Dynamic Media Classic-viewers

Publish uw Adobe Dynamic Media Classic-viewers zodat de viewers (met code voor het bijhouden van gebruikersactiviteiten in Adobe Analytics-rapporten) worden geladen op Adobe Dynamic Media Classic-servers. Nadat u deze gegevens hebt gepubliceerd, worden deze opgenomen in viewers. Gebruik het voor analyse door Adobe Analytics.

Zie [ de configuratieinformatie van Publish ](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Plaats Adobe Dynamic Media Classic-viewers op uw website

Plaats de Adobe Dynamic Media Classic-viewers met de trackingcode voor Adobe Analytics op uw website.

## 5. Test de Adobe Analytics-integratie door een Adobe Analytics-rapport te bekijken

Ga naar de Adobe Analytics-website om Adobe Analytics-rapporten te bekijken. Op de pagina Rapportage kunt u gegevens weergeven en grafieken en grafieken genereren om gebruikersactiviteit met verschillende viewers te meten.

Zie [ de integratie van Adobe Analytics testen door een rapport van Adobe Analytics ](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report) te bekijken.
