---
title: Een viewer instrumenteren met de Adobe Analytics Instrumentation Kit
description: Leer hoe u een viewer kunt instrumenteren met de Adobe Analytics Instrumentation Kit in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 458a80aad6e983dbccfe2108f0a389a4651f9f38
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Een viewer instrumenteren met de Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Met de Adobe Analytics Instrumentation Kit kunt u een HTML5-viewer integreren met Adobe Analytics.

Als u een van de vooraf gedefinieerde Adobe Dynamic Media Classic HTML5 Viewer-voorinstellingen gebruikt, bevatten deze al alle implementatiecode die nodig is om gegevens naar Adobe Analytics te verzenden. U hoeft geen verdere instrumentatie toe te voegen.

## Adobe Analytics-tracking instellen vanuit Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Voeg voor alle HTML5-viewers de volgende JavaScript toe aan de HTML-container, meestal in het element &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Waar `Adobe Dynamic Media Classic Company ID` is ingesteld op de naam van het Adobe Dynamic Media Classic-bedrijf. En `&preset` is optioneel. Als de naam van de bedrijfsvoorinstelling niet `companypreset` is, is deze niet optioneel. In dergelijke gevallen kan dit `companypreset-1, companypreset-2` zijn, enzovoort. Het hogere aantal is een nieuwere instantie van de voorinstelling. Om de correcte naam van de bedrijfvooraf ingestelde waarde te bepalen, selecteer **[!UICONTROL Copy URL]**, en bekijk dan de `preset=` parameter om de bedrijf vooraf ingestelde naam te vinden.

Als u doorgaat, voegt u nu een functie toe die de viewergebeurtenis naar de trackingcode van Adobe Analytics verzendt.

Voeg de functie `s7ComponentEvent()` toe aan de container HTML (of JSP, of ASPX of andere):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

De functienaam is hoofdlettergevoelig. De enige parameter die aan `s7componentEvent` wordt overgegaan die wordt vereist is laatste: `eventData`. Waar `s7track()` is gedefinieerd in s_code.jsp die hierboven is opgenomen. En `s7track` handelt alle tracking per gebeurtenis af. (U kunt gegevens die naar Adobe Analytics worden verzonden, verder aanpassen in dit gebied.)

## HREF- en ITEM-gebeurtenissen inschakelen {#enabling-href-and-item-events}

U kunt HREF-gebeurtenissen (rollover) en ITEM-gebeurtenissen (muisklikken/aanraken) inschakelen in de viewers via Afbeeldingskaart bewerken. Definieer de id&#39;s voor de HREF en het ITEM in de afbeelding met hyperlinks die aan de viewerinhoud zijn gekoppeld. Voeg een parameter `&rolloverKey=` toe aan de HREF-waarde in de Afbeeldingskaart.
