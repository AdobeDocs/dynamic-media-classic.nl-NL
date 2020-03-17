---
title: De map Prullenbak beheren
seo-title: De map Prullenbak beheren
description: 'null'
seo-description: Leer hoe u de prullenmand beheert.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# De map Prullenbak beheren{#managing-the-trash-folder}

De punten die u van het het Publiceren Scene7 Systeem schrapt worden verplaatst naar de omslag van het Afval. Ze blijven zeven dagen in deze map totdat ze worden hersteld of permanent worden verwijderd. U kunt verwijderde items controleren door het prullenbakpictogram onder aan de Asset Library te selecteren en items in de map Prullenbak weer te geven.

Alle gebruikers kunnen items in de map met prullenmand terugzetten naar de mappen waaruit ze zijn verwijderd. Alle gebruikers kunnen ook de prullenmand leeg maken met alle inhoud ervan.

Het schrappen van punten van de omslag van het Afval schrapt permanent punten van het het Publiceren Scene7 Systeem; items die uit de map Prullenbak zijn verwijderd, kunnen niet meer worden hersteld. Zie Algemene instellingen van [toepassing voor informatie over instellingsmeldingen voor bedrijfsbeheerders wanneer elementen automatisch uit de prullenbak moeten worden verwijderd](application-setup.md#general_settings).

>[!NOTE]
>
>De activa die aan de omslag van het Afval zijn verplaatst worden nog geregistreerd op het het Publiceren Scene7 Systeem. Als u een bestand probeert te uploaden dat dezelfde naam heeft als een verwijderd bestand in de map met prullenmand, behandelt Dynamic Media Classic het element dat u wilt uploaden als een gedupliceerd element. Er wordt dan een nummer aan de naam toegevoegd.

## De map Prullenbak {#about-the-trash-folder}

Als u een item in een map verwijdert, wordt het item in de map Prullenbak geplaatst. Het volgende gebeurt wanneer u een item verwijdert en naar de map Prullenbak verplaatst:

* Hoewel het punt uit uw het Publiceren Scene7 de omslagen van het Systeem is verwijderd, kan zijn identiteitskaart niet aan een ander middel worden toegewezen terwijl het in de omslag van het Afval blijft. Als u een element probeert te uploaden met dezelfde naam als een bestand in de map Prullenbak, voegt Dynamic Media Classic een cijfer toe aan de naam van het element.
* Het item kan niet worden gepubliceerd. Zelfs als het item was gemarkeerd voor publicatie toen u het wist, wordt het niet gepubliceerd.
* Het item blijft in de map met prullenmand staan totdat het is hersteld, zeven dagen zijn verstreken of totdat iemand de opdracht Leeg de prullenmand heeft gekozen. Na zeven dagen verwijdert een automatische opschoonbewerking het item definitief.

## Elementen herstellen vanuit de map Prullenmand {#restoring-assets-from-the-trash-folder}

De persoon die een middel heeft verwijderd, hoeft dit niet te herstellen. iedereen kan middelen herstellen vanuit de map Prullenmand. Elementen die worden hersteld, worden geplaatst in de mappen waaruit ze zijn verwijderd. Als deze omslagen niet meer bestaan, creeert het het Publiceren Scene7 Systeem opnieuw hen, en de herstelde activa worden geplaatst in de opnieuw gecreëerde omslagen.

Ga als volgt te werk om middelen van de map Prullenbak te herstellen naar de mappen waaruit ze zijn verwijderd:

1. Klik op het prullenbakpictogram om de map Prullenmand te openen.
1. Selecteer de elementen die u wilt herstellen.
1. Kies Bestand > Herstellen vanuit prullenbak.

## Elementen definitief verwijderen in de map Prullenbak {#permanently-deleting-assets-in-the-trash-folder}

Wanneer u middelen in de omslag van het Afval schrapt, worden de activa permanent geschrapt. Middelen worden na zeven dagen automatisch uit de prullenmand verwijderd.

Als u elementen definitief wilt verwijderen uit de map Prullenbak, selecteert u het prullenbakpictogram om de map Prullenmand te openen. Verwijder vervolgens de afzonderlijke elementen of verwijder alle elementen in de map:

* **Afzonderlijke elementen** verwijderen Selecteer de elementen die u permanent wilt verwijderen en klik op **[!UICONTROL File > Empty From Trash]**.

* **Alle elementen** verwijderen Klik **[!UICONTROL File > Empty Trash]**.

>[!MORELIKETHIS]
>
>* [Elementen verwijderen](moving-renaming-deleting-assets.md#delete_assets)

