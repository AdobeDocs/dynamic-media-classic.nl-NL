---
title: Integratie testen door een Adobe Analytics-rapport te bekijken
seo-title: Integratie testen door een Adobe Analytics-rapport te bekijken
description: 'null'
seo-description: Leren hoe u de integratie kunt testen door een Adobe Analytics-rapport te bekijken.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---


# Integratie testen door een Adobe Analytics-rapport te bekijken{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nadat u de noodzakelijke variabelen in Adobe Analytics hebt gecreeerd, hen met Dynamische Media Classic gebeurtenissen en voltooide de noodzakelijke implementatiestappen koppelt, dan zou u de opstelling moeten testen. U kunt testen en controleren of de gegevens worden vastgelegd in Adobe Analytics zelf. Als de opstelling hier werkt, dan zijn geen verdere stappen nodig. Ervan uitgaande dat u de bovenstaande stappen hebt uitgevoerd en uw Dynamic Media Classic-gebeurtenisgegevens aan een of meer variabelen voor aangepast verkeer hebt gekoppeld, volgt u deze workflow om uw gegevens in Adobe Analytics te testen.

**De integratie testen door een Adobe Analytics-rapport te bekijken**

1. Start een Dynamic Media Classic-viewer van uw account, in het bijzonder een viewer die de metrische gegevens uitzendt die u wilt vastleggen, en communiceer ermee om gebeurtenisgegevens te maken.

   Als u bijvoorbeeld de populairste alternatieve weergaven in een set afbeeldingen wilt meten, bekijkt u eerst een voorvertoning van een set afbeeldingen en klikt u op de verschillende miniatuurafbeeldingen.

1. Ga in Adobe Analytics naar Custom Traffic > Custom Traffic 1-10 > [Name of prop]en selecteer de naam van de verkeersprop in het menu.

   Als u bijvoorbeeld de LoadAsset-proxy wilt openen in onze voorbeeldaccount, hebt u de juiste menukeuze: Custom Traffic > Custom Traffic 1-10 > LoadAsset. Als u meer dan tien aangepaste profielen hebt, ziet u mogelijk ook extra menuopties.

1. Bekijk de kaart die door Adobe Analytics wordt geproduceerd. Merk op dat dit typisch enkel de gegevens voor één enkele metrisch is. Als u ook wilt weten met welk element deze gegevens zijn gekoppeld (bijvoorbeeld welke video naar slechts 50% wordt gecontroleerd of welke afbeelding in een set het populairst is), moet u ook de elementgegevens van deze gebeurtenis vastleggen.

>[!NOTE]
>
>Alle dynamische Media Classic viewergegevens worden weergegeven en gerapporteerd in Custom Traffic-rapporten of Custom Conversion-rapporten van Adobe Analytics.

Zie [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)voor meer informatie.
