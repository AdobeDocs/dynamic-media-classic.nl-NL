---
title: Adobe Analytics-rapporten configureren
seo-title: Adobe Analytics-rapporten configureren
description: 'null'
seo-description: Leer hoe u Adobe Analytics-rapporten configureert.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 0%

---


# Adobe Analytics-rapporten configureren{#configuring-adobe-analytics-reports}

Ga naar het scherm Adobe Analytics Configuration om Adobe Analytics te vertellen welke informatie u wilt opnemen in Adobe Analytics-rapporten. Nadat u rapporten vormt, maakt dit het schermlijsten, voor elke kijkergebeurtenis u informatie over, een overeenkomstige variabele van Adobe Analytics en een Dynamische Klassieke variabele van Media wilt. Deze variabelen van de kijker gebeurtenissen-Adobe Analytics veranderlijk-Dynamische Media Klassieke veranderlijke combinaties bepalen welke informatie wordt gemeld.

Naast het koppelen van viewergebeurtenissen aan variabelen, biedt het Adobe Analytics-configuratiescherm hulpprogramma&#39;s voor het activeren, bewerken en verwijderen van viewergebeurtenissen.

>[!NOTE]
>
>Wanneer u de instellingen voor Adobe Analytics-rapporten wijzigt in Adobe Analytics, moet u zich opnieuw aanmelden bij Adobe Analytics vanuit de Adobe Dynamic Media Classic, de Adobe Analytics-configuratie opnieuw opslaan en vervolgens opnieuw publiceren.

Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Zie [Configuratiegegevens](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)publiceren.

## Adobe Analytics-variabelen toewijzen aan Dynamic Media Classic-viewergebeurtenissen en -variabelen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Gebruik het Adobe Analytics-configuratiescherm om viewergebeurtenissen te koppelen aan Adobe Analytics-variabelen en Dynamic Media Classic-variabelen. Kies voor elke viewergebeurtenis één Adobe Analytics-variabele en één Dynamic Media Classic-variabele. Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)voor instructies over het openen van het configuratiescherm van Adobe Analytics.

**Adobe Analytics-variabelen toewijzen aan Dynamic Media Classic viewer-gebeurtenissen en -variabelen**

