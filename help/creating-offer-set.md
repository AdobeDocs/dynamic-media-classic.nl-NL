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
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---


# Een aanbiedingsset maken{#creating-an-offer-set}

U kunt elk van de volgende soorten aanbiedingen maken:

* Video
* Parameterized malplaatje
* Afbeelding

Voor malplaatjes, klik **toevoegen en Voorproef**, dan plaats de parameters u kiest. De andere soorten aanbiedingen omvatten geen parameters, maar u kunt hen nog aanpassen door **Voorproef** te klikken en de beschikbare voorinstellingen te veranderen.

Dynamic Media Classic bevat gereedschappen voor bewerking en het maken van aanbiedingssets.

>[!NOTE]
>
>Voordat u een set voorstellen maakt, moet u alle elementen publiceren die u voor de set naar Dynamic Media Classic wilt gebruiken. Zie [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

## Soorten aanbiedingsreeksen {#types-of-offer-sets}

Maak een set aanbiedingen op basis van de volgende soorten aanbiedingen:

* ****
AfbeeldingenU kunt afbeeldingen samenstellen voor een set aanbiedingen. Elke afbeelding bevat een andere aanbieding in de set.

* **AfbeeldingssjabloonU kunt**
afbeeldingssjablonen in Dynamic Media Classic waarderen met de opdracht Samenstellen > Sjabloonbasisbeginselen. Via parameters kunnen onderdelen van de sjabloon (de tekst in tekstkaders, de verschillende afbeeldingen) worden omgewisseld en aangepast. Voor een aanbiedingsreeks, kunt u malplaatjeparameters gebruiken om variaties op het zelfde beeld in uw aanbiedingsreeks tot stand te brengen, bijvoorbeeld. Zie Sjabloonparameters maken voor informatie over het maken van afbeeldingssjablonen en het toewijzen van parameters aan deze sjablonen.

* ****
VideoU kunt video samenstellen voor een aanbiedingsset. Elke video heeft een andere aanbieding in de set.

## Een aanbieding maken die is ingesteld met een geparametriseerde sjabloon {#creating-an-offer-set-with-a-parameterized-template}

Wanneer u een set voorstellen maakt, heeft de optie **Publiceren na opslaan** invloed op de set en stelt u leden op de volgende manieren in:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een aanbieding maken die is ingesteld met een geparametriseerde sjabloon**

1. Selecteer de sjabloon of banner.
1. Klik **Build** > **Test&amp;Target Offerset**.

   De pagina met de pagina Set voorstellen voor test&amp;doelaanbiedingen wordt weergegeven in de aangeboden set. Het eerste item in de lijst is het object.

1. Selecteer het object en klik op **Toevoegen en voorvertonen**.

   De linkerkant van de pagina bevat parameters in de sjabloon en de bijbehorende waarden.

1. Wijzig parameterwaarden om de aanbieding te maken. Voer bijvoorbeeld andere tekst in een tekstveld in, wijzig de grootte van een laag, verander een afbeelding door een andere of kies een andere voorinstelling voor de viewer.
1. Klik op **Opslaan** of **Opslaan als** om het aanbod op te slaan als onderdeel van de aanbiedingsset.

   Op de pagina Set Test&amp;Target-voorstellen staan de aanbiedingen die u hebt gemaakt.

1. Herhaal stap 3 tot en met 5 om meer aanbiedingen voor de set te maken.
1. Als u klaar bent, controleert u of u in de rechterbenedenhoek van de pagina **Publiceren na opslaan** hebt geselecteerd (standaardinstelling).
1. Klik **Close**, ga een naam voor de aanbiedingsreeks in, en klik dan **Save**.

Voordat u de pagina Set Test&amp;Target-aanbiedingen sluit, drukt u op de aanbieding die is ingesteld op Target Standard/Premium. Zie [Push-aanbiedingssets op Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set aanbiedingen maken met afbeeldingen of video&#39;s {#creating-an-offer-set-with-images-or-videos}

Wanneer u een set voorstellen maakt, heeft de optie **Publiceren na opslaan** invloed op de set en stelt u leden op de volgende manieren in:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set aanbiedingen maken met afbeeldingen of video&#39;s**

1. Stel afbeeldingen of video&#39;s samen voor de ingestelde aanbieding. Begin in het Test&amp;Target Vastgestelde scherm van de Aanbieding of in de Mening van het Net of de Mening van de Lijst en gebruik één van de volgende methodes:

   * **Test&amp;Target-aanbieding instellen**
op schermKlikken  **[!UICONTROL Build > Test&Target Offer Set]**. Sleep afbeeldingen of video&#39;s naar het scherm. Als u video&#39;s of afbeeldingen van verschillende grootten wilt maken, sleept u in meerdere exemplaren van de afbeelding of video en stelt u elke grootte afzonderlijk in.

   * **De raster- of lijstweergave**
Selecteer de afbeeldingen of video&#39;s en klik op  **[!UICONTROL Build > Test&Target Offer Set]**.

1. Selecteer desgewenst een afbeelding of video en klik op **Voorvertoning**. Op de pagina Voorvertoningsaanbiedingen kunt u de grootte en het uiterlijk wijzigen van de afbeelding of video die u hebt geselecteerd. U kunt ook alle afbeeldingen of video&#39;s in de set met aanbiedingen wijzigen.

   * Kies een voorinstelling om het uiterlijk en de grootte van de afbeelding of video te wijzigen.
   * Klik op het selectievakje Voorinstellingen op alle selecteren om de voorinstelling die u hebt gekozen, toe te passen op alle aanbiedingen in de aanbiedingsset.

   Klik op **Opslaan** om uw wijzigingen in de afbeelding of videopresentatie op te slaan. Klik vervolgens op **Close** om terug te keren naar de pagina Set Test&amp;Target-aanbod.

1. Nadat u alle aanbiedingen voor de aanbiedingsset hebt gemaakt en de voorinstellingen voor afbeeldingen hebt gekozen, controleert u of **Publiceren na opslaan** is geselecteerd (standaard).
1. Klik **Opslaan** en voer een naam in voor de aanbiedingsset en klik op **Opslaan**.

Voordat u de pagina Set Test&amp;Target-aanbiedingen sluit, drukt u op de aanbieding die is ingesteld op Target Standard/Premium. Zie [Push-aanbiedingssets op Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set voorstellen bewerken {#editing-an-offer-set}

Afhankelijk van het feit of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, beïnvloedt de optie **Publiceren na opslaan** de set en stelt u de leden als volgt in:

| Reeds gepubliceerd instellen? | De optie Publiceren na opslaan is geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |--- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden van een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set voorstellen bewerken**

1. Als u een aanbiedingsset wilt bewerken, geeft u de aanbieding weer die is ingesteld in de rasterweergave of lijstweergave en klikt u op de desbetreffende **rolloverknop Bewerken**.
1. Voer een of meerdere van de volgende handelingen uit op de pagina Set voorstel testen&amp;Doel:

   * **Een**
aanbieding verwijderenSelecteer de aanbieding en klik vervolgens op 
**Schrap** om een aanbieding uit de reeks te verwijderen.
   * **Het toevoegen van een**
aanbiedingHoe u een aanbieding toevoegt hangt van het type van aanbieding af u met werkt:
   * ****
TemplatesClick 
**Voeg een nieuwe aanbieding toe en geef een voorbeeld** weer en maak op de pagina Aanbiedingen toevoegen en bekijken een nieuwe aanbieding.
   * **Afbeeldingen en**
video&#39;sSleep een afbeelding of video naar de pagina Set Test&amp;Target-aanbiedingen.
   >[!NOTE]
   >
   >U kunt geen aanbiedingsreeks schrappen die met een campagne wordt geassocieerd. Als u een aanbiedingsset wilt verwijderen die is gekoppeld aan een campagne, meldt u zich aan bij Target Standard/Premium en verwijdert u eerst de campagnecategorieën. Zelfs na het niet koppelen van een campagne kan het middel alleen worden verwijderd uit Dyanmische media Classic, waarvoor een aanmelding bij Target Standard/Premium vereist is, en niet uit Target Standard/Premium.

1. Wanneer u klaar bent met bewerken, controleert u of **Publiceren na opslaan** is geselecteerd (standaard).
1. Klik **Opslaan**, selecteer een opslagmap, voer een naam voor de set in en klik op **Opslaan**.

## Een aangeboden set {#deleting-an-offer-set} verwijderen

Wanneer u een set voorstellen verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set voorstellen verwijderen**

1. Selecteer in de rasterweergave, lijstweergave of detailweergave een of meer sets voorstellen.
1. Klik op **Bestand** > **Verwijderen** > **Verwijderen** op de algemene navigatiebalk.

>[!MORELIKETHIS]
>
>* [Sjabloonparameters maken](creating-template-parameters.md#creating_template_parameters)

