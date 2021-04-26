---
title: Een centrifugeerset koppelen aan een webpagina
description: Leer hoe u een centrifugeset koppelt aan een webpagina.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Klassiek,Viewers,Draaiende Reeksen
role: Business Practitioner
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 1%

---

# Een centrifugeerset koppelen aan een webpagina{#linking-a-spin-set-to-a-web-page}

Websites en toepassingen hebben via URL-tekenreeksen of ingesloten code toegang tot Dynamic Media Image Server-inhoud, waaronder Spin Sets. Deze URL-tekenreeksen worden geactiveerd tijdens het publicatieproces. Als u de URL-tekenreeks of de insluitcode voor de desbetreffende centrifugeset op uw webpagina&#39;s en toepassingen wilt plaatsen, kopieert u deze vanuit Dynamic Media Classic.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## URL van een centrifugeerset kopiëren {#copying-a-spin-set-url}

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Asset Browse op **[!UICONTROL Spin Set]**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en het deelvenster Code insluiten rechts van de gewenste viewer op **[!UICONTROL Copy URL]**.
   * Klik op **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en klik vervolgens onder de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Klik op **[!UICONTROL Copy URL]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik op **[!UICONTROL List View]**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Klik op **[!UICONTROL Copy URL]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Klik op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** op dezelfde werkbalk.

      Klik op **[!UICONTROL Copy URL]** onder de kolom Handelingen van de tabel in de Viewer List.

## URL&#39;s van centrifugeset toevoegen aan uw webpagina {#adding-spin-set-urls-to-your-web-page}

De Reeksen van de draaien worden opgesteld als alle gezoemkijkers, door middel van een dynamische pagina (ASPIS of JSP) die de Reeks van de Draai in een gezoemvenster toont. Voor de URL-aanroep naar het Dynamic Media Classic-platform geldt hetzelfde protocol voor de zoomviewer. De naam van de voorinstelling voor de viewer is echter afhankelijk van de voorinstelling die de beheerder heeft gedefinieerd als de standaardvoorinstelling voor de voorinstelling voor de voorinstelling van de centrifuge. Het volgende niet-live URL-syntaxisvoorbeeld bevat bijvoorbeeld de naam `viewer.jsp` van de voorinstelling en de parameter SKU is nu de naam van de voorinstelling:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

In dit URL-syntaxisvoorbeeld (de koppeling is niet live), ziet u een SKU-nummer ( `sku=backpack_spin`). De tekenreeks na `sku=` is de naam van de centrifugeset ( `backpack spin`).

## De insluitcode van een viewer {#copying-the-embed-code-of-a-spin-set-viewer} voor een centrifugeerset kopiëren

Met de functie Code insluiten kunt u de viewercode voor de geselecteerde centrifugeset controleren. U kunt de code ook naar het klembord kopiëren, zodat u de code op uw webpagina&#39;s kunt plakken en de viewer kunt implementeren. Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

**U kopieert de insluitcode van een viewer voor een centrifuge-set:**

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Asset Browse op **[!UICONTROL Spin Set]**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en het deelvenster Code insluiten rechts van de gewenste viewer op **[!UICONTROL Embed Code]**.
   * Klik op **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en klik vervolgens onder de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Klik op **[!UICONTROL Embed Code]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik op **[!UICONTROL List View]**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Klik op **[!UICONTROL Embed Code]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Klik op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** op dezelfde werkbalk.

      Klik op **[!UICONTROL Embed Code]** onder de kolom Handelingen van de tabel in de Viewer List.

1. Klik in het dialoogvenster Code insluiten op **[!UICONTROL Copy to Clipboard]**.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Klik op **[!UICONTROL Close]**.
