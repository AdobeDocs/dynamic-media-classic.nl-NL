---
title: Mediaportaalgroepen maken en beheren
description: Leer hoe u mediaportaalgroepen maakt en beheert in Adobe Dynamic Media Classic.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---

# Mediaportaalgroepen maken en beheren{#creating-and-managing-media-portal-groups}

*Groepen* zijn ontworpen om u te helpen de gebruikers van het Portaal van Media beheren. Om tot activa toegang te hebben, moet een gebruiker een lid van minstens één groep zijn die toestemming heeft om tot dat activa toegang te hebben. Wanneer u een gebruiker toevoegt, wijst u de gebruiker aan een of meer groepen toe. Op die manier verleent u de gebruiker toegang tot mappen waaraan de groep is toegewezen. U kunt ook kiezen welke voorinstellingen voor afbeeldingen beschikbaar zijn voor een groep.

## Groepen gebruiken om de toegang tot mappen, elementen en voorinstellingen voor afbeeldingen te beperken {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Om toegangstoestemming op verschillende niveaus te verlenen, creeert u groepen. Voor elke groep wijst u lees-, schrijf- en verwijdermachtigingen toe aan verschillende mappen en elementen in mappen. U bepaalt ook welke voorinstellingen voor afbeeldingen beschikbaar zijn voor de groep. Vervolgens wijst u gebruikers toe aan groepen. Een gebruiker kan lid zijn van meerdere groepen. Het groepsconcept biedt u de flexibiliteit om toegang toe te wijzen aan beperkte reeksen van de totale inhoud.

Als u niet specifiek groepsmachtigingen toekent aan een middel of map, neemt dat middel of die map de machtigingen over die u aan de bovenliggende map hebt toegewezen (de map erboven in de mappenhiërarchie). Verleen toestemmingen aan een ouderomslag als u wilt ervoor zorgen dat al zijn kindomslagen de zelfde toestemmingen erven.

>[!NOTE]
>
>Gebruikers kunnen tot meerdere groepen behoren. Wanneer een gebruiker tot twee groepen met verschillende toegangstoestemmingen tot een omslag behoort, wordt de gebruiker de hoogste toegang verleend.

## Een groep toevoegen {#adding-a-group}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Selecteren **[!UICONTROL Add]**.
1. Voer in het dialoogvenster Groep toevoegen een naam voor de groep in het vak Groepsnaam in en selecteer vervolgens **[!UICONTROL Add Group]**.
1. Desgewenst kunt u de vakken naast de namen van gebruikers selecteren om gebruikers aan de nieuwe groep toe te voegen.
1. Als u nu toegangsmachtigingen wilt opgeven, selecteert u de optie **[!UICONTROL Asset Access Permissions]** en geeft u de gewenste opties op.

   Zie [Machtigingen instellen voor elementtoegang voor een groep](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Als u wilt kiezen welke Voorinstellingen afbeelding beschikbaar zijn voor de groep, selecteert u de optie **[!UICONTROL Image Preset Access Permissions]** en selecteert u Voorinstellingen afbeelding die de groep kan gebruiken.

   Zie [Toegangsrechten voor een groep kiezen voor Voorinstelling afbeelding](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Selecteren **[!UICONTROL Close]**.

## Machtigingen instellen voor elementtoegang voor een groep {#establishing-asset-access-permissions-for-a-group}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Voer een van de volgende handelingen uit op de lijstpagina Groepen:

   * Als u een groep wilt toevoegen en machtigingen wilt opgeven, selecteert u **[!UICONTROL Add]**. Voer in het dialoogvenster Groep toevoegen een naam voor de groep in en selecteer **[!UICONTROL Add Group]** en voegt u gebruikers toe aan de groep.
   * Als u de machtigingen van een groep wilt bewerken, selecteert u de groep en selecteert u **[!UICONTROL Edit]**.

1. Selecteer in het dialoogvenster Groep toevoegen of groep bewerken de optie **[!UICONTROL Asset Access Permissions]** tab. De rechterkant van de tab biedt vakken voor het instellen van lees-, schrijf- en verwijdermachtigingen voor mappen en elementen. U kunt mappen en submappen in het linkerdeelvenster uit- en samenvouwen.
1. Als u rechten wilt toewijzen aan mappen of afzonderlijke elementen, selecteert u de map in het linkerdeelvenster. De inhoud van de map wordt weergegeven in het rechterdeelvenster. Wijs vervolgens rechten toe aan de groep door de vakken voor de corresponderende bestanden of mappen in het rechterdeelvenster te selecteren.

   In deze tabel worden verschillende taken toegewezen aan het lezen, schrijven en verwijderen van machtigingen.

   | Taak | Lezen | Schrijven | Verwijderen |
   | --- | --- | --- | --- |
   | Door mappen en bestanden bladeren | X |  |  |
   | Bestanden bewerken (uitsnijden, verscherpen, aanpassen) |  | X |  |
   | Bestandsnamen wijzigen |  | X |  |
   | Bestanden verplaatsen naar andere mappen |  | X |  |
   | Bestandsnamen wijzigen |  | X |  |
   | Bestanden verwijderen |  |  | X |

1. Selecteren **[!UICONTROL Close]**.

>[!NOTE]
>
>Toegangsrechten worden ingesteld wanneer u een vak selecteert. Wanneer u rechten toewijst aan een map, krijgen de submappen en alle bestanden in de map dezelfde rechten als de bovenliggende map. U kunt echter verschillende rechten opgeven voor afzonderlijke submappen en elementbestanden.

## Toegangsrechten voor een groep kiezen voor Voorinstelling afbeelding {#choosing-image-preset-access-permissions-for-a-group}

Kies Vooraf ingestelde de toegangstoestemmingen van het Beeld voor een groep als u wilt specificeren welke Vooraf ingestelde Beeld aan groepsleden beschikbaar zijn wanneer zij activa met het Portaal van Media uitvoeren.

Zie ook [Beschikbare exportopties voor gebruikers van Media Portal opgeven](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**U kunt als volgt toegangsmachtigingen voor een groep instellen voor Voorinstelling afbeelding:**

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Voer een van de volgende handelingen uit op de lijstpagina Groepen:

   * Als u een groep wilt toevoegen en wilt opgeven welke voorinstellingen voor afbeeldingen er beschikbaar zijn, selecteert u **[!UICONTROL Add]**. Voer in het dialoogvenster Groep toevoegen een naam voor de groep in en selecteer **[!UICONTROL Add Group]** en voegt u gebruikers toe aan de groep.
   * Als u de voorinstellingsopties voor afbeeldingen van een groep wilt bewerken, selecteert u de groep en selecteert u vervolgens **[!UICONTROL Edit]**.

1. Selecteer in het dialoogvenster Groep toevoegen of groep bewerken de optie **[!UICONTROL Image Preset Access Permissions]** tab.
1. Als u wilt opgeven welke voorinstellingen beschikbaar zijn voor gebruikers van Media Portal wanneer zij elementen exporteren, schakelt u Voorinstellingen afbeelding in of uit.
1. Selecteren **[!UICONTROL Close]**.

## Groepen bewerken en verwijderen {#edit-and-delete-groups}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Selecteer op de pagina Groepenlijst een groep en bewerk of verwijder deze.

   **Een groep bewerken** - Selecteer **[!UICONTROL Edit]** en kies vervolgens opties in het dialoogvenster Groep bewerken.

   **Een groep verwijderen** - Selecteer **[!UICONTROL Delete]**.
