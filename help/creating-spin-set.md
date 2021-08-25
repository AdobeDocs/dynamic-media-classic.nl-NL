---
title: Een centrifugeset maken
description: Leer hoe u een centrifugeset maakt in Dynamic Media Classic.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# Een centrifugeset maken{#creating-a-spin-set}

Als u een effectieve centrifugeset wilt maken, moet u controleren of de afbeeldingen op de juiste wijze zijn opgenomen. U kunt een in Dynamic Media Classic ingestelde Draai maken door de knop Build te selecteren en Draaisets te kiezen. Bewerk de centrifuges in het scherm Spin Sets.

>[!NOTE]
>
>In eerdere versies van Dynamic Media Classic konden geen tweedimensionale centrifuges worden gebruikt. Als u een centrifugeset hebt gemaakt in een vorige versie van Dynamic Media Classic, kunt u de eendimensionale centrifugeset niet opslaan zonder deze eerst onder een andere naam op te slaan. Selecteer **[!UICONTROL Save As]** in het scherm van de Reeks van de Rotatie en ga een nieuwe naam in zodat u het in de Klassiek van Dynamic Media kunt uitgeven.

## Richtlijnen voor het maken van centrifuges {#guidelines-for-shooting-spin-set-images}

Over het algemeen geldt dat hoe meer afbeeldingen u in een centrifugeset hebt, hoe beter het effect van het draaien van de afbeelding is. Als u echter veel afbeeldingen in de set opneemt, neemt de laadtijd van de afbeeldingen toe. Dynamic Media Classic raadt de volgende richtlijnen aan voor het maken van foto&#39;s voor gebruik in centrifuges:

* Gebruik minimaal 8-12 afbeeldingen in een eendimensionale centrifuge en 16-24 afbeeldingen in een tweedimensionale centrifugeset.
* Gebruik een indeling zonder verlies. TIFF en PNG worden aanbevolen.
* Masker alle afbeeldingen zodat het item op een zuiver witte of andere achtergrond met veel contrast wordt weergegeven. Voeg desgewenst schaduwen toe.
* Zorg ervoor dat de productdetails goed verlicht en in nadruk zijn.
* Neem spin beelden voor modekleding met een mannequin of een model. Vaak wordt de mannequin gemaskeerd (met behulp van een glazen mannequin) of wordt in de afbeelding een gestileerde mannequin/dressform weergegeven. U kunt een op-model spin-reeks tot stand brengen door het aantal hoeken te bepalen. Markeer elke hoek met band op de vloer zodat u het model kunt begeleiden en in de richting van elke opname kunt kijken.

## Een centrifugeset maken {#create}

De volgorde waarin de Spin-set is gemaakt of gemaakt in Dynamic Media Classic is belangrijk. Afhankelijk van de volgorde waarin u de elementen ordent wanneer u afbeeldingen naar het raster sleept op de pagina Draaien in set, draait de Spin-set in een bepaalde richting. Daarom is de volgorde waarin het element visueel wordt weergegeven in de builder de manier waarop het wordt gedraaid wanneer een gebruiker de muisaanwijzer beweegt of zijn vinger van links naar rechts beweegt.

Wanneer u een set maakt, heeft de optie **[!UICONTROL Publish after save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL Publish after save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually-publishing-assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually-unpublishing-assets).

Nadat u een Spin-reeks hebt opgeslagen, kunt u Voorvertoning gebruiken in de Build: Met de optie Spin Set kunt u zien hoe de centrifugeset er in de standaardviewer uitziet.

**Een centrifugeset maken:**

1. Selecteer **[!UICONTROL Spin Sets]** in het vervolgkeuzemenu **[!UICONTROL Build]**.
1. Stel in het dialoogvenster Grootte van paginaset het gewenste aantal rijen en cellen in.

   Als u een eendimensionale centrifuge wilt maken, selecteert u slechts één rij.

   Als u een tweedimensionale centrifugeerset wilt maken, selecteert u twee of meer rijen.

1. Selecteer **[!UICONTROL OK]**.
1. Sleep afbeeldingen naar het raster op het scherm Spin Set.
1. Als u klaar bent, gaat u naar de rechterbenedenhoek van de pagina en controleert u of **Publiceren na opslaan** is geselecteerd (standaard).
1. Selecteer **[!UICONTROL Save]**.
1. Selecteer in het dialoogvenster Opslaan een map waarin u de centrifugeset wilt opslaan. Voer in het veld Bestandsnaam de naam van de spin-set in.
1. Selecteer **[!UICONTROL Save]**.

## Een draaiset bewerken {#editing-a-spin-set}

Of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after save]** optie geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually-publishing-assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually-unpublishing-assets).

**Een centrifugeset bewerken:**

1. Selecteer de rollover **[!UICONTROL Edit]**-knop van de centrifugeset.
1. Voer een van de volgende handelingen uit:

   * **Afbeeldingen**  verwijderen: selecteer de afbeelding en selecteer  **[!UICONTROL Delete]**.

   * **Afbeeldingen**  toevoegen: sleep de afbeelding naar een cel.

   * **Rijen opnieuw ordenen (tweedimensionale centrifuges)**  - Selecteer een vak met een rijkiezer (links van de rij) en selecteer  **[!UICONTROL Move Row Down]** of  **[!UICONTROL Move Row Up]**.

   * **Rijen en cellen**  toevoegen - Voer een getal in het vak Rijen en Cellen in om het aantal rijen en het aantal cellen in elke rij te bepalen.

1. Als u klaar bent met bewerken, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Selecteer **[!UICONTROL Save]**, selecteer een opslagomslag, ga een naam voor de reeks in, en selecteer dan **[!UICONTROL Save]**.

## Een centrifugeerset verwijderen {#deleting-a-spin-set}

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually-publishing-assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually-unpublishing-assets).

**Een centrifugeset verwijderen:**

1. Selecteer een of meer centrifuges in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
