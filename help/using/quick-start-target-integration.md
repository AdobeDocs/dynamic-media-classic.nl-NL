---
title: "Snel starten: Adobe Target Standard/Premium-integratie"
description: Een introductie en Snel starten naar Adobe Target Standard/Premium om u te helpen snel aan de slag te gaan met Adobe Target Standard/Premium-integratietechnieken in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Snel starten: Adobe Target Standard/Premium-integratie{#quick-start-target-integration}

Adobe Target Standard/Premium stelt de controle rechtstreeks in handen van marktpartijen. Zo kunt u snel en voortdurend meerdere A/B- en multivariatietests uitvoeren en de doeltreffendheid meten. En, kan het de relevantie van online inhoud door segmentatie, richten, en Automated Personalization verhogen.

Met Adobe Dynamic Media Classic kunt u aanbiedingen en sets aanbiedingen maken voor Adobe Target Standard-/Premium-campagnes. U kunt bijvoorbeeld een set voorstellen maken met drie variaties van hetzelfde rich media-element. Vervolgens kunt u met Adobe Target Standard of Premium bepalen welk element een betere conversielift biedt. U kunt aanbiedingen en sets voorstellen op basis van een standaardsjabloon of op basis van afzonderlijke afbeeldingen. Nadat de set aanbiedingen is geduwd op of opgeslagen op Adobe Target Standard/Premium, waar de aanbiedingen zijn gekoppeld aan vakjes en ervaringen, kunnen er campagnes worden uitgevoerd op Adobe Target Standard/Premium. Deze campagnes bepalen welke variatie van een website waarschijnlijk het beste voor klikdoorloop en omzetting zal presteren.

Gebruik Adobe Target Standard/Premium HTML voor een betere aanpassing van dynamische Adobe Dynamic Media Classic-inhoud. Zie de [Adobe Target Standard/Premium-productdocumentatie](https://experienceleague.adobe.com/en/docs/target) voor meer informatie .

>[!NOTE]
>
>Een geldige Adobe Target Standard/Premium-account is vereist als u Adobe Target Standard/Premium met Adobe Dynamic Media Classic wilt gebruiken.

Deze snelle start is ontworpen om snel aan de slag te gaan met Adobe Target Standard/Premium HTML Offer Sets. Voer stap 1 tot en met 3 uit. Na elke stap, is er een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

## 1. Voer de Adobe Target Standard/Premium-URL in op de pagina Algemene instellingen voor toepassing

Adobe Dynamic Media Classic heeft uw Adobe Target Standard/Premium-URL nodig om te integreren met Adobe Target Standard/Premium. Kopieer het gedeelte van uw Adobe Target Standard/Premium-URL tot en met `.com`en voer deze in de Adobe Dynamic Media Classic in **[!UICONTROL Application General Settings]** pagina, in de **[!UICONTROL Servers]** groep, **[!UICONTROL Test&Target Server Name]** tekstveld. Zie [Adobe Dynamic Media Classic integreren met Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Maak de set voorstellen

Gebruik een of meer geparametriseerde sjablonen om een set aanbiedingen te maken. U kunt de Reeksen van de Aanbieding van de HTML tot stand brengen op de test&amp;Doel pagina van de Aanbieding van de Aanbieding. Als u deze pagina wilt openen, selecteert u de sjabloon of de afbeeldingen en gaat u vervolgens op de algemene navigatiebalk naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

Als u een aanbieding met een sjabloon wilt maken, selecteert u **[!UICONTROL Add & Preview]**. Wijzig parameterwaarden op de pagina Toevoegen en voorvertonen.

Als u een aanbieding met afbeeldingen wilt maken, sleept u de afbeeldingen naar de pagina Set Test&amp;Target-aanbieding. Selecteren **[!UICONTROL Preview]** en kiest u een voorinstelling voor een afbeelding of voor alle afbeeldingen in de set met voorstellen.

Sla de set voorstellen op nadat u deze hebt gemaakt.

Zie [Een aanbiedingsset maken](creating-offer-set.md#creating_an_offer_set).

## 3. Zet de aanbieding op Adobe Target Standard/Premium

Selecteer in de pagina Set Test&amp;Target-aanbiedingen de optie **[!UICONTROL Push Offers]** en voer uw aanmeldgegevens in het dialoogvenster Inloggen bij &amp;doel testen in. Zie [Push-aanbiedingen worden ingesteld op Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
