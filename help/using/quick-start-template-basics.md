---
title: "Snel starten: Sjabloonbasiskennis"
description: Een inleiding en Snel aan de Basisprincipes van het Malplaatje helpen u in Adobe Dynamic Media Classic opstaan en snel in werking stellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Snel starten: Sjabloonbasisbeginselen{#quick-start-template-basics}

De basis van sjablonen wordt dynamisch gemaakt en adresseerbare gelaagde afbeeldingsbestanden, zoals gelaagde bestanden, in beeldbewerkingstoepassingen zoals Adobe Photoshop. In tegenstelling tot een statisch bestand met lagen, zoals een PSD-bestand, kan een sjabloon parameters bevatten. Aan de hand van parameters kunnen de verschillende aspecten van de afbeelding worden benaderd en aangepast.

Een sjabloon kan een willekeurig aantal afbeeldingslagen en tekstlagen bevatten. U kunt een statisch bestand met lagen, zoals een gelaagd PSD-bestand, omzetten naar een sjabloon en sjablonen maken in Adobe Dynamic Media Classic. U kunt tekstlagen in sjablonen maken met lettertypen die u naar Adobe Dynamic Media Classic hebt geüpload. Nadat u tekst aan een sjabloon hebt toegevoegd, kunt u deze opmaken door de uitvulling, het lettertype, de tekengrootte en de kleur ervan te wijzigen.

Met de pagina Parameters kunt u elk aspect van een sjabloon omzetten in een adresseerbare parameter. Zo kunt u wijzigen welke gelaagde afbeelding u wilt gebruiken of welke tekstwaarde u in de sjabloon wilt gebruiken. De parameters worden overgegaan met het koord URL, toestaand u om het even welke parameter te veranderen om het antwoordbeeld dynamisch aan te passen dat van de Server van het Beeld wordt geproduceerd.

Zie ook [Grondbeginselen van sjablonen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) trainingsvideo.

Deze snelle start is ontworpen om u snel aan de slag te krijgen met de basis van sjablonen.

## 1. De bestanden uploaden

Begin door het PSD- of afbeeldingsbestand voor uw sjabloon te uploaden. Adobe Dynamic Media Classic biedt naast PSD ook ondersteuning voor veel bestandsindelingen voor afbeeldingen, maar TIFF- en PNG-afbeeldingen zonder gegevensverlies worden aanbevolen voor sjablonen omdat ze transparantie mogelijk maken.

Als u een PSD-bestand gebruikt om uw sjabloon te maken, selecteert u **[!UICONTROL Create Template]** op de **[!UICONTROL Upload Job Options]** wanneer u het PSD-bestand uploadt. Kies ook een **[!UICONTROL Layer Naming]** zodat Adobe Dynamic Media Classic weet hoe PSD-lagen een naam moeten krijgen wanneer ze naar Adobe Dynamic Media Classic worden geüpload.

Als u afbeeldingsbestanden gebruikt, kunt u de afbeeldingen uitsnijden en ook een masker maken van uitknippaden in de afbeeldingen wanneer u deze uploadt.

Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Upload]** om een PSD-bestand of andere afbeeldingsbestanden vanaf uw computer te uploaden naar een map op Adobe Dynamic Media Classic. Zie [Sjabloonbestanden uploaden](uploading-template-files.md#uploading_template_files).

## 2. Een sjabloon maken

Als u een sjabloon wilt maken van een PSD-bestand, selecteert u **[!UICONTROL Create Template]** wanneer u het bestand uploadt. Als u een sjabloon wilt maken van afbeeldingen, gaat u op de algemene navigatiebalk naar **[!UICONTROL Build]** > **[!UICONTROL Template Basics]** voert u een breedte- en hoogtemeting voor het canvas in. Selecteer in de rechterbovenhoek van de pagina een van de **[!UICONTROL Designer]** of **[!UICONTROL Developer]** en sleep afbeeldingen naar de sjabloonpagina. U kunt ook de afbeeldingen selecteren *voor* ga naar **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. De sjabloonpagina bevat gereedschappen voor:

* Afbeeldingslagen toevoegen. Als u een laag wilt toevoegen, sleept u een afbeelding naar de sjabloonpagina.
* Tekstlagen toevoegen. Selecteer de **[!UICONTROL Text tool]** pictogram. Sleep de aanwijzer om een vak voor de tekstlaag te maken en maak de tekst vervolgens op met gereedschappen op de tekstpagina.
* De grootte en positie van lagen wijzigen.
* De volgorde van lagen wijzigen.
* Schaduw- en gloedeffecten toepassen op afbeeldings- en tekstlagen.

Zie [Een sjabloon maken](creating-template.md#creating_a_template).

## 3. Sjabloonparameters maken

De volgende stap bestaat uit het bepalen van de parameters van de eigenschappen op lagen om te bepalen welke laageigenschappen in het koord URL inbegrepen zijn. De parameters staan u toe om malplaatjes met maximumflexibiliteit te gebruiken. Nadat u een laageigenschap in een parameter hebt gemaakt, kunt u deze dynamisch wijzigen.

Als u parameters wilt opgeven voor een laag, opent u de sjabloon in de sjabloonpagina en selecteert u **[!UICONTROL Parameters]** naast een laagnaam. Selecteer op de pagina Parameters de optie naast elke parameter die u wilt toevoegen. Zie [Sjabloonparameters maken](creating-template-parameters.md#creating_template_parameters).

## 4. Sjablonen publiceren

Als u uw sjabloon publiceert, wordt deze op Dynamic Media Image Servers geplaatst, zodat deze dynamisch aan uw website of toepassing kan worden geleverd. Met Publiceren wordt de URL ook geactiveerd om de sjabloon vanaf Dynamic Media Image Servers naar uw website of toepassing te bellen.

Zorg ervoor dat u alle afbeeldingen publiceert die aan de sjabloon zijn gekoppeld.

Als u een sjabloon wilt publiceren, markeert u deze voor publicatie en selecteert u op de algemene navigatiebalk **[!UICONTROL Publish]**. Selecteer vervolgens **[!UICONTROL Submit Publish]**. Zie [Sjablonen publiceren](publishing-templates.md#publishing_templates).

## 5. Een sjabloon aan een webpagina koppelen

Dynamic Media Classic maakt URL&#39;s voor sjablonen en activeert de URL&#39;s wanneer u sjablonen publiceert naar Dynamic Media Image Servers. U kunt deze URL-tekenreeksen kopiëren vanaf de pagina Sjabloonvoorbeeld.

Selecteer uw malplaatje in het Browse Comité, en selecteer dan **[!UICONTROL Preview]** om de pagina Sjabloonvoorbeeld te openen. Kies een voorinstelling voor de afbeelding die u als sjabloon wilt gebruiken en selecteer **[!UICONTROL Copy URL]**. Nadat u URL van de pagina van de Voorproef kopieert, kunt u het in uw Website of toepassing gebruiken. Zie [Een sjabloon koppelen aan een webpagina](linking-template-web-page.md#linking_a_template_to_a_web_page).
