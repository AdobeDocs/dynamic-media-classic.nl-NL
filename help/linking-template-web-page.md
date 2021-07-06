---
title: Een sjabloon koppelen aan een webpagina
description: Leer hoe u een sjabloon aan een webpagina koppelt.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# Een sjabloon koppelen aan een webpagina{#linking-a-template-to-a-web-page}

Uw websites en toepassingen hebben via URL-tekenreeksen toegang tot Dynamic Media Image Server-inhoud. Nadat u een sjabloon hebt gepubliceerd, activeert Dynamic Media Classic een URL-tekenreeks die verwijst naar de sjabloon op Dynamic Media Image Servers. U kunt deze URL in een webbrowser plakken om te testen.

Kopieer URL-tekenreeksen vanuit Dynamic Media Classic om deze in uw webpagina&#39;s en toepassingen te plaatsen. Als u een URL-tekenreeks voor een sjabloon wilt verkrijgen die met een voorinstelling voor afbeelding is gegenereerd, gaat u naar het voorvertoningsscherm of het deelvenster Bladeren (in de gedetailleerde weergave). Selecteer vervolgens een voorinstelling voor afbeeldingen en selecteer de knop URL kopiëren.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## Een sjabloon-URL ophalen {#obtaining-a-template-url}

U kunt een sjabloon-URL-tekenreeks die is gegenereerd door een voorinstelling voor afbeelding, verkrijgen via het scherm Sjabloonvoorbeeld. Nadat u de URL hebt gekopieerd, landt deze op het Klembord, zodat u deze desgewenst kunt plakken. Ga als volgt te werk om een sjabloon-URL-tekenreeks te verkrijgen die is gegenereerd met een voorinstelling voor afbeelding op de pagina Sjabloonvoorbeeld:

1. Klik op de rollover-knop **[!UICONTROL Preview]** of kies **[!UICONTROL File]** > **[!UICONTROL Preview]**.
1. Kies in de menu&#39;s van de voorinstelling de voorinstelling voor de afbeelding waarmee u de sjabloonafbeelding wilt leveren. Op de pagina Voorvertoning ziet u hoe de sjabloon eruitziet wanneer deze vanaf de server wordt geleverd.
1. Klik **[!UICONTROL Copy URL]** om URL aan het Klembord te kopiëren.

## Sjabloon-URL&#39;s toevoegen aan uw webpagina {#adding-template-urls-to-your-web-page}

Als u een sjabloon aan uw webpagina wilt toevoegen, neemt u contact op met het ontwikkelingsteam van de webpagina om de tag `<IMG>` in de code van uw HTML-webpagina te wijzigen. Gebruik de Klassieke URL-tekenreeks van Dynamic Media om een aanvraag in te dienen bij Dynamic Media Image Servers. De handelingsmotor of de dynamische Web-paginacode neemt het malplaatjebeeld bij de grootte en met de het formatteren specificatie op die door het Beeld wordt bepaald vooraf instelt u voor uw malplaatje kiest.

>[!MORELIKETHIS]
>
>* [Dynamische afbeeldingen toevoegen aan uw webpagina](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

