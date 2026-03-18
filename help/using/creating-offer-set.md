---
title: Een set voorstellen maken
description: Leer hoe u een set voorstellen maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: 458a80aad6e983dbccfe2108f0a389a4651f9f38
workflow-type: tm+mt
source-wordcount: '1216'
ht-degree: 0%

---

# Een set voorstellen maken {#creating-an-offer-set}

U kunt elk van de volgende soorten sets voorstellen maken:

* Video
* Parameterized malplaatje
* Afbeelding

Selecteer **[!UICONTROL Add and Preview]** voor sjablonen en stel vervolgens de parameters in die u kiest. Andere typen Aanbiedingssets bevatten geen parameters, maar u kunt deze nog steeds aanpassen door **[!UICONTROL Preview]** te selecteren en de beschikbare voorinstellingen te wijzigen.

Adobe Dynamic Media Classic biedt tools voor bewerking en het maken van offsets.

>[!NOTE]
>
>Voordat u een set voorstellen maakt, moet u alle elementen publiceren die u voor de set op Adobe Dynamic Media Classic wilt gebruiken. Zie [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

## Soorten aanbiedingssets {#types-of-offer-sets}

Maak een set aanbiedingen op basis van de volgende typen aanbiedingen:

* **Beelden**: U kunt beelden voor een Reeks van de Aanbieding assembleren. Elke afbeelding bevat een andere aanbieding in de set.

* **malplaatje van het Beeld**: U kunt van beeldmalplaatjes in Adobe Dynamic Media Classic parameters bepalen met **[!UICONTROL Build]** > het bevel van de Grondbeginselen van het Malplaatje. Via parameters kunnen onderdelen van de sjabloon, de tekst in tekstkaders en de verschillende afbeeldingen worden omgewisseld en aangepast. Voor een set aanbiedingen kunt u sjabloonparameters gebruiken om bijvoorbeeld variaties te maken op dezelfde afbeelding in de set met aanbiedingen. Voor informatie over het creëren van en het bepalen van parameters van beeldmalplaatjes, zie [&#x200B; malplaatjeparameters &#x200B;](creating-template-parameters.md#creating_template_parameters) creëren.

Zie ook [&#128279;](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) de opleidingsvideo van de Grondbeginselen van het 0&rbrace; Malplaatje &lbrace;.

* **Video**: U kunt video voor een Reeks van de Aanbieding assembleren. Elke video heeft een andere aanbieding in de set.

## Een set voorstellen maken met een geparametriseerde sjabloon {#creating-an-offer-set-with-a-parameterized-template}

Wanneer u een set voorstellen maakt, heeft de optie **[!UICONTROL Publish after a save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL Publish after a save]** geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Aanbieding tot stand te brengen die met een geparameterized malplaatje wordt geplaatst:**

1. Selecteer de sjabloon of banner.
1. Ga naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]** .

   De pagina met de paginaset Test&amp;Target-aanbod wordt weergegeven met de aanbiedingen in de set Aanbiedingen. Het eerste item in de lijst is het object.

1. Selecteer het object en selecteer **[!UICONTROL Add & Preview]** .

   De linkerkant van de pagina bevat parameters in de sjabloon en de bijbehorende waarden.

1. Wijzig parameterwaarden om de aanbieding te maken. Voer bijvoorbeeld andere tekst in een tekstveld in, wijzig de grootte van een laag, wijzig de ene afbeelding in een andere of kies een andere voorinstelling voor de viewer.
1. Selecteer **[!UICONTROL Save]** of **[!UICONTROL Save As**]** om het aanbod op te slaan als onderdeel van de set met voorstellen.

   Op de pagina Set Test&amp;Target-voorstellen staan de aanbiedingen die u hebt gemaakt.

1. Herhaal stap 3 tot en met 5 om meer aanbiedingen voor de set te maken.
1. Als u klaar bent, controleert u of **[!UICONTROL Publish after a save*]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Close]**, voer een naam in voor de set met voorstellen en selecteer vervolgens **[!UICONTROL Save]** .

Voordat u de pagina Set Test&amp;Target-aanbiedingen sluit, drukt u op de optie Aanbiedingsset op Adobe Target Standard/Premium. Zie [&#x200B; de Reeksen van het Aanbod van de Duw aan Test&amp;Doel &#x200B;](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set aanbiedingen maken met afbeeldingen of video&#39;s {#creating-an-offer-set-with-images-or-videos}

Wanneer u een set voorstellen maakt, heeft de optie **[!UICONTROL Publish after a save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL Publish after a save]** geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Reeks van de Aanbieding met beelden of video&#39;s tot stand te brengen:**

1. Stel afbeeldingen of video&#39;s samen voor de set met voorstellen. Begin in het Test&amp;Target Vastgestelde scherm van de Aanbieding of in de Mening van het Net of de Mening van de Lijst en gebruik één van de volgende methodes:

   * **de Reeks scherm van de Aanbieding van de Test&amp;Doel**: Ga naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**. Sleep afbeeldingen of video&#39;s naar het scherm. Als u video&#39;s of afbeeldingen van verschillende grootten wilt maken, sleept u in meerdere exemplaren van de afbeelding of video en stelt u elke grootte afzonderlijk in.

   * **de Mening van het Net of de Mening van de Lijst**: Selecteer de beelden of de video&#39;s, en ga dan naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

1. Selecteer desgewenst een afbeelding of video en selecteer **[!UICONTROL Preview]** . Op de pagina Voorvertoningsaanbiedingen kunt u de grootte en het uiterlijk wijzigen van de afbeelding of video die u hebt geselecteerd. U kunt ook alle afbeeldingen of video&#39;s in de set Aanbiedingen wijzigen.

   * Kies een voorinstelling om het uiterlijk en de grootte van de afbeelding of video te wijzigen.
   * Schakel het selectievakje **`Select Presets to All`** in als u de voorinstelling die u hebt gekozen, wilt toepassen op alle aanbiedingen in de set Aanbiedingen.

   Selecteer **[!UICONTROL Save]** om uw wijzigingen in de afbeelding of het videoaanbod op te slaan. Selecteer vervolgens **[!UICONTROL Close]** om terug te keren naar de pagina Set Test&amp;Target-aanbiedingen.

1. Nadat u alle aanbiedingen voor de set Aanbiedingen hebt gemaakt en de voorinstellingen voor afbeeldingen hebt gekozen, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteer **[!UICONTROL Save]** , voer een naam in voor de set met voorstellen en selecteer **[!UICONTROL Save]** .

Voordat u de pagina Set Test&amp;Target-aanbiedingen sluit, drukt u op de optie Aanbiedingsset op Adobe Target Standard/Premium. Zie [&#x200B; de Reeksen van het Aanbod van de Duw aan Test&amp;Doel &#x200B;](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set voorstellen bewerken {#editing-an-offer-set}

Of u nu een gepubliceerde set of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after a save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after a save]** geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Reeks van de Aanbieding uit te geven:**

1. Als u een set voorstellen wilt bewerken, geeft u de set Aanbiedingen weer in de rasterweergave of de lijstweergave en selecteert u vervolgens de **[!UICONTROL Edit]** rolloverknop.
1. Voer een of meerdere van de volgende handelingen uit op de pagina Set voorstel testen&amp;Doel:

   * **Verwijderend een aanbieding**: Selecteer de aanbieding, en selecteer dan **[!UICONTROL Delete]** om een aanbieding uit de reeks te verwijderen.
   * **Toevoegend een aanbieding**: Hoe u een aanbieding toevoegt hangt van het type van Vastgestelde Aanbieding af u met werkt:
      * **Malplaatjes**: Selecteer **[!UICONTROL Add & Preview]**, en op Add &amp; de pagina van de Aanbiedingen van de Voorproef, creeer een andere aanbieding.
      * **Beelden en video&#39;s**: Sleep een beeld of een video op de Test&amp;Target Vastgestelde pagina van de Aanbieding.

   >[!NOTE]
   >
   >U kunt geen set voorstellen verwijderen die aan een campagne is gekoppeld. Als u een set voorstellen die aan een campagne is gekoppeld, wilt verwijderen, meldt u zich aan bij Adobe Target Standard/Premium en verwijdert u eerst de koppeling naar de campagne. Zelfs nadat u zich niet aan een campagne hebt gekoppeld, kan het actief alleen uit Adobe Dynamic Media Classic worden verwijderd, waarvoor een aanmelding bij Adobe Target Standard/Premium vereist is, en niet vanuit Adobe Target Standard/Premium.

1. Als u klaar bent met bewerken, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]** , selecteer een opslagmap, voer een naam voor de set in en selecteer vervolgens **[!UICONTROL Save]** .

## Een aangeboden set verwijderen {#delet-an-offer-set}

Wanneer u een set voorstellen verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Reeks van de Aanbieding te schrappen:**

1. Selecteer in de rasterweergave, de lijstweergave of de detailweergave een of meer sets voorstellen.
1. Voor de Globale Bar van de Navigatie, ga **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Schrapping**.

>[!MORELIKETHIS]
>
>* [&#x200B; Creërend malplaatjeparameters &#x200B;](creating-template-parameters.md#creating_template_parameters)
