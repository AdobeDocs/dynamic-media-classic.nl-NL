---
title: Elementen verplaatsen, hernoemen en verwijderen
seo-title: Elementen verplaatsen, hernoemen en verwijderen
description: 'null'
seo-description: Leer hoe u elementen verplaatst, hernoemt en verwijdert.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---


# Elementen verplaatsen, hernoemen en verwijderen{#moving-renaming-and-deleting-assets}

U kunt elementen verplaatsen, hernoemen en verwijderen vanuit het deelvenster Bladeren. Bovendien kunt u veel elementen tegelijk met een tekstbestand verwijderen.

## Elementen {#move-assets} verplaatsen

U kunt elementen naar verschillende mappen verplaatsen in het deelvenster Bladeren.

1. Selecteer de elementen in het deelvenster Bladeren en voer een van de volgende handelingen uit:

   * Geef de map weer waarnaar u de elementen wilt verplaatsen in de elementenbibliotheek en sleep de elementen naar de map.
   * Kies Bestand > Verplaatsen, selecteer een map in het venster Middelen verplaatsen en selecteer Verplaatsen.

## Naam van elementen wijzigen {#rename-assets}

De naam van een element wijzigen:

1. Selecteer het element in het deelvenster Bladeren en voer een van de volgende handelingen uit:

   * Selecteer de naam, typ een nieuwe naam en druk op Enter of klik buiten de naam.
   * Kies Bestand > Naam wijzigen. De naam van het element wordt gemarkeerd. Voer een nieuwe naam in en druk op Enter.

Zorg ervoor dat u de naam van een bestaand Dynamic Media Classic-element niet invoert.

## Elementen {#delete-assets} verwijderen

U kunt geselecteerde elementen verwijderen uit het deelvenster Bladeren en volledige mappen verwijderen. Verwijderde middelen en mappen worden naar de prullenmand verplaatst, waar ze zeven dagen blijven voordat ze definitief worden verwijderd.

Wanneer u een element verwijdert, worden ook alle elementen die ervan zijn afgeleid, verwijderd. Als u bijvoorbeeld een afbeelding verwijdert waarvoor u zoomdoelen hebt gemaakt, worden de zoomdoelen samen met de afbeelding verwijderd.

>[!NOTE]
>
>Zoomdoelen, afbeeldingskenmerken en historiegegevens worden permanent verwijderd wanneer u de elementen verwijdert waaruit ze afkomstig zijn. Ze worden niet samen met het element verplaatst naar de map Prullenbak. ze kunnen niet vanuit de prullenbak worden hersteld.

1. Voer een van de volgende handelingen uit:

   * Als u een of meer elementen wilt verwijderen, selecteert u de elementen in het deelvenster Bladeren en drukt u op Verwijderen of kiest u Bestand > Verwijderen.
   * Als u een map wilt verwijderen, selecteert u de map in de elementenbibliotheek en klikt u op **Map verwijderen**.

      Als u een map verwijdert, worden de map, alle elementen in de map en alle elementen in de submappen verwijderd.

>[!NOTE]
>
>Dynamic Media Classic raadt aan elementbestanden te overschrijven in plaats van ze te verwijderen als het verwijderen van een elementbestand ertoe leidt dat het bestand met dezelfde naam door een ander bestand wordt vervangen.

## Meerdere elementen verwijderen met een tekstbestand {#delete-multiple-assets-with-a-text-file}

Als u veel elementen tegelijk wilt verwijderen uit de hele bibliotheek met middelen, kunt u de elementen die u wilt verwijderen, in een tekstbestand weergeven en de lijst naar Dynamic Media Classic verzenden.

Maak een lijst met klassieke Dynamic Media-id&#39;s en sla deze op als tekstbestand (.txt). Elke klassieke Dynamic Media-id moet op een eigen regel staan (gevolgd door een harde return).

Nadat u de lijst hebt gemaakt, voert u de volgende stappen uit om elementen te verwijderen:

1. Kies Bestand > Lijst met elementen verwijderen.
1. Blader in de lijst Elementen verwijderen of typ het pad naar het tekstbestand met de lijst met elementen die u wilt verwijderen.
1. Klik op de knop Verwijderen.

Als u elementen verwijdert uit een tekstbestand en er geen klassieke Dynamic Media-id in de lijst staat, wordt een bericht weergegeven met de mededeling dat Dynamic Media Classic &quot;Kan deze items in de lijst niet valideren:&quot; is, samen met de lijst met vermeldingen. Dynamic Media Classic genereert echter geen fout op het taakscherm.

>[!MORELIKETHIS]
>
>* [Elementen selecteren in het deelvenster Bladeren](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Elementen en mappen voorbereiden voor uploaden](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Elementen herstellen vanuit de map Prullenmand](trash-folder.md#restoring_assets_from_the_trash_folder)

