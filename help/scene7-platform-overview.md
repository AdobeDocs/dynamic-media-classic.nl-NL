---
title: Overzicht van het Adobe Dynamic Media Classic-platform
seo-title: Overzicht van het Adobe Dynamic Media Classic-platform
description: 'null'
seo-description: Een overzicht van het Dynamic Media Classic-platform en workflowproces.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Overzicht van het Adobe Dynamic Media Classic-platform{#adobe-scene-platform-overview}

Dynamic Media Classic is een geïntegreerde, rijke omgeving voor mediabeheer, publicaties en het bedienen van omgevingen. De rijke media kunnen aan alle marketing en verkoopkanalen, met inbegrip van het Web, drukmateriaal, e-mailcampagnes, Webportals, Desktops, en apparaten worden geleverd.

## Workflowproces {#workflow-process}

De belangrijkste stappen in de dynamische Klassieke workflow van Media zijn:

* **Upload en beheer uw elementen** Upload uw media-elementen naar SPS. U kunt middelen op het systeem organiseren, doorbladeren en zoeken. U kunt ook metagegevens toepassen op elementen. Als u de Desktoptoepassing van het Publiceren van het Systeem van Adobe Scene7 installeert, kunt u dossiers en omslagen uploaden door hen van uw Desktop aan een upload omslag te slepen.

* **Creeer rijke media** creeer verschillende configuraties van uw activa zoals eCatalogi, de Reeksen van het Beeld, de Reeksen van de Draai, de Reeksen van het Monster, Gemengde Reeksen van Media, basisMalplaatjes, en Malplaatjes FXG. Zie Informatie over rijke media voor meer informatie.

* **Publiceer en beheer** publiceer activa aan het Dynamische Netwerk van de Klassieke Saas van Media, evenals controleer de status van activa wanneer zij worden gepubliceerd, beheer gebruikersrechten, en handhaaf veiligheid.

* **Media van Dynamic Media Classic SaaS-netwerk** leveren aan webpagina&#39;s, toepassingen en mobiele apparaten; de media zijn geoptimaliseerd voor prestaties en worden geleverd met CDN-caching. Dynamic Media Classic biedt u een URL voor elk element. Nadat u het element hebt gepubliceerd, wordt de URL actief.

![Het dynamische Klassieke werkschemaproces van Media](/help/assets/gs_workflow.png)

## Enkele hoofdafbeeldingen en enkele URL-aanroepen {#single-master-images-and-single-url-calls}

Dynamic Media Classic is fundamenteel anders dan andere systemen, omdat u met Dynamic Media Classic media media dynamisch media kunt leveren op basis van enkelvoudige hoofdelementen en URL-aanroepen.

De URL-tekenreeksen die u genereert met Dynamic Media Classic bevatten instructies die de server vertellen hoe het element moet worden weergegeven wanneer het wordt geleverd. Dezelfde hoofdafbeelding kan bijvoorbeeld worden geleverd in verschillende formaten, indelingen, gewichten, kleuren en zoomweergaven. Als onderdeel van het bouwen en publiceren van media activa met Dynamische Klassieke Media, vormt u visueel de gevolgen. Op deze manier maakt u de URL-aanroepen die de server correct vertellen hoe u het hoofdelement aan toepassingen moet presenteren.

![Dynamic Media Classic kan dezelfde hoofdafbeelding leveren aan verschillende media in verschillende formaten en formaten.](/help/assets/gs_dynamic_publishing.png)

## Inhoud in cache plaatsen {#content-caching}

De beelden die de Dynamische Klassiek van Media dynamisch produceren zijn geheim voorgeheugen-vriendelijk; in de meeste gevallen zijn het JPEG-afbeeldingen met unieke URL-aanroepen die ze identificeren. De beelden worden geleverd op het netwerk van de inhoudslevering (CDN), een systeem van servers die samen op Internet worden genetwerkt om inhoud sneller te leveren. De beelden worden verdeeld van servers globaal, en dan aan computers worden gevestigd. Wanneer het uitvoeren van een caching mechanisme gebruikend om het even welke verkoper CDN, verandert u eenvoudig de servernaam om naar de CDN-Toegelaten Dynamische Server van het Beeld van Media te richten. Alle dynamische media Klassieke edities bevatten gebundelde CDN-caching.
