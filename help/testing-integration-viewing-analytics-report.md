---
title: Integratie testen door een Adobe Analytics-rapport te bekijken
description: Leren hoe u de integratie kunt testen door een Adobe Analytics-rapport te bekijken.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# De integratie testen door een Adobe Analytics-rapport te bekijken{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nadat u de benodigde variabelen in Adobe Analytics hebt gemaakt, deze aan Dynamic Media Classic-gebeurtenissen hebt gekoppeld en de benodigde implementatiestappen hebt uitgevoerd, kunt u de instellingen testen. U kunt testen en controleren of de gegevens worden vastgelegd in Adobe Analytics zelf. Als de opstelling hier werkt, dan zijn geen verdere stappen nodig. Ervan uitgaande dat u de bovenstaande stappen hebt uitgevoerd en uw Dynamic Media Classic-gebeurtenisgegevens aan een of meer variabelen voor aangepast verkeer hebt gekoppeld, volgt u deze workflow om uw gegevens in Adobe Analytics te testen.

**U kunt als volgt de integratie testen door een Adobe Analytics-rapport te bekijken:**

1. Start een Dynamic Media Classic viewer van uw account, met name een account dat de metrische gegevens die u wilt ophalen uitzendt, en communiceer ermee om gebeurtenisgegevens te maken.

   Als u bijvoorbeeld populaire alternatieve weergaven in een set afbeeldingen wilt meten, geeft u een voorbeeld van een set afbeeldingen weer en klikt u op de verschillende miniatuurafbeeldingen.

1. Ga in Adobe Analytics naar **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Naam van profiel] en selecteer de naam van de verkeersproxy in het menu.

   Als u bijvoorbeeld toegang wilt krijgen tot de **[!UICONTROL LoadAsset]**-proxy in de voorbeeldaccount, is de juiste menukeuze **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Als u meer dan tien aangepaste opdrachten hebt, ziet u ook andere menuopties.

1. Bekijk de kaart die door Adobe Analytics wordt geproduceerd. Deze grafiek is typisch enkel de gegevens voor één enkele metrisch. Als u ook wilt weten met welk element deze gegevens zijn gekoppeld, vraagt u de elementgegevens van deze gebeurtenis op. Het is bijvoorbeeld vaak handig om te weten welke video wordt bekeken naar slechts 50% of welke afbeelding in een set populair is.

>[!NOTE]
>
>Alle Dynamic Media Classic viewergegevens worden weergegeven en gerapporteerd in Custom Traffic-rapporten of Custom Conversion-rapporten van Adobe Analytics.

Zie [Analytische Tutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html) voor meer informatie.