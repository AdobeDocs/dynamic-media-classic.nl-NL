---
title: Aanbiedingssets worden ingesteld op Adobe Target Standard/Premium
description: Leer hoe u sets met aanbiedingen naar Adobe Target Standard/Premium kunt verzenden.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Aanbiedingssets worden ingesteld op Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Nadat u een aanbiedingsset hebt gemaakt of bewerkt, gaat u als volgt te werk naar Adobe Target Standard/Premium:

1. Klik op **[!UICONTROL Push Offers]** in het scherm Set Test&amp;Target-aanbieding.
1. Voer uw clientcode en aanmeldingsgegevens in.
1. Klik op **[!UICONTROL Login]**.

Tijdens de overdracht naar Adobe Target Standard/Premium wordt het voorvoegsel `S7_` automatisch toegevoegd aan het begin van de aanbiedingsnamen. Dit voorvoegsel wordt toegevoegd om ervoor te zorgen dat u gemakkelijk Dynamic Media Classic aanbiedingen in de de aanbiedingenlijst van de Test&amp;Target kunt vinden. De aanbieding wordt bijvoorbeeld weergegeven als `S7_<name of offer set>_<offer name>`.

Dynamic Media Classic duikt in Adobe Target Standard/Premium-widgetaanbiedingen. Met Widget-aanbiedingen kunt u uw eigen aanbiedingsinhoud hosten buiten Adobe Target Standard/Premium. Widget-aanbiedingen zijn vergelijkbaar met een standaardaanbieding die buiten Adobe Target Standard/Premium wordt gehost. Ze stellen Adobe Target Standard/Premium in staat inhoud te implementeren die op uw server is opgeslagen, zodat u geavanceerder en dynamisch gebruik kunt maken. Met Widget kunt u inhoud ophalen van een URL en deze inhoud gedurende ongeveer twee uur in cache plaatsen. Widget-aanbiedingen bieden enkele mogelijkheden voor het genereren van dynamische inhoud die andere aanbiedingen buiten Adobe Target Standard/Premium niet bieden. Als de box die de aanbieding aanbiedt, mbox-parameters bevat zoals `mboxProductID` en `mbox.offerId`, worden de URL-parameters `productId=[PRODUCT_ID]`en `offerID=[OFFERID]` aan de gevraagde URL toegevoegd. Deze parameters kunnen worden gebruikt door een service die beschikbaar is via de URL van de widget-aanbieding voor het retourneren van inhoud buiten Adobe Target Standard/Premium die product- of bestelgegevens uit uw vakken gebruikt. De Widget-aanbieding is ook toegankelijk via de API voor het programmatisch maken van aanbiedingen buiten Adobe Target Standard/Premium.
