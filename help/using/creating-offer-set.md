---
title: Een set voorstellen maken
description: Leer hoe u een set voorstellen maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 0%

---

# Een set voorstellen maken {#creating-an-offer-set}

U kunt elk van de volgende soorten sets voorstellen maken:

* Video
* Parameterized malplaatje
* Afbeelding

Selecteer voor sjablonen de optie **[!UICONTROL Add and Preview]** stelt u vervolgens de gewenste parameters in. Andere soorten Aanbiedingsreeks bevatten geen parameters, maar u kunt deze nog steeds aanpassen door **[!UICONTROL Preview]** en wijzigt u de beschikbare voorinstellingen.

Adobe Dynamic Media Classic biedt tools voor bewerking en het maken van offsets.

>[!NOTE]
>
>Voordat u een set voorstellen maakt, moet u alle elementen publiceren die u voor de set op Adobe Dynamic Media Classic wilt gebruiken. Zie [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

## Soorten aanbiedingssets {#types-of-offer-sets}

Maak een set aanbiedingen op basis van de volgende typen aanbiedingen:

* **Afbeeldingen**: U kunt afbeeldingen samenstellen voor een set voorstellen. Elke afbeelding bevat een andere aanbieding in de set.

* **Afbeeldingssjabloon**: U kunt in Adobe Dynamic Media Classic parameters instellen voor afbeeldingssjablonen met de opdracht **[!UICONTROL Build]** > Sjabloonbasisbeginselen, opdracht. Via parameters kunnen onderdelen van de sjabloon, de tekst in tekstkaders en de verschillende afbeeldingen worden omgewisseld en aangepast. Voor een set aanbiedingen kunt u sjabloonparameters gebruiken om bijvoorbeeld variaties te maken op dezelfde afbeelding in de set met aanbiedingen. Voor informatie over het maken van afbeeldingssjablonen en het bepalen van parameters, raadpleegt u [Sjabloonparameters maken](creating-template-parameters.md#creating_template_parameters).

Zie ook [Grondbeginselen van sjablonen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) trainingsvideo.

* **Video**: U kunt video samenstellen voor een set voorstellen. Elke video heeft een andere aanbieding in de set.

## Een set voorstellen maken met een geparametriseerde sjabloon {#creating-an-offer-set-with-a-parameterized-template}

Wanneer u een set aanbiedingen maakt, worden de **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| **[!UICONTROL Publish after a save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set voorstellen maken met een sjabloon met parameters:**

1. Selecteer de sjabloon of banner.
1. Ga naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

   De pagina met de paginaset Test&amp;Target-aanbod wordt weergegeven met de aanbiedingen in de set Aanbiedingen. Het eerste item in de lijst is het object.

1. Selecteer het object en selecteer **[!UICONTROL Add & Preview]**.

   De linkerkant van de pagina bevat parameters in de sjabloon en de bijbehorende waarden.

1. Wijzig parameterwaarden om de aanbieding te maken. Voer bijvoorbeeld andere tekst in een tekstveld in, wijzig de grootte van een laag, wijzig de ene afbeelding in een andere of kies een andere voorinstelling voor de viewer.
1. Selecteren **[!UICONTROL Save]** of **[!UICONTROL Save As**]** om het voorstel op te slaan als onderdeel van de set voorstellen.

   Op de pagina Set Test&amp;Target-voorstellen staan de aanbiedingen die u hebt gemaakt.

1. Herhaal stap 3 tot en met 5 om meer aanbiedingen voor de set te maken.
1. Wanneer u klaar bent, gaat u naar de rechterbenedenhoek van de pagina en zorgt u ervoor dat **[!UICONTROL Publish after a save*]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Close]** voert u een naam in voor de set Aanbiedingen en selecteert u **[!UICONTROL Save]**.

Voordat u de pagina Set Test&amp;Target-aanbiedingen sluit, drukt u op de optie Aanbiedingsset op Adobe Target Standard/Premium. Zie [Stelt&amp;s voor pushaanbiedingen in op testen](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set aanbiedingen maken met afbeeldingen of video&#39;s {#creating-an-offer-set-with-images-or-videos}

Wanneer u een set aanbiedingen maakt, worden de **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| **[!UICONTROL Publish after a save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set voorstellen maken met afbeeldingen of video&#39;s:**

1. Stel afbeeldingen of video&#39;s samen voor de set met voorstellen. Begin in het Test&amp;Target Vastgestelde scherm van de Aanbieding of in de Mening van het Net of de Mening van de Lijst en gebruik één van de volgende methodes:

   * **Scherm Aanbiedingset &amp;testen**: Ga naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**. Sleep afbeeldingen of video&#39;s naar het scherm. Als u video&#39;s of afbeeldingen van verschillende grootten wilt maken, sleept u in meerdere exemplaren van de afbeelding of video en stelt u elke grootte afzonderlijk in.

   * **Rasterweergave of Lijstweergave**: Selecteer de afbeeldingen of video&#39;s en ga naar **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

1. Selecteer desgewenst een afbeelding of video en selecteer **[!UICONTROL Preview]**. Op de pagina Voorvertoningsaanbiedingen kunt u de grootte en het uiterlijk wijzigen van de afbeelding of video die u hebt geselecteerd. U kunt ook alle afbeeldingen of video&#39;s in de set Aanbiedingen wijzigen.

   * Kies een voorinstelling om het uiterlijk en de grootte van de afbeelding of video te wijzigen.
   * Als u de voorinstelling die u hebt gekozen, wilt toepassen op alle aanbiedingen in de set Aanbiedingen, selecteert u de optie **[!UICONTROL Select Presets to All]** selectievakje.

   Selecteren **[!UICONTROL Save]** om uw wijzigingen in de afbeelding of het videoaanbod op te slaan. Selecteer vervolgens **[!UICONTROL Close]** om terug te keren naar de pagina Set Test&amp;Target-aanbiedingen.

1. Nadat u alle aanbiedingen voor de set Aanbiedingen hebt gemaakt en Voorinstellingen afbeelding hebt gekozen voor verschillende afbeeldingen, zorgt u ervoor dat **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]** en voer een naam in voor de set voorstellen en selecteer **[!UICONTROL Save]**.

Voordat u de pagina Set Test&amp;Target-aanbiedingen sluit, drukt u op de optie Aanbiedingsset op Adobe Target Standard/Premium. Zie [Stelt&amp;s voor pushaanbiedingen in op testen](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Een set voorstellen bewerken {#editing-an-offer-set}

Of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after a save]** optie geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set voorstellen bewerken:**

1. Als u een set voorstellen wilt bewerken, geeft u de set voorstellen weer in de rasterweergave of de lijstweergave en selecteert u de desbetreffende **[!UICONTROL Edit]** rolloverknop.
1. Voer een of meerdere van de volgende handelingen uit op de pagina Set voorstel testen&amp;Doel:

   * **Een aanbieding verwijderen**: Selecteer de aanbieding en selecteer vervolgens **[!UICONTROL Delete]** om een voorstel uit de set te verwijderen.
   * **Een voorstel toevoegen**: Hoe u een aanbieding toevoegt, hangt af van het type Aanbieding dat u gebruikt:
      * **Sjablonen**: Select **[!UICONTROL Add & Preview]** en maak op de pagina Aanbiedingen toevoegen en voorvertonen nog een voorstel.
      * **Afbeeldingen en video&#39;s**: Sleep een afbeelding of video naar de pagina Set Test&amp;Target-aanbiedingen.

   >[!NOTE]
   >
   >U kunt geen set voorstellen verwijderen die aan een campagne is gekoppeld. Als u een set voorstellen die aan een campagne is gekoppeld, wilt verwijderen, meldt u zich aan bij Adobe Target Standard/Premium en verwijdert u eerst de koppeling naar de campagne. Zelfs nadat u zich niet aan een campagne hebt gekoppeld, kan het actief alleen uit Adobe Dynamic Media Classic worden verwijderd, waarvoor een aanmelding bij Adobe Target Standard/Premium vereist is, en niet vanuit Adobe Target Standard/Premium.

1. Wanneer u klaar bent met bewerken, gaat u naar de rechterbenedenhoek van de pagina en controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**, selecteert u een opslagmap, voert u een naam voor de set in en selecteert u **[!UICONTROL Save]**.

## Een aangeboden set verwijderen {#delet-an-offer-set}

Wanneer u een set voorstellen verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een set voorstellen verwijderen:**

1. Selecteer in de rasterweergave, de lijstweergave of de detailweergave een of meer sets voorstellen.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Verwijderen**.

>[!MORELIKETHIS]
>
>* [Sjabloonparameters maken](creating-template-parameters.md#creating_template_parameters)
