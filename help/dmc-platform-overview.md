---
title: Overzicht van Adobe Dynamic Media Classic-platform
seo-title: Overzicht van Adobe Dynamic Media Classic-platform
description: 'null'
seo-description: Een overzicht van het Dynamic Media Classic platform en workflowproces.
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


# Overzicht van Adobe Dynamic Media Classic-platform{#adobe-scene-platform-overview}

Dynamic Media Classic is een geïntegreerde, rijke media beheer, het publiceren, en het dienen milieu. De rijke media kunnen aan alle marketing en verkoopkanalen, met inbegrip van het Web, drukmateriaal, e-mailcampagnes, Webportals, Desktops, en apparaten worden geleverd.

## Workflowproces {#workflow-process}

De belangrijkste Dynamic Media Klassieke workflowstappen zijn:

* **Upload en beheer uw elementen** Upload uw media-elementen naar Dynamic Media Classic. U kunt middelen op het systeem organiseren, doorbladeren en zoeken. U kunt ook metagegevens toepassen op elementen.

* **Creeer rijke media** creeer verschillende configuraties van uw activa zoals eCatalogi, de Reeksen van het Beeld, de Reeksen van de Draai, de Reeksen van het Monster, Gemengde Reeksen van Media, basisMalplaatjes, en Malplaatjes FXG. Zie Informatie over rijke media voor meer informatie.

* **Publiceer en beheer** publiceer activa aan het Netwerk van de Klassieke Saas van Dynamic Media, evenals controleer het statuut van activa wanneer zij worden gepubliceerd, beheer gebruikersrechten, en handhaaf veiligheid.

* **Media leveren** van Dynamic Media Classic SaaS-netwerk naar webpagina&#39;s, toepassingen en mobiele apparaten; de media zijn geoptimaliseerd voor prestaties en worden geleverd met CDN-caching. Dynamic Media Classic biedt u een URL voor elk element. Nadat u het element hebt gepubliceerd, wordt de URL actief.

![Het klassieke workflowproces Dynamic Media](/help/assets/gs_workflow.png)

## Enkele master afbeeldingen en enkele URL-aanroepen {#single-master-images-and-single-url-calls}

Klassieke Dynamic Media is fundamenteel verschillend van andere systemen omdat u Dynamic Media Klassiek kunt gebruiken om media van enige master activa en vraag dynamisch te leveren URL.

De URL-tekenreeksen die u genereert met Dynamic Media Classic bevatten instructies die de server vertellen hoe het element moet worden weergegeven wanneer het wordt geleverd. Dezelfde master afbeelding kan bijvoorbeeld worden geleverd in verschillende formaten, formaten, gewichten, kleuren en zoomweergaven. Als onderdeel van het bouwen van en het publiceren van media activa met Dynamic Media Klassiek, vormt u visueel de gevolgen. Op deze manier maakt u de URL-aanroepen die de server correct vertellen hoe u uw master element aan toepassingen moet presenteren.

![Met Dynamic Media Classic kunt u dezelfde master afbeelding leveren aan verschillende media in verschillende formaten en formaten.](/help/assets/gs_dynamic_publishing.png)

## Inhoud in cache plaatsen {#content-caching}

De beelden die de Klassieke Dynamic Media dynamisch produceren zijn geheim voorgeheugenvriendelijk; in de meeste gevallen zijn het JPEG-afbeeldingen met unieke URL-aanroepen die ze identificeren. De beelden worden geleverd op het netwerk van de inhoudslevering (CDN), een systeem van servers die samen op Internet worden genetwerkt om inhoud sneller te leveren. De beelden worden verdeeld van servers globaal, en dan aan computers worden gevestigd. Wanneer het uitvoeren van een caching mechanisme gebruikend om het even welke verkoper CDN, verandert u eenvoudig de servernaam om naar de CDN-Toegelaten Server van het Beeld van Dynamic Media te richten. Alle Dynamic Media Klassieke edities bevatten gebundelde CDN-caching.
