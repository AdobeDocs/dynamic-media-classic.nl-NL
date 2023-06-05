---
title: Adobe Analytics-videorapporten inschakelen
description: Leer hoe u Adobe Analytics-videoverslagen inschakelt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Adobe Analytics-videorapporten inschakelen{#enabling-adobe-analytics-video-reports}

Als u Adobe Analytics-videoverslagen op basis van hartslag gebruikt, hoeft u de vier videoviewergebeurtenissen (Play, Pause, Stop, Milestone) niet meer in te schakelen wanneer u Adobe Analytics in Adobe Dynamic Media Classic configureert. De videorecart werkt met Adobe Dynamic Media Classic HTML 25 Video en Gemengde Media-viewers buiten de box. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports.

* Voor een inleiding op streamingmedia en &quot;hartslagmeting&quot; raadpleegt u [Informatie over Adobe Analytics voor Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* De integratie van Adobe Analytics-videorapporten met Adobe Dynamic Media Classic ondersteunt oplossingsvariabelen, maar geen aangepaste variabelen.

   Zie [Parameters voor audio en video](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) voor meer informatie over oplossingsvariabelen en douanevariabelen.

* De uit-van-de-doos segmenten van één-minieme toename worden gesteund. Aangepaste segmentrapportage, zoals door de klant gedefinieerde mijlpalen op basis van tijdstappen, procentuele mijlpaal of verschuivingsmijlpalen, wordt echter niet ondersteund.

   Ga voor meer informatie over de vereisten en installatie van streaming media naar [Stromingmedia meten in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Voor informatie over aangepaste en oplossingsvariabelen raadpleegt u [Media-rapporten inschakelen](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Als uw gelicentieerde oplossing van Adobe Analytics Video Heartbeat niet omvat, moet u de stappen blijven gebruiken die in dit hoofdstuk worden beschreven om de variabelen van Adobe Analytics aan de gebeurtenissen en de variabelen van de Adobe Dynamic Media Classic viewer toe te wijzen.
