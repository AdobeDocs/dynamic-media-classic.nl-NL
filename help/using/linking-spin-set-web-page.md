---
title: Een centrifugeerset koppelen aan een webpagina
description: Leer hoe u een centrifugeset koppelt aan een webpagina in Adobe Dynamic Media Classic.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Een centrifugeerset koppelen aan een webpagina{#linking-a-spin-set-to-a-web-page}

Websites en toepassingen hebben via URL-tekenreeksen of ingesloten code toegang tot Dynamic Media Image Server-inhoud, waaronder Spin Sets. Deze URL-tekenreeksen worden geactiveerd tijdens het publicatieproces. Als u de URL-tekenreeks of de insluitcode voor de desbetreffende centrifugeset op uw webpagina&#39;s en toepassingen wilt plaatsen, kopieert u deze vanuit Adobe Dynamic Media Classic.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## Een URL voor een centrifugeset kopiëren {#copying-a-spin-set-url}

1. Selecteer in de vervolgkeuzelijst Tonen in het deelvenster Middelenbladeren de optie **[!UICONTROL Spin Set]**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteren **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer in de URL&#39;s en het deelvenster Code insluiten aan de rechterkant de optie **[!UICONTROL Copy URL]** rechts van de gewenste viewer.
   * Selecteren **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Copy URL]**.

   * Selecteren **[!UICONTROL List View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens rechts van de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Copy URL]**.

   * Selecteren **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Copy URL]**.

## Spin-set URL&#39;s toevoegen aan uw webpagina {#adding-spin-set-urls-to-your-web-page}

De Reeksen van de draaien worden opgesteld als alle gezoemkijkers, door middel van een dynamische pagina (ASPIS of JSP) die de Reeks van de Draai in een gezoemvenster toont. De URL-aanroep naar het Adobe Dynamic Media Classic-platform volgt hetzelfde protocol op de zoomviewer. De naam van de voorinstelling voor de viewer is echter afhankelijk van de voorinstelling die de beheerder heeft gedefinieerd als de standaardvoorinstelling voor de voorinstelling voor de voorinstelling van de centrifuge. Het volgende niet-live URL-syntaxisvoorbeeld bevat bijvoorbeeld de naam Voorinstelling `viewer.jsp` en de parameter SKU is nu de naam van de centrifuge-set:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Let op een SKU-nummer ( `sku=backpack_spin`). De tekenreeks na `sku=` is de naam van de centrifugeset ( `backpack spin`).

## De insluitcode van een viewer voor een centrifugeset kopiëren {#copying-the-embed-code-of-a-spin-set-viewer}

Met de functie Code insluiten kunt u de viewercode voor de geselecteerde centrifugeset controleren. U kunt de code ook naar het klembord kopiëren, zodat u de code op uw webpagina&#39;s kunt plakken en de viewer kunt implementeren. Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

**U kopieert de insluitcode van een viewer voor een centrifuge-set:**

1. Selecteer in de vervolgkeuzelijst Tonen in het deelvenster Middelenbladeren de optie **[!UICONTROL Spin Set]**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteren **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer in de URL&#39;s en het deelvenster Code insluiten aan de rechterkant de optie **[!UICONTROL Embed Code]** rechts van de gewenste viewer.
   * Selecteren **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Embed Code]**.

   * Selecteren **[!UICONTROL List View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens rechts van de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Embed Code]**.

   * Selecteren **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Embed Code]**.

1. Selecteer in het dialoogvenster Code insluiten de optie **[!UICONTROL Copy to Clipboard]**.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Selecteren **[!UICONTROL Close]**.
