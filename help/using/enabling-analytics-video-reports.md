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
topic: Development, Integrations
level: Experienced
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Adobe Analytics-videorapporten inschakelen{#enabling-adobe-analytics-video-reports}

Als u Adobe Analytics-videoverslagen op basis van hartslag gebruikt, hoeft u de vier videoviewergebeurtenissen (Play, Pause, Stop, Milestone) niet meer in te schakelen wanneer u Adobe Analytics in Adobe Dynamic Media Classic configureert. De videokaart werkt met Adobe Dynamic Media Classic HTML 25 Video en Gemengde Media-viewers buiten de box. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports.

* Voor een inleiding op streamingmedia en &#39;hartslagmeting&#39; raadpleegt u [Informatie over Adobe Analytics para medios de streaming](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* De integratie van Adobe Analytics-videorapporten met Adobe Dynamic Media Classic ondersteunt oplossingsvariabelen, maar geen aangepaste variabelen.

  Zie [Parameters voor audio en video](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) voor meer informatie over oplossingsvariabelen en douanevariabelen.

* De uit-van-de-doos segmenten van één-minieme toename worden gesteund. Aangepaste segmentrapportage, zoals door de klant gedefinieerde mijlpalen op basis van tijdstappen, procentuele mijlpalen of verschuivingsmijlpalen, wordt echter niet ondersteund.

  Ga voor meer informatie over de vereisten en installatie van streaming media naar [Stromingmedia meten in Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Voor informatie over douane en oplossingsvariabelen, zie [Media-rapporten inschakelen](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Als uw gelicentieerde oplossing van Adobe Analytics Video Heartbeat niet omvat, moet u de stappen blijven gebruiken die in dit hoofdstuk worden beschreven om de variabelen van Adobe Analytics aan de gebeurtenissen en de variabelen van de Adobe Dynamic Media Classic viewer toe te wijzen.
