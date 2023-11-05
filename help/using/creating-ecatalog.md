---
title: Een eCatalog maken
description: Leer hoe u een eCatalog maakt in Adobe Dynamic Media Classic.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Een eCatalog maken {#creating-an-ecatalog}

Als u een eCatalog maakt, moet u de pagina&#39;s ordenen, de paginalay-out kiezen en de pagina&#39;s koppelen door Afbeeldingen met hyperlinks te tekenen en rollover- en hypertekstkoppelingsgegevens in te voeren. Desgewenst kunt u de inhoudsopgave aanpassen, zodat de viewers de paginanamen in plaats van de paginanummers in de eCatalog-viewer kunnen zien.

## Een eCatalog maken {#create}

U kunt afbeeldingsbestanden en PDF-bestanden opnemen in uw eCatalog.

Wanneer u een eCatalog creeert, **[!UICONTROL Publish after save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een eCatalog maken:**

1. Maak uw eCatalog met een van de volgende technieken:

   * **Selecteer eerst de bestanden** - Selecteer bestanden in het deelvenster Bladeren en ga vervolgens naar **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Starten vanaf het eCatalog-scherm** - Ga naar **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Selecteer een map in de elementenbibliotheek en sleep bestanden van de map naar het tabblad Order Pages op de pagina eCatalog.

     >[!NOTE]
     >
     >Als u de items in de elementenbibliotheek op naam wilt weergeven in plaats van op miniatuur, selecteert u de optie Naam voor de weergave Standaard in de elementenbibliotheek in Persoonlijke instellingen.

1. Selecteer een algemene lay-out voor uw eCatalog. Selecteren **[!UICONTROL 1 Up]** voor enkele pagina&#39;s, **[!UICONTROL 2 Up]** voor spreads met twee pagina&#39;s, of **[!UICONTROL Custom]** voor paginaspreiding van meer dan twee pagina&#39;s. In de **[!UICONTROL Change eCatalog Layout]** selecteert u het dialoogvenster **[!UICONTROL All Spreads]** en selecteert u **[!UICONTROL OK]**.
1. U kunt desgewenst de indeling van afzonderlijke pagina&#39;s of paginaspread wijzigen door deze te selecteren en vervolgens **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]**, of **[!UICONTROL Custom]** knop. In de **[!UICONTROL Change eCatalog Layout]** selecteert u het dialoogvenster **[!UICONTROL Selected Spreads]** en selecteert u **[!UICONTROL OK]**.
1. U kunt de pagina&#39;s op een van de volgende manieren opnieuw ordenen:

   * **Slepen** - Sleep een pagina of paginaspread naar een nieuwe locatie. Op de verticale balk ziet u waar de pagina wordt verplaatst.

   * **Knop Verplaatsen naar** - Selecteer een pagina of paginaspread, selecteer **[!UICONTROL Move To]** en kiest u de pagina in het menu die u eerder wilt weergeven.

   * **Volgnummer** - Geef in de lijstweergave paginanummers op in de velden Volgnummer.

1. Wanneer u klaar bent, gaat u naar de rechterbenedenhoek van de pagina en zorgt u ervoor dat **[!UICONTROL Publish after save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**.
1. Selecteer in het dialoogvenster Opslaan een map voor het opslaan van uw eCatalog. Voer in het veld Bestandsnaam de naam van de spin-set in.
1. Selecteren **[!UICONTROL Save]**.

   Nadat u de eCatalog hebt opgeslagen, kunt u een voorvertoning weergeven door **[!UICONTROL Preview]**.

## Een eCatalog bewerken {#editing-an-ecatalog}

Of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, **[!UICONTROL Publish after save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| Reeds gepubliceerd instellen? | De optie Publiceren na opslaan is geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een eCatalog bewerken:**

1. De rollover van de eCatalog selecteren **[!UICONTROL Edit]** knop.
1. Breng de gewenste wijzigingen aan.
1. Wanneer u klaar bent met bewerken, gaat u naar de rechterbenedenhoek van de pagina en zorgt u ervoor dat **[!UICONTROL Publish after save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**, selecteert u een opslagmap, voert u een naam voor de set in en selecteert u **[!UICONTROL Save]**.

## Een eCatalog verwijderen {#deleting-an-ecatalog}

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een eCatalog verwijderen:**

1. Selecteer een of meer eCatalogi in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## De inhoudsopgave aanpassen {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic biedt standaardpaginanummers in uw eCatalog op het tabblad Order Pages van het eCatalog-scherm. Voor aangepaste paginanamen kunt u de paginalabels wijzigen die de inhoudsopgave vormen. Het wordt aanbevolen de naam van de voor- en achteromslag te wijzigen. De voorpagina kan bijvoorbeeld &quot;Omslag&quot; in plaats van &quot;Pagina 0-1&quot; lezen.

U kunt handmatig een aangepaste inhoudsopgave (TOC) voor uw eCatalog maken of de paginanamen importeren vanuit een CSV- (alleen Mac) of XML-bestand.

>[!NOTE]
>
>Als u de standaardpaginatitels wilt herstellen, gaat u naar het tabblad **[!UICONTROL Order Pages]** tab, selecteert u **[!UICONTROL TOC Labels]** en selecteer vervolgens **[!UICONTROL Restore Defaults (All)]**.

### Paginanamen handmatig invoeren {#manually-entering-page-names}

Als u de paginanamen een voor een handmatig wilt invoeren, gaat u naar het tabblad Pagina&#39;s bestellen van het eCatalog-scherm. Voer vervolgens in het veld Paginanummer een naam in voor elke pagina die u een naam wilt geven.

### Paginanamen importeren {#importing-page-names}

Het wordt aanbevolen paginanamen te importeren als u te maken hebt met een eCatalog met veel pagina&#39;s. U kunt de namen importeren uit een door tabs gescheiden of XML-bestand.

Het label van de inhoudsopgave wordt opgeslagen in het veld Gebruikersgegevens van een afbeelding; zet deze gegevens op als een lijst met `name=<value>` ` pairs separated by two question marks "??" `. Als u bijvoorbeeld één label wilt instellen voor een veld met inhoudsopgave dat een naam heeft `tocEN`stelt u de gebruikersgegevens van de afbeelding in op:

`tocEN=&lt;EN_page_label>`

Afzonderlijke labels instellen voor inhoudsopgavevelden met de naam `tocEN` en `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Als u het veld Gebruikersgegevens wilt importeren in een door tabs gescheiden bestand, neemt u de gebruikersgegevens van het veld op:

| IPSID | Gebruikersgegevens |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Als u het veld Gebruikersgegevens wilt importeren in een XML-bestand, neemt u het kenmerk op `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Als u paginanamen wilt importeren uit een door tabs gescheiden of XML-bestand, selecteert u de optie **[!UICONTROL TOC Labels]** en selecteert u **[!UICONTROL Import]**. Selecteer in het dialoogvenster Metagegevens uploaden de optie **[!UICONTROL Browse]** en importeer vervolgens het CSV-bestand (alleen Mac) of het XML-bestand dat elke pagina aan een paginanaam koppelt.
