---
title: De integratie testen door een Adobe Analytics-rapport te bekijken
description: Leer hoe u de integratie in Adobe Dynamic Media Classic kunt testen door een Adobe Analytics-rapport te bekijken.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# De integratie testen door een Adobe Analytics-rapport te bekijken{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nadat u de benodigde variabelen in Adobe Analytics hebt gemaakt, deze aan Adobe Dynamic Media Classic-gebeurtenissen hebt gekoppeld en de benodigde implementatiestappen hebt uitgevoerd, kunt u de instellingen testen. U kunt testen en controleren of de gegevens worden vastgelegd in Adobe Analytics zelf. Als de opstelling hier werkt, dan zijn geen verdere stappen nodig. Ervan uitgaande dat u de bovenstaande stappen hebt uitgevoerd en uw Adobe Dynamic Media Classic-gebeurtenisgegevens aan een of meer variabelen voor aangepast verkeer hebt gekoppeld, volgt u deze workflow om uw gegevens in Adobe Analytics te testen.

**U kunt als volgt de integratie testen door een Adobe Analytics-rapport te bekijken:**

1. Start een Adobe Dynamic Media Classic-viewer van uw account, in het bijzonder een viewer die de gewenste metrische gegevens verzendt, en communiceer ermee om gebeurtenisgegevens te maken.

   Als u bijvoorbeeld populaire alternatieve weergaven in een set afbeeldingen wilt meten, geeft u een voorbeeld van een set afbeeldingen weer en klikt u op de verschillende miniatuurafbeeldingen.

1. Ga in Adobe Analytics naar **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Naam van pop]en selecteert u de naam van de verkeersproxy in de menuopties.

   Als u bijvoorbeeld toegang wilt krijgen tot **[!UICONTROL LoadAsset]** in de voorbeeldaccount is de juiste menukeuze: **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Als u meer dan tien aangepaste opdrachten hebt, ziet u ook andere menuopties.

1. Bekijk de kaart die door Adobe Analytics wordt geproduceerd. Deze grafiek is typisch enkel de gegevens voor één enkele metrisch. Als u ook wilt weten met welk element deze gegevens zijn gekoppeld, vraagt u de elementgegevens van deze gebeurtenis op. Het is bijvoorbeeld vaak handig om te weten welke video wordt bekeken naar slechts 50% of welke afbeelding in een set populair is.

>[!NOTE]
>
>Alle Adobe Dynamic Media Classic-viewergegevens worden weergegeven en gerapporteerd in Custom Traffic-rapporten of Custom Conversion-rapporten van Adobe Analytics.

Zie voor meer informatie [Tutorials voor analyse](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).