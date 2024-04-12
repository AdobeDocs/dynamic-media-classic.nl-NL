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
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Een centrifugeset maken{#creating-a-spin-set}

Als u een effectieve centrifugeset wilt maken, moet u controleren of de afbeeldingen op de juiste wijze zijn opgenomen. U kunt een in Adobe Dynamic Media Classic ingestelde centrifugeset maken door de knop Build te selecteren en de optie Spin-sets te kiezen. Bewerk de centrifuges in het scherm Spin Sets.

>[!NOTE]
>
>In eerdere versies van Adobe Dynamic Media Classic konden tweedimensionale centrifuges niet worden gebruikt. Als u een Spin-reeks in een vorige versie van Adobe Dynamic Media Classic creeerde, kunt u niet uw eendimensionale Reeks van de Draai bewaren zonder het onder een verschillende naam eerst op te slaan. Selecteren **[!UICONTROL Save As]** in het scherm Spin Set en voer een nieuwe naam in zodat u deze in Adobe Dynamic Media Classic kunt bewerken.

## Richtlijnen voor het maken van centrifuges {#guidelines-for-shooting-spin-set-images}

Over het algemeen geldt dat hoe meer afbeeldingen u in een centrifugeset hebt, hoe beter het effect van het draaien van afbeeldingen is. Als u echter veel afbeeldingen in de set opneemt, neemt de laadtijd van de afbeeldingen toe. Adobe Dynamic Media Classic raadt de volgende richtlijnen aan voor het maken van foto&#39;s voor gebruik in centrifuges:

* Gebruik minimaal 8-12 afbeeldingen in een eendimensionale centrifuge en 16-24 afbeeldingen in een tweedimensionale centrifugeset.
* Gebruik een indeling zonder verlies. U wordt aangeraden TIFF en PNG te gebruiken.
* Masker alle afbeeldingen zodat het item op een zuiver witte of andere achtergrond met veel contrast wordt weergegeven. Voeg desgewenst schaduwen toe.
* Zorg ervoor dat de productdetails goed verlicht en in nadruk zijn.
* Neem spin beelden voor modekleding met een mannequin of een model. Vaak wordt de mannequin gemaskeerd (met behulp van een glazen mannequin) of wordt in de afbeelding een gestileerde mannequin/dressform weergegeven. U kunt een draaiset van een model maken door het aantal hoeken te definiëren. Markeer elke hoek met band op de vloer zodat u het model kunt begeleiden en in de richting van elke opname kunt kijken.

## Een centrifugeset maken {#create}

De volgorde waarin de Spin-set is gemaakt of gemaakt in Adobe Dynamic Media Classic, is belangrijk. Afhankelijk van de volgorde waarin u de elementen ordent wanneer u afbeeldingen naar het raster sleept op de pagina Draaien en instellen, draait de Spin-set in een bepaalde richting. Daarom is de volgorde waarin het element visueel wordt weergegeven in de builder de manier waarop het wordt gedraaid wanneer een gebruiker de muisaanwijzer beweegt of zijn vinger van links naar rechts beweegt.

Wanneer u een set maakt, **[!UICONTROL Publish after save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| **[!UICONTROL Publish after save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually-publishing-assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually-unpublishing-assets).

Wanneer u een reeks van de Rotatie creeert, adviseert de Adobe de volgende beste praktijken en handhaaft de volgende grens:

| Limiettype voor centrifugeren instellen | Beste praktijken | Oplegde limiet |
| --- | --- | --- |
| Maximumaantal rijen/kolommen per 2D-set | 12-18 afbeeldingen per set | 1000 |

Zie ook [Dynamic Media-beperkingen](/help/using/limitations.md).

Nadat u een Spin-set hebt opgeslagen, kunt u Voorvertoning in de Build: Spin-set gebruiken om te zien hoe de Spin-set er in de standaardviewer uitziet.

**Een centrifugeset maken:**

1. Op de **[!UICONTROL Build]** vervolgkeuzelijst, selecteert u **[!UICONTROL Spin Sets]**.
1. Stel in het dialoogvenster Grootte van paginaset het gewenste aantal rijen en cellen in.

   Als u een eendimensionale centrifuge wilt maken, selecteert u slechts één rij.

   Als u een tweedimensionale centrifugeerset wilt maken, selecteert u twee of meer rijen.

1. Selecteren **[!UICONTROL OK]**.
1. Sleep afbeeldingen naar het raster op het scherm Spin Set.
1. Wanneer u klaar bent, gaat u naar de rechterbenedenhoek van de pagina en zorgt u ervoor dat **Publiceren na opslaan** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**.
1. Selecteer in het dialoogvenster Opslaan een map waarin u de centrifugeset wilt opslaan. Voer in het veld Bestandsnaam de naam van de spin-set in.
1. Selecteren **[!UICONTROL Save]**.

## Een centrifugeset bewerken {#editing-a-spin-set}

Of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, **[!UICONTROL Publish after save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after save]** optie geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually-publishing-assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually-unpublishing-assets).

**Een centrifuusset bewerken:**

1. De rollover van de centrifugeset selecteren **[!UICONTROL Edit]** knop.
1. Voer een van de volgende handelingen uit:

   * **Afbeeldingen verwijderen** - Selecteer de afbeelding en selecteer vervolgens **[!UICONTROL Delete]**.

   * **Afbeeldingen toevoegen** - Sleep de afbeelding naar een cel.

   * **Rijen opnieuw ordenen (tweedimensionale centrifuges)** - Selecteer een vak met een rijkiezer (links van de rij) en selecteer vervolgens **[!UICONTROL Move Row Down]** of **[!UICONTROL Move Row Up]**.

   * **Rijen en cellen toevoegen** - Voer in het vak Rijen en Cellen een getal in om het aantal rijen en het aantal cellen in elke rij te bepalen.

1. Wanneer u klaar bent met bewerken, gaat u naar de rechterbenedenhoek van de pagina en zorgt u ervoor dat **[!UICONTROL Publish after save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**, selecteert u een opslagmap, voert u een naam voor de set in en selecteert u **[!UICONTROL Save]**.

## Een centrifugeset verwijderen

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually-publishing-assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually-unpublishing-assets).

**Een centrifuusset verwijderen:**

1. Selecteer een of meer centrifuges in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
