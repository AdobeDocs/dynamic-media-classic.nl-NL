---
title: '"Snel starten: Adobe Dynamic Media Classic en Adobe Analytics integreren"'
description: Een introductie en Snel aan de integratie van Adobe Dynamic Media Classic en Adobe Analytics om u te helpen snel aan de slag te gaan.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Snel starten: Adobe Dynamic Media Classic en Adobe Analytics integreren {#quick-start-integrating-dmc-analytics}

Adobe Analytics is het toonaangevende product dat marketers één plek biedt waar ze geïntegreerde gegevens van alle online initiatieven via meerdere marketingkanalen kunnen meten, analyseren en optimaliseren.

Nadat u Adobe Analytics hebt geïntegreerd met Adobe Dynamic Media Classic, kunt u meldingen krijgen over het gedrag van websitebezoekers die Adobe Dynamic Media Classic-viewers op uw website gebruiken. Wanneer een websitebezoeker bijvoorbeeld op een zoomdoel in een Adobe Dynamic Media Classic Zoom Viewer klikt, neemt Adobe Analytics deze actie op. Adobe Analytics-rapporten kunnen cumulatieve informatie verzamelen over gebruikersactiviteiten in Klassieke Adobe Dynamic Media-viewers.

Met Adobe Analytics-rapporten krijgt u een duidelijk beeld van de activiteiten van klanten op uw website. U kunt bepalen welke productpresentaties tot conversie leiden en welke niet de interesse van de klant wekken.

Zie ook [Video meten in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Een geldig Adobe Analytics-account is vereist voor het integreren van Analytics met Adobe Dynamic Media Classic en het genereren van Analytics-rapporten.

Deze snelle start is ontworpen om u snel aan de slag te krijgen met Adobe Analytics Instrumentation Kit.

## 1. Meld u aan bij Adobe Analytics via Adobe Dynamic Media Classic en download Adobe Analytics-rapportvariabelen

>[!NOTE]
>
>Alvorens u de rapporten van Adobe Analytics kunt vormen en de rapportvariabelen van Adobe Analytics aan Adobe Dynamic Media Klassieke gebeurtenissen aanpassen, verifieer dat u als lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics wordt toegevoegd. De leden in deze groep kunnen tot alle rapporten in de gespecificeerde rapportreeksen door middel van de Diensten API van het Web van de Marketing Cloud ongeacht de toestemmingen toegang hebben die in de interface worden geplaatst. Als u een lid wilt toevoegen aan de groep, klikt u in Adobe Analytics op **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Nadat u hebt geverifieerd dat u lid bent van de groep van de Toegang van de Dienst van het Web, in Adobe Dynamic Media Klassiek, ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]**. Voor de pagina van de Configuratie van Adobe Analytics, klik **[!UICONTROL Adobe Analytics Login]**.

Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Typ in het dialoogvenster Adobe Analytics-aanmelding uw Marketing Cloud-Org-id (optioneel) en uw volledige referenties en klik vervolgens op **[!UICONTROL Login]**. Selecteer in het keuzemenu Rapportsuite de naam van de rapportsuite die u wilt gebruiken.

## 2. Adobe Analytics-rapportvariabelen toewijzen aan Adobe Dynamic Media Classic viewer-gebeurtenissen en Adobe Dynamic Media Classic-variabelen

Geef op de Adobe Analytics Configuration-pagina de gewenste informatie op in Adobe Analytics-rapporten. Voor elke Adobe Dynamic Media Classic viewer-gebeurtenis van waarover u informatie wilt, kiest u een Adobe Analytics-variabele (uit uw rapportsuite) en een Klassieke Adobe Dynamic Media-variabele.

* Viewergebeurtenissen beschrijven de gebruikersactiviteit die u wilt meten in rapporten.
* De Klassieke variabelen van Adobe Dynamic Media beschrijven de gegevens over gebruikersgebeurtenissen die u de rapporten wilt leveren.

De configuratie van Adobe Analytics biedt ook hulpmiddelen voor het activeren, het uitgeven, en het schrappen van kijkergebeurtenissen.

Nadat u **[!UICONTROL Save]** in de pagina van de Configuratie van Adobe Analytics klikt, wordt de aangepaste het volgen code voor het meten van gebruikersactiviteit opgenomen in de Klassieke kijkers van Dynamic Media van de Adobe. Met deze functionaliteit kunt u gebruikersactiviteiten bijhouden in Adobe Analytics-rapporten.

Zie [Adobe Analytics-rapporten configureren](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Uw Adobe Dynamic Media Classic-viewers publiceren

Publiceer uw Adobe Dynamic Media Classic viewers zodat de viewers (met code voor het bijhouden van gebruikersactiviteiten in Adobe Analytics-rapporten) worden geladen op Adobe Dynamic Media Classic-servers. Nadat u deze gegevens hebt gepubliceerd, worden deze opgenomen in viewers en kunnen deze worden gebruikt voor analyses door Adobe Analytics.

Zie [Configuratiegegevens publiceren](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Adobe Dynamic Media Classic-viewers op uw website plaatsen

Plaats de klassieke Adobe Dynamic Media-viewers met Adobe Analytics-trackingcode op uw website.

## 5. Test de Adobe Analytics-integratie door een Adobe Analytics-rapport te bekijken

Ga naar de Adobe Analytics-website om Adobe Analytics-rapporten te bekijken. Op de pagina Rapportage kunt u gegevens weergeven en grafieken en grafieken genereren om gebruikersactiviteit met verschillende viewers te meten.

Zie [Adobe Analytics-integratie testen door een Adobe Analytics-rapport te bekijken](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
