---
title: Een afbeelding uitsnijden
description: Leer hoe u een afbeelding uitsnijdt in Adobe Dynamic Media Classic.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Een afbeelding uitsnijden{#cropping-an-image}

U kunt afbeeldingen uitsnijden in de Adobe Dynamic Media Classic. Het systeem behoudt informatie over afbeeldingen die zijn uitgesneden, zodat u ze in hun oorspronkelijke staat kunt herstellen. U kunt ook een afbeelding uitsnijden en de bijgesneden versie onder een andere naam opslaan.

U kunt een afbeelding uitsnijden om witruimte rondom de afbeelding te verwijderen of een gedeelte van de afbeelding uit te snijden.

>[!NOTE]
>
>Nadat u hebt uitgesneden, kunt u selecteren **[!UICONTROL Save As]** en sla een bijgesneden versie van de afbeelding op onder een andere naam. Selecteer in het venster Opslaan als de optie **[!UICONTROL Save As New Master]** om een tweede kopie van de afbeelding op te slaan. Selecteren **[!UICONTROL Save As Addition View Of Master]** zodat u het origineel en de bijgesneden versie onder een andere naam kunt opslaan. Selecteren **[!UICONTROL Replace Original]** om het oorspronkelijke bestand te verwijderen waaruit u de afbeelding hebt bijgesneden. Voer vervolgens een naam voor de afbeelding in en selecteer **[!UICONTROL Submit]**.

## Uitsnijden om witruimte rondom een afbeelding te verwijderen {#crop-to-remove-white-space-around-an-image}

U kunt de transparante of effen kleurpixels uitsnijden vanaf de rand van een afbeelding.

1. Als u een afbeelding wilt uitsnijden, selecteert u de rollover **[!UICONTROL Edit]** en selecteert u vervolgens **[!UICONTROL Crop]** of in het deelvenster Bladeren in de detailweergave en selecteer de optie **[!UICONTROL Crop]** knop.
1. Voer een van de volgende handelingen uit op de pagina Snijbewerker:

   * Ga naar **[!UICONTROL Trim]** > **[!UICONTROL Color]**. In de **[!UICONTROL Auto Crop By Color]** selecteert u het dialoogvenster **[!UICONTROL Corner]** en kiest u een hoek met de achtergrondkleur die u wilt wegsnijden. Voer vervolgens een **[!UICONTROL Tolerance]** instelling 0 tot en met 1. Met de instelling 0 worden alleen pixels uitgesneden als deze exact overeenkomen met de kleur die u in de hoek van de afbeelding hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe. Selecteren **[!UICONTROL Crop]**.
   * Ga naar **[!UICONTROL Trim]** > **[!UICONTROL Transparent]**. In de **[!UICONTROL Auto Crop By Transparency]** voert u een tolerantie in tussen 0 en 1. Met de instelling 0 worden alleen pixels uitgesneden als deze transparant zijn. De aantallen dichter aan 1 staan voor meer transparantie toe. Selecteren **[!UICONTROL Crop]**.

1. Selecteren **[!UICONTROL Save]**.

>[!NOTE]
>
>Als u de oorspronkelijke staat van een afbeelding wilt herstellen nadat u de afbeelding hebt bijgesneden, geeft u de afbeelding weer in de Crop Editor-scherm en selecteert u **[!UICONTROL Reset]**.

## Een gebied selecteren voor uitsnijden {#select-an-area-to-crop}

1. Als u een afbeelding wilt uitsnijden, selecteert u de rollover **[!UICONTROL Edit]** en kiest u **[!UICONTROL Crop]**, of toon het in het Browse Comité in de Gedetailleerde Mening en selecteer **[!UICONTROL Crop]**.

1. Plaats in het venster Uitsnijdbewerker het gedeelte van de afbeelding dat u niet wilt uitsnijden in het uitsnijdvak. Wat er in het vak wordt weergegeven, is wat er overblijft als u **[!UICONTROL Save]** en snijd de afbeelding uit.
1. Voer een van de volgende handelingen uit om het snijgebied aan te passen:

   * Sleep een zijde of hoek van het vak. Houd Shift ingedrukt terwijl u sleept om de grootte te wijzigen, maar houd de hoogte-breedteverhouding (de vorm) van het uitsnijdvak behouden.
   * Geef pixelmetingen op in de vakken Grootte.
   * Sleep om het uitsnijdvak te verplaatsen. Plaats de aanwijzer binnen de grens van het vak. Als u de pijl met vier punten ziet, sleept u het vak naar een nieuwe locatie op de afbeelding.

1. Selecteren **[!UICONTROL Save]**.

>[!NOTE]
>
>Als u de oorspronkelijke staat van een afbeelding wilt herstellen nadat u de afbeelding hebt bijgesneden, geeft u de afbeelding weer in de Crop Editor-scherm en selecteert u **[!UICONTROL Reset]**.

>[!MORELIKETHIS]
>
>* [Opties voor het bewerken van afbeeldingen tijdens het uploaden](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Witruimte uitsnijden vanuit een PDF-bestand](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Uitsnijden vanaf de zijkanten van PDF pagina&#39;s](pdfs.md#cropping_from_the_sides_of_pdf_pages)
