---
title: 'Snel starten: Afbeeldingsgrootte'
description: Introductie en Snel starten naar afbeeldingsgrootte om u te helpen snel aan de slag te gaan met technieken voor afbeeldingsgrootte in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Snel starten: Afbeeldingsgrootte{#quick-start-image-sizing}

Afbeeldingsgrootte heeft betrekking op de mogelijkheid van Adobe Dynamic Media Classic om meerdere afgeleide afbeeldingen te maken op basis van één afbeelding met hoge resolutie. In plaats van handmatig meerdere afbeeldingen voor uw website of toepassing te maken, bijvoorbeeld een miniatuur en een afbeelding in een vergrote weergave, geeft u één primaire afbeelding op. Adobe Dynamic Media Classic genereert alle gewijzigde afbeeldingen op dezelfde manier als u ze vraagt. Het dynamisch leveren van afbeeldingen op basis van één primaire afbeelding heeft veel voordelen:

* Het is niet nodig handmatig meerdere exemplaren van de afbeelding van verschillende grootten te maken. U levert één primaire afbeelding aan Adobe Dynamic Media Classic en Adobe Dynamic Media Classic genereert derivaten van verschillende grootte van de primaire afbeelding.
* U kunt de grootte van een beeldtype door uw Website of toepassing snel veranderen. Als u bijvoorbeeld alle miniatuurafbeeldingen wilt wijzigen, kunt u de voorinstelling &quot;miniatuurafbeelding&quot; wijzigen. Een vooraf ingestelde afbeelding - Deze afbeelding lijkt op een macro-afbeelding en bestaat uit een verzameling kenmerken voor grootte en opmaak. U kunt de voorinstelling &quot;miniatuurafbeelding&quot; wijzigen om de grootte van alle miniatuurafbeeldingen te wijzigen in de hele website of toepassing.
* U hoeft de primaire bestanden en alle verschillende derivaten niet intern of extern te beheren in een van uw systemen voor inhoud- of middelenbeheer.

![ u kunt veelvoudige afgeleide beelden bij verschillende grootte van het zelfde high-resolution primaire dossier tot stand brengen.](/help/using/assets/is_derivative_sizes_popup.png)

Zie [ Beeld rangschikken: Dynamic Imaging ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) trainingsvideo.

De volgende snelstarthandleidingen voor Afbeeldingsgrootte zijn ontworpen om u te helpen snel aan de slag te gaan met technieken voor afbeeldingsgrootte in Adobe Dynamic Media Classic. Voer de stappen 1 tot en met 5 uit. Na elke stap is er een kruisverwijzing waar u meer informatie kunt vinden als u die nodig hebt.

## 1. primaire afbeeldingen uploaden

Begin door uw primaire afbeeldingen naar Adobe Dynamic Media Classic te uploaden. Wat de grootte betreft, raadt Adobe Dynamic Media Classic aan afbeeldingen te gebruiken die de grootste grootte hebben die u op uw website of toepassing wilt gebruiken. Als u bijvoorbeeld wilt dat gebruikers in- of uitzoomen op afbeeldingen, uploadt u afbeeldingen die minstens 2000 pixels groot zijn. Adobe Dynamic Media Classic ondersteunt veel bestandsindelingen voor afbeeldingen, maar TIFF- en PNG-afbeeldingen zonder gegevensverlies worden aanbevolen.

Selecteer op de algemene navigatiebalk **[!UICONTROL Upload]** om bestanden van uw computer te uploaden naar een map op Adobe Dynamic Media Classic. Zie [ primaire beelden ](uploading-master-images.md#uploading_master_images) uploaden.

## 2. Voorinstellingen afbeelding instellen

Net als bij een macro is een voorinstelling voor afbeeldingen een verzameling vooraf gedefinieerde opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met een voorinstelling voor afbeeldingen bepaalt u de grootte en opmaak van afbeeldingen die worden geleverd op Dynamic Media Image Servers. U kunt de Voorinstellingen van het opstellingsBeeld op uw plaatsen als u de status van de Beheerder van het Bedrijf hebt. U kunt dynamisch afbeeldingen leveren met de standaardvoorinstellingen voor afbeeldingen die al bij Adobe Dynamic Media Classic worden geleverd.

Ga op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Image Presets]** om een voorinstelling voor afbeeldingen te maken (als u een beheerder bent). Selecteer vervolgens **[!UICONTROL Add]** om een voorinstelling voor afbeeldingen te maken of selecteer **[!UICONTROL Edit]** om een bestaande voorinstelling voor afbeeldingen te wijzigen.

De voorinstelling Afbeelding die u maakt, wordt toegevoegd aan het menu Voorinstelling afbeelding op de pagina Voorvertoning. U kunt uw nieuwe Vooraf ingestelde Beeld gebruiken om beelden dynamisch op uw Websites en toepassingen te tonen. Zie [ Voorinstellingen van het Beeld van de Opstelling ](setting-image-presets.md#setting_up_image_presets).

## 3. Voorinstellingen voorvertoning afbeelding

In de volgende stap kunt u een voorvertoning weergeven van de voorinstellingen voor afbeeldingen die uw beheerder heeft ingesteld op verschillende vooraf ingestelde formaten.

Als u Voorinstellingen afbeelding wilt bekijken, gaat u op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** en bladert u naar een voorinstelling voor afbeeldingen.

Experimenteer met de verschillende voorinstellingen voor afbeeldingen. Kom te weten hoe uw beeld verschijnt wanneer het dynamisch aan uw Website of toepassing bij verschillende grootte wordt geleverd.

Zie [ Voorproef een beeldactiva die op zijn Vooraf ingesteld Beeld ](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset) wordt gebaseerd.

## 4. Publish uw primaire afbeeldingen

Het publiceren van uw primaire afbeeldingsbestanden heeft twee essentiële doelen:

* Uw primaire afbeeldingen publiceren naar Dynamic Media Image Servers zodat afbeeldingen dynamisch kunnen worden geleverd aan uw website en toepassing.
* Met Publiceren activeert u de URL-tekenreeksen voor het aanroepen van afbeeldingen van Dynamic Media Image Servers naar uw website of toepassing. Na publicatie kunt u waar nodig de door Adobe Dynamic Media Classic gegenereerde URL&#39;s kopiëren en plaatsen in uw website of toepassing.

Selecteer op de algemene navigatiebalk **[!UICONTROL Publish]** om een publicatietaak te starten. Selecteer **[!UICONTROL Submit Publish]** in het dialoogvenster Publiceren. Zie [ primaire beelden van Publish ](publishing-master-images.md#publishing_master_images).

## 5. Koppel URL&#39;s aan uw webtoepassing

Adobe Dynamic Media Classic maakt URL-bijschrifttekenreeksen voor afbeeldingen. Wanneer u afbeeldingen publiceert naar Dynamic Media Image Servers, worden de URL&#39;s actief. U kunt deze URL-tekenreeksen kopiëren vanuit het deelvenster Bladeren (in de gedetailleerde weergave) of het scherm Voorvertoning. Nadat u de koorden URL kopieert, kunt u hen in uw Website en toepassingen gebruiken. De URL voor Afbeeldingsgrootte vervangt de verwijzing naar een statische beeldnaam in uw code van de Web-pagina. De URL verwijst naar een primaire afbeeldingsnaam die de database vervangt voor elke nieuwe afbeelding die moet worden weergegeven.

URL-tekenreeksen die zijn gegenereerd met Voorinstellingen afbeelding bevatten de naam van een voorinstelling voor afbeeldingen. Deze naam is ingesloten in dollartekens (`$`). `$thumbnail$` kan bijvoorbeeld de voorinstelling Afbeelding zijn die is ontworpen om primaire afbeeldingen met een miniatuurgrootte weer te geven. Zie [ Verbinding URLs aan uw toepassing van het Web ](linking-urls-web-application.md#linking_urls_to_your_web_application).
