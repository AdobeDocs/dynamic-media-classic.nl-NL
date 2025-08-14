---
title: Een afbeelding uitsnijden
description: Leer hoe u een afbeelding uitsnijdt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Een afbeelding uitsnijden{#cropping-an-image}

U kunt afbeeldingen uitsnijden in de Adobe Dynamic Media Classic. Het systeem behoudt informatie over afbeeldingen die zijn uitgesneden, zodat u ze in hun oorspronkelijke staat kunt herstellen. U kunt ook een afbeelding uitsnijden en de bijgesneden versie onder een andere naam opslaan.

U kunt een afbeelding uitsnijden om witruimte rondom de afbeelding te verwijderen of een gedeelte van de afbeelding uit te snijden.

>[!NOTE]
>
>Na het uitsnijden kunt u **[!UICONTROL Save As]** selecteren en een uitgesneden versie van de afbeelding onder een andere naam opslaan. Selecteer **[!UICONTROL Save As New Primary]** in het venster Opslaan als om een tweede kopie van de afbeelding op te slaan. Selecteer **[!UICONTROL Save As Addition View Of Primary]** om het origineel en de bijgesneden versie onder een andere naam op te slaan. Selecteer **[!UICONTROL Replace Original]** om het originele bestand te verwijderen waaruit u de afbeelding hebt bijgesneden. Voer vervolgens een naam voor de afbeelding in en selecteer **[!UICONTROL Submit]** .

## Uitsnijden om witruimte rondom een afbeelding te verwijderen {#crop-to-remove-white-space-around-an-image}

U kunt de transparante of effen kleurpixels uitsnijden vanaf de rand van een afbeelding.

1. Als u een afbeelding wilt uitsnijden, selecteert u de rolloverknop **[!UICONTROL Edit]** en selecteert u **[!UICONTROL Crop]** . U kunt de afbeelding ook weergeven in het deelvenster Bladeren in de gedetailleerde weergave en de knop **[!UICONTROL Crop]** selecteren.
1. Voer een van de volgende handelingen uit op de pagina Uitsnijdbewerker:

   * Als u kleurpixels wilt bijsnijden, gaat u naar **[!UICONTROL Trim]** > **[!UICONTROL Color]** . Selecteer in het dialoogvenster **[!UICONTROL Auto Crop By Color]** het menu **[!UICONTROL Corner]** en kies een hoek met de achtergrondkleur die u wilt wegsnijden. Voer vervolgens een **[!UICONTROL Tolerance]** instelling in van 0 tot en met 1. Met de instelling 0 worden alleen pixels uitgesneden als deze exact overeenkomen met de kleur die u in de hoek van de afbeelding hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe. Selecteer **[!UICONTROL Crop]** .
   * Als u transparante pixels wilt bijsnijden, gaat u naar **[!UICONTROL Trim]** > **[!UICONTROL Transparent]** . Voer in het dialoogvenster **[!UICONTROL Auto Crop By Transparency]** een tolerantiewaarde in tussen 0 en 1. Met de instelling 0 worden alleen pixels uitgesneden als deze transparant zijn. De aantallen dichter aan 1 staan voor meer transparantie toe. Selecteer **[!UICONTROL Crop]** .

1. Selecteer **[!UICONTROL Save]** .

>[!NOTE]
>
>Als u de oorspronkelijke staat van een afbeelding wilt herstellen nadat u de afbeelding hebt bijgesneden, geeft u de afbeelding weer in de Uitsnijdeditor en selecteert u **[!UICONTROL Reset]** .

## Een gebied selecteren voor uitsnijden {#select-an-area-to-crop}

1. Als u een afbeelding wilt uitsnijden, selecteert u de rolloverknop **[!UICONTROL Edit]** en kiest u **[!UICONTROL Crop]** . U kunt de afbeelding ook weergeven in het deelvenster Bladeren in de gedetailleerde weergave en u kunt **[!UICONTROL Crop]** selecteren.

1. Plaats in het venster Uitsnijdbewerker het gedeelte van de afbeelding dat u niet wilt uitsnijden in het uitsnijdvak. Wat er in het vak wordt weergegeven, is wat er overblijft als u **[!UICONTROL Save]** selecteert en de afbeelding bijsnijdt.
1. Voer een van de volgende handelingen uit om het snijgebied aan te passen:

   * Sleep een zijde of hoek van het vak. Houd Shift ingedrukt terwijl u sleept om de grootte te wijzigen, maar houd de hoogte-breedteverhouding (de vorm) van het uitsnijdvak behouden.
   * Geef pixelmetingen op in de vakken Grootte.
   * Sleep om het uitsnijdvak te verplaatsen. Plaats de aanwijzer binnen de grens van het vak. Als u de pijl met vier punten ziet, sleept u het vak naar een nieuwe locatie op de afbeelding.

1. Selecteer **[!UICONTROL Save]** .

>[!NOTE]
>
>Als u de oorspronkelijke staat van een afbeelding wilt herstellen nadat u de afbeelding hebt bijgesneden, geeft u de afbeelding weer in de Uitsnijdeditor en selecteert u **[!UICONTROL Reset]** .

>[!MORELIKETHIS]
>
>* [ Opties voor beeld-uitgeeft bij upload ](image-editing-options-upload.md#image-editing-options-at-upload)
>* [ het witte ruimte van het Gewas van een dossier van PDF ](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [ Gewas van de kanten van de pagina&#39;s van PDF ](pdfs.md#cropping_from_the_sides_of_pdf_pages)
