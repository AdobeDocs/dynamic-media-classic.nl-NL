---
title: Een gemengde mediaset maken
description: Leer hoe u een gemengde mediaset maakt.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Klassiek,Viewers,Gemengde Mediasets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
source-git-commit: 5f7e0c821dc2a34170e811157c9e689370d36d21
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Een gemengde mediaset maken{#creating-a-mixed-media-set}

Maak een gemengde mediaset als u meerdere typen viewers in één presentatie wilt combineren. Zorg ervoor dat de bestanden, afbeeldingssets, stalensets en centrifuges klaar zijn om te worden gepubliceerd voordat u ze aan de gemengde mediaset toevoegt.

![Gemengde mediaset](/help/assets/mm_mixed_media_set.png)

## Een gemengde mediaset maken {#create-a-mixed-media-set}

Wanneer u een set maakt, heeft de optie **Publiceren na opslaan** op de volgende manieren invloed op de set en stelt u leden in:

| De optie Publiceren na opslaan is geselecteerd voordat u het bestand opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een gemengde mediaset maken:**

1. Klik op **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]**.
1. Sleep de video&#39;s, de Reeksen van het Beeld, de Reeksen van de Rotatie, en de monsters van de Bibliotheek van Activa aan het Gemengde scherm van de Plaats van Media.

   >[!NOTE]
   >
   >Een gemengde mediaset ondersteunt geen elementen met bestandsnamen die een van de volgende tekens bevatten: `( ) { }`.

1. Voer een van de volgende handelingen uit:

   * Als u een soundtrack wilt toevoegen, sleept u een audiobestand uit de elementenbibliotheek naar het vak Soundtrack. De soundtrack wordt afgespeeld terwijl afbeeldingen worden weergegeven. Het stopt wanneer video wordt afgespeeld.
   * Als u de volgorde van sets wilt wijzigen, sleept u deze naar nieuwe locaties in het scherm Gemengde mediaset. De volgorde van sets op het scherm bepaalt de volgorde van links naar rechts waarin gebruikers sets zien in de Gemengde Media Set Viewer.
   * (Optioneel) Als u een aangepaste miniatuur wilt toevoegen om een video in de viewer te vertegenwoordigen, sleept u een afbeeldingsbestand van de elementenbibliotheek naar het vak voor de plaatsaanduiding van miniaturen.

1. Zorg dat in de rechterbenedenhoek van de pagina **[!UICONTROL Publish after save]** is geselecteerd (standaardwaarde).
1. Klik **[!UICONTROL Save]**, selecteer een omslag voor het opslaan van uw Gemengde Reeks van Media, ga een naam voor de reeks in, en klik **[!UICONTROL Save]**.

   Klik op **[!UICONTROL Preview]** om te zien hoe de set met comboafbeeldingen er in een Image Set Viewer uitziet.

## Een gemengde mediaset bewerken {#edit-a-mixed-media-set}

U kunt een gemengde Mediaset bewerken. Als u een set in een gemengde mediaset wilt bewerken, opent u die set afzonderlijk, bewerkt u de set en slaat u deze op. De bewerkingen worden weergegeven in de set Gemengde media.

Of u een gepubliceerde of een niet-gepubliceerde set bewerkt, de optie **[!UICONTROL Publish after save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | De optie Publiceren na opslaan is geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |--- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een gemengde mediaset bewerken:**

1. Klik op de rollover **[!UICONTROL Edit]**-knop van de gemengde mediaset.
1. Voer een van de volgende handelingen uit:

   * Als u items wilt verwijderen, selecteert u de items en klikt u op **[!UICONTROL Delete]**.
   * Als u de volgorde van de items wilt wijzigen, sleept u ze naar nieuwe locaties.

1. Als u klaar bent met het bewerken van de set, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Klik op **[!UICONTROL Save]** of **[!UICONTROL Save As]**.

## Een gemengde mediaset verwijderen {#deleting-a-mixed-media-set}

Wanneer u een set verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een gemengde mediaset verwijderen:**

1. Selecteer een of meer gemengde mediasets in de rasterweergave, lijstweergave of detailweergave.
1. Klik op **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** op de algemene navigatiebalk.
