---
title: Een sjabloon maken
description: Leer hoe u een sjabloon maakt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '3261'
ht-degree: 0%

---

# Een sjabloon maken

Ga naar **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Selecteer Designer of Developer. Op deze pagina kunt u afbeeldings- en tekstlagen toevoegen. U kunt lagen ook opnieuw ordenen, de grootte en positie van lagen wijzigen en schaduw- en gloedeffecten toepassen op afbeeldingen en tekst.

Zie ook [Grondbeginselen van sjablonen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) trainingsvideo.

>[!NOTE]
>
>Als u een sjabloon bewerkt die in een eerdere versie van Adobe Dynamic Media Classic is gemaakt, wordt u gevraagd of u de sjabloon wilt opslaan. Wilt u een canvaslaag toevoegen? Selecteren **[!UICONTROL No]** om te voorkomen dat u een basislaag toevoegt. Als u per ongeluk **[!UICONTROL Yes]**, de `&allowCanvasPrompt` en `&layer=0` modifiers in URL en druk **[!UICONTROL Enter]** of **[!UICONTROL Return]**.

## De eerste sjabloon maken {#creating-the-initial-template}

Wanneer u een sjabloonset maakt, kunt u **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| **[!UICONTROL Publish after a save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

U kunt een sjabloon maken op basis van een bestaande sjabloon. Open de sjabloon en selecteer **[!UICONTROL Save As]** en voert u een nieuwe naam in het dialoogvenster Opslaan als in.

**De eerste sjabloon maken:**

1. Gebruik een van de volgende methoden om uw oorspronkelijke sjabloon te maken:

   * **Selecteer eerst de PSD of afbeeldingen**: Selecteer in het deelvenster Bladeren het PSD-bestand of de afbeeldingen die u voor de sjabloon wilt gebruiken, ga naar **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**.

   * **Beginnen vanaf het scherm Sjabloon**: Ga naar **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Selecteer Designer of Developer.

1. Voer in het dialoogvenster Canvasgrootte invoeren de afmetingen voor breedte en hoogte van de sjabloon in.
1. Selecteer een map in de elementenbibliotheek en sleep het gewenste PSD-bestand of de gewenste afbeeldingen voor de sjabloon naar het scherm Sjabloon.
1. Wanneer u klaar bent, gaat u naar de rechterbenedenhoek van de pagina en zorgt u ervoor dat **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**.
1. Selecteer een map waarin u de sjabloon wilt opslaan, voer een naam voor de sjabloon in en selecteer **[!UICONTROL Submit]**.

   Adobe Dynamic Media Classic verkleint afbeeldingen indien nodig om deze op het canvas te passen, het gebied op het scherm Sjabloon waarin u de sjabloon kunt definiëren.

## Een sjabloonset bewerken {#editing-a-template-set}

Of u een gepubliceerde set of een niet-gepubliceerde sjabloonset bewerkt, **[!UICONTROL Publish after a save]** Deze optie is op de volgende manieren van invloed op de set en de set leden:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after a save]** optie geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
| --- | --- | --- | --- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een sjabloonset bewerken:**

1. Blader in de rasterweergave naar een Sjabloonset en selecteer vervolgens onder de afbeelding de optie **[!UICONTROL Edit]**.
1. Wijzig de sjabloon naar wens.
1. Wanneer u klaar bent met bewerken, gaat u naar de rechterbenedenhoek van de pagina en zorgt u ervoor dat **[!UICONTROL Publish after a save]** is geselecteerd (standaard).
1. Selecteren **[!UICONTROL Save]**, selecteert u een opslagmap, voert u een naam voor de set in en selecteert u **[!UICONTROL Save]**.

## Een sjabloon verwijderen

Wanneer u een Sjabloonset verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een sjabloon verwijderen:**

