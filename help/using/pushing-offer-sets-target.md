---
title: Push-aanbiedingen worden ingesteld op Adobe Target Standard/Premium
description: Leer hoe u sets met aanbiedingen naar Adobe Target Standard/Premium vanuit Adobe Dynamic Media Classic kunt duwen.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Push-aanbiedingen worden ingesteld op Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Nadat u een aanbiedingsset hebt gemaakt of bewerkt, gaat u als volgt te werk naar Adobe Target Standard/Premium:

1. Selecteer in het scherm Testo&amp;reet doelaanbieding de optie **[!UICONTROL Push Offers]**.
1. Voer uw clientcode en aanmeldingsgegevens in.
1. Selecteren **[!UICONTROL Login]**.

Tijdens de overdracht naar Adobe Target Standard/Premium wordt het voorvoegsel weergegeven `S7_` wordt automatisch toegevoegd aan het begin van aanbiedingsnamen. Dit voorvoegsel is toegevoegd om ervoor te zorgen dat je Adobe Dynamic Media Classic-aanbiedingen gemakkelijk kunt vinden in de aanbiedingenlijst Test&amp;Target. De aanbieding wordt bijvoorbeeld weergegeven als `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic gaat over naar de Adobe Target Standard/Premium-widgetaanbiedingen. Met Widget-aanbiedingen kunt u uw eigen aanbiedingsinhoud hosten buiten Adobe Target Standard/Premium. Widget-aanbiedingen zijn vergelijkbaar met een standaardaanbieding die buiten Adobe Target Standard/Premium wordt gehost. Ze stellen Adobe Target Standard/Premium in staat inhoud te implementeren die op uw server is opgeslagen, zodat u geavanceerder en dynamisch gebruik kunt maken. Widget-aanbiedingen kunnen inhoud ophalen van een URL, deze inhoud in cache plaatsen en deze inhoud gedurende ongeveer twee uur bedienen. Widget-aanbiedingen bieden enkele mogelijkheden voor het genereren van dynamische inhoud die andere aanbiedingen buiten Adobe Target Standard/Premium niet bieden. Als de mbox die de aanbieding van de aanbieding voorziet mbox parameters zoals bevat `mboxProductID` en `mbox.offerId`de `productId=[PRODUCT_ID]`en `offerID=[OFFERID]` URL-parameters worden toegevoegd aan de aangevraagde URL. Deze parameters kunnen worden gebruikt door een service die beschikbaar is via de URL van de widget-aanbieding voor het retourneren van inhoud buiten Adobe Target Standard/Premium die product- of bestelgegevens uit uw vakken gebruikt. De Widget-aanbieding is ook toegankelijk via de API voor het programmatisch maken van aanbiedingen buiten Adobe Target Standard/Premium.
