---
title: Aanbiedingssets worden ingesteld op Adobe Target Standard/Premium
description: Leer hoe u sets met aanbiedingen naar Adobe Target Standard/Premium kunt verzenden.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Aanbiedingssets worden ingesteld op Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Nadat u een aanbiedingsreeks creeert of uitgeeft, duw het aan Standaard/Premium van Doel door deze stappen te volgen:

1. Klik op **[!UICONTROL Push Offers]** in het scherm Set Test&amp;Target-aanbieding.
1. Voer uw clientcode en aanmeldingsgegevens in.
1. Klik op **[!UICONTROL Login]**.

Tijdens de overdracht aan de Norm van het Doel/Premium, wordt het prefix S7_ automatisch verbonden aan het begin van aanbiedingsnamen. Dit voorvoegsel wordt toegevoegd om ervoor te zorgen dat u gemakkelijk Dynamic Media Classic aanbiedingen in de de aanbiedingenlijst van de Test&amp;Target kunt vinden. De aanbieding wordt bijvoorbeeld weergegeven als S7_&lt;naam van aanbiedingsset>_&lt;naam aanbieding>.

Dynamic Media Classic plaatst de widget Target Standard/Premium in de aanbieding. U kunt de aanbiedingen van Widget gebruiken om uw eigen aanbiedingsinhoud buiten de Norm van het Doel te ontvangen/Premium. Widget-aanbiedingen zijn vergelijkbaar met een standaardaanbieding die buiten Target Standard/Premium wordt gehost. Ze stellen Target Standard/Premium in staat inhoud te implementeren die op uw server is opgeslagen, zodat u geavanceerder en dynamisch gebruik kunt maken. Met Widget kunt u inhoud ophalen van een URL en deze inhoud gedurende ongeveer twee uur in cache plaatsen. Widget-aanbiedingen bieden enkele mogelijkheden voor het genereren van dynamische inhoud die andere aanbiedingen buiten de Target Standard/Premium-opties niet bieden. Als de box die de aanbieding aanbiedt, mbox-parameters bevat zoals `mboxProductID` en `mbox.offerId`, worden de URL-parameters `productId=[PRODUCT_ID]`en `offerID=[OFFERID]` aan de gevraagde URL toegevoegd. Deze parameters kunnen worden gebruikt door een service die beschikbaar is op de URL van de widget-aanbieding om inhoud te retourneren buiten de Target Standard/Premium die product- of bestelgegevens uit uw vakken gebruikt. De Widget-aanbieding is ook toegankelijk via de API voor het programmatisch maken van aanbiedingen buiten Target Standard/Premium.
