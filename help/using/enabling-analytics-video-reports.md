---
title: Adobe Analytics-videorapporten inschakelen
description: Leer hoe u Adobe Analytics-videoverslagen inschakelt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: 458a80aad6e983dbccfe2108f0a389a4651f9f38
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Adobe Analytics-videorapporten inschakelen{#enabling-adobe-analytics-video-reports}

Als u Adobe Analytics-videoverslagen op basis van hartslag gebruikt, hoeft u de vier videoviewergebeurtenissen (Play, Pause, Stop, Milestone) niet meer in te schakelen wanneer u Adobe Analytics in Adobe Dynamic Media Classic configureert. De functie Videohartslag werkt met Adobe Dynamic Media Classic HTML5-viewers voor video en gemengde media die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics-videorapporten.

* Voor een inleiding aan het stromen media en &quot;hartslagmeting,&quot;zie [&#x200B; Ongeveer Analytics van Adobe voor het Streamen van Media &#x200B;](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* De integratie van Adobe Analytics-videorapporten met Adobe Dynamic Media Classic ondersteunt oplossingsvariabelen, maar geen aangepaste variabelen.

  Zie [&#x200B; Audio en Video parameters &#x200B;](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) voor meer informatie over oplossingsvariabelen en douanevariabelen.

* De uit-van-de-doos segmenten van één-minieme toename worden gesteund. Aangepaste segmentrapportage, zoals door de klant gedefinieerde mijlpalen op basis van tijdstappen, procentuele mijlpalen of verschuivingsmijlpalen, wordt echter niet ondersteund.

  Voor meer informatie over het stromen media vereisten en opstelling, zie [&#x200B; Stromende Media van de Meetlat in Adobe Analytics &#x200B;](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Voor informatie over douane en oplossingsvariabelen, zie [&#x200B; de rapporten van Media enablement &#x200B;](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Als uw gelicentieerde oplossing van Adobe Analytics Video Heartbeat niet omvat, blijf het gebruiken van de stappen die in dit hoofdstuk worden beschreven om de variabelen van Adobe Analytics aan de gebeurtenissen en de variabelen van de viewer van Adobe Dynamic Media Classic toe te wijzen.
