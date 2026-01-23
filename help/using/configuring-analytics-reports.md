---
title: Adobe Analytics-rapporten configureren
description: Leer hoe u Adobe Analytics-rapporten configureert in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 0%

---

# Adobe Analytics-rapporten configureren{#configuring-adobe-analytics-reports}

Ga naar het scherm Adobe Analytics Configuration om Adobe Analytics te vertellen welke informatie u wilt opnemen in Adobe Analytics-rapporten. Na uw configuratierapporten, maakt dit scherm een lijst, voor elke kijkergebeurtenis u informatie over, een overeenkomstige variabele van Adobe Analytics en een variabele van Adobe Dynamic Media Classic wilt. Deze variabele-variabele-Adobe Dynamic Media Classic van viewergebeurtenissen-Adobe Analytics bepalen welke informatie wordt gerapporteerd.

Naast het koppelen van viewergebeurtenissen aan variabelen, biedt het scherm Adobe Analytics Configuration hulpprogramma&#39;s voor het activeren, bewerken en verwijderen van viewergebeurtenissen.

>[!NOTE]
>
>Wanneer u de Adobe Analytics-rapportinstellingen in Adobe Analytics wijzigt, moet u zich vanuit Adobe Dynamic Media Classic opnieuw aanmelden bij Adobe Analytics, de Adobe Analytics-configuratie-instellingen opnieuw opslaan en vervolgens opnieuw publiceren.

