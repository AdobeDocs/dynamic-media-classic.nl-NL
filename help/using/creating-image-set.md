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

Wanneer u een set maakt, heeft de optie **[!UICONTROL Publish after a save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL `Publish after a save`]** geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

Als u een Afbeeldingsset maakt, raadt Adobe de volgende aanbevolen procedures aan en past het de volgende limieten toe:

| Type limiet | Beste praktijken | Oplegde limiet |
| --- | --- | --- |
| Aantal dubbele elementen per set | Geen duplicaten | 20‡ |
| Maximumaantal afbeeldingen per set | 5-10 afbeeldingen per set | 1000 |

‡ De beste manier is om geen dubbele elementen in een set te hebben. De limiet is 20 duplicaten voor één element. Als u binnen de set nog een duplicaat voor dat element toevoegt, geeft de aanvraag een fout of wordt het duplicaat genegeerd.

Zie ook [&#x200B; Dynamische beperkingen van Media &#x200B;](/help/using/limitations.md).

**om een Reeks van het Beeld tot stand te brengen:**

1. Voer een van de volgende handelingen uit:

   * **selecteer eerst de beelden**: In het Browse paneel, selecteer de beelden u voor uw Reeks van het Beeld wilt, ga **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**.

   * **Begin van het Vastgestelde scherm van het Beeld**: Ga naar **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**. Het scherm Afbeeldingsset wordt geopend. Selecteer een map in de elementenbibliotheek en sleep de afbeeldingen die u voor de afbeeldingsset wilt instellen naar het scherm Afbeeldingsset.

1. Als u de volgorde van de afbeeldingen wilt wijzigen, sleept u de afbeeldingen naar nieuwe locaties.
1. Zorg dat rechts onder op de pagina de optie **[!UICONTROL Publish after a save]** is geselecteerd (standaardwaarde).
1. Selecteer **[!UICONTROL Save]**, selecteer een map voor het opslaan van de afbeeldingsset, voer een naam voor de set in en selecteer vervolgens **[!UICONTROL Save]** .
1. Selecteer **[!UICONTROL Preview]** in het scherm Afbeeldingsset om de Afbeeldingsset weer te geven die in de viewer voor de afbeeldingsset is ingesteld. U kunt staalminiaturen selecteren in de Image Set Viewer om te zien hoe ze zich gedragen.

## Een afbeeldingsset bewerken {#editing-an-image-set}

Of u nu een gepubliceerde of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after a save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL `Publish after a save`]** geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Reeks van het Beeld uit te geven:**

1. Blader in de rasterweergave naar een ImageSet en selecteer vervolgens **[!UICONTROL Edit]** onder de afbeelding.
1. Voer een van de volgende handelingen uit:

   * Als u een (gepubliceerde of niet-gepubliceerde) afbeelding wilt toevoegen, sleept u deze uit een map in Assets toevoegen naar de pagina **[!UICONTROL Views]** van de Afbeeldingsset.
   * Als u een afbeelding wilt verwijderen, selecteert u deze en selecteert u vervolgens **[!UICONTROL Delete]** op de werkbalk.
   * Als u de volgorde van afbeeldingen wilt wijzigen, sleept u een afbeelding naar een nieuwe positie.

1. Als u klaar bent met het bewerken van de set, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard) rechtsonder op de pagina.
1. Selecteer **[!UICONTROL Save]**, selecteer een opslagmap voor de set, voer een naam voor de set in en selecteer vervolgens **[!UICONTROL Save]** .

## Een afbeeldingsset verwijderen

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Reeks van het Beeld te schrappen:**

1. Selecteer in de rasterweergave, lijstweergave of detailweergave een of meer afbeeldingssets.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** .
