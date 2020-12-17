---
title: Overzicht van Adobe Dynamic Media Classic-platform
seo-title: Overzicht van Adobe Dynamic Media Classic-platform
description: 'null'
seo-description: Een overzicht van het Dynamic Media Classic-platform en workflowproces.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---


# Adobe Dynamic Media Classic-platform - overzicht{#adobe-scene-platform-overview}

Dynamic Media Classic is een geïntegreerde, rijke omgeving voor mediabeheer, -publicatie en -gebruik. De rijke media kunnen aan alle marketing en verkoopkanalen, met inbegrip van het Web, drukmateriaal, e-mailcampagnes, Webportals, Desktops, en apparaten worden geleverd.

## Werkstroomproces {#workflow-process}

De belangrijkste Dynamic Media Classic workflowstappen zijn:

* **Upload en beheer uw**
middelenUpload uw media-elementen naar Dynamic Media Classic. U kunt middelen op het systeem organiseren, doorbladeren en zoeken. U kunt ook metagegevens toepassen op elementen.

* **Maak rijke**
mediaMaak verschillende configuraties van uw elementen, zoals eCatalogs, Afbeeldingssets, Draaisets, Staalsets, Gemengde-mediasets, Standaard-sjablonen en FXG-sjablonen. Zie Informatie over rijke media voor meer informatie.

* **Publiceer en beheer**
publiceer activa aan het netwerk van de Klassieke Zas van Dynamic Media, evenals controleer de status van activa wanneer zij worden gepubliceerd, beheer gebruikersrechten, en handhaaf veiligheid.

* **Media**
leveren van Dynamic Media Classic SaaS-netwerk naar webpagina&#39;s, toepassingen en mobiele apparaten; de media zijn geoptimaliseerd voor prestaties en worden geleverd met CDN-caching. Dynamic Media Classic biedt u een URL voor elk element. Nadat u het element hebt gepubliceerd, wordt de URL actief.

![Het Dynamic Media Classic-workflowproces](/help/assets/gs_workflow.png)

## Enkele master afbeeldingen en enkele URL-aanroepen {#single-master-images-and-single-url-calls}

Dynamic Media Classic is fundamenteel anders dan andere systemen, omdat u Dynamic Media Classic kunt gebruiken om media dynamisch te leveren van enkele master elementen en URL-aanroepen.

De URL-tekenreeksen die u genereert met Dynamic Media Classic bevatten instructies die de server vertellen hoe het element moet worden weergegeven wanneer het wordt geleverd. Dezelfde master afbeelding kan bijvoorbeeld worden geleverd in verschillende formaten, formaten, gewichten, kleuren en zoomweergaven. Als onderdeel van het maken en publiceren van media-elementen met Dynamic Media Classic, kunt u de effecten visueel configureren. Op deze manier maakt u de URL-aanroepen die de server correct vertellen hoe u uw master element aan toepassingen moet presenteren.

![Dynamic Media Classic kan dezelfde master afbeelding leveren aan verschillende media in verschillende formaten en formaten.](/help/assets/gs_dynamic_publishing.png)

## Inhoud in cache plaatsen {#content-caching}

De afbeeldingen die Dynamic Media Classic dynamisch genereert, zijn cachegvriendelijk. in de meeste gevallen zijn het JPEG-afbeeldingen met unieke URL-aanroepen die ze identificeren. De beelden worden geleverd op het netwerk van de inhoudslevering (CDN), een systeem van servers die samen op Internet worden genetwerkt om inhoud sneller te leveren. De beelden worden verdeeld van servers globaal, en dan aan computers worden gevestigd. Wanneer u een cachemechanisme implementeert met een CDN-leverancier, wijzigt u gewoon de servernaam zodat deze naar de Dynamic Media Image Server met CDN-ondersteuning verwijst. Alle Dynamic Media Classic-edities bevatten CDN-caching in een pakket.
