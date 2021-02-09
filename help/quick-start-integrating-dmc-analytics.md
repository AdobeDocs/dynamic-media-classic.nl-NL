---
title: '"Snel starten: Dynamic Media Classic en Adobe Analytics integreren"'
description: Een inleiding en Snel aan de integratie van Dynamic Media Classic en Adobe Analytics om u te helpen snel aan de slag te gaan.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---


# Snel starten: Integratie van Dynamic Media Classic en Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics is het toonaangevende product dat marketers één plek biedt waar ze geïntegreerde gegevens van alle online initiatieven via meerdere marketingkanalen kunnen meten, analyseren en optimaliseren.

Nadat u Adobe Analytics hebt geïntegreerd met Dynamic Media Classic, kunt u meldingen krijgen over het gedrag van websitebezoekers die Dynamic Media Classic-viewers gebruiken op uw website. Wanneer een websitebezoeker bijvoorbeeld op een zoomdoel in een Dynamic Media Classic Zoom Viewer klikt, neemt Adobe Analytics deze actie op. Adobe Analytics-rapporten kunnen cumulatieve informatie verzamelen over gebruikersactiviteiten in Dynamic Media Classic-viewers.

Met Adobe Analytics-rapporten krijgt u een duidelijk beeld van de activiteiten van klanten op uw website. U kunt bepalen welke productpresentaties tot conversie leiden en welke geen interesse van de klant wekken.

Zie ook [Video meten in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Er is een geldig Adobe Analytics-account vereist om Analytics te integreren met Dynamic Media Classic en analyserapporten te genereren.

**Snel starten**

Deze snelle start is ontworpen om u snel aan de slag te krijgen met Adobe Analytics Instrumentation Kit.

**1. Meld u aan bij Adobe Analytics via Dynamic Media Classic en download Adobe Analytics-rapportvariabelen**

>[!NOTE]
>
>Alvorens u de rapporten van Adobe Analytics kunt vormen en de rapportvariabelen van Adobe Analytics aan de Klassieke gebeurtenissen van Dynamic Media aanpassen, verifieer dat u als lid van de groep van de Toegang van de Dienst van het Web in Adobe Analytics wordt toegevoegd. De leden in deze groep kunnen tot alle rapporten in de gespecificeerde rapportreeksen door middel van de Diensten API van het Web van de Marketing Cloud ongeacht de toestemmingen toegang hebben die in de interface worden geplaatst. Als u een lid wilt toevoegen aan de groep, klikt u in Adobe Analytics op **Admin Tools** > **Gebruikersbeheer** > **Groepen bewerken**.

Nadat u hebt geverifieerd dat u lid bent van de groep van de Toegang van de Dienst van het Web, in Dynamic Media Klassiek, klik **Opstelling** > **Toepassing Opstelling** > **Adobe Analytics**. Voor de pagina van de Configuratie van Adobe Analytics, klik **Login van Adobe Analytics**.

Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Typ in het dialoogvenster Adobe Analytics-aanmelding uw Marketing Cloud-organisatie-id (optioneel) en uw volledige referenties en klik vervolgens op **Aanmelden**. Selecteer in het keuzemenu Rapportsuite de naam van de rapportsuite die u wilt gebruiken.

**2. Adobe Analytics-rapportvariabelen toewijzen aan Dynamic Media Classic viewer-gebeurtenissen en aan Dynamic Media Classic-variabelen**

Geef op de Adobe Analytics Configuration-pagina de gewenste informatie op in Adobe Analytics-rapporten. Voor elke klassieke Dynamic Media-viewergebeurtenis waarover u informatie wilt, kiest u een Adobe Analytics-variabele (uit uw rapportsuite) en een Klassieke Dynamic Media-variabele.

* Viewergebeurtenissen beschrijven de gebruikersactiviteit die u wilt meten in rapporten.
* De Klassieke variabelen van Dynamic Media beschrijven de gegevens over gebruikersgebeurtenissen die u de rapporten wilt leveren.

De configuratie van Adobe Analytics biedt ook hulpmiddelen voor het activeren, het uitgeven, en het schrappen van kijkergebeurtenissen.

Nadat u op Opslaan in het scherm Adobe Analytics Configuration hebt geklikt, wordt de aangepaste trackingcode voor het meten van de gebruikersactiviteit ingevoegd in de Klassieke Dynamic Media-viewers. Met deze functionaliteit kunt u gebruikersactiviteiten bijhouden in Adobe Analytics-rapporten.

Zie [Adobe Analytics-rapporten configureren](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Uw Dynamic Media Classic-viewers publiceren**

Publiceer uw Dynamic Media Classic-viewers zodat de viewers (met code voor het bijhouden van gebruikersactiviteiten in Adobe Analytics-rapporten) worden geladen op Dynamic Media Classic-servers. Nadat u deze gegevens hebt gepubliceerd, worden deze opgenomen in viewers en kunnen deze worden gebruikt voor analyses door Adobe Analytics.

Zie [Configuratiegegevens publiceren](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Dynamic Media Classic-viewers op uw website plaatsen**

Plaats de klassieke Dynamic Media-viewers met Adobe Analytics-trackingcode op uw website.

**5. Test de Adobe Analytics-integratie door een Adobe Analytics-rapport te bekijken**

Ga naar de Adobe Analytics-website om Adobe Analytics-rapporten te bekijken. Op de pagina Rapportage kunt u gegevens weergeven en grafieken en grafieken genereren om gebruikersactiviteit met verschillende viewers te meten.

Zie [Adobe Analytics-integratie testen door een Adobe Analytics-rapport te bekijken](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
