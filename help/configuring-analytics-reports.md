---
title: Adobe Analytics-rapporten configureren
description: Leer hoe u Adobe Analytics-rapporten configureert.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,beheerder,Business Practice
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---


# Adobe Analytics-rapporten configureren{#configuring-adobe-analytics-reports}

Ga naar het scherm Adobe Analytics Configuration om Adobe Analytics te vertellen welke informatie u wilt opnemen in Adobe Analytics-rapporten. Nadat u rapporten vormt, maakt dit het schermlijsten, voor elke kijkergebeurtenis u informatie over, een overeenkomstige variabele van Adobe Analytics en de Klassieke variabele van Dynamic Media wilt. Deze combinaties van viewergebeurtenissen, Adobe Analytics variable-Dynamic Media Classic, bepalen welke informatie wordt gerapporteerd.

Naast het koppelen van viewergebeurtenissen aan variabelen, biedt het Adobe Analytics-configuratiescherm hulpprogramma&#39;s voor het activeren, bewerken en verwijderen van viewergebeurtenissen.

>[!NOTE]
>
>Wanneer u de instellingen voor Adobe Analytics-rapporten wijzigt in Adobe Analytics, moet u zich opnieuw aanmelden bij Adobe Analytics vanuit Adobe Dynamic Media Classic, de Adobe Analytics-configuratie opnieuw opslaan en vervolgens opnieuw publiceren.

Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Zie [Configuratiegegevens publiceren](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Adobe Analytics-variabelen toewijzen aan Dynamic Media Classic viewer-gebeurtenissen en -variabelen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Gebruik het Adobe Analytics-configuratiescherm om viewergebeurtenissen te koppelen aan Adobe Analytics-variabelen en Dynamic Media Classic-variabelen. Kies voor elke viewergebeurtenis één Adobe Analytics-variabele en één Classic-variabele van Dynamic Media. Zie [Aanmelden bij Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics) voor instructies over het openen van het scherm Adobe Analytics Configuration.

**Adobe Analytics-variabelen toewijzen aan Dynamic Media Classic viewer-gebeurtenissen en -variabelen**

1. Nadat u zich bij Adobe Analytics van binnen Classic Dynamic Media hebt aangemeld en een rapportreeks selecteert, op de pagina van de Configuratie van Adobe Analytics, in de uiterst juiste kolom van de tabel, activeert u een viewergebeurtenis door op **Inschakelen** te klikken.
1. Geef onder de kolom Variabelen de optie voor het variabele paar weer door op de pijlknop voor de gewenste Viewer-gebeurtenis te klikken.

   Zie [Viewergebeurtenissen](configuring-analytics-reports.md#viewer_events).

1. Voeg een klassieke Dynamic Media-variabele toe.

   Zie [Klassieke variabelen van Dynamic Media](configuring-analytics-reports.md#scene7_variables).

1. Voeg een Adobe Analytics-variabele toe.
1. (Optioneel) Als u een ander variabelepaar wilt toevoegen, klikt u op **Toevoegen**.
1. Klik **Opslaan**.

   Nadat u op Opslaan hebt geklikt, worden de viewergebeurtenis, de Adobe Analytics-variabele en de bijbehorende Klassieke Dynamic Media-variabele weergegeven in het scherm Adobe Analytics Configuration.

1. Klik in de rechterbenedenhoek op **Close**.
1. Klik **Publiceren** > **Publiceren verzenden** om een publicatiebericht voor een afbeelding uit te voeren.

   Publiceren is nodig, zodat de informatie in de viewers beschikbaar is op de Classic-servers van Dynamic Media.

### Viewergebeurtenissen {#viewer-events}

Viewergebeurtenissen beschrijven acties die gebruikers uitvoeren met Dynamic Media Classic-viewers. Wanneer een gebruiker een bepaalde actie start, zoals klikken op een miniatuur of een video starten of stoppen, &quot;zendt de viewer&quot; een gebeurtenis naar de webpagina, samen met de gegevens die aan die gebeurtenis zijn gekoppeld.

In de volgende tabel worden de viewergebeurtenissen beschreven die u kunt toevoegen aan het Adobe Analytics-configuratiescherm.

| Viewer-gebeurtenis | Ondersteuning voor HTML5 Viewer Platform en viewers | Beschrijving |
|--- |--- |--- |
| LADEN | **X** (eCatalog, Flyout, SpinSet, Video, Zoomen) | Wanneer een gebruiker de viewer start. |
| PAGINA | **X**   (eCatalog) | in eCatalogs, wanneer een gebruiker een pagina draait; in doelviewers, wanneer een gebruiker op een ander doel of een kleurstaal klikt. |
| SWAP | **X**  (eCatalog, Flyout, SpinSet, Video, Zoomen) | Wanneer een gebruiker op een andere miniatuur klikt om een andere afbeelding weer te geven. |
| ITEM | **X**   (eCatalog) | In viewers die afbeeldingen met hyperlinks ondersteunen waarin rollovers zijn gedefinieerd, beweegt de gebruiker de aanwijzer over een afbeelding met hyperlinks om de rollovertekst te lezen. |
| HREF | **X**   (eCatalog) | Wanneer een gebruiker op een URL in een afbeelding met hyperlinks klikt in viewers die afbeeldingen met hyperlinks ondersteunen. |
| DOEL |  | Wanneer een gebruiker in doelviewers op een zoomdoel klikt om naar een gedeelte van een afbeelding te zoomen. |
| ZOEKEN |  | In eCatalogs, wanneer een gebruiker een woordonderzoek voert. |
| AFSPELEN | **X**   (video) | Wanneer een gebruiker in videoviewers op Afspelen klikt om een video af te spelen.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewer-gebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De functie Videohartslag werkt met Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| PAUZEREN | **X**  (video) | Wanneer een gebruiker in videoviewers op Pauzeren klikt om een video te pauzeren.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewer-gebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De functie Videohartslag werkt met Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| STOPPEN | **X**  (video) | Wanneer een gebruiker in videoviewers op Stoppen klikt om het afspelen van een video te stoppen.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewer-gebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De functie Videohartslag werkt met Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| MILESTONE | **X**   (video) | In videoviewers worden mijlpaalgebeurtenissen gegenereerd wanneer de gebruiker 0, 25, 50, 75 of 100 procent van de video afspeelt.<br><br>**Opmerking:** Als u op Adobe Analytics gebaseerde videoverslagen gebruikt, hoeft u geen variabelen aan deze viewer-gebeurtenis toe te wijzen wanneer u Adobe Analytics configureert in Dynamic Media Classic. De functie Videohartslag werkt met Dynamic Media Classic HTML5 Video- en MixedMedia-viewers die niet in de verpakking staan. De videospeler genereert trackinggegevens voor weergave in Adobe Analytics Video Reports. Zie [Adobe Analytics-videorapporten inschakelen](enabling-analytics-video-reports.md). |
| STAAL | X (Vliegen, Zoomen) | Deze viewergebeurtenis wordt toegewezen aan de PAGE-viewergebeurtenis in Dynamic Media Classic. |
| ZOOMEN | **X**  (eCatalog, SpinSet, Zoom) | Niet bijgehouden door Adobe Analytics.<br> |
| PAN | **X**  (eCatalog, SpinSet, Zoom) | Niet bijgehouden door Adobe Analytics.<br> |
| SPIN | **X**  (SpinSet) | Niet bijgehouden door Adobe Analytics.<br> |


### Dynamic Media Klassieke variabelen {#scene-variables}

Voor elke viewergebeurtenis op het scherm van de Configuratie van Adobe Analytics, kies een variabele van Adobe Analytics en een *Klassieke variabele van Dynamic Media*. Klassieke Dynamic Media-variabelen vertegenwoordigen gegevens die u voor een rapport kunt verkrijgen. De variabele `searchTerm` bevat bijvoorbeeld trefwoorden die worden gebruikt in zoekopdrachten in eCatalog.

In de volgende tabel worden de klassieke Dynamic Media-variabelen beschreven.

| Dynamic Media Classic-variabele | Beschrijving |
|--- |:--- |
| element | Dynamic Media Klassieke element-id of videopadbestand. |
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

## Viewergebeurtenissen {#activating-editing-and-deleting-viewer-events} activeren, bewerken en verwijderen

In het configuratiescherm van Adobe Analytics kunt u viewergebeurtenissen activeren, bewerken en verwijderen:

* **Klik**
activeren  **[!UICONTROL Enable]** om een geselecteerde viewergebeurtenis te activeren of  **[!UICONTROL Disable]** te deactiveren.

* ****
BewerkenSelecteer een viewergebeurtenis en klik op de knop  **[!UICONTROL View/Edit]** Variabelen grijs. Kies in de vervolgkeuzelijst Klassieke variabele Dynamic Media en Adobe Analytics-variabele een andere variabele uit elke respectievelijke lijst. Zie Adobe Analytics-variabelen toewijzen aan Klassieke Dynamic Media-viewergebeurtenissen en -variabelen voor meer informatie.

* ****
VerwijderenSelecteer een viewergebeurtenis en klik op de grijze knop  **[!UICONTROL View/Edit]** Variabelen. Klik op **[!UICONTROL Delete]**.