1. Nadat u zich bij Adobe Analytics van binnen Dynamische Media Klassiek en selecteert een rapportreeks, op de pagina van de Configuratie van Adobe Analytics, in de uiterst juiste kolom van de lijst, activeert een kijkergebeurtenis door te klikken **toelaten**.
1. Geef onder de kolom Variabelen de optie voor het variabele paar weer door op de pijlknop voor de gewenste Viewer-gebeurtenis te klikken.

   Zie [Viewer-gebeurtenissen](configuring-analytics-reports.md#viewer_events).

1. Voeg een dynamische Klassieke variabele van Media toe.

   Zie [Dynamic Media Classic-variabelen](configuring-analytics-reports.md#scene7_variables).

1. Voeg een Adobe Analytics-variabele toe.
1. (Optioneel) Als u nog een variabelepaar wilt toevoegen, klikt u op **Toevoegen**.
1. Klik op **Opslaan**.

   Nadat u op Opslaan hebt geklikt, worden de viewergebeurtenis, de Adobe Analytics-variabele en de variabele Dynamic Media Classic weergegeven in het scherm Adobe Analytics Configuration.

1. Klik in de rechterbenedenhoek op **Sluiten**.
1. Klik op **Publiceren** > **Publiceren** verzenden om een publicatiebericht voor afbeeldingen uit te voeren.

   Publiceren is nodig, zodat de informatie in de viewers beschikbaar is op Dynamic Media Classic-servers.

### Viewer-gebeurtenissen {#viewer-events}

Viewergebeurtenissen beschrijven acties die gebruikers uitvoeren met Dynamic Media Classic-viewers. Wanneer een gebruiker een bepaalde actie start, zoals klikken op een miniatuur of een video starten of stoppen, &quot;zendt de viewer&quot; een gebeurtenis naar de webpagina, samen met de gegevens die aan die gebeurtenis zijn gekoppeld.

In de volgende tabel worden de viewergebeurtenissen beschreven die u kunt toevoegen aan het Adobe Analytics-configuratiescherm.

| Viewer-gebeurtenis | Ondersteuning voor HTML5 Viewer Platform en viewers | Beschrijving |
|--- |--- |--- |
| LADEN | **X** (eCatalog, Flyout, SpinSet, Video, Zoomen) | Wanneer een gebruiker de viewer start. |
| PAGINA | **X** (eCatalog) | in eCatalogs, wanneer een gebruiker een pagina draait; in doelviewers, wanneer een gebruiker op een ander doel of een kleurstaal klikt. |
| SWAP | **X** (eCatalog, Flyout, SpinSet, Video, Zoomen) | Wanneer een gebruiker op een andere miniatuur klikt om een andere afbeelding weer te geven. |
| ITEM | **X** (eCatalog) | In viewers die afbeeldingen met hyperlinks ondersteunen waarin rollovers zijn gedefinieerd, beweegt de gebruiker de aanwijzer over een afbeelding met hyperlinks om de rollovertekst te lezen. |
| HREF | **X** (eCatalog) | Wanneer een gebruiker op een URL in een afbeelding met hyperlinks klikt in viewers die afbeeldingen met hyperlinks ondersteunen. |
| DOEL |  | Wanneer een gebruiker in doelviewers op een zoomdoel klikt om naar een gedeelte van een afbeelding te zoomen. |
| ZOEKEN |  | In eCatalogs, wanneer een gebruiker een woordonderzoek voert. |
| AFSPELEN | **X** (video) | Wanneer een gebruiker in videoviewers op Afspelen klikt om een video af te spelen.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De videokaart werkt met out-of-the-box Dynamic Media Classic HTML5 Video en MixedMedia-viewers. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten](enabling-analytics-video-reports.md)inschakelen. |
| PAUZEREN | **X** (video) | Wanneer een gebruiker in videoviewers op Pauzeren klikt om een video te pauzeren.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De videokaart werkt met out-of-the-box Dynamic Media Classic HTML5 Video en MixedMedia-viewers. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten](enabling-analytics-video-reports.md)inschakelen. |
| STOPPEN | **X** (video) | Wanneer een gebruiker in videoviewers op Stoppen klikt om het afspelen van een video te stoppen.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De videokaart werkt met out-of-the-box Dynamic Media Classic HTML5 Video en MixedMedia-viewers. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten](enabling-analytics-video-reports.md)inschakelen. |
| MILESTONE | **X** (video) | In videoviewers worden mijlpaalgebeurtenissen gegenereerd wanneer de gebruiker 0, 25, 50, 75 of 100 procent van de video afspeelt.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewergebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De videokaart werkt met out-of-the-box Dynamic Media Classic HTML5 Video en MixedMedia-viewers. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten](enabling-analytics-video-reports.md)inschakelen. |
| STAAL | X (Vliegen, Zoomen) | Deze viewergebeurtenis wordt toegewezen aan de PAGE-viewergebeurtenis in Dynamic Media Classic. |
| ZOOMEN | **X** (eCatalog, SpinSet, Zoom) | Niet bijgehouden door Adobe Analytics.<br> |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Niet bijgehouden door Adobe Analytics.<br> |
| SPIN | **X** (SpinSet) | Niet bijgehouden door Adobe Analytics.<br> |


### Dynamische variabelen van Media Classic {#scene-variables}

Kies voor elke viewergebeurtenis in het configuratiescherm van Adobe Analytics een Adobe Analytics-variabele en een *Dynamic Media Classic-variabele*. De dynamische Klassieke variabelen van Media vertegenwoordigen gegevens u voor een rapport kunt verkrijgen. De `searchTerm` variabele bevat bijvoorbeeld trefwoorden die worden gebruikt in zoekopdrachten in eCatalog.

In de volgende tabel worden de variabelen Dynamic Media Classic beschreven.

| Dynamic Media Classic-variabele | Beschrijving |
|--- |:--- |
| element | Dynamic Media Classic-element-id of videopadbestand. |
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

* **Activeren** Klik **[!UICONTROL Enable]** om een geselecteerde viewergebeurtenis te activeren of **[!UICONTROL Disable]** te deactiveren.

* **Bewerken** Selecteer een viewergebeurtenis en klik op de grijze knop **[!UICONTROL View/Edit]** Variabelen. Kies in de vervolgkeuzelijst Dynamische mediavariabele en Adobe Analytics-variabele een andere variabele in elke respectievelijke lijst. Zie Adobe Analytics-variabelen toewijzen aan Dynamic Media Classic-viewergebeurtenissen en -variabelen voor meer informatie.

* **Verwijderen** Selecteer een viewergebeurtenis en klik op de grijze knop **[!UICONTROL View/Edit]** Variabelen. Klik op **[!UICONTROL Delete]**.
