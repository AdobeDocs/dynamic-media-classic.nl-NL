---
title: De map Prullenmand beheren
description: Leer hoe u de prullenmand beheert.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# De map Prullenmand beheren{#managing-the-trash-folder}

Items die u verwijdert uit Adobe Dynamic Media Classic, worden verplaatst naar de map Prullenbak. Het verwijderde bestand blijft zeven dagen in deze map staan totdat het wordt hersteld of definitief wordt verwijderd. U kunt verwijderde items controleren door op het pictogram **[!UICONTROL Trash]** onder aan de elementenbibliotheek te klikken en items op de mappagina Prullenbak weer te geven.

Alle gebruikers kunnen items in de map met prullenmand terugzetten naar de mappen waaruit ze zijn verwijderd. Alle gebruikers kunnen ook de prullenmand leeg maken met alle inhoud ervan.

Als u items verwijdert uit de map Prullenbak, worden items definitief verwijderd uit Adobe Dynamic Media Classic. items die uit de map Prullenbak zijn verwijderd, kunnen niet meer worden hersteld. Zie [Algemene instellingen van toepassing](application-setup.md#general_settings) voor informatie over het instellen van meldingen voor bedrijfsbeheerders wanneer elementen automatisch uit de prullenbak moeten worden verwijderd.

>[!NOTE]
>
>Elementen die naar de map Prullenmand zijn verplaatst, worden nog steeds geregistreerd bij Adobe Dynamic Media Classic. Als u een bestand probeert te uploaden dat dezelfde naam heeft als een verwijderd bestand in de map met prullenmand, behandelt Adobe Dynamic Media Classic het element dat u wilt uploaden als een gedupliceerd element. Er wordt dan een nummer aan de naam toegevoegd.

## De map Prullenbak {#about-the-trash-folder}

Als u een item in een map verwijdert, wordt het item in de map Prullenbak geplaatst. Het volgende gebeurt wanneer u een item verwijdert en naar de map Prullenbak verplaatst:

* Hoewel het item is verwijderd uit uw Klassieke Adobe Dynamic Media-mappen, kan de id ervan niet worden toegewezen aan een ander element zolang het zich in de prullenmand bevindt. Als u middelen probeert te uploaden met dezelfde naam als een bestand in de map Prullenmand, voegt Adobe Dynamic Media Classic een cijfer toe aan de naam van het element.
* Het item kan niet worden gepubliceerd. Zelfs als het item was gemarkeerd voor publicatie toen u het wist, wordt het niet gepubliceerd.
* Het item blijft in de map met prullenmand staan totdat het is hersteld, zeven dagen zijn verstreken of totdat iemand de opdracht **[!UICONTROL Empty the Trash]** heeft gekozen. Na zeven dagen verwijdert een automatische opschoonbewerking het item definitief.

## Elementen herstellen vanuit de map Prullenbak {#restoring-assets-from-the-trash-folder}

Het is niet nodig dat de persoon die een actief heeft verwijderd, het terugzet; iedereen kan middelen herstellen vanuit de map Prullenmand. Elementen die worden hersteld, worden geplaatst in de mappen waaruit ze zijn verwijderd. Als deze mappen niet meer bestaan, maakt Adobe Dynamic Media Classic ze opnieuw en worden de herstelde elementen in de opnieuw gemaakte mappen geplaatst.

Ga als volgt te werk om middelen van de map Prullenmand te herstellen naar de mappen waaruit ze zijn verwijderd:

1. Selecteer onder aan het deelvenster Elementenbibliotheek het pictogram **[!UICONTROL Trash]** om de prullenmand te openen.
1. Selecteer de elementen die u wilt herstellen.
1. Ga naar **[!UICONTROL File]** > **[!UICONTROL Restore from trash]**.

## Elementen definitief verwijderen in de map Prullenbak {#permanently-deleting-assets-in-the-trash-folder}

Wanneer u middelen in de omslag van het Afval schrapt, worden de activa permanent geschrapt. Middelen worden na zeven dagen automatisch uit de prullenmand verwijderd.

Als u elementen definitief wilt verwijderen uit de map met prullenmand, selecteert u het pictogram **[!UICONTROL Trash]**. Voer op de mappagina Prullenbak een van de volgende handelingen uit:

* **Afzonderlijke elementen**  verwijderen - Selecteer de elementen die u permanent wilt verwijderen en ga vervolgens naar  **[!UICONTROL File]** >  **[!UICONTROL Empty From Trash]**.

* **Alle elementen**  verwijderen - Ga naar  **[!UICONTROL File]** >  **[!UICONTROL Empty trash]**.

>[!MORELIKETHIS]
>
>* [Elementen verwijderen](moving-renaming-deleting-assets.md#delete_assets)

