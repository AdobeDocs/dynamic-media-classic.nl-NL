---
title: Aanbiedingsets overslaan naar Adobe Target Classic
seo-title: Aanbiedingsets overslaan naar Adobe Target Classic
description: 'null'
seo-description: Leer hoe u sets met aanbiedingen naar Adobe Target Classic kunt duwen.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Aanbiedingsets overslaan naar Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

Nadat u een aanbiedingsreeks creeert of uitgeeft, duw het aan Doel Klassiek door deze stappen te volgen:

1. Klik in het scherm Klassieke doelaanbiedingsset op de knop Push Offers.
1. Voer uw aanmeldingsgegevens in.
1. Klik op de knop Aanmelden.

Tijdens de overdracht aan het Klassieke Doel, wordt prefix S7_ automatisch in bijlage aan het begin van aanbiedingsnamen. Dit voorvoegsel is in bijlage om ervoor te zorgen dat u de Dynamische Klassieke aanbiedingen van Media in de Klassieke de aanbiedingslijst van het Doel gemakkelijk kunt vinden. De aanbieding wordt bijvoorbeeld weergegeven als S7_&lt;naam van aanbiedingsset>_&lt;naam aanbieding>.

SPS duwt in de Klassieke de widgetaanbiedingen van het Doel. U kunt de aanbiedingen van Widget gebruiken om uw eigen aanbiedingsinhoud buiten Klassiek van het Doel te ontvangen. Widget-aanbiedingen zijn vergelijkbaar met een standaardaanbieding die buiten Target Classic wordt gehost. Ze staan Target Classic toe om aanbiedingsinhoud te implementeren die op uw server is opgeslagen, zodat u geavanceerder en dynamisch gebruik kunt maken. Met Widget kunt u inhoud ophalen van een URL en deze inhoud gedurende ongeveer twee uur in cache plaatsen. Widget-aanbiedingen bieden enkele mogelijkheden voor het genereren van dynamische inhoud die andere aanbiedingen buiten Target Classic niet bieden. Als de mbox die de aanbieding aanbiedt parameters mbox zoals `mboxProductID` en `mbox.offerId`, bevat, worden de parameters `productId=[PRODUCT_ID]`en `offerID=[OFFERID]` URL toegevoegd aan gevraagde URL. Deze parameters kunnen door de dienst beschikbaar bij de aanbieding URL van Widget worden gebruikt om inhoud buiten Klassiek van het Doel terug te keren die product of ordeinformatie van uw dozen gebruikt. De aanbieding van Widget is ook toegankelijk door API om aanbiedingen buiten Klassiek van het Doel programmatically tot stand te brengen.
