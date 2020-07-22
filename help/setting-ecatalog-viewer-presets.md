---
title: Voorinstellingen eCatalog-viewer instellen
seo-title: Voorinstellingen eCatalog-viewer instellen
description: 'null'
seo-description: Leer hoe u voorinstellingen voor eCatalog-viewers instelt.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# Voorinstellingen eCatalog-viewer instellen{#setting-up-ecatalog-viewer-presets}

De eCatalog Viewer-voorinstellingen bepalen de stijl, het gedrag en de vormgeving van eCatalog-viewers. De Klassieke van Dynamic Media verstrekt eCatalogKijker vooraf instelt, en u kunt uw eigen eCatalogKijker tot stand brengen vooraf instelt evenals als u een beheerder bent.

Als u een nieuwe voorinstelling wilt maken, begint u helemaal opnieuw of begint u met een op Dynamic Media gebaseerde voorinstelling voor de eCatalog Viewer en slaat u deze onder een andere naam op. U kunt uw eigen voorinstellingen voor de eCatalog-viewer maken om afgedrukt materiaal in de kleuren van uw bedrijf weer te geven en de toon in te stellen.

Voorinstellingen voor eCatalog Viewer bieden veel instellingen voor het schakelen tussen pagina&#39;s, zoomen, zoeken en kiezen van &#39;skins&#39;. Hoe deze besturingselementen eruitzien en hoe de viewer er zelf uitziet, is afhankelijk van uw keuze voor eCatalog Viewer-voorinstellingen.

Ga als volgt te werk om een voorinstelling voor een eCatalog-viewer te maken (u dient beheerder te zijn):

1. Klik op **Instellen** > Voorinstellingen **van viewer**.
1. Maak in het scherm Voorinstellingen viewer een voorinstelling voor de eCatalog-viewer door een nieuwe voorinstelling te starten of door te beginnen met een bestaande voorinstelling voor de eCatalog-viewer:

   * **Een voorinstelling voor een eCatalog-viewer maken** Klik op Toevoegen. Kies een platform in het dialoogvenster Viewer-voorinstelling toevoegen, kies eCatalog Viewer en klik op 
**Toevoegen**.

   * **Een voorinstelling voor een eCatalog-viewer bewerken** Selecteer een voorinstelling voor een eCatalog-viewer en klik op Bewerken. Klikken 
**Opslaan als** nadat u de voorinstelling hebt gemaakt.

1. Voer in het scherm Viewer configureren een naam in voor uw voorinstelling voor de eCatalog-viewer.
1. Stel in het scherm Viewer configureren de gewenste opties in.

   Klik op het pictogram Info Tip naast de optie om de beschrijving van de optie weer te geven.

   In het voorvertoningsscherm wordt de viewer weergegeven terwijl u instellingen bijwerkt en wijzigt.

1. (Optioneel) In de instellingen van het deelvenster Info kan de optie Informatieserver de volgende speciale tokens bevatten, die door de viewer worden vervangen:

   | Token | Vervangen door | Notities |
   |--- |--- |--- |
   | `$1$` | rollover_key, waarde | De item-id van het `<area>` element van de kaart. |
   | `$2$` | frame | Het volgnummer van het momenteel weergegeven frame in de afbeeldingsset. |
   | `$3$` | imageroot | Het eerste padelement van het eerste item dat is opgegeven in de opdracht Afbeelding (doorgaans de afbeeldingencatalogus-id van het item in de catalogus die de afbeeldingsset opgeeft). |

1. (Optioneel) Typ in het vak Instellingen van deelvenster Info in het vak Reactiesjabloon de tekst die u wilt weergeven als bij Dynamic Media Classic een fout optreedt bij het ophalen van informatie voor een afbeeldingskaart. Als het systeem bijvoorbeeld een bedrijfsnaam en een eCatalog-naam ontvangt, maar geen rollover-id, wordt dit bericht voor de gebruiker weergegeven.

>[!NOTE]
>
>Als u dit antwoordsjabloon wilt gebruiken in plaats van de sjabloon die in de eCatalog zelf is gedefinieerd, voegt u &quot;fmt=1&quot; toe aan het einde van de URL van de Informatieserver. Bijvoorbeeld: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Klik op **Opslaan**.
1. Klik op Standaard als u wilt dat de door u gemaakte voorinstelling voor de eCatalog-viewer de voorinstelling is die wordt gebruikt om eCatalogs weer te geven op uw webpagina.

Als u een voorinstelling voor een eCatalog-viewer wilt verwijderen, selecteert u deze in het scherm Voorinstellingen viewer en klikt u op **Verwijderen**.

>[!MORELIKETHIS]
>
>* [Voorinstellingen viewer](application-setup.md#viewer_presets)

