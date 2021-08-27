---
title: Voorinstellingen eCatalog-viewer instellen
description: Leer hoe u voorinstellingen voor eCatalog-viewers instelt in Adobe Dynamic Media Classic.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: fa0a3992e02f70e5fb4a54e770e2fe2b4f0371e1
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Voorinstellingen eCatalog-viewer instellen{#setting-up-ecatalog-viewer-presets}

De eCatalog Viewer-voorinstellingen bepalen de stijl, het gedrag en de vormgeving van eCatalog-viewers. Adobe Dynamic Media Classic biedt voorinstellingen voor eCatalog-viewers en u kunt ook uw eigen voorinstellingen voor eCatalog-viewers maken als beheerder.

Als u een voorinstelling wilt maken, begint u helemaal opnieuw of begint u met een door de Adobe Dynamic Media Classic geleverde voorinstelling voor de eCatalog Viewer en slaat u deze onder een andere naam op. U kunt uw eigen voorinstellingen voor de eCatalog-viewer maken om afgedrukt materiaal in de kleuren van uw bedrijf weer te geven en de toon in te stellen.

Voorinstellingen voor eCatalog Viewer bieden veel instellingen voor het schakelen tussen pagina&#39;s, zoomen, zoeken en kiezen van &#39;skins&#39;. Hoe deze besturingselementen eruitzien en hoe de viewer wordt weergegeven, is afhankelijk van uw keuze voor Voorinstellingen voor eCatalog-viewer.

Voer de volgende stappen uit, zodat u een voorinstelling voor een eCatalog-viewer kunt maken (u dient beheerder te zijn):

1. Ga op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Maak in het scherm Voorinstellingen viewer een voorinstelling voor de eCatalog-viewer door een nieuwe voorinstelling te starten of door te beginnen met een bestaande voorinstelling voor de eCatalog-viewer:

   * **Een voorinstelling**  voor een eCatalog-viewer maken - Selecteren  **[!UICONTROL Add]**. Kies in het dialoogvenster Voorinstelling viewer toevoegen een platform, kies eCatalog Viewer en selecteer **[!UICONTROL Add]**.

   * **Een voorinstelling**  voor een eCatalog-viewer bewerken - Selecteer een voorinstelling voor een eCatalog-viewer en selecteer  **[!UICONTROL Edit]**. Selecteer **[!UICONTROL Save As]** nadat u klaar bent met het maken van de voorinstelling.

1. Voer in het scherm Viewer configureren een naam in voor uw voorinstelling voor de eCatalog-viewer.
1. Stel in het scherm Viewer configureren de gewenste opties in.

   Selecteer het **[!UICONTROL Info Tip]** pictogram naast de optie als u zijn beschrijving wilt lezen.

   Op de pagina Voorbeeld wordt de viewer weergegeven terwijl u instellingen bijwerkt en wijzigt.

1. (Optioneel) In de **[!UICONTROL Info Panel Settings]** kan de optie **[!UICONTROL Information Server URL]** de volgende speciale tokens bevatten, die door de viewer worden vervangen:

   | Token | Vervangen door | Notities |
   | --- | --- | --- |
   | `$1$` | rollover_key, waarde | De item-id van het element `<area>` van de kaart. |
   | `$2$` | frame | Het volgnummer van het momenteel weergegeven frame in de afbeeldingsset. |
   | `$3$` | hoofdafbeelding | Het eerste padelement van het eerste item dat is opgegeven in de opdracht Afbeelding (doorgaans de afbeeldingencatalogus-id van het item in de catalogus die de afbeeldingsset opgeeft). |

1. (Optioneel) Typ in het tekstvak **[!UICONTROL Info Panel Settings]** de tekst die u wilt weergeven als bij Adobe Dynamic Media Classic een fout optreedt bij het ophalen van informatie voor een afbeeldingskaart. **[!UICONTROL Response Template]** Als het systeem bijvoorbeeld een bedrijfsnaam en een eCatalog-naam ontvangt, maar geen rollover-id, wordt dit bericht voor de gebruiker weergegeven.

>[!NOTE]
>
>Als u deze antwoordsjabloon wilt gebruiken in plaats van de sjabloon die in de eCatalog zelf is gedefinieerd, voegt u `fmt=1` toe aan het einde van de URL van de Informatieserver. Bijvoorbeeld: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Selecteer **[!UICONTROL Save]**.
1. Selecteer **[!UICONTROL Default]** als u wilt dat de eCatalog Viewer-voorinstelling die u hebt gemaakt de voorinstelling is die wordt gebruikt om eCatalogi op uw webpagina weer te geven.

Als u een voorinstelling voor een eCatalog-viewer wilt verwijderen, selecteert u deze in het scherm Voorinstellingen viewer en selecteert u **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Voorinstellingen viewer](application-setup.md#viewer_presets)

