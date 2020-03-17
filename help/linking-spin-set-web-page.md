---
title: Een centrifugeerset koppelen aan een webpagina
seo-title: Een centrifugeerset koppelen aan een webpagina
description: 'null'
seo-description: Leer hoe u een centrifugeset aan een webpagina koppelt.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Een centrifugeerset koppelen aan een webpagina{#linking-a-spin-set-to-a-web-page}

Websites en toepassingen hebben via URL-tekenreeksen of ingesloten code toegang tot de inhoud van Dynamic Media Image Server, inclusief de inhoud van de Spin-sets. Deze URL-tekenreeksen worden geactiveerd tijdens het publicatieproces. Om het koord URL of bedt code voor uw Vastgestelde Spin in uw Web-pagina&#39;s en toepassingen te plaatsen, kopieert u het van het het Publiceren Scene7 Systeem.

>[!NOTE]
>
>De URL is pas actief als u het element publiceert.

## URL van een centrifugeerset kopiëren {#copying-a-spin-set-url}

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Middelenbladeren op **Draaiset**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **Rasterweergave**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en in het deelvenster Code insluiten aan de rechterkant op URL **** kopiëren rechts van de gewenste viewer.
   * Klik op **Rasterweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens onder de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik op URL **** kopiëren onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik op **Lijstweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik op URL **** kopiëren onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik op **Rasterweergave**, **Lijstweergave** of **Gedetailleerde weergave**. Klik op dezelfde werkbalk op **Voorvertoning** > **Viewer List**.

      Klik op URL **** kopiëren onder de kolom Handelingen van de tabel in de Viewer List.

## URL&#39;s van centrifuges toevoegen aan uw webpagina {#adding-spin-set-urls-to-your-web-page}

De Reeksen van de draaien worden opgesteld als alle gezoemkijkers, door middel van een dynamische pagina (ASPIS of JSP) die de Reeks van de Draai in een gezoemvenster toont. Voor de URL-aanroep naar het Dynamic Media Classic-platform geldt hetzelfde protocol voor de zoomviewer. De naam van de voorinstelling voor de viewer is echter afhankelijk van de voorinstelling die de beheerder heeft gedefinieerd als de standaardvoorinstelling voor de voorinstelling voor de voorinstelling van de centrifuge. Het volgende niet-live URL-syntaxisvoorbeeld bevat bijvoorbeeld een naam voor een voorinstelling die wordt aangeroepen `viewer.jsp` en de SKU-parameter is nu de naam van de spellingset:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

In dit URL-syntaxisvoorbeeld (de koppeling is niet live), ziet u een SKU-nummer ( `sku=backpack_spin`). De volgende tekenreeks `sku=` is de naam van de centrifugeset ( `backpack spin`).

## De insluitcode van een viewer voor een centrifugeset kopiëren {#copying-the-embed-code-of-a-spin-set-viewer}

Met de functie Code insluiten kunt u de viewercode voor de geselecteerde centrifugeset controleren. U kunt de code ook naar het klembord kopiëren, zodat u de code op uw webpagina&#39;s kunt plakken en de viewer kunt implementeren. Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

**De insluitcode van een viewer voor een centrifuge-set kopiëren**

1. Klik in de vervolgkeuzelijst Tonen in het deelvenster Middelenbladeren op **Draaiset**.
1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die de Spin-set bevat waarvan u de insluitcode wilt kopiëren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **Rasterweergave**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en in het deelvenster Code insluiten rechts van de gewenste viewer op Code **** insluiten.
   * Klik op **Rasterweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens onder de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik op de pagina Viewer List onder de kolom Acties van de tabel op Code **** insluiten.

   * Klik op **Lijstweergave**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **Voorvertoning** > **Viewer List**.

      Klik op de pagina Viewer List onder de kolom Acties van de tabel op Code **** insluiten.

   * Klik op **Rasterweergave**, **Lijstweergave** of **Gedetailleerde weergave**. Klik op dezelfde werkbalk op **Voorvertoning** > **Viewer List**.

      Klik op de pagina Viewer List onder de kolom Acties van de tabel op Code **** insluiten.

1. Klik in het dialoogvenster Code insluiten op **Kopiëren naar klembord**.

   Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

1. Klik op Sluiten.

