---
title: '"Snel starten: Basisbeginselen van sjablonen"'
seo-title: '"Snel starten: Basisbeginselen van sjablonen"'
description: 'null'
seo-description: Een inleiding en Snel Begin aan de Grondbeginselen van het Malplaatje helpen u aan de slag snel.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Snel starten: Grondbeginselen van sjablonen{#quick-start-template-basics}

De basis van sjablonen wordt dynamisch gemaakt en adresseerbare gelaagde afbeeldingsbestanden, zoals gelaagde bestanden, in beeldbewerkingstoepassingen zoals Adobe Photoshop. In tegenstelling tot een statisch bestand met lagen, zoals een PSD-bestand, kan een sjabloon parameters bevatten. Aan de hand van parameters kunnen de verschillende aspecten van de afbeelding worden benaderd en aangepast.

>[!NOTE]
>
>U kunt ook sjablonen maken op basis van lay-outontwerpen met behulp van Sjabloonpublicatie en bestanden uit Adobe Illustrator en Adobe InDesign. Zie [Sjabloonpublicatie](quick-start-template-publishing.md) .

Een sjabloon kan een willekeurig aantal afbeeldingslagen en tekstlagen bevatten. U kunt een statisch bestand met lagen, zoals een gelaagd PSD-bestand, omzetten in een sjabloon en sjablonen maken in Dynamic Media Classic. U kunt tekstlagen in sjablonen maken met lettertypen die u naar SPS hebt geüpload. Nadat u tekst aan een sjabloon hebt toegevoegd, kunt u deze opmaken door de uitvulling, lettertypen, tekengrootte en kleur ervan te wijzigen.

Met het scherm Parameters kunt u elk aspect van een sjabloon omzetten in een adresseerbare parameter. Op deze manier kunt u wijzigen welke gelaagde afbeelding moet worden gebruikt of welke tekstwaarde in de sjabloon moet worden gebruikt. De parameters worden overgegaan met het koord URL, toestaand u om het even welke parameter te veranderen om het antwoordbeeld dynamisch aan te passen dat van de beeldserver wordt geproduceerd.

**Snel starten**

Dit snelle Begin wordt ontworpen om snel met de Grondbeginselen van het Malplaatje in gebruik te worden.

**1. De bestanden uploaden**

Begin door het PSD-bestand of afbeeldingsbestand voor uw sjabloon te uploaden. Dynamic Media Classic ondersteunt naast PSD vele afbeeldingsbestandsindelingen, maar TIFF- en PNG-afbeeldingen zonder gegevensverlies worden aanbevolen voor sjablonen omdat ze transparantie mogelijk maken.

Als u een PSD-bestand gebruikt om uw sjabloon te maken, selecteert u de optie Sjabloon maken in het dialoogvenster Taakopties uploaden wanneer u het PSD-bestand uploadt. Kies ook een optie voor het benoemen van lagen om dynamische media Klassiek te vertellen hoe te om lagen PSD te noemen wanneer zij aan het het Publiceren Scene7 Systeem worden geupload.

Als u afbeeldingsbestanden gebruikt, kunt u de afbeeldingen uitsnijden en ook een masker maken van uitknippaden in de afbeeldingen wanneer u deze uploadt.

Selecteer de knop Uploaden op de algemene navigatiebalk om een PSD-bestand of andere afbeeldingsbestanden van uw computer te uploaden naar een map op de SPS. Zie Sjabloonbestanden [](uploading-template-files.md#uploading_template_files)uploaden.

**2. Een sjabloon maken**

Als u een sjabloon wilt maken van een PSD-bestand, selecteert u de optie Sjabloon maken wanneer u het bestand uploadt. Als u een sjabloon wilt maken op basis van afbeeldingen, kiest u Samenstellen > Sjabloonbasisbeginselen, voert u een breedte- en hoogtemeting voor het canvas in, selecteert u Designer of Developer en sleept u afbeeldingen naar het scherm Sjabloon. U kunt de afbeeldingen ook selecteren voordat u Build > Sjabloonbasisbeginselen kiest. Het scherm van het Malplaatje biedt hulpmiddelen voor:

* Afbeeldingslagen toevoegen. Als u een laag wilt toevoegen, sleept u een afbeelding naar het scherm Sjabloon.
* Tekstlagen toevoegen. Selecteer het gereedschap Tekst en sleep om een vak voor de tekstlaag te tekenen. Maak de tekst vervolgens op met gereedschappen in het tekstscherm.
* De grootte en positie van lagen wijzigen.
* De volgorde van lagen wijzigen.
* Schaduw- en gloedeffecten toepassen op afbeeldings- en tekstlagen.

Zie Een sjabloon [maken](creating-template.md#creating_a_template).

**3. Sjabloonparameters maken**

De volgende stap bestaat uit het bepalen van de parameters van de eigenschappen op lagen om te bepalen welke laageigenschappen in het koord URL worden omvat. De parameters staan u toe om malplaatjes met maximumflexibiliteit te gebruiken. Nadat u een laageigenschap in een parameter hebt gemaakt, kunt u deze dynamisch wijzigen.

Als u parameters wilt opgeven voor een laag, opent u de sjabloon in het scherm Sjabloon en selecteert u de knop Parameters naast een laagnaam. Selecteer in het scherm Parameters de optie naast elke parameter die u wilt toevoegen. Zie Sjabloonparameters [maken](creating-template-parameters.md#creating_template_parameters).

**4. Sjablonen publiceren**

Wanneer u de sjabloon publiceert, wordt deze op Dynamic Media Image Servers geplaatst, zodat deze dynamisch aan uw website of toepassing kan worden geleverd. Met Publiceren wordt de URL ook geactiveerd om de sjabloon vanaf Dynamic Media Image Servers naar uw website of toepassing aan te roepen.

Zorg ervoor dat u alle afbeeldingen publiceert die aan de sjabloon zijn gekoppeld.

Als u een sjabloon wilt publiceren, markeert u deze voor publicatie en selecteert u de knop Publiceren op de algemene navigatiebalk. Selecteer vervolgens de knop Publiceren starten. Zie [Sjablonen](publishing-templates.md#publishing_templates)publiceren.

**5. Een sjabloon koppelen aan een webpagina**

Dynamic Media Classic maakt URL&#39;s voor sjablonen en activeert de URL&#39;s wanneer u sjablonen publiceert naar Dynamic Media Image Servers. U kunt deze URL-tekenreeksen kopiëren vanuit het scherm Sjabloonvoorbeeld.

Selecteer de sjabloon in het deelvenster Bladeren en klik op de knop Voorvertoning om het scherm Sjabloonvoorvertoning te openen. Kies vervolgens een voorinstelling voor afbeeldingen die uw sjabloon aflevert en selecteer de knop URL kopiëren. Nadat u de URL vanuit het voorvertoningsscherm hebt gekopieerd, kunt u deze in uw website of toepassing gebruiken. Zie Een sjabloon [koppelen aan een webpagina](linking-template-web-page.md#linking_a_template_to_a_web_page).