---
title: '"Snel starten: Dynamic Media Classic en Adobe Analytics integreren "'
seo-title: '"Snel starten: Dynamic Media Classic en Adobe Analytics integreren "'
description: 'null'
seo-description: Een inleiding en Snel aan de integratie van Dynamic Media Classic en Adobe Analytic waarmee u snel aan de slag kunt.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Snel starten: Dynamic Media Classic en Adobe Analytics integreren {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics is het toonaangevende product dat marketers één locatie biedt waar ze geïntegreerde gegevens van alle online initiatieven via meerdere marketingkanalen kunnen meten, analyseren en optimaliseren.

Nadat Adobe Analytics met het het Publiceren Scene7 Systeem is geïntegreerd, kunt u rapporten over het gedrag van websitebezoekers krijgen gebruikend de Dynamische Klassieke kijkers van Media op uw website. Wanneer een websitebezoeker bijvoorbeeld op een zoomdoel in een Dynamic Media Classic Zoom Viewer klikt, wordt deze actie door Adobe Analytics vastgelegd. Rapporten van Adobe Analytics kunnen cumulatieve informatie over gebruikersactiviteit in Dynamische Media Classic viewers verzamelen.

Met Adobe Analytics-rapporten kunt u een duidelijk beeld krijgen van de activiteiten van klanten op uw website. U kunt bepalen welke productpresentaties tot conversie leiden en welke geen interesse van de klant wekken.

Zie ook Video [meten in Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Een geldig account van Adobe Analytics is vereist om Analytics met het het Publiceren Scene7 Systeem te integreren en de rapporten van Analytics te produceren.

**Snel starten**

Deze snelle start is ontworpen om snel aan de slag te gaan met Adobe Analytics Instrumentation Kit.

**1. Meld u aan bij Adobe Analytics via Dynamic Media Classic en download de rapportvariabelen van Adobe Analytics**

>[!NOTE]
>
>Voordat u Adobe Analytics-rapporten kunt configureren en Adobe Analytics-rapportvariabelen kunt afstemmen op Dynamic Media Classic-gebeurtenissen, moet u controleren of u bent toegevoegd als lid van de Web Service Access-groep in Adobe Analytics. De leden in deze groep kunnen tot alle rapporten in de gespecificeerde rapportreeksen door middel van de Diensten API van het Web van de Wolk van de Marketing toegang hebben ongeacht de toestemmingen die in de interface worden geplaatst. Als u een lid wilt toevoegen aan de groep, klikt u in Adobe Analytics op **Beheer Extra** > **Gebruikersbeheer** > Groepen **** bewerken.

Nadat u hebt geverifieerd dat u lid bent van de groep van de Toegang van de Dienst van het Web, in Dynamische Klassieke Media, klik **Opstelling** > de Opstelling **van de** Toepassing > **Analytics** van Adobe. Klik op de configuratiepagina van Adobe Analytics op **Adobe Analytics Login**.

Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Typ in het dialoogvenster Aanmelden voor Adobe Analytics uw organisatie-id voor de marketingcloud (optioneel) en uw volledige referenties en klik vervolgens op **Aanmelden**. Selecteer in het keuzemenu Rapportsuite de naam van de rapportsuite die u wilt gebruiken.

**2. Rapportvariabelen voor Adobe Analytics toewijzen aan dynamische media Classic-viewergebeurtenissen en dynamische media Classic-variabelen**

Geef op de pagina Configuratie Adobe Analytics de gewenste informatie op in Adobe Analytics-rapporten. Voor elke dynamische Media Classic viewer-gebeurtenis waarover u informatie wilt, kiest u een Adobe Analytics-variabele (uit uw rapportsuite) en een Dynamic Media Classic-variabele.

* Viewergebeurtenissen beschrijven de gebruikersactiviteit die u wilt meten in rapporten.
* De dynamische Klassieke variabelen van Media beschrijven de gegevens over gebruikersgebeurtenissen die u de rapporten wilt leveren.

De configuratie van de Analytics van Adobe biedt ook hulpmiddelen voor het activeren van, het uitgeven van, en het schrappen van kijkergebeurtenissen.

Nadat u in het scherm Configuratie van de Analyse van Adobe sparen klikt, wordt de aangepaste het volgen code voor het meten van gebruikersactiviteit opgenomen in de Dynamische Klassieke kijkers van Media. Met deze functionaliteit kunt u gebruikersactiviteiten bijhouden in Adobe Analytics-rapporten.

Zie [Adobe Analytics-rapporten](configuring-analytics-reports.md#configuring_adobe_analytics_reports)configureren.

**3. Uw dynamische Media Classic-viewers publiceren**

Publiceer uw Dynamic Media Classic-viewers zodat de viewers (met code voor het bijhouden van gebruikersactiviteiten in Adobe Analytics-rapporten) worden geladen op Dynamic Media Classic-servers. Nadat u deze gegevens hebt gepubliceerd, worden deze opgenomen in viewers en kunnen deze worden gebruikt voor analyses van Adobe Analytics.

Zie [Configuratiegegevens](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)publiceren.

**4. Dynamische media Klassieke viewers op uw website plaatsen**

Plaats de Dynamic Media Classic-viewers met de trackingcode voor Adobe Analytics op uw website.

**5. Test de integratie met Adobe Analytics door een Adobe Analytics-rapport te bekijken**

Ga naar de website Adobe Analytics als u Adobe Analytics-rapporten wilt weergeven. Op de pagina Rapportage kunt u gegevens weergeven en grafieken en grafieken genereren om gebruikersactiviteit met verschillende viewers te meten.

Zie De integratie van Adobe Analytics [testen door een Adobe Analytics-rapport](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)te bekijken.
