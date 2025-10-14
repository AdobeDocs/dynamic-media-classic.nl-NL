---
title: Een gemengde mediaset maken
description: Leer hoe u een gemengde mediaset maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Een gemengde mediaset maken{#creating-a-mixed-media-set}

Maak een gemengde mediaset als u meerdere typen viewers in één presentatie wilt combineren. Zorg ervoor dat de bestanden, afbeeldingssets, stalensets en centrifuges klaar zijn om te worden gepubliceerd voordat u ze aan de gemengde mediaset toevoegt.

![&#x200B; Gemengde Geplaatste Media &#x200B;](/help/using/assets/mm_mixed_media_set.png)

## Een gemengde mediaset maken {#create-a-mixed-media-set}

Wanneer u een reeks creeert, publiceert **na sparen** optie beïnvloedt de reeks en vastgestelde leden op de volgende manieren:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Gemengde Reeks van Media tot stand te brengen:**

1. Ga naar **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]** .
1. Sleep de video&#39;s, de Reeksen van het Beeld, de Reeksen van de Rotatie, en de monsters van de Bibliotheek van Activa aan het Gemengde scherm van de Plaats van Media.

   >[!NOTE]
   >
   >Een gemengde mediaset ondersteunt geen elementen met bestandsnamen die de volgende tekens bevatten: `( ) { }` .

1. Voer een van de volgende handelingen uit:

   * Als u een soundtrack wilt toevoegen, sleept u een audiobestand uit de elementenbibliotheek naar het vak Soundtrack. De soundtrack wordt afgespeeld terwijl afbeeldingen worden weergegeven. De video stopt wanneer een video wordt afgespeeld.
   * Als u de volgorde van sets wilt wijzigen, sleept u deze naar nieuwe locaties in het scherm Gemengde mediaset. De volgorde van sets op het scherm bepaalt de volgorde van links naar rechts waarin gebruikers sets zien in de Gemengde Media Set Viewer.
   * (Optioneel) Als u een aangepaste miniatuur wilt toevoegen om een video in de viewer te vertegenwoordigen, sleept u een afbeeldingsbestand van de elementenbibliotheek naar het vak voor de plaatsaanduiding van miniaturen.

1. Zorg dat rechts onder op de pagina de optie **[!UICONTROL Publish after a save]** is geselecteerd (standaardwaarde).
1. Selecteer **[!UICONTROL Save]** .
1. Selecteer een map voor het opslaan van de gemengde mediaset en voer een naam voor de set in.
1. Selecteer **[!UICONTROL Save]** .

   Selecteer **[!UICONTROL Preview]** om te zien hoe de set met combo-afbeeldingen er in een Afbeeldingsset-viewer uitziet.

## Een gemengde mediaset bewerken {#edit-a-mixed-media-set}

U kunt een gemengde Mediaset bewerken. Als u een set in een gemengde mediaset wilt bewerken, opent u die set afzonderlijk, bewerkt u de set en slaat u deze op. De bewerkingen worden weergegeven in de gemengde mediaset.

Of u nu een gepubliceerde of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after a save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after a save]** geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- |--- |--- |--- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Gemengde Reeks van Media uit te geven:**

1. Selecteer de rollover-knop van de gemengde mediaset **[!UICONTROL Edit]** .
1. Voer een van de volgende handelingen uit:

   * Als u items wilt verwijderen, selecteert u deze en selecteert u **[!UICONTROL Delete]** .
   * Als u de volgorde van de items wilt wijzigen, sleept u ze naar nieuwe locaties.

1. Als u klaar bent met het bewerken van de set, controleert u of **[!UICONTROL Publish after a save]** is geselecteerd (standaard) rechtsonder op de pagina.
1. Selecteer **[!UICONTROL Save]** of **[!UICONTROL Save As]** .

## Een gemengde mediaset verwijderen

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [&#x200B; manueel het publiceren activa &#x200B;](publishing-files.md#manually_publishing_assets) en [&#x200B; manueel unpublishing activa &#x200B;](publishing-files.md#manually_unpublishing_assets).

**om een Gemengde Reeks van Media te schrappen:**

1. Selecteer een of meer gemengde mediasets in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** .
