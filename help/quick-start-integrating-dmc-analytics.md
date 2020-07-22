---
title: '"Snel starten: Dynamic Media Classic en Adobe Analytics integreren "'
seo-title: '"Snel starten: Dynamic Media Classic en Adobe Analytics integreren "'
description: 'null'
seo-description: Introductie en Snel aan de integratie van Dynamic Media Classic en Adobe Analytic om u te helpen snel aan de slag te gaan.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: 7c9b1976ced6ef5ad48b624b99aeeffed380168a
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---


# Snel starten: Dynamic Media Classic en Adobe Analytics integreren {#quick-start-integrating-dmc-analytics}

Adobe Analytics is het toonaangevende product dat marketers één locatie biedt waar ze geïntegreerde gegevens van alle online initiatieven via meerdere marketingkanalen kunnen meten, analyseren en optimaliseren.

Nadat u Adobe Analytics hebt geïntegreerd met Dynamic Media Classic, kunt u meldingen krijgen over het gedrag van websitebezoekers die Dynamic Media Classic-viewers op uw website gebruiken. Wanneer een websitebezoeker bijvoorbeeld op een zoomdoel in een klassieke zoomviewer voor Dynamic Media klikt, wordt deze handeling door Adobe Analytics vastgelegd. Adobe Analytics-rapporten kunnen cumulatieve informatie verzamelen over gebruikersactiviteiten in Dynamic Media Classic-viewers.

Met Adobe Analytics-rapporten krijgt u een duidelijk beeld van de activiteiten van klanten op uw website. U kunt bepalen welke productpresentaties tot conversie leiden en welke geen interesse van de klant wekken.

Zie ook Video [meten in Adobe Analytics](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Een geldig Adobe Analytics-account is vereist om Analytics te integreren met Dynamic Media Classic en Analytics-rapporten te genereren.

**Snel starten**

Deze snelle start is ontworpen om snel aan de slag te gaan met Adobe Analytics Instrumentation Kit.

**1. Meld u aan bij Adobe Analytics via Dynamic Media Classic en download Adobe Analytics-rapportvariabelen**

>[!NOTE]
>
>Voordat u Adobe Analytics-rapporten kunt configureren en Adobe Analytics-rapportvariabelen kunt afstemmen op Dynamic Media Classic-gebeurtenissen, moet u controleren of u bent toegevoegd als lid van de Web Service Access-groep in Adobe Analytics. De leden in deze groep kunnen tot alle rapporten in de gespecificeerde rapportreeksen door middel van de Diensten API van het Web van de Wolk van de Marketing toegang hebben ongeacht de toestemmingen die in de interface worden geplaatst. Als u een lid wilt toevoegen aan de groep, klikt u in Adobe Analytics op **Beheertools** > **Gebruikersbeheer** > Groepen **** bewerken.

Nadat u hebt geverifieerd dat u lid bent van de groep van de Toegang van de Dienst van het Web, in de Klassieke Dynamic Media, klik **Opstelling** > de Opstelling **van de** Toepassing > **Adobe Analytics**. Klik op de configuratiepagina van Adobe Analytics op Aanmelden bij **Adobe Analytics**.

Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Typ in het dialoogvenster Adobe Analytics-aanmelding uw Org-id voor de marketingcloud (optioneel) en uw volledige referenties en klik vervolgens op **Aanmelden**. Selecteer in het keuzemenu Rapportsuite de naam van de rapportsuite die u wilt gebruiken.

**2. Adobe Analytics-rapportvariabelen toewijzen aan Dynamic Media Classic viewer-gebeurtenissen en Dynamic Media Classic-variabelen**

Geef op de configuratiepagina van Adobe Analytics de gewenste informatie op in Adobe Analytics-rapporten. Voor elke Dynamic Media Classic viewer-gebeurtenis waarover u informatie wilt, kiest u een Adobe Analytics-variabele (uit uw rapportsuite) en een Dynamic Media Classic-variabele.

* Viewergebeurtenissen beschrijven de gebruikersactiviteit die u wilt meten in rapporten.
* De Klassieke variabelen van Dynamic Media beschrijven de gegevens over gebruikersgebeurtenissen die u de rapporten wilt leveren.

De configuratie van Adobe Analytics bevat ook gereedschappen voor het activeren, bewerken en verwijderen van viewergebeurtenissen.

Nadat u op Opslaan in het configuratiescherm van Adobe Analytics hebt geklikt, wordt de aangepaste trackingcode voor het meten van de gebruikersactiviteit ingevoegd in Dynamic Media Classic-viewers. Met deze functionaliteit kunt u gebruikersactiviteiten bijhouden in Adobe Analytics-rapporten.

Zie Adobe Analytics-rapporten [configureren](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Uw Dynamic Media Klassieke viewers publiceren**

Publiceer uw Dynamic Media Klassieke viewers zodat de viewers (met code voor het bijhouden van gebruikersactiviteiten in Adobe Analytics-rapporten) worden geladen op Dynamic Media Klassieke servers. Nadat u deze gegevens hebt gepubliceerd, worden deze opgenomen in viewers en kunnen deze worden gebruikt voor analyses door Adobe Analytics.

Zie [Configuratiegegevens](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)publiceren.

**4. Dynamic Media Klassieke viewers op uw website plaatsen**

Plaats de klassieke Dynamic Media-viewers met de trackingcode van Adobe Analytics op uw website.

**5. Test de integratie van Adobe Analytics door een Adobe Analytics-rapport te bekijken**

Ga naar de Adobe Analytics-website om Adobe Analytics-rapporten te bekijken. Op de pagina Rapportage kunt u gegevens weergeven en grafieken en grafieken genereren om gebruikersactiviteit met verschillende viewers te meten.

Zie De integratie van Adobe Analytics [testen door een Adobe Analytics-rapport](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)te bekijken.
