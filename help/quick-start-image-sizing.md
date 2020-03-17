---
title: '"Snel starten: Afbeeldingsgrootte"'
seo-title: '"Snel starten: Afbeeldingsgrootte"'
description: 'null'
seo-description: Een inleiding en Snel aan de Grootte van het Beeld beginnen om u te helpen snel met de technieken van de Grootte van het Beeld aan de slag gaan.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Snel starten: Afbeeldingsgrootte{#quick-start-image-sizing}

Afbeeldingsgrootte heeft betrekking op de mogelijkheid van Dynamic Media Classic om meerdere afgeleide afbeeldingen te maken op basis van één afbeelding met hoge resolutie. In plaats van handmatig meerdere afbeeldingen voor uw website of toepassing te maken, bijvoorbeeld een miniatuur en een afbeelding in een vergrote weergave, geeft u één hoofdafbeelding op. Met Dynamic Media Classic worden alle gewijzigde afbeeldingen op dezelfde manier gegenereerd als u ze aanvraagt. Het dynamisch leveren van afbeeldingen op basis van één hoofdafbeelding heeft veel voordelen:

* U hoeft niet handmatig meerdere exemplaren van de afbeelding met verschillende grootten te maken. U levert één hoofdafbeelding aan Dynamic Media Classic en Dynamic Media Classic genereert derivaten van verschillende grootte van de hoofdafbeelding.
* U kunt de grootte van een afbeeldingstype snel wijzigen op uw website of in de toepassing. Als u bijvoorbeeld alle miniatuurafbeeldingen wilt wijzigen, kunt u de voorinstelling &quot;miniatuurafbeelding&quot; wijzigen. Een voorinstelling voor afbeeldingen, die lijkt op een macro, is een verzameling kenmerken voor grootte en opmaak. U kunt de voorinstelling &quot;miniatuurafbeelding&quot; wijzigen om de grootte van alle miniatuurafbeeldingen te wijzigen op de hele website of in de toepassing.
* U hoeft de stramienen en alle verschillende derivaten niet intern of extern te beheren in een van uw systemen voor inhoud of middelenbeheer.

![U kunt meerdere afgeleide afbeeldingen maken met verschillende grootten van hetzelfde hoofdbestand met hoge resolutie.](/help/assets/is_derivative_sizes_popup.png)

**Snel starten**

Dit Beeld dat Snel Begin rangschikt van het Beeld wordt ontworpen om u te helpen snel met de technieken van de Grootte van het Beeld in het het Publiceren Scene7 Systeem opduiken. Voer de stappen 1 tot en met 5 uit. Na elke stap is een kruisverwijzing waar u meer informatie kunt vinden als u die nodig hebt.

**1. Stramienafbeeldingen uploaden**

Begin door uw hoofdbeelden aan het het Publiceren Scene7 Systeem te uploaden. Met betrekking tot de grootte raadt Dynamic Media Classic u aan afbeeldingen te gebruiken die de grootst mogelijke grootte hebben die u op uw website of toepassing wilt gebruiken. Als u bijvoorbeeld wilt dat gebruikers in- of uitzoomen op afbeeldingen, uploadt u afbeeldingen die minstens 2000 pixels groot zijn. Dynamic Media Classic ondersteunt veel bestandsindelingen voor afbeeldingen, maar het wordt aanbevolen afbeeldingen zonder verlies in de indeling TIFF en PNG te gebruiken.

Selecteer de Upload knoop op de Globale bar van de Navigatie om dossiers van uw computer aan een omslag op het het Publiceren Scene7 Systeem te uploaden. Zie [Stramienafbeeldingen](uploading-master-images.md#uploading_master_images)uploaden.

**2. Voorinstellingen afbeelding instellen**

Net als bij een macro is een voorinstelling voor afbeeldingen een verzameling vooraf gedefinieerde opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met een voorinstelling voor afbeeldingen bepaalt u de grootte en de opmaak van de afbeeldingen die worden geleverd op de dynamische mediageleveranciers. U kunt de Voorinstellingen van het beeld op uw plaatsen als u de status van de bedrijfbeheerder hebt. Dynamic Media Classic wordt ook geleverd met standaardvoorinstellingen voor afbeeldingen en u kunt deze gebruiken om afbeeldingen dynamisch te leveren.

Als u een voorinstelling voor afbeeldingen wilt maken (als u een beheerder bent), kiest u Instellen > Toepassing instellen. Voor het scherm van de Opstelling, toon de opties van de Opstelling van de Toepassing en kies Beeld vooraf instelt. Klik vervolgens op **Toevoegen** of **Bewerken** om een voorinstelling voor afbeeldingen te maken.

De voorinstelling Afbeelding die u maakt, wordt toegevoegd aan het menu Voorinstelling afbeelding in het voorvertoningsscherm. Met de nieuwe voorinstelling voor afbeeldingen kunt u afbeeldingen dynamisch weergeven op uw websites en toepassingen. Zie [Voorinstellingen](setting-image-presets.md#setting_up_image_presets)afbeelding instellen.

**3. Voorinstellingen afbeelding voorvertonen**

In de volgende stap kunt u een voorvertoning weergeven van de voorinstellingen voor afbeeldingen die uw beheerder heeft ingesteld op verschillende vooraf ingestelde formaten.

Als u Voorinstellingen afbeelding wilt bekijken, klikt u op **Instellingen** > Voorinstellingen **afbeelding** en bladert u naar een voorinstelling voor afbeeldingen.

Experimenteer met de verschillende voorinstellingen voor afbeeldingen. Bekijk hoe de afbeelding eruitziet als deze dynamisch bij verschillende grootten wordt geleverd aan uw website of toepassing.

Zie Een [voorvertoning weergeven van een afbeeldingselement op basis van de voorinstelling](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)voor afbeeldingen.

**4. Stramienafbeeldingen publiceren**

Het publiceren van uw hoofdafbeeldingsbestanden heeft twee essentiële doelen:

* Uw hoofdafbeeldingen publiceren naar Dynamic Media Image Servers, zodat afbeeldingen dynamisch kunnen worden geleverd aan uw website en toepassing.
* Met Publiceren activeert u de URL-tekenreeksen voor het aanroepen van afbeeldingen van Dynamic Media Image Servers naar uw website of toepassing. Na publicatie kunt u waar nodig de door Dynamic Media Classic gegenereerde URL&#39;s kopiëren en plaatsen op uw website of toepassing.

Selecteer de knop Publiceren op de algemene navigatiebalk om een publicatie te starten. Selecteer in het scherm Publiceren de knop Publiceren starten. Zie Stramienafbeeldingen [](publishing-master-images.md#publishing_master_images)publiceren.

**5. URL&#39;s koppelen aan uw webtoepassing**

Met Dynamic Media Classic worden URL-bijschrifttekenreeksen voor afbeeldingen gemaakt. Wanneer u afbeeldingen publiceert naar Dynamic Media Image Servers, worden de URL&#39;s actief. U kunt deze URL-tekenreeksen kopiëren vanuit het deelvenster Bladeren (in de gedetailleerde weergave) of het scherm Voorvertoning. Nadat u de URL-tekenreeksen hebt gekopieerd, kunt u deze gebruiken in uw website en toepassingen. De URL voor afbeeldingsgrootte vervangt de verwijzing naar een statische afbeeldingsnaam in de webpaginacode. De URL verwijst naar de naam van een hoofdafbeelding, die door de database wordt vervangen voor elke nieuwe afbeelding die moet worden weergegeven.

URL-tekenreeksen die zijn gegenereerd met Voorinstellingen afbeelding bevatten de naam van een voorinstelling voor afbeeldingen. Deze naam staat in dollartekens (`$`). Dit `$thumbnail$` kan bijvoorbeeld de voorinstelling Afbeelding zijn die is ontworpen om stramienafbeeldingen met een miniatuurgrootte weer te geven. Zie URL&#39;s [koppelen aan uw webtoepassing](linking-urls-web-application.md#linking_urls_to_your_web_application).
