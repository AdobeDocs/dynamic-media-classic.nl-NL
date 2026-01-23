---
title: Een eCatalog aan een Web-pagina koppelen
description: Leer hoe u een eCatalog aan een Web-pagina in Adobe Dynamic Media Classic koppelt.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Een eCatalog aan een Web-pagina koppelen{#linking-an-ecatalog-to-a-web-page}

Uw Websites en toepassingen hebben toegang tot de Dynamische inhoud van de Server van het Beeld van Media, met inbegrip van eCatalogs, als koorden URL of ingebedde code. Deze URL-tekenreeksen worden geactiveerd tijdens het publicatieproces. Als u de URL-tekenreeks of ingesloten code voor uw eCatalog wilt plaatsen in uw webpagina&#39;s en toepassingen, kopieert u deze vanuit Adobe Dynamic Media Classic.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## Een eCatalog-URL kopiëren {#copying-an-ecatalog-url}

1. Selecteer **[!UICONTROL Catalog]** in de vervolgkeuzelijst Tonen in het deelvenster Asset Browse.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de eCatalog bevat waarvan u de code voor insluiten wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteer **[!UICONTROL Grid View]** . Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer rechts in het deelvenster URL&#39;s en Code insluiten de optie **[!UICONTROL Copy URL]** rechts van de gewenste viewer.
   * Selecteer **[!UICONTROL Grid View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL List View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** rechts van de miniatuurafbeelding.

     Selecteer **[!UICONTROL Copy URL]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL Grid View]**, **[!UICONTROL List View]** of **[!UICONTROL Detail View]** . Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     In de pagina van de Lijst van de Kijker, onder de kolom van Acties van de lijst, selecteer **Exemplaar URL**.

## ECatalog URLs aan uw Web-pagina toevoegen {#adding-ecatalog-urls-to-your-web-page}

De gemeenschappelijkste manier om een eCatalog op te stellen is een verbinding in de vorm van een de omslagpagina van de eCatalogduimnagel op uw Web-pagina te plaatsen. Werk samen met uw IT-team om ervoor te zorgen dat de eCatalog wordt gestart in een schoon, gecentreerd pop-upvenster. Vraag uw IT-team om de werkbalk en adresbalk in de browser niet weer te geven.

Voor meer details en codesteekproeven, zie de [&#x200B; Ingebedde Kijker HTML5 eCatalog &#x200B;](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) in de Verwijzing van de Kijkers van Adobe.

## De ingesloten code van een eCatalog-viewer kopiëren {#copying-the-embed-code-of-an-ecatalog-viewer}

Met de ingesloten codefunctie kunt u de viewercode voor de geselecteerde eCatalog controleren. U kunt de code aan het klembord ook kopiëren zodat kunt u het in uw Web-pagina&#39;s voor plaatsing van de kijker kleven. U mag de code niet bewerken in het dialoogvenster Code insluiten.

**om de ingebedde code van een eCatalog kijker te kopiëren:**

1. Selecteer **[!UICONTROL Catalog]** in de vervolgkeuzelijst Tonen in het deelvenster Asset Browse.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de eCatalog bevat waarvan u de code voor insluiten wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteer **[!UICONTROL Grid View]** . Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer **[!UICONTROL Embed Code]** in het deelvenster URL&#39;s aan de rechterkant.
   * Selecteer **[!UICONTROL Grid View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL List View]** . Selecteer in het deelvenster Asset Browse één element en ga vervolgens naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** rechts van de miniatuurafbeelding.

     Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel op de pagina Viewer List.

   * Selecteer **[!UICONTROL Grid View]**, **[!UICONTROL List View]** of **[!UICONTROL Detail View]** . Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .

     Selecteer **[!UICONTROL Embed Code]** onder de kolom Acties van de tabel op de pagina Viewer List.

1. Selecteer **[!UICONTROL Copy to Clipboard]** in het dialoogvenster Code insluiten.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Selecteer **[!UICONTROL Close]** .
