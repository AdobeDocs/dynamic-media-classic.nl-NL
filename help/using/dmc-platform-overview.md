---
title: Overzicht van Adobe Dynamic Media Classic-programma
description: Een overzicht van het Adobe Dynamic Media Classic-programma en het gehele workflowproces.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Overzicht van Adobe Dynamic Media Classic-programma{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic is een geïntegreerde, rijke omgeving voor mediabeheer, -publicatie en -services. Rijke media kunnen aan alle marketing en verkoopkanalen worden geleverd. Deze kanalen omvatten het Web, drukmateriaal, e-mailcampagnes, portals van het Web, Desktops, en apparaten.

Zie ook [&#x200B; het overzicht van het Platform &#x200B;](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) opleidingsvideo.

## Workflowproces {#workflow-process}

De belangrijkste Adobe Dynamic Media Classic-workflowstappen zijn:

* **uploadt en beheert uw activa**: Upload uw media activa aan Adobe Dynamic Media Classic. U kunt middelen op het systeem organiseren, doorbladeren en zoeken. U kunt ook metagegevens toepassen op elementen.

* **creeer rijke media**: Creeer verschillende configuraties van uw activa zoals eCatalogs, de Reeksen van het Beeld, de Reeksen van de Rotatie, de Reeksen van het Monster, Gemengde Reeksen van Media, basisMalplaatjes, en Malplaatjes FXG.

* **publiceer en beheer**: Publiceer activa aan het netwerk van Adobe Dynamic Media Classic SaaS. De status van elementen controleren wanneer deze worden gepubliceerd. Gebruikersrechten beheren en de beveiliging handhaven.

* **Server**: Lever media van het netwerk van Adobe Dynamic Media Classic SaaS aan Web-pagina&#39;s, toepassingen, en mobiele apparaten; de media zijn prestaties-geoptimaliseerd en met CDN caching geleverd. Adobe Dynamic Media Classic biedt u een URL voor elk element. Nadat u het element hebt gepubliceerd, wordt de URL actief.

![&#x200B; het het werkschemaproces van Adobe Dynamic Media Classic &#x200B;](/help/using/assets/gs_workflow.png)

## Eén primaire afbeelding en één URL-aanroep {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic is fundamenteel anders dan andere systemen, omdat u Adobe Dynamic Media Classic kunt gebruiken om media dynamisch te leveren vanaf enkele primaire elementen en URL-aanroepen.

De URL-tekenreeksen die u met Adobe Dynamic Media Classic hebt gegenereerd, bevatten instructies die de server vertellen hoe het element moet worden weergegeven wanneer het wordt geleverd. Dezelfde primaire afbeelding kan bijvoorbeeld worden geleverd in verschillende formaten, formaten, gewichten, kleuren en zoomweergaven. Als onderdeel van het maken en publiceren van media-elementen met Adobe Dynamic Media Classic, kunt u de effecten visueel configureren. Hierbij maakt u de URL-aanroepen die de server correct vertellen hoe u uw primaire element aan toepassingen moet presenteren.

![&#x200B; Adobe Dynamic Media Classic kan het zelfde primaire beeld aan verschillende media in verschillende grootte en formaten leveren.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic zorgt ervoor dat de verenigbare, kwaliteitservaringen aan om het even welk scherm, ongeacht grootte of bandbreedte worden geleverd.*

## Inhoud in cache plaatsen {#content-caching}

De afbeeldingen die Adobe Dynamic Media Classic dynamisch genereert, zijn cachebestanden. Dit zijn doorgaans JPEG-afbeeldingen met unieke URL-aanroepen die ze identificeren. De beelden worden geleverd op het netwerk van de inhoudslevering (CDN), een systeem van servers die samen op Internet worden genetwerkt om inhoud sneller te leveren. De beelden worden verdeeld van servers globaal, en dan aan computers worden gevestigd. Wanneer het uitvoeren van een caching mechanisme gebruikend om het even welke verkoper CDN, verandert u eenvoudig de servernaam om naar de CDN-Toegelaten Dynamische Server van het Beeld van Media te richten. Alle Adobe Dynamic Media Classic-edities bevatten gebundelde CDN-caching.
