---
title: Voorinstellingen eCatalog-viewer instellen
description: Leer hoe u eCatalog Viewer-voorinstellingen instelt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Voorinstellingen eCatalog-viewer instellen{#setting-up-ecatalog-viewer-presets}

De eCatalog Viewer-voorinstellingen bepalen de stijl, het gedrag en de vormgeving van eCatalog-viewers. Adobe Dynamic Media Classic biedt voorinstellingen voor eCatalog-viewers en u kunt ook uw eigen voorinstellingen voor eCatalog-viewers maken als beheerder.

Als u een voorinstelling wilt maken, begint u helemaal opnieuw of begint u met een door Adobe Dynamic Media Classic geleverde voorinstelling voor de eCatalog Viewer en slaat u deze onder een andere naam op. U kunt uw eigen voorinstellingen voor de eCatalog-viewer maken om afgedrukt materiaal in de kleuren van uw bedrijf weer te geven en de toon in te stellen.

Voorinstellingen voor eCatalog Viewer bieden veel instellingen voor het schakelen tussen pagina&#39;s, zoomen, zoeken en kiezen van &#39;skins&#39;. Hoe deze besturingselementen eruitzien en hoe de viewer wordt weergegeven, is afhankelijk van uw keuze voor voorinstellingen voor eCatalog-viewers.

Voer de volgende stappen uit, zodat u een voorinstelling voor een eCatalog-viewer kunt maken (u dient beheerder te zijn):

1. Ga op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** .
1. Maak in het scherm Voorinstellingen viewer een voorinstelling voor de eCatalog-viewer door een nieuwe voorinstelling te starten of door te beginnen met een bestaande voorinstelling voor de eCatalog-viewer:

   * **creeer een Vooraf ingestelde eCatalogKijker**: Selecteer **[!UICONTROL Add]**. Kies in het dialoogvenster Voorinstelling viewer toevoegen een platform, kies eCatalog Viewer en selecteer vervolgens **[!UICONTROL Add]** .

   * **geef een Vooraf ingestelde eCatalogKijker** uit: Selecteer een eCatalogKijker Vooraf ingesteld, dan uitgezocht **[!UICONTROL Edit]**. Selecteer **[!UICONTROL Save As]** nadat u de voorinstelling hebt gemaakt.

1. Voer op de pagina `Configure Viewer` een naam in voor uw voorinstelling voor de eCatalog-viewer.
1. Stel op de pagina `Configure Viewer` de gewenste opties in.

   Selecteer het pictogram **[!UICONTROL Info Tip]** naast de optie als u de beschrijving van de optie wilt lezen.

   Op de pagina Voorbeeld wordt de viewer weergegeven terwijl u instellingen bijwerkt en wijzigt.

1. (Optioneel) In de **[!UICONTROL Info Panel Settings]** -optie kan de optie **[!UICONTROL Information Server URL]** de volgende speciale tokens bevatten, die door de viewer worden vervangen:

   | Token | Vervangen door | Notities |
   | --- | --- | --- |
   | `$1$` | rollover_key, waarde | De item-id van het element `<area>` van de kaart. |
   | `$2$` | frame | Het volgnummer van het momenteel weergegeven frame in de afbeeldingsset. |
   | `$3$` | hoofdafbeelding | Het eerste padelement van het eerste item dat is opgegeven in de opdracht Afbeelding (doorgaans de afbeeldingencatalogus-id van het item in de catalogus die de afbeeldingsset opgeeft). |

1. (Optioneel) Typ in het vak **[!UICONTROL Info Panel Settings]** in **[!UICONTROL Response Template]** de tekst die u wilt weergeven als Adobe Dynamic Media Classic een fout aantreft bij het ophalen van informatie voor een afbeeldingskaart. Als het systeem bijvoorbeeld een bedrijfsnaam en een eCatalog-naam ontvangt, maar geen rollover-id, wordt dit bericht voor de gebruiker weergegeven.

>[!NOTE]
>
>Als u deze antwoordsjabloon wilt gebruiken in plaats van de sjabloon die in de eCatalog zelf is gedefinieerd, voegt u `fmt=1` toe aan het einde van de URL van de Informatieserver. Bijvoorbeeld: `https://.../$3$/$4$/$1$/?FMT=1` .

1. Selecteer **[!UICONTROL Save]** .
1. Selecteer **[!UICONTROL Default]** zodat de voorinstelling voor de eCatalog-viewer die u hebt gemaakt de voorinstelling is die wordt gebruikt om eCatalogs weer te geven op uw webpagina.

Als u een voorinstelling voor een eCatalog-viewer wilt verwijderen, selecteert u deze in het scherm Voorinstellingen viewer en selecteert u **[!UICONTROL Delete]** .

>[!MORELIKETHIS]
>
>* [&#x200B; Kijker stelt vooraf in &#x200B;](application-setup.md#viewer_presets)
