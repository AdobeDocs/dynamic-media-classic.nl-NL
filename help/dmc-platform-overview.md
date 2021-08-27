---
title: Overzicht van Adobe Dynamic Media Classic-programma
description: Een overzicht van het Klassieke Adobe Dynamic Media-programma en workflowproces.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Overzicht van Adobe Dynamic Media Classic-programma{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic is een geïntegreerde, rijke omgeving voor mediabeheer, -publicatie en -gebruik. De rijke media kunnen aan alle marketing en verkoopkanalen, met inbegrip van het Web, drukmateriaal, e-mailcampagnes, Webportals, Desktops, en apparaten worden geleverd.

## Workflowproces {#workflow-process}

De belangrijkste Adobe Dynamic Media Classic workflowstappen zijn:

* **Upload en beheer uw middelen**  - Upload uw media-elementen naar Adobe Dynamic Media Classic. U kunt middelen op het systeem organiseren, doorbladeren en zoeken. U kunt ook metagegevens toepassen op elementen.

* **Rijke media**  maken - verschillende configuraties van uw elementen maken, zoals eCatalogi, Afbeeldingssets, Draaisets, Staalsets, Gemengde Mediasets, Standaardsjablonen en FXG-sjablonen.

* **Publiceer en beheer**  - publiceer activa aan het Adobe Dynamic Media Klassieke netwerk SaaS, evenals controleer het statuut van activa wanneer zij worden gepubliceerd, beheer gebruikersrechten, en handhaaf veiligheid.

* **server** - media leveren van het Klassieke SaaS netwerk van Adobe Dynamic Media aan Web-pagina&#39;s, toepassingen, en mobiele apparaten; de media zijn geoptimaliseerd voor prestaties en worden geleverd met CDN-caching. Adobe Dynamic Media Classic biedt u een URL voor elk element. Nadat u het element hebt gepubliceerd, wordt de URL actief.

![Het Classic-workflowproces van Adobe Dynamic Media](/help/assets/gs_workflow.png)

## Enkele master afbeeldingen en enkele URL-aanroepen {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic is fundamenteel anders dan andere systemen omdat u Adobe Dynamic Media Classic kunt gebruiken om media dynamisch te leveren vanaf één master element en URL-aanroepen.

De URL-tekenreeksen die u genereert met Adobe Dynamic Media Classic bevatten instructies die de server vertellen hoe het element moet worden weergegeven wanneer het wordt geleverd. Dezelfde master afbeelding kan bijvoorbeeld worden geleverd in verschillende formaten, formaten, gewichten, kleuren en zoomweergaven. Als onderdeel van het bouwen en publiceren van media activa met Adobe Dynamic Media Klassiek, vormt u visueel de gevolgen. Op deze manier maakt u de URL-aanroepen die de server correct vertellen hoe u uw master element aan toepassingen moet presenteren.

![Adobe Dynamic Media Classic kan dezelfde master afbeelding leveren aan verschillende media in verschillende formaten en formaten.](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic zorgt ervoor dat consistente ervaringen met kwaliteit op elk scherm worden aangeboden, ongeacht de grootte of bandbreedte.*

## Inhoud in cache plaatsen {#content-caching}

De afbeeldingen die Adobe Dynamic Media Classic dynamisch genereert, zijn cachegvriendelijk. doorgaans zijn het JPEG-afbeeldingen met unieke URL-aanroepen die ze identificeren. De beelden worden geleverd op het netwerk van de inhoudslevering (CDN), een systeem van servers die samen op Internet worden genetwerkt om inhoud sneller te leveren. De beelden worden verdeeld van servers globaal, en dan aan computers worden gevestigd. Wanneer u een cachemechanisme implementeert met een CDN-leverancier, wijzigt u gewoon de servernaam zodat deze naar de Dynamic Media Image Server met CDN-ondersteuning verwijst. Alle Adobe Dynamic Media Classic-edities bevatten gebundelde CDN-caching.
