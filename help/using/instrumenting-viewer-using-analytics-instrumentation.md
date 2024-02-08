---
title: Een viewer instrumenteren met de Adobe Analytics Instrumentation Kit
description: Leer hoe u een viewer kunt instrumenteren met de Adobe Analytics Instrumentation Kit in Adobe Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: a9bd472705bce32f63a5710c3266e51256d17a00
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Een viewer instrumenteren met de Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Met de Adobe Analytics Instrumentation Kit kunt u een HTML5-viewer integreren met Adobe Analytics.

Als u een van de vooraf gedefinieerde Adobe Dynamic Media Classic HTML5-viewervoorinstellingen gebruikt, bevatten deze al de implementatiecode die nodig is om gegevens naar Adobe Analytics te verzenden. U hebt geen verdere instrumentatie meer nodig.

## Adobe Analytics-tracking instellen vanuit Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Voeg voor alle HTML5-viewers de volgende JavaScript-code toe aan de HTML-container, meestal in de map &lt;head> element:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Wanneer `Adobe Dynamic Media Classic Company ID` wordt ingesteld op de naam van het Adobe Dynamic Media Classic-bedrijf. en `&preset` is optioneel, tenzij de naam van de bedrijfsvoorinstelling niet `companypreset`. In dergelijke gevallen kan `companypreset-1, companypreset-2`, enzovoort. Het hogere aantal is een nieuwere instantie van de voorinstelling. Selecteer **[!UICONTROL Copy URL]** en bekijk vervolgens de `preset=`om de naam van de bedrijfsvoorinstelling te zoeken.

Als u doorgaat, voegt u nu een functie toe die de viewergebeurtenis naar de trackingcode van Adobe Analytics verzendt.

Voeg de `s7ComponentEvent()` functie aan container HTML (of JSP, of ASPX of andere):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

De functienaam is hoofdlettergevoelig. De enige parameter die wordt doorgegeven aan `s7componentEvent`dat is de laatste vereiste : `eventData`. Wanneer `s7track()` wordt gedefinieerd in s_code.jsp hierboven. en `s7track` behandelt al het volgen per elke gebeurtenis. (Als u de gegevens die naar Adobe Analytics worden verzonden verder wilt aanpassen, is dit gebied de plaats om ze te maken.)

## HREF- en ITEM-gebeurtenissen inschakelen {#enabling-href-and-item-events}

U kunt HREF-gebeurtenissen (rollover) en ITEM-gebeurtenissen (muisklikken/aanraken) inschakelen in de viewers via Afbeeldingskaart bewerken. Definieer de id&#39;s voor de HREF en het ITEM in de afbeelding met hyperlinks die aan de viewerinhoud zijn gekoppeld. Voeg een `&rolloverKey=` aan de waarde HREF binnen de Kaart van het Beeld.
