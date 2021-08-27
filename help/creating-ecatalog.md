---
title: Een eCatalog maken
description: Leer hoe u een eCatalog maakt in Adobe Dynamic Media Classic.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# Een eCatalog maken {#creating-an-ecatalog}

Als u een eCatalog maakt, moet u de pagina&#39;s ordenen, de paginalay-out kiezen en de pagina&#39;s koppelen door Afbeeldingen met hyperlinks te tekenen en rollover- en hypertekstkoppelingsgegevens in te voeren. Desgewenst kunt u de inhoudsopgave aanpassen, zodat de viewers de paginanamen in plaats van de paginanummers in de eCatalog-viewer kunnen zien.

## Een eCatalog maken {#create}

U kunt afbeeldingsbestanden en PDF-bestanden opnemen in uw eCatalog.

Wanneer u een eCatalog creeert, beïnvloedt de **[!UICONTROL Publish after save]** optie de reeks en vastgestelde leden op de volgende manieren:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een eCatalog maken:**

1. Maak uw eCatalog met een van de volgende technieken:

   * **Selecteer eerst**  de bestanden in het deelvenster Bladeren en selecteer vervolgens de gewenste bestanden. Ga vervolgens naar  **[!UICONTROL Build]** >  **[!UICONTROL eCatalogs]**.

   * **Begin in het eCatalog-scherm**  - Ga naar  **[!UICONTROL Build]** >  **[!UICONTROL eCatalogs]**. Selecteer een map in de elementenbibliotheek en sleep bestanden van de map naar het tabblad Order Pages op de pagina eCatalog.

      >[!NOTE]
      >
      >Als u de items in de elementenbibliotheek op naam wilt weergeven in plaats van op miniatuur, selecteert u de optie Naam voor de weergave Standaard in de elementenbibliotheek in Persoonlijke instellingen.

1. Selecteer een algemene lay-out voor uw eCatalog. Selecteer **[!UICONTROL 1 Up]** voor enkele pagina&#39;s, **[!UICONTROL 2 Up]** voor spreads met twee pagina&#39;s of **[!UICONTROL Custom]** voor spreads met meer dan twee pagina&#39;s. Selecteer in het dialoogvenster **[!UICONTROL Change eCatalog Layout]** de opties **[!UICONTROL All Spreads]** en selecteer **[!UICONTROL OK]**.
1. Wijzig desgewenst de indeling van afzonderlijke pagina&#39;s of paginaspread door deze te selecteren en vervolgens **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** of **[!UICONTROL Custom]** te kiezen. Selecteer in het dialoogvenster **[!UICONTROL Change eCatalog Layout]** de opties **[!UICONTROL Selected Spreads]** en selecteer **[!UICONTROL OK]**.
1. U kunt de pagina&#39;s op een van de volgende manieren opnieuw ordenen:

   * **Slepen**  - Sleep een pagina of paginaspread naar een nieuwe locatie. Op de verticale balk ziet u waar de pagina wordt verplaatst.

   * **Ga naar knop**  - Selecteer een pagina of paginaspread, selecteer  **[!UICONTROL Move To]** en kies de pagina in het menu die u wilt weergeven vóór.

   * **Reeks #** - in de Mening van de Lijst, ga paginaaantallen in de Reeks # gebieden in.

1. Als u klaar bent, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]**.
1. Selecteer in het dialoogvenster Opslaan een map voor het opslaan van uw eCatalog. Voer in het veld Bestandsnaam de naam van de spin-set in.
1. Selecteer **[!UICONTROL Save]**.

   U kunt een voorvertoning van de eCatalog weergeven nadat u de catalogus hebt opgeslagen door **[!UICONTROL Preview]** te selecteren.

## Een eCatalog bewerken {#editing-an-ecatalog}

Of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | De optie Publiceren na opslaan is geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een eCatalog bewerken:**

1. Selecteer de rollover- **[!UICONTROL Edit]**-knop van de eCatalog.
1. Breng de gewenste wijzigingen aan.
1. Als u klaar bent met bewerken, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]**, selecteer een opslagomslag, ga een naam voor de reeks in, en selecteer dan **[!UICONTROL Save]**.

## Een eCatalog verwijderen {#deleting-an-ecatalog}

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een eCatalog verwijderen:**

1. Selecteer een of meer eCatalogi in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## De inhoudsopgave aanpassen {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic biedt standaardpaginanummers in uw eCatalog op het tabblad Order Pages van het scherm eCatalog. Voor aangepaste paginanamen kunt u de paginalabels wijzigen die de inhoudsopgave vormen. Het wordt aanbevolen de naam van de voor- en achteromslag te wijzigen. De voorpagina kan bijvoorbeeld &quot;Omslag&quot; in plaats van &quot;Pagina 0-1&quot; lezen.

U kunt handmatig een aangepaste inhoudsopgave (TOC) voor uw eCatalog maken of de paginanamen importeren vanuit een CSV- (alleen Mac) of XML-bestand.

>[!NOTE]
>
>Als u de standaardpaginatitels wilt herstellen, selecteert u **[!UICONTROL TOC Labels]** op het tabblad **[!UICONTROL Order Pages]** en selecteert u **[!UICONTROL Restore Defaults (All)]**.

### Paginanamen handmatig invoeren {#manually-entering-page-names}

Als u de paginanamen een voor een handmatig wilt invoeren, gaat u naar het tabblad Pagina&#39;s bestellen van het eCatalog-scherm. Voer vervolgens in het veld Paginanummer een naam in voor elke pagina die u een naam wilt geven.

### Paginanamen importeren {#importing-page-names}

Het wordt aanbevolen paginanamen te importeren als u te maken hebt met een eCatalog met veel pagina&#39;s. U kunt de namen importeren uit een door tabs gescheiden of XML-bestand.

Het label van de inhoudsopgave wordt opgeslagen in het veld Gebruikersgegevens van een afbeelding. formatteren deze gegevens als lijst van `name=<value>` ` pairs separated by two question marks “??” `. Als u bijvoorbeeld één label wilt instellen voor een inhoudsopgaveveld met de naam `tocEN`, stelt u de gebruikersgegevens van de afbeelding in op:

`tocEN=&lt;EN_page_label>`

Als u afzonderlijke labels wilt instellen voor inhoudsopgavevelden met de namen `tocEN` en `tocFR`:

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

Als u paginanamen wilt importeren uit een door tabs gescheiden of XML-bestand, selecteert u de knop **[!UICONTROL TOC Labels]** en selecteert u **[!UICONTROL Import]**. Selecteer **[!UICONTROL Browse]** in het dialoogvenster Metagegevens uploaden en importeer vervolgens het CSV-bestand (alleen Mac) of XML-bestand dat elke pagina aan een paginanaam koppelt.
