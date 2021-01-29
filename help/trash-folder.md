---
title: De map Prullenbak beheren
description: Leer hoe u de prullenmand beheert.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---


# De prullenmand beheren{#managing-the-trash-folder}

Items die u uit Dynamic Media Classic verwijdert, worden naar de map Prullenbak verplaatst. Ze blijven zeven dagen in deze map totdat ze worden hersteld of permanent worden verwijderd. U kunt verwijderde items controleren door het prullenbakpictogram onder aan de Asset Library te selecteren en items in de map Prullenbak weer te geven.

Alle gebruikers kunnen items in de map met prullenmand terugzetten naar de mappen waaruit ze zijn verwijderd. Alle gebruikers kunnen ook de prullenmand leeg maken met alle inhoud ervan.

Als u items verwijdert uit de map Prullenmand, worden deze items definitief verwijderd uit Dynamic Media Classic. items die uit de map Prullenbak zijn verwijderd, kunnen niet meer worden hersteld. Zie [Algemene instellingen van toepassing](application-setup.md#general_settings) voor informatie over het instellen van meldingen voor bedrijfsbeheerders wanneer elementen automatisch uit de prullenbak moeten worden verwijderd.

>[!NOTE]
>
>Elementen die naar de map Prullenmand zijn verplaatst, worden nog steeds geregistreerd bij Dynamic Media Classic. Als u een bestand probeert te uploaden dat dezelfde naam heeft als een verwijderd bestand in de map met prullenmand, behandelt Dynamic Media Classic het element dat u wilt uploaden als een gedupliceerd element. Er wordt dan een nummer aan de naam toegevoegd.

## Informatie over de map Prullenbak {#about-the-trash-folder}

Als u een item in een map verwijdert, wordt het item in de map Prullenbak geplaatst. Het volgende gebeurt wanneer u een item verwijdert en naar de map Prullenbak verplaatst:

* Hoewel het item uit uw Klassieke Dynamic Media-mappen is verwijderd, kan de id niet aan een ander element worden toegewezen zolang het in de prullenmand blijft staan. Als u middelen probeert te uploaden met dezelfde naam als een bestand in de map met prullenmand, voegt Dynamic Media Classic een cijfer toe aan de naam van het element.
* Het item kan niet worden gepubliceerd. Zelfs als het item was gemarkeerd voor publicatie toen u het wist, wordt het niet gepubliceerd.
* Het item blijft in de map met prullenmand staan totdat het is hersteld, zeven dagen zijn verstreken of totdat iemand de opdracht Leeg de prullenmand heeft gekozen. Na zeven dagen verwijdert een automatische opschoonbewerking het item definitief.

## Elementen herstellen vanuit de map Prullenmand {#restoring-assets-from-the-trash-folder}

De persoon die een middel heeft verwijderd, hoeft dit niet te herstellen. iedereen kan middelen herstellen vanuit de map Prullenmand. Elementen die worden hersteld, worden geplaatst in de mappen waaruit ze zijn verwijderd. Als deze mappen niet meer bestaan, maakt Dynamic Media Classic ze opnieuw en worden de herstelde elementen in de opnieuw gemaakte mappen geplaatst.

Ga als volgt te werk om middelen van de map Prullenbak te herstellen naar de mappen waaruit ze zijn verwijderd:

1. Klik op het prullenbakpictogram om de map Prullenmand te openen.
1. Selecteer de elementen die u wilt herstellen.
1. Kies Bestand > Herstellen vanuit prullenbak.

## Elementen definitief verwijderen in de map met prullenmand {#permanently-deleting-assets-in-the-trash-folder}

Wanneer u middelen in de omslag van het Afval schrapt, worden de activa permanent geschrapt. Middelen worden na zeven dagen automatisch uit de prullenmand verwijderd.

Als u elementen definitief wilt verwijderen uit de map Prullenbak, selecteert u het prullenbakpictogram om de map Prullenmand te openen. Verwijder vervolgens de afzonderlijke elementen of verwijder alle elementen in de map:

* **Afzonderlijke** elementen verwijderenSelecteer de elementen die u permanent wilt verwijderen en klik op  **[!UICONTROL File > Empty From Trash]**.

* **Alle** elementen verwijderenKlik op  **[!UICONTROL File > Empty Trash]**.

>[!MORELIKETHIS]
>
>* [Elementen verwijderen](moving-renaming-deleting-assets.md#delete_assets)

