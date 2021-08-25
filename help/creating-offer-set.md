---
title: Een aanbiedingsset maken
description: Klik hier als je wilt weten hoe je een voorstel maakt dat is ingesteld in Dynamic Media Classic.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# Een aanbiedingsset maken {#creating-an-offer-set}

U kunt elk van de volgende soorten aanbiedingen maken:

* Video
* Parameterized malplaatje
* Afbeelding

Voor malplaatjes, selecteer **[!UICONTROL Add and Preview]**, dan plaats de parameters u kiest. De andere soorten aanbiedingsreeksen omvatten geen parameters, maar u kunt hen nog aanpassen door **[!UICONTROL Preview]** te selecteren en de beschikbare voorinstellingen te veranderen.

Dynamic Media Classic bevat gereedschappen voor bewerking en het maken van aanbiedingssets.

>[!NOTE]
>
>Voordat u een set voorstellen maakt, moet u alle elementen publiceren die u voor de set naar Dynamic Media Classic wilt gebruiken. Zie [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

## Soorten aanbiedingen {#types-of-offer-sets}

Maak een set aanbiedingen op basis van de volgende soorten aanbiedingen:

* **Afbeeldingen**  - U kunt afbeeldingen samenstellen voor een set aanbiedingen. Elke afbeelding bevat een andere aanbieding in de set.

* **Afbeeldingssjabloon**  - U kunt afbeeldingssjablonen in Dynamic Media Classic waarderen aan de hand van de opdracht Samenstellen > Sjabloonbasisbeginselen. Via parameters kunnen onderdelen van de sjabloon (de tekst in tekstkaders, de verschillende afbeeldingen) worden omgewisseld en aangepast. Voor een aanbiedingsreeks, kunt u malplaatjeparameters gebruiken om variaties op het zelfde beeld in uw aanbiedingsreeks tot stand te brengen, bijvoorbeeld. Zie Sjabloonparameters maken voor informatie over het maken van afbeeldingssjablonen en het toewijzen van parameters aan deze sjablonen.

* **Video**  - U kunt video samenstellen voor een aanbiedingsset. Elke video heeft een andere aanbieding in de set.

## Een aanbiedingsset maken met een geparametriseerde sjabloon {#creating-an-offer-set-with-a-parameterized-template}

Wanneer u een set voorstellen maakt, heeft de optie **[!UICONTROL Publish after save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL Publish after save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Om een aanbieding te creëren die met een parameterized malplaatje wordt geplaatst:**

1. Selecteer de sjabloon of banner.
1. Ga naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

   De pagina met de pagina Set voorstellen voor test&amp;doelaanbiedingen wordt weergegeven in de aangeboden set. Het eerste item in de lijst is het object.

1. Selecteer het object en selecteer **[!UICONTROL Add & Preview]**.

   De linkerkant van de pagina bevat parameters in de sjabloon en de bijbehorende waarden.

1. Wijzig parameterwaarden om de aanbieding te maken. Voer bijvoorbeeld andere tekst in een tekstveld in, wijzig de grootte van een laag, verander een afbeelding door een andere of kies een andere voorinstelling voor de viewer.
1. Selecteer **[!UICONTROL Save]** of **[!UICONTROL Save As**]** om de aanbieding als deel van de aanbiedingsreeks op te slaan.

   Op de pagina Set Test&amp;Target-voorstellen staan de aanbiedingen die u hebt gemaakt.

1. Herhaal stap 3 tot en met 5 om meer aanbiedingen voor de set te maken.
1. Als u klaar bent, controleert u of **[!UICONTROL Publish after save*]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Close]**, ga een naam voor de aanbiedingsreeks in, en selecteer dan **[!UICONTROL Save]**.

Druk op de aanbieding die is ingesteld op Adobe Target Standard/Premium voordat u de pagina Set Test&amp;Target-aanbiedingen sluit. Zie [Push-aanbiedingssets op Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set aanbiedingen maken met afbeeldingen of video&#39;s {#creating-an-offer-set-with-images-or-videos}

Wanneer u een set voorstellen maakt, heeft de optie **[!UICONTROL Publish after save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL Publish after save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set aanbiedingen maken met afbeeldingen of video&#39;s:**

1. Stel afbeeldingen of video&#39;s samen voor de ingestelde aanbieding. Begin in het Test&amp;Target Vastgestelde scherm van de Aanbieding of in de Mening van het Net of de Mening van de Lijst en gebruik één van de volgende methodes:

   * **Scherm**  Testi&amp;Target-aanbieding instellen - Ga naar  **[!UICONTROL Build]** >  **[!UICONTROL Test&Target Offer Set]**. Sleep afbeeldingen of video&#39;s naar het scherm. Als u video&#39;s of afbeeldingen van verschillende grootten wilt maken, sleept u in meerdere exemplaren van de afbeelding of video en stelt u elke grootte afzonderlijk in.

   * **Rasterweergave of Lijstweergave**  - Selecteer de afbeeldingen of video&#39;s en ga vervolgens naar  **[!UICONTROL Build]** >  **[!UICONTROL Test&Target Offer Set]**.

1. Selecteer desgewenst een afbeelding of video en selecteer **[!UICONTROL Preview]**. Op de pagina Voorvertoningsaanbiedingen kunt u de grootte en het uiterlijk wijzigen van de afbeelding of video die u hebt geselecteerd. U kunt ook alle afbeeldingen of video&#39;s in de set met aanbiedingen wijzigen.

   * Kies een voorinstelling om het uiterlijk en de grootte van de afbeelding of video te wijzigen.
   * Als u de voorinstelling die u hebt gekozen, wilt toepassen op alle aanbiedingen in de aanbiedingsset, schakelt u het selectievakje **[!UICONTROL Select Presets to All]** in.

   Selecteer **[!UICONTROL Save]** om uw wijzigingen in het beeld of de videoaanbieding op te slaan. Selecteer vervolgens **[!UICONTROL Close]** om terug te keren naar de pagina Set Test&amp;Target-aanbiedingen.

1. Nadat u alle aanbiedingen voor de aanbiedingsset hebt gemaakt en de voorinstellingen voor afbeeldingen hebt gekozen, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard).
1. Selecteer **[!UICONTROL Save]** en voer een naam voor de aanbiedingsreeks in, en selecteer **[!UICONTROL Save]**.

Druk voordat u de pagina Set Test&amp;Target-aanbiedingen sluit op Adobe Target Standard/Premium. Zie [Push-aanbiedingssets op Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een aanbiedingsset bewerken {#editing-an-offer-set}

Of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after save]** optie geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set voorstellen bewerken:**

1. Als u een aanbiedingsset wilt bewerken, geeft u de aanbieding weer die is ingesteld in de rasterweergave of lijstweergave en selecteert u de desbetreffende **[!UICONTROL Edit]**-rolloverknop.
1. Voer een of meerdere van de volgende handelingen uit op de pagina Set voorstel testen&amp;Doel:

   * **Een aanbieding**  verwijderen - Selecteer de aanbieding en kies  **[!UICONTROL Delete]** om een aanbieding uit de set te verwijderen.
   * **Een aanbieding**  toevoegen - Hoe je een aanbieding toevoegt, hangt af van het soort voorstel dat je gebruikt:
      * **Sjablonen**  - Selecteer  **[!UICONTROL Add & Preview]** en maak een andere aanbieding op de pagina Aanbiedingen toevoegen en voorvertonen.
      * **Afbeeldingen en video** : sleep een afbeelding of video naar de pagina Set Test&amp;Target-aanbiedingen.

   >[!NOTE]
   >
   >U kunt geen aanbiedingsreeks schrappen die met een campagne wordt geassocieerd. Als u een set aanbiedingen die aan een campagne is gekoppeld wilt verwijderen, meldt u zich aan bij Adobe Target Standard/Premium en verwijdert u eerst de campagnecorracties. Zelfs nadat u zich niet aan een campagne hebt gekoppeld, kan het middel alleen worden verwijderd uit Dynamic Media Classic, waarvoor u zich moet aanmelden bij Adobe Target Standard/Premium, en niet uit Adobe Target Standard/Premium.

1. Als u klaar bent met bewerken, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]**, selecteer een opslagomslag, ga een naam voor de reeks in, en selecteer dan **[!UICONTROL Save]**.

## Een aanbiedingsset verwijderen {#deleting-an-offer-set}

Wanneer u een set voorstellen verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een aanbiedingsset verwijderen:**

1. Selecteer in de rasterweergave, de lijstweergave of de detailweergave een of meer aanbiedingssets.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Delete**.

>[!MORELIKETHIS]
>
>* [Sjabloonparameters maken](creating-template-parameters.md#creating_template_parameters)

