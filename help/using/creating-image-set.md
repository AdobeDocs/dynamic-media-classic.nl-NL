---
title: Een afbeeldingsset maken
description: Leer hoe u een Afbeeldingsset maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Een afbeeldingsset maken{#creating-an-image-set}

Als u een Afbeeldingsset met meerdere weergaven wilt maken, hebt u afbeeldingen nodig die een item vanuit verschillende gezichtspunten weergeven of verschillende aspecten van hetzelfde item weergeven. Het doel is om kijkers beelden van een punt te presenteren zodat krijgen zij een stevig idee van wat een punt kijkt of doet.

## Een afbeeldingsset maken {#create}

Wanneer u een set maakt, **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| **[!UICONTROL `Publish after a save`]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

Wanneer u een Reeks van het Beeld creeert, beveelt de Adobe de volgende beste praktijken aan en handhaaft de volgende grenzen:

| Type limiet | Beste praktijken | Oplegde limiet |
| --- | --- | --- |
| Aantal dubbele elementen per set | Geen duplicaten | 20‡ |
| Maximumaantal afbeeldingen per set | 5-10 afbeeldingen per set | 1000 |

‡ De beste manier is om geen dubbele elementen in een set te hebben. De limiet is 20 duplicaten voor één element. Als u binnen de set nog een duplicaat voor dat element toevoegt, geeft de aanvraag een fout of wordt het duplicaat genegeerd.

Zie ook [Dynamic Media-beperkingen](/help/using/limitations.md).

**Een afbeeldingsset maken:**

1. Voer een van de volgende handelingen uit:

   * **Selecteer eerst de afbeeldingen**: Selecteer in het deelvenster Bladeren de afbeeldingen die u als afbeeldingsset wilt gebruiken, ga naar **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**.

   * **Begin van het Vastgestelde scherm van het Beeld**: Ga naar **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**. Het scherm Afbeeldingsset wordt geopend. Selecteer een map in de elementenbibliotheek en sleep de afbeeldingen die u voor de afbeeldingsset wilt instellen naar het scherm Afbeeldingsset.

1. Als u de volgorde van de afbeeldingen wilt wijzigen, sleept u de afbeeldingen naar nieuwe locaties.
1. Zorg ervoor dat rechts onder op de pagina de volgende informatie wordt weergegeven: **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]** selecteert u een map waarin u de afbeeldingsset wilt opslaan, geeft u een naam voor de set op en selecteert u **[!UICONTROL Save]**.
1. Selecteer **[!UICONTROL Preview]** op het scherm Afbeeldingsset. U kunt staalminiaturen selecteren in de Image Set Viewer om te zien hoe ze zich gedragen.

## Een afbeeldingsset bewerken {#editing-an-image-set}

Of u een gepubliceerde of een niet-gepubliceerde set bewerkt, **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| Reeds gepubliceerd instellen? | **[!UICONTROL `Publish after a save`]** optie geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een afbeeldingsset bewerken:**

1. Blader in de rasterweergave naar een ImageSet en selecteer vervolgens onder de afbeelding de optie **[!UICONTROL Edit]**.
1. Voer een van de volgende handelingen uit:

   * Als u een (gepubliceerde of niet-gepubliceerde) afbeelding wilt toevoegen, sleept u deze uit een map in Middelen toevoegen naar de afbeeldingsset **[!UICONTROL Views]** pagina.
   * Als u een afbeelding wilt verwijderen, selecteert u deze en selecteert u vervolgens **[!UICONTROL Delete]** op de werkbalk.
   * Als u de volgorde van afbeeldingen wilt wijzigen, sleept u een afbeelding naar een nieuwe positie.

1. Wanneer u klaar bent met het bewerken van de set, in de rechterbenedenhoek van de pagina, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**, selecteert u een opslagmap voor de set, voert u een naam voor de set in en selecteert u **[!UICONTROL Save]**.

## Een afbeeldingsset verwijderen

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een afbeeldingsset verwijderen:**

1. Selecteer in de rasterweergave, lijstweergave of detailweergave een of meer afbeeldingssets.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
