---
title: Een aanbiedingsset maken
seo-title: Een aanbiedingsset maken
description: 'null'
seo-description: Leer hoe u een set voorstellen maakt.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---


# Een aanbiedingsset maken{#creating-an-offer-set}

U kunt elk van de volgende soorten aanbiedingen maken:

* Video
* Parameterized malplaatje
* Afbeelding

Klik voor sjablonen op **Toevoegen en Voorvertoning** en stel de gewenste parameters in. De andere typen aanbiedingssets bevatten geen parameters, maar u kunt deze nog steeds aanpassen door op **Voorvertoning** te klikken en de beschikbare voorinstellingen te wijzigen.

Dynamic Media Classic biedt tools voor bewerking en het maken van aanbiedingssets.

>[!NOTE]
>
>Voordat u een set aanbiedingen maakt, moet u alle elementen publiceren die u wilt gebruiken voor de set Dynamic Media Classic. Zie [Elementen](publishing-files.md#manually_publishing_assets) handmatig publiceren en [elementen](publishing-files.md#manually_unpublishing_assets)handmatig verwijderen.

## Soorten aanbiedingen {#types-of-offer-sets}

Maak een set aanbiedingen op basis van de volgende soorten aanbiedingen:

* **Afbeeldingen** U kunt afbeeldingen samenstellen voor een set aanbiedingen. Elke afbeelding bevat een andere aanbieding in de set.

* **Afbeeldingssjabloon** U kunt afbeeldingssjablonen in Dynamic Media Classic waarderen met de opdracht Samenstellen > Sjabloonbasisbeginselen. Via parameters kunnen onderdelen van de sjabloon (de tekst in tekstkaders, de verschillende afbeeldingen) worden omgewisseld en aangepast. Voor een aanbiedingsreeks, kunt u malplaatjeparameters gebruiken om variaties op het zelfde beeld in uw aanbiedingsreeks tot stand te brengen, bijvoorbeeld. Zie Sjabloonparameters maken voor informatie over het maken van afbeeldingssjablonen en het toewijzen van parameters aan deze sjablonen.

* **Video** U kunt video samenstellen voor een aanbiedingsset. Elke video heeft een andere aanbieding in de set.

## Een aanbieding maken die is ingesteld met een geparametriseerde sjabloon {#creating-an-offer-set-with-a-parameterized-template}

Wanneer u een set voorstellen maakt, heeft de optie **Publiceren na opslaan** invloed op de set en stelt u leden als volgt in:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen](publishing-files.md#manually_publishing_assets) handmatig publiceren en [elementen](publishing-files.md#manually_unpublishing_assets)handmatig verwijderen.

**Een aanbieding maken die is ingesteld met een geparametriseerde sjabloon**

1. Selecteer de sjabloon of banner.
1. Klik op **Samenstellen** > **Aanbiedingsset** testen en Target testen.

   Op de pagina Testi&amp;Target-aanbiedingsset vindt u de aanbiedingen in de aangeboden set. Het eerste item in de lijst is het object.

1. Selecteer het object en klik op **Toevoegen en voorvertonen**.

   De linkerkant van de pagina bevat parameters in de sjabloon en de bijbehorende waarden.

1. Wijzig parameterwaarden om de aanbieding te maken. Voer bijvoorbeeld andere tekst in een tekstveld in, wijzig de grootte van een laag, verander een afbeelding door een andere of kies een andere voorinstelling voor de viewer.
1. Klik op **Opslaan** of **Opslaan als** om het voorstel op te slaan als onderdeel van de set met aanbiedingen.

   Op de pagina Testi&amp;Target Offerteset worden de aanbiedingen weergegeven die u hebt gemaakt.

1. Herhaal stap 3 tot en met 5 om meer aanbiedingen voor de set te maken.
1. Als u klaar bent, controleert u of **Publiceren na opslaan** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Klik op **Sluiten**, voer een naam in voor de aanbiedingsset en klik op **Opslaan**.

Druk op de aanbieding op Target Standard/Premium voordat u de pagina Set Test&amp;Target-aanbiedingen sluit. Zie Aanbiedingsets [Pushing to Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set aanbiedingen maken met afbeeldingen of video&#39;s {#creating-an-offer-set-with-images-or-videos}

Wanneer u een set voorstellen maakt, heeft de optie **Publiceren na opslaan** invloed op de set en stelt u leden als volgt in:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen](publishing-files.md#manually_publishing_assets) handmatig publiceren en [elementen](publishing-files.md#manually_unpublishing_assets)handmatig verwijderen.

**Een set aanbiedingen maken met afbeeldingen of video&#39;s**

1. Stel afbeeldingen of video&#39;s samen voor de ingestelde aanbieding. Start in het scherm Test&amp;Target Offset of in de rasterweergave of lijstweergave en gebruik een van de volgende methoden:

   * **Scherm** Klikken testen en Target-aanbod instellen **[!UICONTROL Build > Test&Target Offer Set]**. Sleep afbeeldingen of video&#39;s naar het scherm. Als u video&#39;s of afbeeldingen van verschillende grootten wilt maken, sleept u in meerdere exemplaren van de afbeelding of video en stelt u elke grootte afzonderlijk in.

   * **De raster- of lijstweergave** Selecteer de afbeeldingen of video&#39;s en klik op **[!UICONTROL Build > Test&Target Offer Set]**.

1. Selecteer eventueel een afbeelding of video en klik op **Voorvertoning**. Op de pagina Voorvertoningsaanbiedingen kunt u de grootte en het uiterlijk wijzigen van de afbeelding of video die u hebt geselecteerd. U kunt ook alle afbeeldingen of video&#39;s in de set met aanbiedingen wijzigen.

   * Kies een voorinstelling om het uiterlijk en de grootte van de afbeelding of video te wijzigen.
   * Klik op het selectievakje Voorinstellingen op alle selecteren om de voorinstelling die u hebt gekozen, toe te passen op alle aanbiedingen in de aanbiedingsset.

   Klik op **Opslaan** om de wijzigingen in de afbeelding of het videoaanbod op te slaan. Klik vervolgens op **Sluiten** om terug te keren naar de pagina Set Test&amp;Target-aanbiedingen.

1. Nadat u alle aanbiedingen voor de aanbiedingsset hebt gemaakt en de voorinstellingen voor afbeeldingen hebt gekozen, controleert u of **Publiceren na opslaan** is geselecteerd (standaard).
1. Klik op **Opslaan** en voer een naam in voor de aanbiedingsset en klik op **Opslaan**.

Druk voordat u de pagina Set Test&amp;Target-aanbiedingen sluit op Target Standard/Premium. Zie Aanbiedingsets [Pushing to Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set voorstellen bewerken {#editing-an-offer-set}

Afhankelijk van het feit of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, heeft de optie **Publiceren na opslaan** op de volgende manieren invloed op de set en stelt u leden in:

| Reeds gepubliceerd instellen? | De optie Publiceren na opslaan is geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |--- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden van een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen](publishing-files.md#manually_publishing_assets) handmatig publiceren en [elementen](publishing-files.md#manually_unpublishing_assets)handmatig verwijderen.

**Een set voorstellen bewerken**

1. Als u een aanbiedingsset wilt bewerken, geeft u de aanbieding weer die is ingesteld in de rasterweergave of de lijstweergave en klikt u op de **rolloverknop Bewerken** .
1. Voer een of meerdere van de volgende handelingen uit op de pagina Set Target-aanbiedingen testen:

   * **Een aanbieding** verwijderen Selecteer de aanbieding en klik vervolgens op 
**Schrap** om een aanbieding uit de reeks te verwijderen.
   * **Het toevoegen van een aanbieding** Hoe je een aanbieding toevoegt, hangt af van het soort voorstel dat je gebruikt:
   * **Sjablonen** klikken 
**Voeg een nieuwe aanbieding toe en geef een voorvertoning weer** en maak een nieuwe aanbieding op de pagina Aanbiedingen toevoegen en voorvertonen.
   * **Afbeeldingen en video&#39;s** Sleep een afbeelding of video naar de pagina Set Test&amp;Target-aanbiedingen.
   >[!NOTE]
   >
   >U kunt geen aanbiedingsreeks schrappen die met een campagne wordt geassocieerd. Als u een set aanbiedingen die aan een campagne is gekoppeld wilt verwijderen, meldt u zich aan bij Target Standard/Premium en verwijdert u eerst de campagnecoregelingen. Zelfs na het niet koppelen van een campagne kan het middel alleen worden verwijderd uit Dyanmische media Classic, waarvoor een aanmelding bij Target Standard/Premium is vereist, en niet uit Target Standard/Premium.

1. Als u klaar bent met bewerken, controleert u of **Publiceren na opslaan** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Klik op **Opslaan**, selecteer een opslagmap, voer een naam voor de set in en klik op **Opslaan**.

## Een set voorstellen verwijderen {#deleting-an-offer-set}

Wanneer u een set voorstellen verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen](publishing-files.md#manually_publishing_assets) handmatig publiceren en [elementen](publishing-files.md#manually_unpublishing_assets)handmatig verwijderen.

**Een set voorstellen verwijderen**

1. Selecteer in de rasterweergave, lijstweergave of detailweergave een of meer sets voorstellen.
1. Klik op de algemene navigatiebalk op **Bestand** > **Verwijderen** > **Verwijderen**.

>[!MORELIKETHIS]
>
>* [Sjabloonparameters maken](creating-template-parameters.md#creating_template_parameters)

