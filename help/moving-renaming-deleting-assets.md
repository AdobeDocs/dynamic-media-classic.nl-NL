---
title: Elementen verplaatsen, hernoemen en verwijderen
description: Leer hoe u elementen verplaatst, hernoemt en verwijdert in Adobe Dynamic Media Classic.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Elementen verplaatsen, hernoemen en verwijderen{#moving-renaming-and-deleting-assets}

U kunt elementen verplaatsen, hernoemen en verwijderen vanuit het deelvenster Bladeren. Bovendien kunt u veel elementen tegelijk met een tekstbestand verwijderen.

## Elementen verplaatsen {#move-assets}

U kunt elementen naar verschillende mappen verplaatsen in het deelvenster Bladeren.

1. Selecteer de elementen in het deelvenster Bladeren en voer een van de volgende handelingen uit:

   * Geef de map weer waarnaar u de elementen wilt verplaatsen in de elementenbibliotheek en sleep de elementen naar de map.
   * Ga naar **[!UICONTROL File]** > **[!UICONTROL Move]**, selecteer een map in het venster Elementen verplaatsen en selecteer **[!UICONTROL Move]**.

## Elementen hernoemen {#rename-assets}

1. Selecteer het element in het deelvenster Bladeren en voer een van de volgende handelingen uit:

   * Selecteer de naam, typ een nieuwe naam en druk op **[!UICONTROL Enter]** of selecteer een andere naam.
   * Ga naar **[!UICONTROL File]** > **[!UICONTROL Rename]**. De naam van het element wordt gemarkeerd. Voer een nieuwe naam in en druk op **[!UICONTROL Enter]**.

Zorg ervoor dat u de naam van een bestaand Adobe Dynamic Media Classic-element niet invoert.

## Elementen verwijderen {#delete-assets}

U kunt geselecteerde elementen verwijderen uit het deelvenster Bladeren en volledige mappen verwijderen. Verwijderde middelen en mappen worden naar de prullenmand verplaatst, waar ze zeven dagen blijven voordat ze definitief worden verwijderd.

Wanneer u een element verwijdert, worden ook alle elementen die ervan zijn afgeleid, verwijderd. Als u bijvoorbeeld een afbeelding verwijdert waarvoor u zoomdoelen hebt gemaakt, worden de zoomdoelen samen met de afbeelding verwijderd.

>[!NOTE]
>
>Zoomdoelen, afbeeldingskenmerken en historiegegevens worden permanent verwijderd wanneer u de elementen verwijdert waaruit ze afkomstig zijn. Ze worden niet samen met het element verplaatst naar de map Prullenbak. ze kunnen niet vanuit de prullenbak worden hersteld.

1. Voer een van de volgende handelingen uit:

   * Als u een of meer elementen wilt verwijderen, selecteert u de elementen in het deelvenster Bladeren en drukt u op **[!UICONTROL Delete]** of gaat u naar **[!UICONTROL File]** > **[!UICONTROL Delete]**.
   * Als u een map wilt verwijderen, selecteert u de map in de elementenbibliotheek en selecteert u **[!UICONTROL Remove Folder]**.

      Als u een map verwijdert, worden de map, alle elementen in de map en alle elementen in de submappen verwijderd.

>[!NOTE]
>
>Adobe Dynamic Media Classic raadt aan elementbestanden te overschrijven in plaats van ze te verwijderen als het verwijderen van een elementbestand ertoe leidt dat het bestand met dezelfde naam wordt vervangen door een ander bestand.

## Meerdere elementen met een tekstbestand verwijderen {#delete-multiple-assets-with-a-text-file}

Als u veel elementen tegelijk wilt verwijderen in de Middelenbibliotheek, kunt u de elementen die u wilt verwijderen, in een tekstbestand weergeven en de lijst naar Adobe Dynamic Media Classic verzenden.

Maak een lijst met klassieke id&#39;s van Adobe Dynamic Media en sla deze op als tekstbestand (.txt). Elke Adobe Dynamic Media Classic-id moet op een eigen regel staan (gevolgd door een harde return).

Nadat u de lijst hebt gemaakt, voert u de volgende stappen uit om elementen te verwijderen:

1. Ga naar **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**.
1. Blader in het dialoogvenster Lijst met elementen verwijderen naar het tekstbestand of typ het pad naar het tekstbestand met de lijst met elementen die u wilt verwijderen.
1. Selecteer **[!UICONTROL Delete]**.

Wanneer u elementen met een tekstbestand verwijdert en geen Adobe Dynamic Media Classic ID in de lijst voorkomt, wordt het bericht &quot;Kan deze items in de lijst niet valideren:&quot; weergegeven en de lijst met vermeldingen. Adobe Dynamic Media Classic genereert echter geen fout op de taakpagina.

>[!MORELIKETHIS]
>
>* [Elementen selecteren in het deelvenster Bladeren](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Elementen en mappen voorbereiden voor uploaden](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Elementen herstellen vanuit de map Prullenbak](trash-folder.md#restoring_assets_from_the_trash_folder)

