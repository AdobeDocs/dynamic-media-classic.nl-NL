---
title: Zoomviewers koppelen aan uw webpagina's
description: Leer hoe u zoomviewers kunt koppelen aan uw webpagina's in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Zoomviewers koppelen aan uw webpagina&#39;s{#linking-zoom-viewers-to-your-web-pages}

Uw websites en toepassingen hebben toegang tot de inhoud van Dynamic Media Image Server via URL-tekenreeksen of ingesloten code. Deze toegang omvat primaire afbeeldingen en de bijbehorende zoomdoelen. Dit omvat ook voorinstellingen voor zoomviewers. Deze URL-tekenreeksen worden geactiveerd tijdens het publicatieproces. Als u deze URL-tekenreeksen of de ingesloten code op uw webpagina&#39;s en toepassingen wilt plaatsen, kopieert u deze vanuit Adobe Dynamic Media Classic.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## Een zoomviewer-URL kopiëren {#copying-a-zoom-viewer-url}

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de zoomviewer bevat waarvan u de URL wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteer **[!UICONTROL Grid View]** of **[!UICONTROL List View]** . Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer rechts in het deelvenster URL&#39;s en Code insluiten de optie **[!UICONTROL Copy URL]** rechts van de gewenste viewer.
   * Selecteer **[!UICONTROL Grid View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL List View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** rechts van de miniatuurafbeelding.

     Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL Grid View]**, **[!UICONTROL List View]** of **[!UICONTROL Detail View]** . Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel op de pagina Viewer List.

## URL&#39;s voor een zoomviewer toevoegen aan uw webpagina {#adding-zoom-viewer-urls-to-your-web-page}

Doorgaans zoomen bezoekers op afbeeldingen op een website door eerst een zoompictogram te selecteren (vaak wordt met het pictogram de afbeelding van een vergrootglas weergegeven). Als u dit pictogram selecteert, wordt een dynamische webpagina (ASP of JSP) gestart die de afbeelding in een pop-upvenster weergeeft. In het pop-upvenster zoomen bezoekers daadwerkelijk op de afbeelding.

Voor meer details en codesteekproeven, zie [&#x200B; HTML5 Basis de Kijker van het Gezoem in de Gids van de Verwijzing van de Kijkers van Adobe &#x200B;](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) inbedden.

## De ingesloten kopie van een zoomviewer kopiëren {#copying-the-embed-copy-of-a-zoom-viewer}

Met de functie Code insluiten kunt u de viewercode voor de geselecteerde zoomviewer controleren. U kunt de code aan het klembord ook kopiëren zodat kunt u het in uw Web-pagina&#39;s voor plaatsing van de kijker kleven. U mag de code niet bewerken in het dialoogvenster Code insluiten.

**om de Embed Code van een kijker van het Gezoem te kopiëren:**

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de zoomviewer bevat waarvan u de code voor insluiten wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteer **[!UICONTROL Grid View]** . Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer rechts in het deelvenster URL&#39;s en Code insluiten de optie **[!UICONTROL Embed Code]** rechts van de gewenste viewer.
   * Selecteer **[!UICONTROL Grid View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL List View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** rechts van de miniatuurafbeelding.

     Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL Grid View]**, **[!UICONTROL List View]** of **[!UICONTROL Detail View]** . Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel op de pagina Viewer List.

1. Selecteer **[!UICONTROL Copy to Clipboard]** in het dialoogvenster Code insluiten.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Selecteer **[!UICONTROL Close]** .
