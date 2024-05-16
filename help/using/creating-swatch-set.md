---
title: Een stalenset maken
description: Leer hoe u een stalenset maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Een stalenset maken{#creating-a-swatch-set}

Met een stalenset kunnen gebruikers een item in een andere kleur, in een ander patroon of in een andere afwerking bekijken. Als u een stalenset met kleurstalen wilt maken, hebt u één afbeelding nodig voor elke andere kleur, elk patroon of elke afwerking die u aan de gebruikers wilt presenteren. Voor elke kleur, elk patroon of elke afwerking hebt u ook één kleur-, patroon- of eindstaal nodig.

Stel dat u afbeeldingen van uiteinden met verschillende kleurrekeningen wilt weergeven. De rekeningen zijn rood, groen en blauw. In dit geval hebt u drie opnamen van hetzelfde kapje nodig. Je hebt een opname nodig met een rood, een met een groen en een met een blauwe rekening. U hebt ook een rood, groen en blauw kleurenstaal nodig. De kleurstalen fungeren als de miniaturen die gebruikers in de Staalset-viewer selecteren om de rode, groene of blauwe rechthoek te zien.

## Een stalenset maken {#create}

Wanneer u een set maakt, **Publiceren na opslaan** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| **[!UICONTROL Publish after a save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een stalenset maken:**

1. Voer een van de volgende handelingen uit:

   * **Selecteer eerst de afbeeldingen**: Selecteer de afbeeldingen in het deelvenster Bladeren en ga vervolgens naar **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**.

   * **Starten vanaf het scherm Staalset**: Ga naar **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**. Selecteer een map in de elementenbibliotheek en sleep de afbeeldingen naar de sectie Weergaven van de pagina Staalset.

1. Sleep staalkleuren, patronen of voltooit in het vak Stalen van de pagina Staalset.

   Zorg ervoor dat het kleur-, patroon- of eindstaal dat u naar elke plaatsaanduiding sleept, de kleur, het patroon of het einde van de aangrenzende afbeelding vertegenwoordigt.

1. Als u de volgorde van afbeeldingen in uw stalenset wilt wijzigen, sleept u de afbeeldingen naar nieuwe locaties.
1. Zorg ervoor dat rechts onder op de pagina de volgende informatie wordt weergegeven: **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]** selecteert u een map waarin u de kleurstaalset wilt opslaan, voert u een naam in voor de set en selecteert u **[!UICONTROL Submit]**.
1. Selecteer **[!UICONTROL Preview]** op het scherm Staalset. U kunt staalminiaturen selecteren in de Staalset Viewer om te zien hoe ze zich gedragen.

## Een stalenset bewerken {#editing-a-swatch-set}

Of u een gepubliceerde of een niet-gepubliceerde set bewerkt, **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after a save]** optie opslaan geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een stalenset bewerken:**

1. Blader in de rasterweergave naar een SwatchSet en selecteer vervolgens onder de afbeelding de optie **[!UICONTROL Edit]**.
1. Voer een van de volgende handelingen uit:

   * Als u een (gepubliceerde of niet-gepubliceerde) afbeelding wilt toevoegen, sleept u deze uit een map in Elementen toevoegen naar de stalenset **[!UICONTROL Views]** pagina.
   * Als u een afbeelding wilt verwijderen, selecteert u deze en selecteert u vervolgens **[!UICONTROL Delete]** op de werkbalk.
   * Als u de volgorde van afbeeldingen wilt wijzigen, sleept u een afbeelding naar een nieuwe positie.

1. Wanneer u klaar bent met het bewerken van de set, in de rechterbenedenhoek van de pagina, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**, selecteert u een opslagmap, voert u een naam voor de set in en selecteert u **[!UICONTROL Save]**.

## Een stalenset verwijderen

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een stalenset verwijderen:**

1. Selecteer een stalenset of meer in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
