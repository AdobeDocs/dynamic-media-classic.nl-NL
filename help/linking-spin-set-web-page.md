---
title: Een centrifugeerset koppelen aan een webpagina
description: Leer hoe u een centrifugeset koppelt aan een webpagina.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---


# Een centrifugeerset koppelen aan een webpagina{#linking-a-spin-set-to-a-web-page}

Websites en toepassingen hebben via URL-tekenreeksen of ingesloten code toegang tot Dynamic Media Image Server-inhoud, waaronder Spin Sets. Deze URL-tekenreeksen worden geactiveerd tijdens het publicatieproces. Als u de URL-tekenreeks of de insluitcode voor de desbetreffende centrifugeset op uw webpagina&#39;s en toepassingen wilt plaatsen, kopieert u deze vanuit Dynamic Media Classic.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## URL van een centrifugeerset kopiëren {#copying-a-spin-set-url}

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Bladeren van element op **Set draaien**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik **Rasterweergave**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en het deelvenster Code insluiten aan de rechterkant op **URL kopiëren** rechts van de gewenste viewer.
   * Klik **Rasterweergave**. Selecteer in het deelvenster Asset Browse één element en klik vervolgens onder de miniatuurafbeelding op **Voorvertoning** > **Viewerlijst**.

      Klik onder de kolom Acties van de tabel in de pagina Viewer List op **URL kopiëren**.

   * Klik **Lijstweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik onder de kolom Acties van de tabel in de pagina Viewer List op **URL kopiëren**.

   * Klik **Rasterweergave**, **Lijstweergave** of **Detailweergave**. Klik op **Voorvertoning** > **Viewerlijst** op dezelfde werkbalk.

      Klik onder de kolom Acties van de tabel in de pagina Viewer List op **URL kopiëren**.

## URL&#39;s van centrifugeset toevoegen aan uw webpagina {#adding-spin-set-urls-to-your-web-page}

De Reeksen van de draaien worden opgesteld als alle gezoemkijkers, door middel van een dynamische pagina (ASPIS of JSP) die de Reeks van de Draai in een gezoemvenster toont. Voor de URL-aanroep naar het Dynamic Media Classic-platform geldt hetzelfde protocol voor de zoomviewer. De naam van de voorinstelling voor de viewer is echter afhankelijk van de voorinstelling die de beheerder heeft gedefinieerd als de standaardvoorinstelling voor de voorinstelling voor de voorinstelling van de centrifuge. Het volgende niet-live URL-syntaxisvoorbeeld bevat bijvoorbeeld de naam `viewer.jsp` van de voorinstelling en de parameter SKU is nu de naam van de voorinstelling:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

In dit URL-syntaxisvoorbeeld (de koppeling is niet live), ziet u een SKU-nummer ( `sku=backpack_spin`). De tekenreeks na `sku=` is de naam van de centrifugeset ( `backpack spin`).

## De insluitcode van een viewer {#copying-the-embed-code-of-a-spin-set-viewer} voor een centrifugeerset kopiëren

Met de functie Code insluiten kunt u de viewercode voor de geselecteerde centrifugeset controleren. U kunt de code ook naar het klembord kopiëren, zodat u de code op uw webpagina&#39;s kunt plakken en de viewer kunt implementeren. Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

**De insluitcode van een viewer voor een centrifuge-set kopiëren**

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Bladeren van element op **Set draaien**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik **Rasterweergave**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik rechts in het deelvenster URL&#39;s en Code insluiten op **Code insluiten** rechts van de gewenste viewer.
   * Klik **Rasterweergave**. Selecteer in het deelvenster Asset Browse één element en klik vervolgens onder de miniatuurafbeelding op **Voorvertoning** > **Viewerlijst**.

      Klik onder de kolom Acties van de tabel in de pagina Viewer List op **Code insluiten**.

   * Klik **Lijstweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik onder de kolom Acties van de tabel in de pagina Viewer List op **Code insluiten**.

   * Klik **Rasterweergave**, **Lijstweergave** of **Detailweergave**. Klik op **Voorvertoning** > **Viewerlijst** op dezelfde werkbalk.

      Klik onder de kolom Acties van de tabel in de pagina Viewer List op **Code insluiten**.

1. Klik in het dialoogvenster Code insluiten op **Kopiëren naar klembord**.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Klik op Sluiten.

