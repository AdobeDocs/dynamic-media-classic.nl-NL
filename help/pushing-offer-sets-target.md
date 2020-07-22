---
title: Aanbiedingssets worden ingesteld op Adobe Target Standard/Premium
seo-title: Aanbiedingssets worden ingesteld op Adobe Target Standard/Premium
description: 'null'
seo-description: Leer hoe u sets met aanbiedingen naar Adobe Target Standard/Premium kunt verzenden.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Aanbiedingssets worden ingesteld op Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Nadat u een aanbiedingsset hebt gemaakt of bewerkt, gaat u als volgt te werk naar Target Standard/Premium:

1. Klik in het scherm Testi&amp;Target-aanbiedingsset **[!UICONTROL Push Offers]**.
1. Voer uw clientcode en aanmeldingsgegevens in.
1. Klik op **[!UICONTROL Login]**.

Tijdens de overdracht naar Target Standard/Premium wordt het voorvoegsel S7_ automatisch toegevoegd aan het begin van de aanbiedingsnamen. Dit voorvoegsel is in bijlage om ervoor te zorgen dat u Dynamic Media Klassieke aanbiedingen in de de aanbiedingenlijst van de Test&amp;Target gemakkelijk kunt vinden. De aanbieding wordt bijvoorbeeld weergegeven als S7_&lt;naam van aanbiedingsset>_&lt;naam aanbieding>.

Met Dynamic Media Classic worden de aanbiedingen van de Target Standard/Premium-widget geactiveerd. Met Widget-aanbiedingen kunt u uw eigen aanbiedingsinhoud hosten buiten Target Standard/Premium. Widget-aanbiedingen zijn vergelijkbaar met standaardaanbiedingen die buiten Target Standard/Premium worden gehost. Target Standard/Premium kan hiermee inhoud aanbieden die op uw server is opgeslagen, zodat u over meer geavanceerde en dynamische toepassingen beschikt. Met Widget kunt u inhoud ophalen van een URL en deze inhoud gedurende ongeveer twee uur in cache plaatsen. Widget-aanbiedingen bieden enkele mogelijkheden voor het genereren van dynamische inhoud die andere aanbiedingen buiten Target Standard/Premium niet bieden. Als de mbox die de aanbieding aanbiedt parameters mbox zoals `mboxProductID` en `mbox.offerId`, bevat, worden de parameters `productId=[PRODUCT_ID]`en `offerID=[OFFERID]` URL toegevoegd aan gevraagde URL. Deze parameters kunnen worden gebruikt door een service die beschikbaar is via de URL van de widget-aanbieding voor het retourneren van inhoud buiten Target Standard/Premium die product- of bestelgegevens uit uw vakken gebruikt. De Widget-aanbieding is ook toegankelijk via de API voor het programmatisch maken van aanbiedingen buiten Target Standard/Premium.
