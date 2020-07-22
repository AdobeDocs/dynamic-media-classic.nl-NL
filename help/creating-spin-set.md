---
title: Een centrifugeset maken
seo-title: Een centrifugeset maken
description: 'null'
seo-description: Leer hoe u een centrifugeset maakt.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---


# Een centrifugeset maken{#creating-a-spin-set}

Als u een effectieve centrifugeset wilt maken, moet u controleren of de afbeeldingen op de juiste wijze zijn opgenomen. U kunt een centrifugeset maken in Dynamic Media Klassiek door de knop Samenstellen te selecteren en Draaisets te kiezen. Bewerk de centrifuges in het scherm Spin Sets.

>[!NOTE]
>
>In eerdere versies van Dynamic Media Classic konden geen tweedimensionale centrifuges worden gebruikt. Als u een centrifugeset hebt gemaakt in een vorige versie van Dynamic Media Classic, kunt u de eendimensionale centrifugeset niet opslaan zonder deze eerst onder een andere naam op te slaan. Klik op Opslaan als in het scherm Spin-set en voer een nieuwe naam in zodat u deze kunt bewerken in Dynamic Media Classic.

## Richtlijnen voor het maken van centrifuges {#guidelines-for-shooting-spin-set-images}

Over het algemeen geldt dat hoe meer afbeeldingen u in een centrifugeset hebt, hoe beter het effect van het draaien van de afbeelding is. Als u echter veel afbeeldingen in de set opneemt, neemt de laadtijd van de afbeeldingen toe. Dynamic Media Classic raadt deze richtlijnen aan voor het maken van foto&#39;s voor gebruik in centrifuges:

* Gebruik minimaal 8-12 afbeeldingen in een eendimensionale centrifuge en 16-24 afbeeldingen in een tweedimensionale centrifugeset.
* Gebruik een indeling zonder verlies. TIFF en PNG worden aanbevolen.
* Masker alle afbeeldingen zodat het item op een zuiver witte of andere achtergrond met veel contrast wordt weergegeven. Voeg desgewenst schaduwen toe.
* Zorg ervoor dat de productdetails goed verlicht en in nadruk zijn.
* Neem spin beelden voor modekleding met een mannequin of een model. Vaak wordt de mannequin volledig gemaskeerd (met behulp van een glazen mannequin) of wordt in de afbeelding een gestileerde mannequin/dressform weergegeven. U kunt een op-model spin-reeks tot stand brengen door het aantal hoeken te bepalen. Markeer elke hoek met band op de vloer om het model te begeleiden en in de richting van elke opname te kijken.

## Een centrifugeset maken {#create}

Houd er rekening mee dat de volgorde waarin de centrifugeset is gemaakt of gemaakt in Classic Dynamic Media belangrijk is. Afhankelijk van de volgorde waarin u de elementen ordent wanneer u afbeeldingen naar het raster sleept op de pagina Draaien in set, draait de Spin-set in een bepaalde richting. Daarom is de volgorde waarin het element visueel wordt weergegeven in de builder de manier waarop het wordt gedraaid wanneer een gebruiker de muisaanwijzer beweegt of met zijn vinger naar rechts beweegt.

Wanneer u een set maakt, heeft de optie **Publiceren na opslaan** op de volgende manieren invloed op de set en stelt u leden in:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen](publishing-files.md#manually-publishing-assets) handmatig publiceren en [elementen](publishing-files.md#manually-unpublishing-assets)handmatig verwijderen.

Nadat u een Spin-reeks hebt opgeslagen, kunt u Voorvertoning gebruiken in de Build: Met de optie Spin Set kunt u zien hoe de centrifugeset er in de standaardviewer uitziet.

**Een centrifugeerset maken**

1. Klik in het vervolgkeuzemenu **Build** op **Spin Sets**.
1. Stel in het dialoogvenster Grootte van paginaset het gewenste aantal rijen en cellen in.

   Als u een eendimensionale centrifuge wilt maken, selecteert u slechts één rij.

   Als u een tweedimensionale centrifugeerset wilt maken, selecteert u twee of meer rijen.

1. Klik op **OK**.
1. Sleep afbeeldingen naar het raster op het scherm Spin Set.
1. Als u klaar bent, controleert u of **Publiceren na opslaan** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Klik op **Opslaan**.
1. Selecteer in het dialoogvenster Opslaan een map waarin u de centrifugeset wilt opslaan. Voer in het veld Bestandsnaam de naam van de spin-set in.
1. Klik op **Opslaan**.

## Een centrifugeset bewerken {#editing-a-spin-set}

Afhankelijk van het feit of u een gepubliceerde set of een niet-gepubliceerde set bewerkt, heeft de optie **Publiceren na opslaan** op de volgende manieren invloed op de set en stelt u leden in:

| Reeds gepubliceerd instellen? | De optie Publiceren na opslaan is geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |--- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden van een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen](publishing-files.md#manually-publishing-assets) handmatig publiceren en [elementen](publishing-files.md#manually-unpublishing-assets)handmatig verwijderen.

**Een centerset bewerken**

1. Klik op de knop **Bewerken** van de rollover-set.
1. Voer een van de volgende handelingen uit:

   * **Afbeeldingen verwijderen** Selecteer de afbeelding en klik vervolgens op 
**Verwijderen**.

   * **Afbeeldingen** toevoegen Sleep de afbeelding naar een cel.

   * **Rijen opnieuw rangschikken (tweedimensionale reeksen van de Draai)** Klik een rij-selecteervakje (links van de rij) en klik dan 
**Rij omlaag** of **rij omhoog** verplaatsen.

   * **Rijen en cellen** toevoegen Voer een getal in het vak Rijen en Cellen in om het aantal rijen en het aantal cellen in elke rij te bepalen.

1. Als u klaar bent met bewerken, controleert u of **Publiceren na opslaan** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Klik op **Opslaan**, selecteer een opslagmap, voer een naam voor de set in en klik op **Opslaan**.

## Een centrifugeerset verwijderen {#deleting-a-spin-set}

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen](publishing-files.md#manually-publishing-assets) handmatig publiceren en [elementen](publishing-files.md#manually-unpublishing-assets)handmatig verwijderen.

**Een centrierset verwijderen**

1. Selecteer een of meer centrifuges in de rasterweergave, lijstweergave of detailweergave.
1. Klik op de algemene navigatiebalk op **Bestand** > **Verwijderen** > **Verwijderen**.

