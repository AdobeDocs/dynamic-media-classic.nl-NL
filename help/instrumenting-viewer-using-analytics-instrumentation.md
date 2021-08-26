---
title: Een viewer instrumenteren met de Adobe Analytics Instrumentation Kit
description: Leer hoe u een viewer kunt instrumenteren met de Adobe Analytics Instrumentation Kit in Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: bb387446f294cf1e90d26ae1df4422879ad29db7
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Een viewer instrumenteren met de Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Met de Adobe Analytics Instrumentation Kit kunt u een HTML5-viewer integreren met Adobe Analytics.

Als u een van de vooraf gedefinieerde Dynamic Media Classic HTML5-viewervoorinstellingen gebruikt, bevatten deze al alle implementatiecode die nodig is om gegevens naar Adobe Analytics te verzenden. u hebt geen verdere instrumentatie nodig.

## Adobe Analytics-tracking instellen vanuit Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Voeg voor alle HTML5-viewers de volgende JavaScript-code toe aan de HTML-container, meestal in het element &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Waar `Dynamic Media Classic Company ID` wordt geplaatst aan de Klassieke bedrijfsnaam van Dynamic Media. En `&preset` is optioneel tenzij de naam van de bedrijfsvoorinstelling niet `companypreset` is. In dergelijke gevallen kan het `companypreset-1, companypreset-2` zijn, enzovoort. Het hogere aantal is een nieuwere instantie van de voorinstelling. Als u de juiste naam van de bedrijfsvoorinstelling wilt bepalen, selecteert u **[!UICONTROL Copy URL]** en zoekt u vervolgens de `preset=`parameter om de naam van de bedrijfsvoorinstelling te zoeken.

Als u doorgaat, voegt u nu een functie toe die de viewergebeurtenis naar de trackingcode van Adobe Analytics verzendt.

Voeg de functie `s7ComponentEvent()` aan de container HTML (of JSP, of ASPX of andere) toe:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

De functienaam is hoofdlettergevoelig. De enige parameter die wordt doorgegeven aan `s7componentEvent`dat is vereist, is de laatste parameter: `eventData`. Waar `s7track()` in s_code.jsp hierboven wordt bepaald. En `s7track` behandelt al het volgen per elke gebeurtenis. (Als u de gegevens die naar Adobe Analytics worden verzonden verder wilt aanpassen, is dit gebied de plaats om ze te maken.)

## HREF- en ITEM-gebeurtenissen inschakelen {#enabling-href-and-item-events}

U kunt HREF-gebeurtenissen (rollover) en ITEM-gebeurtenissen (muisklikken/aanraken) inschakelen in de viewers via Afbeeldingskaart bewerken. Definieer de id&#39;s voor de HREF en het ITEM in de afbeelding met hyperlinks die aan de viewerinhoud zijn gekoppeld. Voeg een `&rolloverKey=` parameter aan de waarde HREF binnen de Kaart van het Beeld toe.
