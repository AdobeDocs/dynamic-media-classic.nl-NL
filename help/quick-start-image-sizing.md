---
title: '"Snel starten: Afbeeldingsgrootte"'
description: Een inleiding en Snel aan de Grootte van het Beeld beginnen om u te helpen snel met de technieken van de Grootte van het Beeld aan de slag gaan.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic, beheer van bedrijfsmiddelen
role: Business Practitioner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Snel starten: Afbeeldingsgrootte{#quick-start-image-sizing}

Afbeeldingsgrootte heeft betrekking op de mogelijkheid van Dynamic Media Classic om meerdere afgeleide afbeeldingen te maken op basis van één afbeelding met hoge resolutie. In plaats van handmatig meerdere afbeeldingen voor uw website of toepassing te maken, bijvoorbeeld een miniatuur en een afbeelding in een vergrote weergave, geeft u één master afbeelding op. Dynamic Media Classic genereert alle gewijzigde afbeeldingen op dezelfde manier als u ze aanvraagt. Het dynamisch leveren van afbeeldingen op basis van één master afbeelding heeft veel voordelen:

* U hoeft niet handmatig meerdere exemplaren van de afbeelding met verschillende grootten te maken. U levert één master afbeelding aan Dynamic Media Classic en Dynamic Media Classic genereert derivaten van verschillende grootte van de master afbeelding.
* U kunt de grootte van een afbeeldingstype snel wijzigen op uw website of in de toepassing. Als u bijvoorbeeld alle miniatuurafbeeldingen wilt wijzigen, kunt u de voorinstelling &quot;miniatuurafbeelding&quot; wijzigen. Een voorinstelling voor afbeeldingen, die lijkt op een macro, is een verzameling kenmerken voor grootte en opmaak. U kunt de voorinstelling &quot;miniatuurafbeelding&quot; wijzigen om de grootte van alle miniatuurafbeeldingen te wijzigen op de hele website of in de toepassing.
* U hoeft de stramienen en alle verschillende derivaten niet intern of extern te beheren in een van uw systemen voor inhoud of middelenbeheer.

![U kunt meerdere afgeleide afbeeldingen maken met een verschillende grootte en hetzelfde master bestand met hoge resolutie.](/help/assets/is_derivative_sizes_popup.png)

Deze Snel starten met afbeeldingsgrootte is ontworpen om u te helpen snel aan de slag te gaan met technieken voor afbeeldingsgrootte in Dynamic Media Classic. Voer de stappen 1 tot en met 5 uit. Na elke stap is een kruisverwijzing waar u meer informatie kunt vinden als u die nodig hebt.

## 1. Master afbeeldingen uploaden

Begin door uw master afbeeldingen te uploaden naar Dynamic Media Classic. Wat de grootte betreft, raadt Dynamic Media Classic u aan afbeeldingen te gebruiken van het grootste formaat dat u op uw website of toepassing wilt gebruiken. Als u bijvoorbeeld wilt dat gebruikers in- of uitzoomen op afbeeldingen, uploadt u afbeeldingen die minstens 2000 pixels groot zijn. Dynamic Media Classic biedt ondersteuning voor veel bestandsindelingen voor afbeeldingen, maar het wordt aanbevolen afbeeldingen zonder verlies in de indeling TIFF en PNG te gebruiken.

Klik op de algemene navigatiebalk op **[!UICONTROL Upload]** om bestanden van uw computer te uploaden naar een map op Dynamic Media Classic. Zie [master afbeeldingen uploaden](uploading-master-images.md#uploading_master_images).

## 2. Voorinstellingen afbeelding instellen

Net als bij een macro is een voorinstelling voor afbeeldingen een verzameling vooraf gedefinieerde opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met een voorinstelling voor afbeeldingen bepaalt u de grootte en opmaak van afbeeldingen die worden geleverd op Dynamic Media Image Servers. U kunt de Voorinstellingen van het beeld op uw plaatsen als u de status van de bedrijfbeheerder hebt. Dynamic Media Classic wordt ook geleverd met standaardvoorinstellingen voor afbeeldingen en u kunt deze gebruiken om afbeeldingen dynamisch te leveren.

Als u een voorinstelling voor afbeeldingen wilt maken (als u een beheerder bent), klikt u op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Image Presets]** op de algemene navigatiebalk. Klik vervolgens op **[!UICONTROL Add]** om een voorinstelling voor afbeeldingen te maken of klik op **[!UICONTROL Edit]** om een bestaande voorinstelling voor afbeeldingen te wijzigen.

De voorinstelling Afbeelding die u maakt, wordt toegevoegd aan het menu Voorinstelling afbeelding op de pagina Voorvertoning. Met de nieuwe voorinstelling voor afbeeldingen kunt u afbeeldingen dynamisch weergeven op uw websites en toepassingen. Zie [Voorinstellingen voor afbeeldingen instellen](setting-image-presets.md#setting_up_image_presets).

## 3. Voorinstellingen afbeelding voorvertonen

In de volgende stap kunt u een voorvertoning weergeven van de voorinstellingen voor afbeeldingen die uw beheerder heeft ingesteld op verschillende vooraf ingestelde formaten.

Als u Voorinstellingen afbeelding wilt bekijken, klikt u op **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** op de algemene navigatiebalk en bladert u naar een voorinstelling voor afbeeldingen.

Experimenteer met de verschillende voorinstellingen voor afbeeldingen. Ontdek hoe uw afbeelding eruitziet wanneer deze dynamisch bij verschillende formaten wordt geleverd aan uw website of toepassing.

Zie [Een voorvertoning weergeven van een afbeeldingselement op basis van de voorinstelling voor afbeelding](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Master afbeeldingen publiceren

Het publiceren van master afbeeldingsbestanden heeft twee essentiële doelen:

* Uw master afbeeldingen publiceren naar Dynamic Media Image Servers (Image Servers), zodat afbeeldingen dynamisch kunnen worden geleverd aan uw website en toepassing.
* Met Publiceren activeert u de URL-tekenreeksen voor het aanroepen van afbeeldingen van Dynamic Media Image Servers naar uw website of toepassing. Na publicatie kunt u waar nodig de door Dynamic Media gegenereerde klassieke URL&#39;s kopiëren en plaatsen op uw website of toepassing.

Klik op **[!UICONTROL Publish]** op de algemene navigatiebalk om een publicatietaak te starten. Klik in het dialoogvenster Publiceren op **[!UICONTROL Submit Publish]**. Zie [master afbeeldingen publiceren](publishing-master-images.md#publishing_master_images).

## 5. URL&#39;s koppelen aan uw webtoepassing

Dynamic Media Classic maakt URL-callouttekenreeksen voor afbeeldingen. Wanneer u afbeeldingen publiceert naar Dynamic Media Image Servers, worden de URL&#39;s actief. U kunt deze URL-tekenreeksen kopiëren vanuit het deelvenster Bladeren (in de gedetailleerde weergave) of het scherm Voorvertoning. Nadat u de URL-tekenreeksen hebt gekopieerd, kunt u deze gebruiken in uw website en toepassingen. De URL voor afbeeldingsgrootte vervangt de verwijzing naar een statische afbeeldingsnaam in de webpaginacode. De URL verwijst naar een master afbeeldingsnaam die door de database wordt vervangen voor elke nieuwe afbeelding die moet worden weergegeven.

URL-tekenreeksen die zijn gegenereerd met Voorinstellingen afbeelding bevatten de naam van een voorinstelling voor afbeeldingen. Deze naam staat in dollartekens (`$`). `$thumbnail$` kan bijvoorbeeld de voorinstelling Afbeelding zijn die is ontworpen om master afbeeldingen met miniatuurgrootte weer te geven. Zie [URL&#39;s koppelen aan uw webtoepassing](linking-urls-web-application.md#linking_urls_to_your_web_application).
