---
title: Overzicht van Adobe Dynamic Media Classic-programma
description: Een overzicht van het Adobe Dynamic Media Classic-programma en het gehele workflowproces.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Overzicht van Adobe Dynamic Media Classic-programma{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic is een geïntegreerde, rijke omgeving voor mediabeheer, -publicatie en -services. De rijke media kunnen aan alle marketing en verkoopkanalen, met inbegrip van het Web, drukmateriaal, e-mailcampagnes, Webportals, Desktops, en apparaten worden geleverd.

Zie ook [Overzicht van Platform](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) trainingsvideo.

## Workflowproces {#workflow-process}

De belangrijkste Adobe Dynamic Media Classic-workflowstappen zijn:

* **Uw elementen uploaden en beheren** - Upload uw media-elementen naar Adobe Dynamic Media Classic. U kunt middelen op het systeem organiseren, doorbladeren en zoeken. U kunt ook metagegevens toepassen op elementen.

* **Rijke media maken** - Maak verschillende configuraties van uw elementen, zoals eCatalogs, Afbeeldingssets, Draaisets, Staalsets, Gemengde Mediasets, Basissjablonen en FXG-sjablonen.

* **Publiceren en beheren** - Elementen publiceren naar het Adobe Dynamic Media Classic SaaS-netwerk. De status van elementen controleren wanneer deze worden gepubliceerd. Gebruikersrechten beheren en de beveiliging handhaven.

* **Serve** - Media leveren van het Adobe Dynamic Media Classic SaaS-netwerk naar webpagina&#39;s, toepassingen en mobiele apparaten; de media zijn geoptimaliseerd voor prestaties en worden geleverd met CDN-caching. Adobe Dynamic Media Classic biedt u een URL voor elk element. Nadat u het element hebt gepubliceerd, wordt de URL actief.

![Het Adobe Dynamic Media Classic-workflowproces](/help/using/assets/gs_workflow.png)

## Eén primaire afbeelding en één URL-aanroep {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic is fundamenteel anders dan andere systemen, omdat u Adobe Dynamic Media Classic kunt gebruiken om media dynamisch te leveren vanaf enkele primaire elementen en URL-aanroepen.

De URL-tekenreeksen die u genereert met Adobe Dynamic Media Classic bevatten instructies die de server vertellen hoe het element moet worden weergegeven wanneer het wordt geleverd. Dezelfde primaire afbeelding kan bijvoorbeeld worden geleverd in verschillende formaten, formaten, gewichten, kleuren en zoomweergaven. Als onderdeel van het maken en publiceren van media-elementen met Adobe Dynamic Media Classic, kunt u de effecten visueel configureren. Op deze manier maakt u de URL-aanroepen die de server correct vertellen hoe u uw primaire element aan toepassingen moet presenteren.

![Adobe Dynamic Media Classic kan dezelfde primaire afbeelding in verschillende formaten en formaten aan verschillende mediums leveren.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic zorgt ervoor dat consistente ervaringen met kwaliteit op elk scherm worden aangeboden, ongeacht de grootte of bandbreedte.*

## Inhoud in cache plaatsen {#content-caching}

De afbeeldingen die Adobe Dynamic Media Classic dynamisch genereert, zijn cachebestanden. doorgaans zijn het JPEG-afbeeldingen met unieke URL-aanroepen die ze identificeren. De beelden worden geleverd op het netwerk van de inhoudslevering (CDN), een systeem van servers die samen op Internet worden genetwerkt om inhoud sneller te leveren. De beelden worden verdeeld van servers globaal, en dan aan computers worden gevestigd. Wanneer u een cachemechanisme implementeert met een CDN-leverancier, wijzigt u gewoon de servernaam zodat deze naar de Dynamic Media Image Server met CDN-ondersteuning verwijst. Alle Adobe Dynamic Media Classic-edities bevatten gebundelde CDN-caching.
