---
title: "Snel starten: Adobe Target Standard/Premium-integratie"
description: Een introductie en Snel starten naar Adobe Target Standard/Premium om u te helpen snel aan de slag te gaan met Adobe Target Standard/Premium-integratietechnieken in Adobe Dynamic Media Classic.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Snel starten: Adobe Target Standard/Premium-integratie{#quick-start-target-integration}

Met Adobe Target Standard/Premium wordt de controle rechtstreeks bij de marketers gelegd om snel en voortdurend meerdere A/B- en multivariate-tests uit te voeren, de doeltreffendheid te meten en de relevantie van online-inhoud te vergroten door segmentatie, doelgerichtheid en Automated Personalization.

Met Adobe Dynamic Media Classic kunt u aanbiedingen maken en sets aanbieden voor Adobe Target Standard/Premium-campagnes. U kunt bijvoorbeeld een aanbiedingsset maken met drie variaties van hetzelfde rich media-element. Vervolgens kunt u met Adobe Target Standard/Premium bepalen welk element een betere conversielift biedt. U kunt aanbiedingen maken en sets aanbieden op basis van een standaardsjabloon of op basis van afzonderlijke afbeeldingen. Nadat de aanbiedingsreeks is geduwd op of opgeslagen aan Adobe Target Standard/Premium, waar de aanbiedingen aan dozen en ervaringen worden geassocieerd, kan Adobe Target Standard/Premium campagnes voeren. Deze campagnes bepalen welke variatie van een website waarschijnlijk het beste voor klikdoorloop en omzetting zal presteren.

Gebruik Adobe Target Standard/Premium HTML voor een betere aanpassing van dynamische Adobe Dynamic Media Classic-inhoud. Zie de [Adobe Target Standard/Premium-productdocumentatie](https://experienceleague.adobe.com/docs/target.html) voor meer informatie .

>[!NOTE]
>
>Een geldige Adobe Target Standard/Premium-account is vereist als u Adobe Target Standard/Premium met Adobe Dynamic Media Classic wilt gebruiken.

Deze snelle start is ontworpen om u snel aan de slag te krijgen met Adobe Target Standard/Premium HTML-aanbiedingen. Voer stap 1 tot en met 3 uit. Na elke stap, is er een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

## 1. Voer de Adobe Target Standard/Premium-URL in op de pagina Algemene instellingen voor toepassing

Adobe Dynamic Media Classic heeft uw Adobe Target Standard/Premium-URL nodig om te integreren met Adobe Target Standard/Premium. Kopieer het gedeelte van uw Adobe Target Standard/Premium-URL tot en met `.com`en voer deze in de Adobe Dynamic Media Classic in **[!UICONTROL Application General Settings]** pagina, in de **[!UICONTROL Servers]** groep, **[!UICONTROL Test&Target Server Name]** tekstveld. Zie [Adobe Dynamic Media Classic integreren met Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. De aanbiedingsset maken

Gebruik een geparametriseerde sjabloon of afbeeldingen om een aanbiedingsset te maken. U maakt HTML-aanbiedingssets op de pagina Set Test&amp;Target-aanbiedingen. Als u deze pagina wilt openen, selecteert u de sjabloon of de afbeeldingen en gaat u vervolgens op de algemene navigatiebalk naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

Als u een aanbieding met een sjabloon wilt maken, selecteert u **[!UICONTROL Add & Preview]**. Wijzig parameterwaarden op de pagina Toevoegen en voorvertonen.

Als u een aanbieding met afbeeldingen wilt maken, sleept u afbeeldingen naar de pagina Set Test&amp;Target-aanbieding. Selecteren **[!UICONTROL Preview]** en kiest u een voorinstelling voor afbeeldingen of alle afbeeldingen in de aanbiedingsset.

Sla de aangeboden set op nadat u deze hebt gemaakt.

Zie [Een aanbiedingsset maken](creating-offer-set.md#creating_an_offer_set).

## 3. Push the aanbieding set to Adobe Target Standard/Premium

Selecteer in de pagina Set Test&amp;Target-aanbiedingen de optie **[!UICONTROL Push Offers]** en voer uw aanmeldgegevens in het dialoogvenster Inloggen bij &amp;doel testen in. Zie [Push-aanbiedingen worden ingesteld op Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