Zie [&#x200B; Logon aan Adobe Analytics &#x200B;](log-analytics.md#log_in_to_adobe_analytics).

Zie [&#x200B; publiceren configuratieinformatie &#x200B;](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Adobe Analytics-variabelen toewijzen aan Adobe Dynamic Media Classic-viewergebeurtenissen en -variabelen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Gebruik het Adobe Analytics-configuratiescherm om viewergebeurtenissen te koppelen aan Adobe Analytics-variabelen en Adobe Dynamic Media Classic-variabelen. Kies voor elke viewergebeurtenis één Adobe Analytics-variabele en één Adobe Dynamic Media Classic-variabele. Voor instructies over het openen van het scherm van de Configuratie van Adobe Analytics, zie [&#x200B; Aanmelding aan Adobe Analytics &#x200B;](log-analytics.md#log_in_to_adobe_analytics).

**om de variabelen van Adobe Analytics aan de kijkersgebeurtenissen en variabelen van Adobe Dynamic Media Classic toe te wijzen:**

1. Nadat u zich vanuit Dynamic Media Classic hebt aangemeld bij Adobe Analytics en een rapportsuite hebt geselecteerd, activeert u in de rechtertabelkolom op de pagina Adobe Analytics Configuration een viewergebeurtenis door **[!UICONTROL Enable]** te selecteren.
1. Geef onder de kolom Variabelen de optie voor het variabele paar weer door de pijlknop voor de gewenste viewergebeurtenis te selecteren.

   Zie [&#x200B; gebeurtenissen van de Kijker &#x200B;](configuring-analytics-reports.md#viewer_events).

1. Voeg een Adobe Dynamic Media Classic-variabele toe.

   Zie [&#x200B; variabelen van Adobe Dynamic Media Classic &#x200B;](configuring-analytics-reports.md#scene7_variables).

1. Voeg een Adobe Analytics-variabele toe.
1. (Optioneel) Als u nog een variabelepaar wilt toevoegen, selecteert u **[!UICONTROL Add]** .
1. Selecteer **[!UICONTROL Save]** .

   Nadat u **[!UICONTROL Save]** hebt geselecteerd, worden de viewergebeurtenis, de Adobe Analytics-variabele en de Adobe Dynamic Media Classic-variabele weergegeven in het scherm Adobe Analytics Configuration.

1. Selecteer **[!UICONTROL Close]** in de rechterbenedenhoek.
1. Ga naar **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** om een publicatiebericht voor de afbeeldingsserver uit te voeren.

   Publiceren is nodig, zodat de informatie in de viewers beschikbaar is op Adobe Dynamic Media Classic-servers.

### Viewer-gebeurtenissen {#viewer-events}

Viewergebeurtenissen beschrijven acties die gebruikers met Dynamic Media Classic-viewers uitvoeren. Wanneer een gebruiker een actie, zoals het selecteren van een duimnagel of het beginnen of het tegenhouden van een video in werking stelt, &quot;uitzendt de kijker&quot;een gebeurtenis aan de Web-pagina. Gegevens die aan die gebeurtenis zijn gekoppeld, worden ook geduwd.

In de volgende tabel worden de viewergebeurtenissen beschreven die u kunt toevoegen aan het Adobe Analytics-configuratiescherm.

| Viewer-gebeurtenis | HTML5 Viewer Platform-ondersteuning en -viewers | Beschrijving |
| --- | --- | --- |
| LADEN | **X** (eCatalog, Flyout, SpinSet, Video, Gezoem) | Wanneer een gebruiker een viewer start |
| PAGINA | **X** (eCatalog) | In eCatalogs, wanneer een gebruiker een pagina draait; in gerichte gezoemkijkers, wanneer een gebruiker een verschillend doel of een kleurenmonster selecteert. |
| WISSELEN | **X** (eCatalog, Flyout, SpinSet, Video, Gezoem) | Wanneer een gebruiker een andere miniatuur selecteert om een andere afbeelding weer te geven. |
| ITEM | **X** (eCatalog) | In viewers die afbeeldingen met hyperlinks ondersteunen waarin rollovers zijn gedefinieerd, beweegt de gebruiker de aanwijzer over een afbeelding met hyperlinks om de rollovertekst te lezen. |
| HREF | **X** (eCatalog) | Wanneer een gebruiker een URL selecteert in een Afbeeldingskaart in viewers die afbeeldingen met hyperlinks ondersteunen. |
| DOEL | | Wanneer een gebruiker in beoogde zoomviewers een zoomdoel selecteert om naar een gedeelte van een afbeelding te zoomen. |
| ZOEKEN | | In eCatalogs, wanneer een gebruiker een woordonderzoek voert. |
| AFSPELEN | **X** (Video) | Wanneer een gebruiker in videoviewers Afspelen selecteert om een video af te spelen.<br><br>**Nota:** als u op hartslag-gebaseerde video die van Adobe Analytics gebruikt, te hoeven u om het even welke variabelen aan deze kijkersgebeurtenis in kaart te brengen wanneer u Adobe Analytics in Adobe Dynamic Media Classic vormt. De functie Videohartslag werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [&#x200B; Adobe Analytics VideoRapporten &#x200B;](enabling-analytics-video-reports.md) toelaten. |
| PAUZE | **X** (Video) | Wanneer een gebruiker in Video-viewers **[!UICONTROL Pause]** selecteert om een video te bevriezen.<br><br>**Nota:** als u op hartslag-gebaseerde video die van Adobe Analytics gebruikt, te hoeven u om het even welke variabelen aan deze kijkersgebeurtenis in kaart te brengen wanneer u Adobe Analytics in Adobe Dynamic Media Classic vormt. De functie Videohartslag werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [&#x200B; Adobe Analytics VideoRapporten &#x200B;](enabling-analytics-video-reports.md) toelaten. |
| STOPPEN | **X** (Video) | Wanneer een gebruiker in videoviewers **[!UICONTROL Stop]** selecteert om te stoppen met het afspelen van een video.<br><br>**Nota:** als u op hartslag-gebaseerde video die van Adobe Analytics gebruikt, te hoeven u om het even welke variabelen aan deze kijkersgebeurtenis in kaart te brengen wanneer u Adobe Analytics in Adobe Dynamic Media Classic vormt. De functie Videohartslag werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [&#x200B; Adobe Analytics VideoRapporten &#x200B;](enabling-analytics-video-reports.md) toelaten. |
| MILESTONE | **X** (Video) | In videoviewers worden mijlpaalgebeurtenissen gegenereerd wanneer de gebruiker 0, 25, 50, 75 of 100 procent van de video afspeelt.<br><br>**Nota:** als u op hartslag-gebaseerde video die van Adobe Analytics gebruikt, te hoeven u om het even welke variabelen aan deze kijkersgebeurtenis in kaart te brengen wanneer u Adobe Analytics in Adobe Dynamic Media Classic vormt. De functie Videohartslag werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [&#x200B; Adobe Analytics VideoRapporten &#x200B;](enabling-analytics-video-reports.md) toelaten. |
| STAAL | **X** (Vliegen, Gezoem) | Deze viewergebeurtenis wordt toegewezen aan de PAGE-viewergebeurtenis in Adobe Dynamic Media Classic. |
| ZOOMEN | **X** (eCatalog, SpinSet, Gezoem) | Niet bijgehouden door Adobe Analytics. |
| PAN | **X** (eCatalog, SpinSet, Gezoem) | Niet bijgehouden door Adobe Analytics. |
| SPIN | **X** (SpinSet) | Niet bijgehouden door Adobe Analytics. |

### Adobe Dynamic Media Classic-variabelen {#scene-variables}

Voor elke viewergebeurtenis op het scherm van de Configuratie van Adobe Analytics, kies een variabele van Adobe Analytics en een *variabele van Adobe Dynamic Media Classic*. Adobe Dynamic Media Classic-variabelen vertegenwoordigen gegevens die u voor een rapport kunt verkrijgen. De variabele `searchTerm` bevat bijvoorbeeld trefwoorden die worden gebruikt in zoekopdrachten in eCatalog.

In de volgende tabel worden Adobe Dynamic Media Classic-variabelen beschreven:

| Adobe Dynamic Media Classic-variabele | Beschrijving |
| --- | --- |
| element | Adobe Dynamic Media Classic-element-id of videopadbestand. |
| viewerId | Een willekeurig getal dat aan elk ander viewertype wordt toegewezen. |
| pageLabel | In eCatalogs, de pagina die een kijker toont. |
| label | De labelwaarde (een tekenreeks). |
| frame | De pagina of pagina waarnaar wordt verwezen in een Afbeeldingsset. |
| rollover_keyRaw | De gehele HREF-waarde, niet alleen een verwerkt deel ervan. |
| rollover_keyProc | De id van een item waarnaar wordt verwezen in een afbeelding met hyperlinks (geldig voor href- en itemgebeurtenissen). |
| searchTerm | Een term die wordt gebruikt in het zoeken naar eCatalog. |
| timeStamp | Afspelen, Stoppen en Pauzeren gekozen in videoviewers. |
| vordering | Het percentage van een gebeurtenis milestone dat is voltooid. |
| targetId | De id-waarde (een getal). |

## Viewer-gebeurtenissen activeren, bewerken en verwijderen {#activating-editing-and-deleting-viewer-events}

In het configuratiescherm van Adobe Analytics kunt u viewergebeurtenissen activeren, bewerken en verwijderen:

* **activeer**: Selecteer **[!UICONTROL Enable]** om te activeren of **[!UICONTROL Disable]** om een geselecteerde viewergebeurtenis te deactiveren.

* **geeft** uit: Selecteer een kijkergebeurtenis en selecteer de **[!UICONTROL View/Edit]** grijze knoop van Variabelen. Kies in de vervolgkeuzelijsten met de variabelen Adobe Dynamic Media Classic en Adobe Analytics een andere variabele uit elke respectievelijke lijst. Voor meer informatie, zie [&#x200B; Toewijzend de variabelen van Adobe Analytics aan de kijkersgebeurtenissen en variabelen van Adobe Dynamic Media Classic &#x200B;](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Schrapping**: Selecteer een kijkergebeurtenis, en selecteer de **[!UICONTROL View/Edit]** grijze knoop van Variabelen. Selecteer **[!UICONTROL Delete]** .
