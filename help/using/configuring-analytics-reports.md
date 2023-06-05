---
title: Adobe Analytics-rapporten configureren
description: Leer hoe u Adobe Analytics-rapporten configureert in Adobe Dynamic Media Classic.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1214'
ht-degree: 0%

---

# Adobe Analytics-rapporten configureren{#configuring-adobe-analytics-reports}

Ga naar het scherm Adobe Analytics Configuration om Adobe Analytics te vertellen welke informatie u wilt opnemen in Adobe Analytics-rapporten. Nadat u rapporten hebt geconfigureerd, wordt in dit scherm voor elke viewergebeurtenis waarover u informatie wilt, een corresponderende Adobe Analytics-variabele en een Adobe Dynamic Media Classic-variabele weergegeven. Deze variabele-variabele-Adobe Dynamic Media Classic van viewergebeurtenissen-Adobe Analytics bepalen welke informatie wordt gerapporteerd.

Naast het koppelen van viewergebeurtenissen aan variabelen, biedt het scherm Adobe Analytics Configuration hulpprogramma&#39;s voor het activeren, bewerken en verwijderen van viewergebeurtenissen.

>[!NOTE]
>
>Wanneer u de instellingen voor Adobe Analytics-rapporten wijzigt in Adobe Analytics, moet u zich vanuit Adobe Dynamic Media Classic opnieuw aanmelden bij Adobe Analytics, de Adobe Analytics-configuratie-instellingen opnieuw opslaan en vervolgens opnieuw publiceren.

Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Zie [Configuratiegegevens publiceren](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Adobe Analytics-variabelen toewijzen aan Adobe Dynamic Media Classic-viewergebeurtenissen en -variabelen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Gebruik het Adobe Analytics-configuratiescherm om viewergebeurtenissen te koppelen aan Adobe Analytics-variabelen en Adobe Dynamic Media Classic-variabelen. Kies voor elke viewergebeurtenis één Adobe Analytics-variabele en één Adobe Dynamic Media Classic-variabele. Ga voor instructies over het openen van het Adobe Analytics-configuratiescherm naar [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Adobe Analytics-variabelen toewijzen aan Adobe Dynamic Media Classic-viewergebeurtenissen en -variabelen:**

1. Nadat u zich bij Adobe Analytics van binnen Adobe Dynamic Media Classic hebt aangemeld en een rapportreeks, op de pagina van de Configuratie van Adobe Analytics, in de juiste lijstkolom selecteert, activeer een kijkersgebeurtenis door te selecteren **[!UICONTROL Enable]**.
1. Geef onder de kolom Variabelen de optie voor het variabele paar weer door de pijlknop voor de gewenste Viewer-gebeurtenis te selecteren.

   Zie [Viewer-gebeurtenissen](configuring-analytics-reports.md#viewer_events).

1. Voeg een Adobe Dynamic Media Classic-variabele toe.

   Zie [Adobe Dynamic Media Classic-variabelen](configuring-analytics-reports.md#scene7_variables).

1. Voeg een Adobe Analytics-variabele toe.
1. (Optioneel) Selecteer **[!UICONTROL Add]**.
1. Selecteren **[!UICONTROL Save]**.

   Nadat u **[!UICONTROL Save]** De viewergebeurtenis, de Adobe Analytics-variabele en de Adobe Dynamic Media Classic-variabele worden weergegeven in het scherm Adobe Analytics Configuration.

1. Selecteer in de rechterbenedenhoek de optie **[!UICONTROL Close]**.
1. Ga naar **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** om een publicatiebericht met de afbeeldingsserver uit te voeren.

   Publiceren is nodig, zodat de informatie in de viewers beschikbaar is op Adobe Dynamic Media Classic-servers.

### Viewer-gebeurtenissen {#viewer-events}

Viewergebeurtenissen beschrijven acties die gebruikers met Adobe Dynamic Media Classic-viewers uitvoeren. Wanneer een gebruiker een bepaalde actie start, zoals het selecteren van een miniatuur of het starten of stoppen van een video, &quot;zendt de viewer&quot; een gebeurtenis naar de webpagina, samen met de gegevens die aan die gebeurtenis zijn gekoppeld.

In de volgende tabel worden de viewergebeurtenissen beschreven die u kunt toevoegen aan het Adobe Analytics-configuratiescherm.

| Viewer-gebeurtenis | Ondersteuning voor HTML5 Viewer-Platforms en viewers | Beschrijving |
| --- | --- | --- |
| LADEN | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | Wanneer een gebruiker een viewer start |
| PAGINA | **X**  (eCatalog) | in eCatalogs, wanneer een gebruiker een pagina draait; in beoogde zoomviewers, wanneer een gebruiker een ander doel of een kleurstaal selecteert. |
| SWAP | **X**  (eCatalog, Flyout, SpinSet, Video, Zoom) | Wanneer een gebruiker een andere miniatuur selecteert om een andere afbeelding weer te geven. |
| ITEM | **X**  (eCatalog) | In viewers die afbeeldingen met hyperlinks ondersteunen waarin rollovers zijn gedefinieerd, beweegt de gebruiker de aanwijzer over een afbeelding met hyperlinks om de rollovertekst te lezen. |
| HREF | **X**  (eCatalog) | Wanneer een gebruiker een URL selecteert in een Afbeeldingskaart in viewers die afbeeldingen met hyperlinks ondersteunen. |
| DOEL |  | Wanneer een gebruiker in beoogde zoomviewers een zoomdoel selecteert om naar een gedeelte van een afbeelding te zoomen. |
| ZOEKEN |  | In eCatalogs, wanneer een gebruiker een woordonderzoek voert. |
| AFSPELEN | **X**  (Video) | Wanneer een gebruiker in videoviewers Afspelen selecteert om een video af te spelen.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics in Adobe Dynamic Media Classic configureert. De videorecart werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers buiten de box. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| PAUZEREN | **X** (Video) | Wanneer een gebruiker in videoviewers **[!UICONTROL Pause]** om een video te bevriezen.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics in Adobe Dynamic Media Classic configureert. De videorecart werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers buiten de box. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| STOPPEN | **X** (Video) | Wanneer een gebruiker in videoviewers **[!UICONTROL Stop]** om het afspelen van een video te stoppen.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics in Adobe Dynamic Media Classic configureert. De videorecart werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers buiten de box. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Video) | In videoviewers worden mijlpaalgebeurtenissen gegenereerd wanneer de gebruiker 0, 25, 50, 75 of 100 procent van de video afspeelt.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics in Adobe Dynamic Media Classic configureert. De videorecart werkt met Adobe Dynamic Media Classic HTML5 Video- en MixedMedia-viewers buiten de box. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| STAAL | **X** (Flyout, Zoom) | Deze viewergebeurtenis wordt toegewezen aan de PAGE-viewergebeurtenis in Adobe Dynamic Media Classic. |
| ZOOMEN | **X** (eCatalog, SpinSet, Zoom) | Niet bijgehouden door Adobe Analytics. |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Niet bijgehouden door Adobe Analytics. |
| SPIN | **X** (SpinSet) | Niet bijgehouden door Adobe Analytics. |

### Adobe Dynamic Media Classic-variabelen {#scene-variables}

Kies voor elke viewergebeurtenis in het configuratiescherm van Adobe Analytics een Adobe Analytics-variabele en een *Adobe Dynamic Media Classic-variabele*. Adobe Dynamic Media Classic-variabelen vertegenwoordigen gegevens die u voor een rapport kunt verkrijgen. De `searchTerm` De variabele maakt een lijst van sleutelwoorden die in eCatalog onderzoeken worden gebruikt.

In de volgende tabel worden Adobe Dynamic Media Classic-variabelen beschreven:

| Adobe Dynamic Media Classic-variabele | Beschrijving |
| --- | --- |
| element | Adobe Dynamic Media Classic-element-id of videopadbestand. |
| viewerId | Een willekeurig getal dat aan elk ander viewertype wordt toegewezen. |
| pageLabel | In eCatalogs, de pagina die een kijker toont. |
| label | De labelwaarde (een tekenreeks). |
| frame | De pagina of paginaverwijzing in een Afbeeldingsreeks. |
| rollover_keyRaw | De gehele HREF-waarde, niet alleen een verwerkt deel ervan. |
| rollover_keyProc | De id van een item waarnaar wordt verwezen in een afbeelding met hyperlinks (geldig voor href- en itemgebeurtenissen). |
| searchTerm | Een term die wordt gebruikt in het zoeken naar eCatalog. |
| timeStamp | Afspelen, Stoppen en Pauzeren gekozen in videoviewers. |
| vordering | Het percentage van een gebeurtenis milestone dat is voltooid. |
| targetId | De id-waarde (een getal). |

## Viewer-gebeurtenissen activeren, bewerken en verwijderen {#activating-editing-and-deleting-viewer-events}

In het configuratiescherm van Adobe Analytics kunt u viewergebeurtenissen activeren, bewerken en verwijderen:

* **Activeren** - Selecteer **[!UICONTROL Enable]** om te activeren of **[!UICONTROL Disable]** om een geselecteerde viewergebeurtenis te deactiveren.

* **Bewerken** - Selecteer een viewergebeurtenis en selecteer **[!UICONTROL View/Edit]** De grijze knop Variabelen. Kies in de vervolgkeuzelijst Adobe Dynamic Media Classic-variabele en Adobe Analytics-variabele een andere variabele in elke respectievelijke lijst. Zie voor meer informatie [Adobe Analytics-variabelen toewijzen aan Adobe Dynamic Media Classic-viewergebeurtenissen en -variabelen](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Verwijderen** - Selecteer een viewergebeurtenis en selecteer **[!UICONTROL View/Edit]** De grijze knop Variabelen. Selecteren **[!UICONTROL Delete]**.
