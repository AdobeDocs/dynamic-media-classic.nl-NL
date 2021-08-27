---
title: Een stalenset maken
description: Leer hoe u een stalenset maakt in Adobe Dynamic Media Classic.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Een stalenset maken{#creating-a-swatch-set}

Met een stalenset kunnen gebruikers een item in een andere kleur, in een ander patroon of in een andere afwerking bekijken. Als u een stalenset met kleurstalen wilt maken, hebt u één afbeelding nodig voor elke andere kleur, elk patroon of elke afwerking die u aan de gebruikers wilt presenteren. Voor elke kleur, elk patroon of elke afwerking hebt u ook één kleur-, patroon- of eindstaal nodig.

Stel dat u afbeeldingen van uiteinden met verschillende kleurrekeningen wilt weergeven. de rekeningen zijn rood , groen en blauw . In dit geval hebt u drie opnamen van hetzelfde kapje nodig. Je hebt een opname nodig met een rood, een met een groen en een met een blauwe rekening. U hebt ook een rood, groen en blauw kleurenstaal nodig. De kleurstalen fungeren als de miniaturen die gebruikers in de Staalset-viewer selecteren om de rode, groene of blauwe rechthoek te zien.

## Een stalenset maken {#create}

Wanneer u een set maakt, heeft de optie **Publiceren na opslaan** op de volgende manieren invloed op de set en stelt u leden in:
| **[!UICONTROL Publish after save]** optie geselecteerd voordat u opslaat? | Staat van vestiging na opslag | Staat van het aantal leden na het opslaan |
| — | — | — |
| Ja | Gepubliceerd | gepubliceerd |
| Neen | Niet gepubliceerd | Leden instellen behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een stalenset maken:**

1. Voer een van de volgende handelingen uit:

   * **Selecteer eerst**  de afbeeldingen in het deelvenster Bladeren, selecteer de afbeeldingen en ga vervolgens naar  **[!UICONTROL Build]** >  **[!UICONTROL Swatch Sets]**.

   * **Begin in het scherm**  Staalset - Ga naar  **[!UICONTROL Build]** >  **[!UICONTROL Swatch Sets]**. Selecteer een map in de elementenbibliotheek en sleep de afbeeldingen naar de sectie Weergaven van de pagina Staalset.

1. Sleep staalkleuren, patronen of zet deze om in het vak Stalen in de pagina Staalset.

   Zorg ervoor dat het kleur-, patroon- of eindstaal dat u naar elke plaatsaanduiding sleept, de kleur, het patroon of het einde van de aangrenzende afbeelding vertegenwoordigt.

1. Als u de volgorde van afbeeldingen in uw stalenset wilt wijzigen, sleept u de afbeeldingen naar nieuwe locaties.
1. Zorg dat in de rechterbenedenhoek van de pagina **[!UICONTROL Publish after save]** is geselecteerd (standaardwaarde).
1. Selecteer **[!UICONTROL Save]**, selecteer een omslag voor het opslaan van uw reeks van het kleurenmonster, ga een naam voor de reeks in, en selecteer **[!UICONTROL Submit]**.
1. Selecteer **[!UICONTROL Preview]** in het scherm Staalset om de Staalset weer te geven in de Staalsetviewer. U kunt staalminiaturen selecteren in de Staalset Viewer om te zien hoe ze zich gedragen.

## Een stalenset bewerken {#editing-a-swatch-set}

Of u een gepubliceerde of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after]** optie opslaan geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |--- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een stalenset bewerken:**

1. Blader in de rasterweergave naar een SwatchSet en selecteer **[!UICONTROL Edit]** onder de afbeelding.
1. Voer een van de volgende handelingen uit:

   * Als u een afbeelding wilt toevoegen (gepubliceerd of niet gepubliceerd), sleept u deze uit een map in Elementen toevoegen naar de pagina **[!UICONTROL Views]** van de stalenset.
   * Als u een afbeelding wilt verwijderen, selecteert u deze en selecteert u **[!UICONTROL Delete]** op de werkbalk.
   * Als u de volgorde van afbeeldingen wilt wijzigen, sleept u een afbeelding naar een nieuwe positie.

1. Als u klaar bent met het bewerken van de set, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]**, selecteer een opslagomslag, ga een naam voor de reeks in, en selecteer dan **[!UICONTROL Save]**.

## Een stalenset verwijderen {#deleting-a-swatch-set}

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een stalenset verwijderen:**

1. Selecteer een stalenset of meer in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
