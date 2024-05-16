---
title: Een sjabloon koppelen aan een webpagina
description: Leer hoe u een sjabloon koppelt aan een webpagina in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Een sjabloon koppelen aan een webpagina{#linking-a-template-to-a-web-page}

Uw websites en toepassingen hebben via URL-tekenreeksen toegang tot Dynamic Media Image Server-inhoud. Nadat u een sjabloon hebt gepubliceerd, activeert Adobe Dynamic Media Classic een URL-tekenreeks die verwijst naar de sjabloon op Dynamic Media Image Servers. U kunt deze URL in een webbrowser plakken om te testen.

Kopieer URL-tekenreeksen vanuit Adobe Dynamic Media Classic om deze in uw webpagina&#39;s en toepassingen te plaatsen. Als u een URL-tekenreeks voor een sjabloon wilt verkrijgen die met een voorinstelling voor afbeelding is gegenereerd, gaat u naar het voorvertoningsscherm of het deelvenster Bladeren (in de gedetailleerde weergave). Selecteer vervolgens een voorinstelling voor afbeeldingen en selecteer de knop URL kopiëren.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## Een sjabloon-URL verkrijgen {#obtaining-a-template-url}

U kunt een sjabloon-URL-tekenreeks die is gegenereerd door een voorinstelling voor afbeelding, verkrijgen via het scherm Sjabloonvoorbeeld. Nadat u de URL hebt gekopieerd, landt deze op het Klembord, zodat u deze desgewenst kunt plakken. Ga als volgt te werk om een sjabloon-URL-tekenreeks te verkrijgen die is gegenereerd met een voorinstelling voor afbeelding op de pagina Sjabloonvoorbeeld:

1. De rollover van de sjabloon selecteren **[!UICONTROL Preview]** of ga naar **[!UICONTROL File]** > **[!UICONTROL Preview]**.
1. Kies in de menu&#39;s van de voorinstelling de voorinstelling voor de afbeelding waarmee u de sjabloonafbeelding wilt leveren. Op de pagina Voorvertoning ziet u hoe de sjabloon eruitziet wanneer deze vanaf de server wordt geleverd.
1. Selecteren **[!UICONTROL Copy URL]** zodat u de URL naar het Klembord kunt kopiëren.

## Sjabloon-URL&#39;s toevoegen aan uw webpagina {#adding-template-urls-to-your-web-page}

Om een malplaatje aan uw Web-pagina toe te voegen, raadpleeg uw team van de Web-pagina ontwikkeling om te wijzigen `<IMG>` tag in uw HTML Web-pagina code. Gebruik de URL-tekenreeks van Adobe Dynamic Media Classic om een aanvraag in te dienen bij Dynamic Media Image Servers. De handelingsmotor of de dynamische Web-pagina code neemt het malplaatjebeeld bij de grootte en met de het formatteren specificatie op die door het Beeld wordt bepaald vooraf ingesteld u voor uw malplaatje kiest.

>[!MORELIKETHIS]
>
>* [Dynamische afbeeldingen toevoegen aan uw webpagina](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
