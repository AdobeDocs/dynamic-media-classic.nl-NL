---
title: Een sjabloon koppelen aan een webpagina
seo-title: Een sjabloon koppelen aan een webpagina
description: 'null'
seo-description: Leer hoe u een sjabloon aan een webpagina koppelt.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Een sjabloon koppelen aan een webpagina{#linking-a-template-to-a-web-page}

Uw websites en toepassingen hebben via URL-tekenreeksen toegang tot inhoud van Dynamic Media Image Server. Nadat u een sjabloon publiceert, activeert Dynamic Media Classic een URL-tekenreeks die verwijst naar de sjabloon op Dynamic Media Image Servers. U kunt deze URL in een webbrowser plakken om te testen.

Om koorden URL in uw Web-pagina&#39;s en toepassingen te plaatsen, kopieer hen van het het Publiceren Scene7 Systeem. Als u een URL-tekenreeks voor een sjabloon wilt verkrijgen die met een voorinstelling voor afbeelding is gegenereerd, gaat u naar het voorvertoningsscherm of het deelvenster Bladeren (in de gedetailleerde weergave). Selecteer vervolgens een voorinstelling voor afbeeldingen en selecteer de knop URL kopiëren.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## Een sjabloon-URL ophalen {#obtaining-a-template-url}

U kunt een sjabloon-URL-tekenreeks die is gegenereerd door een voorinstelling voor afbeelding, verkrijgen via het scherm Sjabloonvoorbeeld. Nadat u de URL hebt gekopieerd, landt deze op het Klembord, zodat u deze desgewenst kunt plakken. Ga als volgt te werk om een sjabloon-URL-tekenreeks te verkrijgen die is gegenereerd met een voorinstelling voor afbeelding in het scherm Sjabloonvoorbeeld:

1. Klik op de knop Voorvertoning rollover van de sjabloon of kies Bestand > Voorvertoning. Het voorvertoningsscherm wordt geopend.
1. Kies in de menu&#39;s van de voorinstelling de voorinstelling voor de afbeelding waarmee u de sjabloonafbeelding wilt leveren. Het scherm van de Voorproef toont u hoe het malplaatje kijkt wanneer het van de server wordt geleverd.
1. Klik op de knop URL kopiëren om de URL naar het klembord te kopiëren.

## Sjabloon-URL&#39;s toevoegen aan uw webpagina {#adding-template-urls-to-your-web-page}

Als u een sjabloon aan uw webpagina wilt toevoegen, neemt u contact op met het ontwikkelingsteam van de webpagina om de `<IMG>` tag in uw HTML-webpaginacode aan te passen met de tekenreeks Dynamic Media Classic URL om een aanvraag in te dienen bij Dynamic Media Image Servers. De handelingsmotor of de dynamische Web-pagina code neemt het malplaatjebeeld bij de grootte en met de het formatteren specificatie op die door het Beeld wordt bepaald vooraf instelt u voor uw malplaatje kiest.

>[!MORELIKETHIS]
>
>* [Dynamische afbeeldingen toevoegen aan uw webpagina](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
