---
title: Een eCatalog maken
description: Leer hoe u een eCatalog maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Een eCatalog maken {#creating-an-ecatalog}

Als u een eCatalog maakt, moet u de pagina&#39;s ordenen, de paginalay-out kiezen en de pagina&#39;s koppelen door Afbeeldingen met hyperlinks te tekenen. Hiervoor moeten ook gegevens voor rollover- en hypertextkoppelingen worden ingevoerd. Desgewenst kunt u de inhoudsopgave aanpassen, zodat de viewers de paginanamen in plaats van de paginanummers in de eCatalog-viewer kunnen zien.

## Een eCatalog maken {#create}

U kunt afbeeldingsbestanden en PDF-bestanden opnemen in uw eCatalog.

Wanneer u een eCatalog maakt, beïnvloedt de optie **[!UICONTROL Publish after a save]** de reeks en plaatst leden op de volgende manieren:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een eCatalog tot stand te brengen:**

1. Maak uw eCatalog met een van de volgende technieken:

   * **selecteer eerst de dossiers**: In het Browse paneel, selecteer dossiers en ga dan naar **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Begin van het eCatalog scherm**: Ga naar **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Selecteer een map in de elementenbibliotheek. Sleep bestanden van de map naar het tabblad Order Pages van de pagina eCatalog.

     >[!NOTE]
     >
     >Als u de items in de elementenbibliotheek op naam wilt weergeven in plaats van op miniatuur, selecteert u de optie Naam voor de weergave Standaard in de elementenbibliotheek in Persoonlijke instellingen.

1. Selecteer een algemene lay-out voor uw eCatalog. Selecteer **[!UICONTROL 1 Up]** voor enkele pagina&#39;s, **[!UICONTROL 2 Up]** voor spreads met twee pagina&#39;s of **[!UICONTROL Custom]** voor spreads met meer dan twee pagina&#39;s. Selecteer in het dialoogvenster **[!UICONTROL Change eCatalog Layout]** de **[!UICONTROL All Spreads]** -opties en selecteer **[!UICONTROL OK]** .
1. U kunt desgewenst de indeling van afzonderlijke pagina&#39;s of paginaspread wijzigen door deze te selecteren en vervolgens **[!UICONTROL 1 Up]** , **[!UICONTROL 2 Up]** of **[!UICONTROL Custom]** te kiezen. Selecteer in het dialoogvenster **[!UICONTROL Change eCatalog Layout]** de **[!UICONTROL Selected Spreads]** -opties en selecteer **[!UICONTROL OK]** .
1. U kunt de pagina&#39;s op een van de volgende manieren opnieuw ordenen:

   * **het slepen**: Sleep een pagina of een paginaspread aan een nieuwe plaats. Op de verticale balk ziet u waar de pagina wordt verplaatst.

   * **Beweging aan knoop**: Selecteer een pagina of een paginaspread, selecteer **[!UICONTROL Move To]**, en kies de pagina op het menu dat u uw pagina vóór wilt verschijnen.

   * **Opeenvolging #**: In de Mening van de Lijst, ga paginaaantallen op de gebieden van Opeenvolging # in.

1. Als u klaar bent, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]** .
1. Selecteer in het dialoogvenster Opslaan een map voor het opslaan van uw eCatalog. Voer in het veld Bestandsnaam de naam van de centrifugeset in.
1. Selecteer **[!UICONTROL Save]** .

   U kunt een voorvertoning van de eCatalog weergeven nadat u deze hebt opgeslagen door **[!UICONTROL Preview]** te selecteren.

## Een eCatalog bewerken {#editing-an-ecatalog}

Of u nu een gepubliceerde set of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after a save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | De optie Publiceren na opslaan is geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een eCatalog uit te geven:**

1. Selecteer de rollover-knop van de eCatalog **[!UICONTROL Edit]** .
1. Breng de gewenste wijzigingen aan.
1. Als u klaar bent met bewerken, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]** , selecteer een opslagmap, voer een naam voor de set in en selecteer vervolgens **[!UICONTROL Save]** .

## Een eCatalog verwijderen

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een eCatalog te schrappen:**

1. Selecteer een of meer eCatalogi in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** .

## De inhoudsopgave aanpassen {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic biedt standaardpaginanummers in uw eCatalog op het tabblad Order Pages van het eCatalog-scherm. Voor aangepaste paginanamen kunt u de paginalabels wijzigen die de inhoudsopgave vormen. Het wordt aanbevolen de naam van de voor- en achteromslag te wijzigen. De voorpagina kan bijvoorbeeld &quot;Omslag&quot; in plaats van &quot;Pagina 0-1&quot; lezen.

U kunt handmatig een aangepaste inhoudsopgave (TOC) voor uw eCatalog maken. U kunt de paginanamen ook importeren vanuit een CSV- (alleen Mac) of XML-bestand.

>[!NOTE]
>
>Als u de standaardpaginatitels wilt herstellen, selecteert u op het tabblad **[!UICONTROL Order Pages]** **[!UICONTROL TOC Labels]** en selecteert u vervolgens **[!UICONTROL Restore Defaults (All)]** .

### Paginanamen handmatig invoeren {#manually-entering-page-names}

Voer handmatig paginanamen een voor een in door naar het tabblad Order Pages van het eCatalog-scherm te gaan. Voer vervolgens in het veld Paginanummer een naam in voor elke pagina die u een naam wilt geven.

### Paginanamen importeren {#importing-page-names}

Het wordt aanbevolen paginanamen te importeren als u te maken hebt met een eCatalog met veel pagina&#39;s. U kunt de namen importeren uit een door tabs gescheiden of XML-bestand.

Het label van de inhoudsopgave wordt opgeslagen in het veld Gebruikersgegevens van een afbeelding. Gebruik deze gegevens als een lijst van `name=<value>` ` pairs separated by two question marks "??" ` . Als u bijvoorbeeld één label wilt instellen voor een inhoudsopgaveveld met de naam `tocEN` , stelt u de gebruikersgegevens van de afbeelding in op:

`tocEN=&lt;EN_page_label>`

Als u afzonderlijke labels wilt instellen voor inhoudsopgavevelden met de namen `tocEN` en `tocFR` :

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Als u het veld Gebruikersgegevens wilt importeren in een door tabs gescheiden bestand, neemt u de gebruikersgegevens van het veld op:

| IPSID | Gebruikersgegevens |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Als u het veld Gebruikersgegevens wilt importeren in een XML-bestand, neemt u het kenmerk `vc_userdata` op:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Als u paginanamen wilt importeren uit een door tabs gescheiden of XML-bestand, selecteert u de knop **[!UICONTROL TOC Labels]** en selecteert u **[!UICONTROL Import]** . Selecteer **[!UICONTROL Browse]** in het dialoogvenster Metagegevens uploaden en importeer vervolgens het CSV-bestand (alleen Mac) of het XML-bestand dat elke pagina aan een paginanaam koppelt.
