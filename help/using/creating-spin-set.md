---
title: Een centrifugeset maken
description: Leer hoe u een Spin-set maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Een centrifugeset maken{#creating-a-spin-set}

Als u een effectieve centrifugeset wilt maken, moet u controleren of de afbeeldingen op de juiste wijze zijn opgenomen. U kunt een in Adobe Dynamic Media Classic ingestelde centrifugeset maken door de knop Build te selecteren en de optie Spin-sets te kiezen. Bewerk de centrifuges in het scherm Spin Sets.

>[!NOTE]
>
>In eerdere versies van Adobe Dynamic Media Classic konden tweedimensionale centrifuges niet worden gebruikt. Als u een Spin-reeks in een vorige versie van Adobe Dynamic Media Classic creeerde, bewaar het onder een verschillende naam, dan kunt u uw eendimensionale Reeks van de Draai bewaren. Selecteer **[!UICONTROL Save As]** in het scherm van de Vastgestelde draaien en ga een nieuwe naam in zodat u het in Adobe Dynamic Media Classic kunt uitgeven.

## Richtlijnen voor het maken van centrifuges {#guidelines-for-shooting-spin-set-images}

Over het algemeen geldt dat hoe meer afbeeldingen u in een centrifugeset hebt, hoe beter het effect van het draaien van afbeeldingen is. Als u echter veel afbeeldingen in de set opneemt, neemt de laadtijd van de afbeeldingen toe. Adobe Dynamic Media Classic raadt de volgende richtlijnen aan voor het maken van foto&#39;s voor gebruik in centrifuges:

* Gebruik minimaal 8-12 afbeeldingen in een eendimensionale centrifugeset en 16-24 afbeeldingen in een tweedimensionale centrifugeset.
* Gebruik een indeling zonder verlies. TIFF en PNG worden aanbevolen.
* Masker alle afbeeldingen zodat het item op een zuiver witte of andere achtergrond met veel contrast wordt weergegeven. Voeg desgewenst schaduwen toe.
* Zorg ervoor dat de productdetails goed verlicht en in nadruk zijn.
* Neem spin beelden voor modekleding met een mannequin of een model. Vaak wordt de mannequin gemaskeerd (met behulp van een glazen mannequin) of wordt in de afbeelding een gestileerde mannequin/dressform weergegeven. U kunt op model een Vastgestelde Rotatie tot stand brengen door het aantal hoeken te bepalen. Markeer elke hoek met band op de vloer zodat u het model kunt begeleiden en in de richting van elke opname kunt kijken.

## Een centrifugeset maken {#create}

De volgorde waarin de draaiende set is gemaakt of gemaakt in Adobe Dynamic Media Classic, is belangrijk. Afhankelijk van de volgorde waarin u de elementen ordent wanneer u afbeeldingen naar het raster sleept op de pagina Draaien en instellen, draait de Spin-set in een bepaalde richting. Daarom is de volgorde waarin het element visueel wordt weergegeven in de builder de manier waarop het wordt gedraaid wanneer een gebruiker de muisaanwijzer beweegt of zijn vinger van links naar rechts beweegt.

Wanneer u een set maakt, heeft de optie **[!UICONTROL Publish after a save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL Publish after a save]** geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [ manueel het publiceren activa ](publishing-files.md#manually-publishing-assets) en [ manueel unpublishing activa ](publishing-files.md#manually-unpublishing-assets).

Als u een Spin-set maakt, raadt Adobe de volgende aanbevolen procedures aan en past het de volgende limiet toe:

| Limiettype voor centrifugeren instellen | Beste praktijken | Oplegde limiet |
| --- | --- | --- |
| Maximumaantal rijen/kolommen per 2D-set | 12-18 afbeeldingen per set | 1000 |

Zie ook [ Dynamische beperkingen van Media ](/help/using/limitations.md).

Nadat u een Spin-set hebt opgeslagen, kunt u Voorvertoning in de Build: Spin-set gebruiken om te zien hoe de Spin-set er in de standaardviewer uitziet.

**om een Reeks van de Draai tot stand te brengen:**

1. Selecteer **[!UICONTROL Build]** in de vervolgkeuzelijst **[!UICONTROL Spin Sets]** .
1. Stel in het dialoogvenster Grootte van paginaset het gewenste aantal rijen en cellen in.

   Als u een eendimensionale centrifugeset wilt maken, selecteert u slechts één rij.

   Als u een tweedimensionale centrifugeerset wilt maken, selecteert u twee of meer rijen.

1. Selecteer **[!UICONTROL OK]** .
1. Sleep afbeeldingen naar het raster op het scherm Spin Set.
1. Wanneer u, dichtbij de laag-juiste hoek van de pagina wordt gebeëindigd, zorg ervoor dat **na sparen** (gebrek) wordt geselecteerd publiceert.
1. Selecteer **[!UICONTROL Save]** .
1. Selecteer in het dialoogvenster Opslaan een map waarin de centrifugeset moet worden opgeslagen. Voer in het veld Bestandsnaam de naam van de centrifugeset in.
1. Selecteer **[!UICONTROL Save]** .

## Een centrifugeset bewerken {#editing-a-spin-set}

Of u nu een gepubliceerde set of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after a save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after a save]** geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [ manueel het publiceren activa ](publishing-files.md#manually-publishing-assets) en [ manueel unpublishing activa ](publishing-files.md#manually-unpublishing-assets).

**om een Reeks van de Rotatie uit te geven:**

1. Selecteer de rollover **[!UICONTROL Edit]** -knop van de draaiende set.
1. Voer een van de volgende handelingen uit:

   * **het Verwijderen van beelden**: Selecteer het beeld, en selecteer dan **[!UICONTROL Delete]**.

   * **Toevoegend beelden**: Sleep het beeld in een cel.

   * **het Herordenen van rijen (tweedimensionale Reeksen van de Draai)**: Selecteer een rij-selecteurvakje (links van de rij) en selecteer dan **[!UICONTROL Move Row Down]** of **[!UICONTROL Move Row Up]**.

   * **Toevoegend rijen en cellen**: ga een aantal in de doos van Rijen en van Cellen in om het aantal rijen en het aantal cellen in elke rij te bepalen.

1. Als u klaar bent met bewerken, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]** , selecteer een opslagmap, voer een naam voor de set in en selecteer vervolgens **[!UICONTROL Save]** .

## Een centrifugeset verwijderen

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [ manueel het publiceren activa ](publishing-files.md#manually-publishing-assets) en [ manueel unpublishing activa ](publishing-files.md#manually-unpublishing-assets).

**om een Reeks van de Rotatie te schrappen:**

1. Selecteer een of meer centrifuges in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** .