1. Selecteer een of meer sjablonen in de rasterweergave, lijstweergave of detailweergave.
1. Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Het scherm Sjabloon begrijpen {#understanding-the-template-screen}

Het scherm van het Malplaatje biedt hulpmiddelen om lagen te manipuleren en te bepalen.

Gebruik deze gereedschappen op het scherm Sjabloon, zodat u sjablonen kunt maken:

* **[!UICONTROL Pan]**: Hiermee kunt u lagen selecteren, deze verplaatsen rond het canvas, de grootte ervan wijzigen of de lagen roteren.

* **[!UICONTROL Text]**: Hiermee maakt u een tekstlaag. Sleep op het canvas om een tekstlaag te maken en voer de tekst in de laag in. Zie [Een tekstlaag maken](#creating-a-text-layer).

* **[!UICONTROL Preview]**: Hiermee opent u het voorvertoningsscherm en geeft u de sjabloon weer in een zoomviewer. U ziet hoe het malplaatje aan gebruikers op uw Website of toepassing kijkt.

* **[!UICONTROL Parameter Summary]** Hiermee opent u het scherm Parameter Summary. U kunt de naam van elke laag in een malplaatje zien, en op elke laag, de namen van parameters die zijn geactiveerd.

* **[!UICONTROL Text Editor v4.3 and Text Editor v4.2]**: Gebruik de meest recente en meest uitgebreide teksteditor. U kunt kiezen om Teksteditor v4.3 of de vorige Teksteditor, Teksteditor v4.2, te gebruiken. Bij het maken van sjablonen is Teksteditor v4.3 standaard geselecteerd. Als u oudere sjablonen bewerkt, is Teksteditor v4.2 standaard geselecteerd. Teksteditor v4.3 biedt momenteel geen ondersteuning voor tekstomloop, dus wanneer u oudere sjablonen bewerkt die tekstomloop gebruiken, gebruikt u Teksteditor v4.2 om de kwaliteit van de sjabloon volledig intact te houden. Als uw oudere sjabloon geen tekstomloop gebruikt, kunt u Teksteditor v4.3 kiezen om te profiteren van de vele nieuwe functies die deze biedt. U kunt bijvoorbeeld Marges verhogen, Marges verlagen, tekst in hoofdletters instellen en tekst passend maken kopiëren.

  >[!NOTE]
  >
  >Teksteditor v4.2 is bedoeld om als optie te worden verwijderd in Adobe Dynamic Media Classic. U wordt aangeraden om teksteditor 4.3 zo veel mogelijk te gebruiken. De **[!UICONTROL Word Wrap]** Deze optie wordt opgenomen in een toekomstige versie van de Teksteditor.

* **[!UICONTROL Designer and Developer]**: Selecteer de optie die uw rol het best beschrijft.

* **[!UICONTROL Canvas]**: definieert het totale beschikbare gebied, in pixels, voor het definiëren van de sjabloon. De standaardgrootte is 300 × 300 pixels. Lagen worden op het canvas geplaatst.

* **[!UICONTROL Layers list]**: Hiermee geeft u de naam van lagen in de sjabloon weer. Als u een laag wilt selecteren, selecteert u de naam ervan in de lijst Lagen. De lijst Lagen bevat gereedschappen voor het toevoegen van effecten aan lagen, het verwijderen van lagen, het opnieuw ordenen van lagen en het bepalen van parameters voor lagen. Zie [Werken met lagen](#working-with-layers).

* **[!UICONTROL Layer Properties area]**: In dit gebied kunt u de achtergrondkleur, dekking, grootte en positie van een laag wijzigen. U kunt ook de achtergrondkleur, dekking en grootte van het canvas wijzigen. U kunt ook schaduw- en gloedeffecten aanpassen. Zie [Werken met lagen](#working-with-layers).

## Afbeeldingslagen maken {#creating-image-layers}

1. Sleep de afbeelding van de elementenbibliotheek naar het canvas.

   De id-naam van de afbeelding wordt weergegeven in de lijst Lagen.

   >[!NOTE]
   >
   >Indien nodig verkleint Adobe Dynamic Media Classic de afbeeldingen, zodat deze op het canvas passen wanneer u een afbeeldingslaag maakt.

## Een tekstlaag maken {#creating-a-text-layer}

1. Selecteer de **[!UICONTROL Text]** gebruiken.
1. Sleep om een tekstvak te maken op het canvas of op een afbeelding.
1. Voeg in het tekstscherm dat wordt geopend, tekst toe door een van de volgende handelingen uit te voeren op het tabblad Voorbeeld:

   * Typ tekst in het tekstvak. Kies Tekst passend maken om de tekst in het tekstvak te laten passen.
   * Plak tekst van het klembord in het tekstvak.

1. Selecteren **[!UICONTROL Apply]** en sluit vervolgens het tekstscherm.

### Tekst opmaken {#format-text}

Ga als volgt te werk om tekst in een tekstlaag op te maken:

1. Dubbelklik in de lijst Lagen op de naam van het tekstvak met tekst die u wilt bewerken. De Teksteditor wordt geopend.
1. Selecteer in het tekstvak van de Teksteditor de tekst die u wilt opmaken. U kunt alle tekst, delen van de tekst of afzonderlijke tekens selecteren.
1. Geef de volgende opmaakopties op en selecteer **[!UICONTROL Apply]**.

   * **[!UICONTROL Font]**: Kies een lettertype in het menu Lettertype. Als het gewenste lettertype niet in het menu staat, kunt u het naar de Adobe Dynamic Media Classic uploaden. Zie Lettertypen.

   * **[!UICONTROL Font Size]**: Kies een tekengrootte in het menu, typ een specifieke grootte in het vak of selecteer de optie **[!UICONTROL Up]** of **[!UICONTROL Down]** pijlen om de grootte met twee punten te vergroten of te verkleinen.

   * **[!UICONTROL Color]**: Selecteer deze optie om een kleur voor tekst te kiezen.

   * **[!UICONTROL Bold]**, **[!UICONTROL Italic]**, of **[!UICONTROL Underline]**: Selecteer de tekst en selecteer vervolgens het pictogram voor het type opmaak dat u op de tekst wilt toepassen.

   * **[!UICONTROL All Caps]**, **[!UICONTROL Superscript]**, of **[!UICONTROL Subscript]**: Selecteer de tekst en selecteer vervolgens het pictogram voor het type opmaak dat u op de tekst wilt toepassen.

   * **[!UICONTROL Alignment]**: Kies een uitlijningsknop om tekst in de tekstlaag links uit te lijnen, te centreren of rechts uit te lijnen.

   * **[!UICONTROL Tracking]**: Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen woorden wilt aanpassen.

   * **[!UICONTROL Kerning]**: Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen tekens wilt aanpassen.

   * **[!UICONTROL Line Spacing]**: Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen regels wilt aanpassen.

   * **[!UICONTROL Baseline Shift]**: Typ of selecteer een numerieke waarde waarmee u een geselecteerd teken omhoog of omlaag wilt verplaatsen ten opzichte van de basislijn van de omringende tekst. Deze optie is vooral handig wanneer u breuken handmatig instelt of de positie van inline-afbeeldingen aanpast.

>[!NOTE]
>
>Selecteren **[!UICONTROL Undo]** als u de laatste handeling wilt omkeren. Selecteren **[!UICONTROL Redo]** als u van gedachten verandert over het omkeren van een handeling nadat u **[!UICONTROL Undo]**.

### Alinea&#39;s opmaken {#format-paragraphs}

1. Dubbelklik in de lijst Lagen op de naam van het tekstvak met tekst die u wilt bewerken. De Teksteditor wordt geopend.
1. Selecteer de alinea die u wilt opmaken.
1. Geef de volgende opmaakopties op en selecteer **[!UICONTROL Apply]**.

   * **[!UICONTROL Alignment]**: Geef het type uitlijning op door op **[!UICONTROL Align left]**, **[!UICONTROL Align center]**, **[!UICONTROL Align right]**, of **[!UICONTROL Justify]**.

   * **[!UICONTROL End of Paragraph Justification]**: Selecteer deze optie om het type uitvulling voor de laatste regel in de alinea op te geven: de laatste regel wordt links uitgelijnd, de laatste regel wordt gecentreerd en de laatste regel wordt rechts uitgelijnd.

   * **[!UICONTROL Line Spacing]**: Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen alle regels in de alinea wilt aanpassen.

   * **[!UICONTROL Indent All]**: Selecteer deze optie om de mate waarin de tekst wordt ingesprongen te verhogen.

   * **[!UICONTROL Remove Indent]**: Selecteer deze optie om de inspringing van de tekst te verminderen.

   * **[!UICONTROL Indent First Line]**: Geef de hoeveelheid op waarmee u de eerste tekstregel wilt laten inspringen.

   * **[!UICONTROL Space Before Paragraph]**: Geef de hoeveelheid ruimte op die boven de eerste tekstregel in de alinea moet worden weergegeven.

   * **[!UICONTROL Space After Paragraph]**: Geef de hoeveelheid ruimte op die u onder de laatste tekstregel in de alinea wilt weergeven.

   * **[!UICONTROL Vertical Align]**: Selecteer waar u de tekst verticaal in het tekstvak wilt weergeven: Boven, Midden, Onder.

   * **[!UICONTROL Text Direction]**: Selecteer de richting waarin de tekst moet worden weergegeven: Van rechts naar links of van links naar rechts.

### Eigenschappen van tekstlagen aanpassen {#adjust-text-layer-properties}

1. Selecteer in het scherm Sjabloonbasisbeginselen het tekstvak dat u wilt aanpassen.
1. Selecteer in het deelvenster Laageigenschappen een van de volgende opties:

   * **[!UICONTROL Shrink Text (Text Editor v4.2 only)]**: Selecteer deze optie om de tekst te verkleinen zodat deze in het tekstvak past.

   * **[!UICONTROL Word Wrap (Text Editor v4.2 only)]**: Selecteer een omloopoptie om op te geven of en hoe de tekst omloopt:

   * **[!UICONTROL Wrap]**: Hiermee loopt u de tekst rond zodat deze in een te klein, horizontaal tekstvak past.

   * **[!UICONTROL No Wrap]**: laat de tekst niet omlopen wanneer het tekstvak te klein is, in plaats daarvan knipt u een gedeelte van de tekst weg.

   * **[!UICONTROL Nonbreaking Wrap]**: Hiermee loopt u tekst rond zodat deze in een tekstvak past en worden woorden niet afgebroken.

   * **[!UICONTROL Position]**: Geeft de locatie van het tekstvak op het canvas aan.

   * **[!UICONTROL Padding]**: Hiermee voegt u marges toe of snijdt u de laagrechthoek bij. Geef het aantal pixels op dat u voor Links, Boven, Onder en Rechts wilt toevoegen of verwijderen. Voer positieve getallen in als u een marge of negatieve getallen aan het uitsnijden wilt toevoegen.

### Tekstbroncode weergeven en bewerken {#view-and-edit-text-source-code}

De informatie op het tabblad Bron van de Teksteditor dient ter referentie. Bewerk de tekst alleen als u bekend bent met het bewerken van broncode.

1. Dubbelklik in de lijst Lagen op de naam van het tekstvak met tekst die u wilt bewerken. De Teksteditor wordt geopend.
1. Selecteer in de Teksteditor de optie **[!UICONTROL Source]** in de Teksteditor.
1. Bekijk of bewerk de tekst naar wens.

   De wijzigingen blijven intact als u heen en weer schakelt tussen de voorvertoning en de bronweergave.

1. Selecteren **[!UICONTROL Apply]** om de bewerkingen te renderen.

## Werken met lagen {#working-with-layers}

Gebruik de lijst Lagen en het gebied Laageigenschappen om met lagen te werken. U kunt lagen opnieuw ordenen, de grootte en de positie van lagen wijzigen, lagen roteren en de achtergrondkleur, de voorgrondkleur, de dekking en de overvloeimodus van een laag bepalen.

U kunt ook de grootte van het canvas wijzigen, de achtergrondkleur kiezen en de instelling voor de dekking wijzigen.

### Lagen opnieuw ordenen {#reordering-layers}

Het wijzigen van de laagvolgorde kan van invloed zijn op de vormgeving, vooral wanneer er sprake is van transparantie of overdrukken. Bekijk een voorvertoning van het resultaat voordat u de wijzigingen doorvoert.

1. Gebruik een van de volgende technieken om de lagen in een sjabloon opnieuw te ordenen:

   * Selecteer een laag in de lijst Lagen. Selecteer vervolgens **[!UICONTROL Up]** of **[!UICONTROL Down]** zo vaak als nodig is om het op de juiste positie in de lijst te plaatsen.
   * Sleep een laag omhoog of omlaag in de lijst Lagen.

### De grootte en positie van lagen en het canvas wijzigen {#changing-the-size-and-position-of-layers-and-the-canvas}

Lagen moeten klein genoeg zijn om op het canvas te passen. U kunt de grootte van een laag of het canvas handmatig wijzigen of maatmetingen invoeren. U kunt de positie van een laag handmatig wijzigen of verschuivingsmetingen invoeren. U kunt een laag ook roteren.

>[!NOTE]
>
>Adobe Dynamic Media Classic raadt u aan een voorinstelling voor afbeeldingen te maken die de exacte grootte van uw sjabloon heeft. Als u de grootte van de voorinstelling Afbeelding afstemt op de sjabloongrootte, weet u zeker dat de uiteindelijke uitvoergrootte en de verscherpingsopties voor de sjabloon correct zijn ingesteld. Nadat u deze Voorinstelling afbeelding hebt gemaakt, kunt u deze kiezen in het menu Voorinstelling toepassen op het scherm Sjabloonvoorvertoning. Het scherm toont u hoe het beeld eruit ziet wanneer het van de server wordt geleverd. Zie [Voorinstellingen afbeelding instellen](setting-image-presets.md#setting_up_image_presets).

* **De grootte van een laag wijzigen**: Als u de grootte van een laag of het canvas wilt wijzigen, selecteert u de laag of het canvas in de lijst Lagen en gebruikt u een van de volgende technieken:

* **Grootte handmatig wijzigen**: Selecteer en sleep een hoek van de laag of het canvas. Met tekstlagen kunt u ook een zijde van de laag slepen. Houd Shift ingedrukt terwijl u sleept om de grootte te wijzigen, maar de hoogte-breedteverhouding (de vorm) te behouden.

* **Metingen voor laaggrootte invoeren**: Voer pixelmetingen in de tekstvakken B (Breedte) en H (Hoogte) in het gebied Laageigenschappen in.

U kunt een laag niet alleen vergroten of verkleinen, maar ook verkleinen. Voer hiertoe een opvullingsmeting in in het vak Links, Rechts, Boven en Onder in het gebied Laageigenschappen. Door opvulling wordt een marge aan de huidige laag toegevoegd die wordt verschoven ten opzichte van de omtrek van de basislaag. Opvulling is handig als u een slagschaduw of een effect Buitenste gloed toevoegt en u het effect beter zichtbaar wilt maken. Door opvulling wordt een laag groter en wordt de achtergrondkleur weergegeven in het uitgebreide gebied met opvulling. De basislaag verplaatst zichzelf ten opzichte van de nieuwe grootte van de laag. Als de huidige laag bijvoorbeeld is gecentreerd op de basislaag en u de linkerzijde van de laag uitbreidt, wordt deze verder naar rechts van de basislaag verplaatst.

* **De positie van een laag wijzigen**: Als u de positie van een laag op het canvas wilt wijzigen, selecteert u de naam van de laag in de lijst Lagen en gebruikt u een van de volgende technieken:

* **Positie handmatig wijzigen**: Verplaats de aanwijzer naar de rand van een laag, maar niet naar de rand van een laag. Als u de cursor met vier pijlpunten ziet, selecteert en begint u te slepen.

* **Positieverschuivingsmetingen invoeren**: Voer de X- en Y-verschuivingsmetingen in de tekstvakken X en Y in. Deze metingen vertegenwoordigen de x- en y-verschuiving van het ankerpunt in pixels.

* **Een laag roteren**: In het vak Roteren wordt de hoek weergegeven waarop de laag is geroteerd. Als u een laag wilt roteren, selecteert u de naam van de laag in de lijst Lagen en gebruikt u een van de volgende technieken:

* **Handmatig roteren**: Verplaats de cursor naar een hoek van de laag, maar niet naar een hoek. Wanneer u de rotatiecursor ziet, sleept u de hoek van de laag. Houd Shift tijdens het slepen ingedrukt om in stappen van 15 graden te roteren.

* **Een gradenmaat invoeren**: Voer het aantal graden in om de laag te roteren. De rotatie is rechtsom. Als u de selectie linksom wilt roteren, voert u een negatief getal in.

**Een laag of een laageffect verbergen:**

U kunt een laag- of laageffect verbergen door het oogpictogram naast de naam van een laag of effect te selecteren. Verborgen lagen worden niet weergegeven in voorvertoningen of uitvoer. De laaggegevens worden niet verwijderd uit de URL. In plaats daarvan, `hide=1` wordt toegevoegd aan de URL om te zien dat de laag verborgen is. Bijvoorbeeld:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### De achtergrondkleur, dekking en overvloeimodus bepalen

Als u een achtergrondkleur, dekking en overvloeimodus voor een laag of het canvas wilt kiezen, selecteert u de laag of het canvas en gebruikt u de volgende technieken:

* **Voorgrondkleur**: Select **[!UICONTROL Foreground Color]** en kiest u een kleurstaal om de kleur van de schaduw of gloed te wijzigen. U kunt ook een parameter color-value in het vak invoeren. De achtergrondkleur is alleen van toepassing op lagen die transparantie gebruiken. Het is bijvoorbeeld van toepassing op een gedeeltelijk transparante laag in een prijstag of de achtergrond van een tekstveld. Lagen die bestaan uit een PSD-, TIFF- of PNG-afbeelding waarop transparantie is ingeschakeld, kunnen een transparante achtergrond hebben.

* **Achtergrondkleur**: Select **[!UICONTROL Background Color]** en kiest u een kleurstaal om de kleur van de opgevulde gebieden te wijzigen.

* **Dekking**: Sleep de schuifregelaar Dekking om een laag doorzichtig te maken, zodat een deel van de onderliggende afbeelding zichtbaar is. De instelling van 100 procent is dekkend en 0 is transparant.

* **Overvloeimodus**: Als u een van de overvloeimodi wilt simuleren die beschikbaar zijn in Photoshop, kiest u een optie. De opties zijn Normaal, Verspreiden, Lichter, Donkerder, Vermenigvuldigen en Scherm. Deze opties zijn beschikbaar voor lagen, niet voor het canvas.

## Schaduw- en gloedeffecten gebruiken op lagen {#using-shadow-and-glow-effects-on-layers}

U kunt een schaduw of gloed op een laag toepassen. De schaduw of gloed wordt toegepast op de omtrek van de laag en wordt naar binnen of naar buiten uitgebreid, afhankelijk van de optie voor schaduw of gloed die u kiest. Als uw sjabloon is gemaakt met een PSD-bestand met schaduw- en gloedeffecten, kunt u deze effecten aanpassen in Adobe Dynamic Media Classic.

Nadat u een schaduw- of gloedeffect hebt toegepast, kunt u de grootte, kleur, dekking en positie aanpassen in het gedeelte Laageigenschappen van het scherm Sjabloon.

### Pas een schaduw- of gloedeffect toe op een laag {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Selecteer een laag in de lijst Lagen.
1. Selecteer de **[!UICONTROL `Add Effect`]** en kiest u een optie:

   * **[!UICONTROL Drop Shadow]**: Hiermee past u een schaduw toe op de onder- en rechterzijde van de laag.

   * **[!UICONTROL Inner Shadow]**: Hiermee past u een schaduweffect toe binnen alle randen van de laag.

   * **[!UICONTROL Outer Glow]**: past een gloedeffect toe rond alle randen van de laag.

   * **[!UICONTROL Inner Glow]**: past een gloedeffect toe binnen alle randen van de laag.

Nadat u een effect hebt toegepast, wordt in de lijst Lagen een effectnaam weergegeven. Als u een effect wilt verwijderen, selecteert u de naam in de lijst Lagen en selecteert u vervolgens **[!UICONTROL Delete]**.

>[!NOTE]
>
>Soms kunt u het effect van een slagschaduw of gloed buiten niet zien als de onderliggende laag niet groot genoeg is om deze weer te geven. Als u de schaduw of gloed niet kunt zien, kunt u overwegen waarden voor opvulling aan de laag toe te voegen of de laag opnieuw te ordenen. Zie [De grootte en positie van lagen en het canvas wijzigen](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) en [Lagen opnieuw ordenen](creating-template.md#reordering_layers).

### Een schaduw- of gloedeffect aanpassen {#adjusting-a-shadow-or-glow-effect}

Als u een schaduw- of gloedeffect wilt aanpassen, selecteert u eerst de naam van het effect in de lijst Lagen. Wijzig vervolgens de instellingen in het gedeelte Laageigenschappen van het scherm Sjabloon:

* **[!UICONTROL Color]**: Selecteer de knop Kleur en kies een kleurstaal om de kleur van de schaduw of gloed te wijzigen. U kunt ook een parameter color-value in het vak invoeren.

* **[!UICONTROL Opacity]**: Sleep de schuifregelaar om de intensiteit van het effect te bepalen. Minder dekkende effecten zijn transparanter.

* **[!UICONTROL Blend Mode]**: Als u een van de overvloeimodi wilt simuleren die beschikbaar zijn in Photoshop, kiest u een optie. De opties zijn Normaal, Verspreiden, Lichter, Donkerder, Vermenigvuldigen en Scherm.

* **[!UICONTROL Size]**: Voer metingen in het vak X en Y in om het schaduweffect te vergroten of te verkleinen. Grootteopties zijn alleen beschikbaar voor binnenschaduwen en slagschaduwen.

* **[!UICONTROL Grow]**: Sleep de schuifregelaar om het effect naar binnen of naar buiten uit te breiden.

* **[!UICONTROL Blur]**: Sleep de schuifregelaar om doezelen aan de randen van het effect te bepalen. Effecten met meer vervaging zijn doezelder.

## Lagen maskeren {#masking-layers}

De lijst Lagen bevat een knop Masker die aangeeft hoe het masker of het alfakanaal van een laag wordt gebruikt. Met de knop Masker kunt u het effect van een achtergrondlaag toepassen op een bepaalde laag of op de gehele bovenliggende laag in de sjabloon. Selecteer een laag in de lijst Lagen en selecteer **[!UICONTROL Mask]** deze staten doorlopen :

* De achtergrond van de laag is dekkend.
* De laaginhoud wordt omgekeerd en de achtergrond van de laag wordt gevuld met effen zwart.
* De achtergrond van de laag wordt gevuld met effen zwart.
