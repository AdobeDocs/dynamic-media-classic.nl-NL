---
title: Een sjabloon maken
description: Leer hoe u een sjabloon maakt in Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
translation-type: tm+mt
source-git-commit: 223bbacab2f244b91763de2ea324a5c8d777feb9
workflow-type: tm+mt
source-wordcount: '3322'
ht-degree: 0%

---

# Een sjabloon maken {#creating-a-template}

Als u een sjabloon wilt maken, klikt u op **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Selecteer Designer of Developer. Op deze pagina kunt u afbeeldings- en tekstlagen toevoegen. U kunt lagen ook opnieuw ordenen, de grootte en positie van lagen wijzigen en schaduw- en gloedeffecten toepassen op afbeeldingen en tekst.

>[!NOTE]
>
>Als u een sjabloon bewerkt die in een eerdere versie van Dynamic Media Classic is gemaakt, wordt u bij het opslaan gevraagd of u een canvaslaag wilt toevoegen. Klik **[!UICONTROL No]** vermijden toevoegend een basislaag. Als u per ongeluk **[!UICONTROL Yes]** klikt, schrapt `&allowCanvasPrompt` en `&layer=0` bepalingen in URL en drukt **[!UICONTROL Enter]** of **[!UICONTROL Return]**.

## Het creëren van het aanvankelijke malplaatje {#creating-the-initial-template}

Wanneer u een sjabloonset maakt, heeft de optie **[!UICONTROL Publish after save]** op de volgende manieren invloed op de set en stelt u leden in:

| **[!UICONTROL Publish after save]** optie geselecteerd voor opslaan? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |
| Ja | Gepubliceerd | Gepubliceerd |
| Nee | Ongepubliceerd | Leden met een set behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

U kunt een sjabloon maken op basis van een bestaande sjabloon. Open de sjabloon, klik op **[!UICONTROL Save As]** en voer een nieuwe naam in het dialoogvenster Opslaan als in.

**De eerste set sjablonen maken:**

1. Gebruik een van de volgende methoden om uw oorspronkelijke sjabloon te maken:

   * **Selecteer eerst**  de PSD of de afbeeldingen. Selecteer in het deelvenster Bladeren het PSD-bestand of de afbeeldingen die u voor de sjabloon wilt gebruiken, en klik op  **[!UICONTROL Build]** >  **[!UICONTROL Template Basics]**.

   * **Begin van het scherm**  van het Malplaatje - klik  **[!UICONTROL Build]** >  **[!UICONTROL Template Basics]**. Selecteer Designer of Developer.

1. Voer in het dialoogvenster Canvasgrootte invoeren afmetingen voor de breedte en hoogte van de sjabloon in.
1. Selecteer een map in de elementenbibliotheek en sleep het PSD-bestand of de afbeeldingen die u voor de sjabloon wilt gebruiken naar het scherm Sjabloon.
1. Als u klaar bent, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Klik op **[!UICONTROL Save]**.
1. Selecteer een map waarin u de sjabloon wilt opslaan, voer een naam voor de sjabloon in en klik op **[!UICONTROL Submit]**.

   In Dynamic Media Classic worden afbeeldingen zo nodig verkleind om ze op het canvas te passen, het gebied op het scherm Sjabloon waarin u de sjabloon definieert.

## Een sjabloonset bewerken {#editing-a-template-set}

Of u een gepubliceerde set of een niet-gepubliceerde sjabloonset bewerkt, de optie **[!UICONTROL Publish after save]** heeft op de volgende manieren invloed op de set en stelt leden in:

| Reeds gepubliceerd instellen? | **[!UICONTROL Publish after save]** optie geselecteerd voordat u de bewerking opslaat? | Status van set na opslaan | Status van ingestelde leden na opslaan |
|--- |--- |--- |--- |
| Ja | Ja | Gepubliceerd | Gepubliceerd |
| Ja | Nee | Gepubliceerd | Bestaande leden met een set behouden hun gepubliceerde status. Alle nieuwe leden die u tijdens het bewerken hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |
| Nee | Ja | Gepubliceerd | Gepubliceerd |
| Nee | Nee | Ongepubliceerd | Bestaande leden die zijn ingesteld en eventuele nieuwe leden die u tijdens de bewerking hebt toegevoegd, behouden hun gepubliceerde of niet-gepubliceerde status. |

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een sjabloonset bewerken:**

1. Blader in de rasterweergave naar een Sjabloonset en klik vervolgens onder de afbeelding op **[!UICONTROL Edit]**.
1. Wijzig de sjabloon naar wens.
1. Als u klaar bent met bewerken, controleert u of **[!UICONTROL Publish after save]** is geselecteerd (standaard) in de rechterbenedenhoek van de pagina.
1. Klik **[!UICONTROL Save]**, selecteer een opslagomslag, ga een naam voor de reeks in, en klik dan **[!UICONTROL Save]**.

## Een sjabloon {#deleting-a-template} verwijderen

Wanneer u een Sjabloonset verwijdert, wordt de set zelf naar de prullenbak verplaatst. De leden (of &quot;kinderen&quot;) in die reeks worden echter niet beïnvloed; in plaats daarvan behouden zij elk hun bestaande gepubliceerde of niet - gepubliceerde staat .

Zie ook [Elementen handmatig publiceren](publishing-files.md#manually_publishing_assets) en [Publicaties van elementen handmatig ongedaan maken](publishing-files.md#manually_unpublishing_assets).

**Een sjabloon verwijderen:**

1. Selecteer een of meer sjablonen in de rasterweergave, lijstweergave of detailweergave.
1. Klik op **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** op de algemene navigatiebalk.

## Het scherm Sjabloon {#understanding-the-template-screen}

Het scherm van het Malplaatje biedt hulpmiddelen om lagen te manipuleren en te bepalen.

Gebruik de volgende gereedschappen in het scherm Sjabloon om sjablonen te maken:

* **Gereedschap**  Pannen: hiermee kunt u lagen selecteren, verplaatsen rond het canvas, de grootte ervan wijzigen of de lagen roteren.

* **Gereedschap**  Tekst - maakt een tekstlaag. Sleep op het canvas om een tekstlaag te maken en voer de tekst in de laag in. Zie [Een tekstlaag maken](#creating-a-text-layer).

* **Knop**  Voorvertoning - Hiermee opent u het voorvertoningsscherm en geeft u de sjabloon weer in een zoomviewer. U ziet hoe de sjabloon eruit ziet voor gebruikers op uw website of toepassing.

* **De Summiere** knoop van de parameterOpent het Summiere scherm van de Parameter. U kunt de naam van elke laag in een malplaatje zien, en op elke laag, de namen van parameters die zijn geactiveerd.

* **Teksteditor v4.3 en Teksteditor v4.2**  - U kunt kiezen of u de meest recente en meest volledige teksteditor, de Teksteditor v4.3 of de vorige teksteditor, Text Editor v4.2, wilt gebruiken. Bij het maken van sjablonen is Teksteditor v4.3 standaard geselecteerd. Als u oudere sjablonen bewerkt, is Teksteditor v4.2 standaard geselecteerd. Teksteditor v4.3 biedt momenteel geen ondersteuning voor tekstomloop, dus wanneer u oudere sjablonen bewerkt die tekstomloop gebruiken, gebruikt u Teksteditor v4.2 om de kwaliteit van de sjabloon volledig intact te houden. Als uw oudere sjabloon geen tekstomloop gebruikt, kunt u Teksteditor v4.3 kiezen om te profiteren van de vele nieuwe functies die deze biedt. U kunt bijvoorbeeld Marges verhogen, Marges verlagen, tekst in hoofdletters instellen en tekst passend maken kopiëren.

   >[!NOTE]
   >
   >Teksteditor v4.2 wordt uiteindelijk als een optie verwijderd in Dynamic Media Classic. Het wordt daarom aanbevolen om teksteditor 4.3 zo veel mogelijk te gebruiken. De optie Tekstomloop wordt opgenomen in een toekomstige versie van de Teksteditor.

* **Ontwerper en Ontwikkelaar**  - Selecteer de optie die uw rol het beste beschrijft.

* **Canvas**  - Hiermee definieert u het totale beschikbare gebied, in pixels, voor het definiëren van de sjabloon. De standaardgrootte is 300 x 300 pixels. Lagen worden op het canvas geplaatst.

* **Lagenlijst**  - Hiermee geeft u de naam van de lagen in de sjabloon weer. Als u een laag wilt selecteren, selecteert u de naam van de laag in de lijst Lagen. De lijst Lagen bevat gereedschappen voor het toevoegen van effecten aan lagen, het verwijderen van lagen, het opnieuw ordenen van lagen en het bepalen van parameters voor lagen. Zie [Werken met lagen](#working-with-layers).

* **Gebied**  Laageigenschappen - Hier vindt u gereedschappen voor het wijzigen van de achtergrondkleur, dekking, grootte en positie van een laag en de achtergrondkleur, dekking en grootte van het canvas. U kunt ook schaduw- en gloedeffecten aanpassen. Zie [Werken met lagen](#working-with-layers).

## Afbeeldingslagen {#creating-image-layers} maken

1. Sleep de afbeelding van de elementenbibliotheek naar het canvas.

   De id-naam van de afbeelding wordt weergegeven in de lijst Lagen.

   >[!NOTE]
   >
   >Zo nodig verkleint Dynamic Media Classic afbeeldingen, zodat deze op het canvas passen wanneer u een afbeeldingslaag maakt.

## Een tekstlaag {#creating-a-text-layer} maken

1. Klik op het gereedschap **[!UICONTROL Text]**.
1. Sleep om een tekstvak te maken op het canvas of op een afbeelding.
1. Voeg in het tekstscherm dat wordt geopend, tekst toe door een van de volgende handelingen uit te voeren op het tabblad Voorbeeld:

   * Typ tekst in het tekstvak. Kies Tekst passend maken om de tekst in het tekstvak te laten passen.
   * Plak tekst van het klembord in het tekstvak.

1. Klik **[!UICONTROL Apply]**, en sluit dan het scherm van de Tekst.

### Tekst {#format-text} opmaken

Ga als volgt te werk om tekst in een tekstlaag op te maken:

1. Dubbelklik in de lijst Lagen op de naam van het tekstvak met tekst die u wilt bewerken. De Teksteditor wordt geopend.
1. Selecteer in het tekstvak de tekst die u wilt opmaken. U kunt alle tekst, delen van de tekst of afzonderlijke tekens selecteren.
1. Geef een van deze opmaakopties op en klik op **[!UICONTROL Apply]**.

   * **Lettertype**  - Kies een lettertype in het menu Lettertype. Als een lettertype dat u wilt gebruiken niet in het menu staat, kunt u het naar de Dynamic Media Classic uploaden. Zie Lettertypen.

   * **Tekengrootte**  - Kies een tekengrootte in het menu, typ een specifieke grootte in het vak of klik op de pijl  **[!UICONTROL Up]** of de  **[!UICONTROL Down]** pijl om de grootte met twee punten te vergroten of te verkleinen.

   * **Kleur**  - Klik om een kleur voor tekst te kiezen.

   * **Vet, Cursief of Onderstrepen**  - Selecteer de tekst en klik op het pictogram voor het type opmaak dat u op de tekst wilt toepassen.

   * **Alle Kapitalen, Superscript, of Subscript**  - selecteer de tekst, en klik dan het pictogram voor het type van het formatteren u op de tekst wilt toepassen.

   * **Uitlijning**  - kies een knoop van de Uitlijning om tekst in de tekstlaag links uit te lijnen, te centreren, of juist te richten.

   * **Tekstspatiëring**  - Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen woorden wilt aanpassen.

   * **Tekenspatiëring**  - Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen tekens wilt aanpassen.

   * **Regelafstand**  - Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen regels wilt aanpassen.

   * **Basislijnverschuiving**  - Typ of selecteer een numerieke waarde waarmee u een geselecteerd teken omhoog of omlaag wilt verplaatsen ten opzichte van de basislijn van de omringende tekst. Deze optie is vooral handig wanneer u breuken handmatig instelt of de positie van inline-afbeeldingen aanpast.

>[!NOTE]
>
>Klik **[!UICONTROL Undo]** om uw laatste actie om te keren. Klik **[!UICONTROL Redo]** als u van mening verandert over het omkeren van een actie nadat u **[!UICONTROL Undo]** klikt.

### Alinea&#39;s {#format-paragraphs} opmaken

1. Dubbelklik in de lijst Lagen op de naam van het tekstvak met tekst die u wilt bewerken. De Teksteditor wordt geopend.
1. Selecteer de alinea die u wilt opmaken.
1. Geef een van deze opmaakopties op en klik op **[!UICONTROL Apply]**.

   * **Uitlijning**  - Klik om het type uitlijning op te geven: Hiermee lijnt u links uit, lijnt u het middelpunt uit, lijnt u rechts uit of rechtvaardigt u het uitvullen.

   * **Uitvulling**  van einde alinea - Klik om het type uitvulling voor de laatste regel in de alinea op te geven: laatste regel links uitgelijnd; laatste regel wordt gecentreerd; en laatste regel rechts uitgelijnd.

   * **Regelafstand**  - Typ of selecteer een numerieke waarde waarmee u de hoeveelheid ruimte tussen alle regels in de alinea wilt aanpassen.

   * **Alles**  inspringen - Klik om de mate van inspringing van de tekst te verhogen.

   * **Inspringen**  verwijderen - Klik om de hoeveelheid ingesprongen tekst te verminderen.

   * **Inspringen eerste regel**  - Geef de hoeveelheid op waarmee u de eerste regel tekst wilt laten inspringen.

   * **Witruimte voor alinea**  - Geef de hoeveelheid ruimte op die boven de eerste tekstregel in de alinea moet komen.

   * **Ruimte na alinea**  - Geef de hoeveelheid ruimte op die u onder de laatste tekstregel in de alinea wilt weergeven.

   * **Verticaal uitlijnen**  - Selecteer waar de tekst verticaal in het tekstvak moet worden weergegeven: Boven, Midden, Onder.

   * **Tekstrichting**  - Selecteer de richting waarin de tekst moet worden weergegeven: Van rechts naar links of van links naar rechts.

### Eigenschappen van tekstlagen aanpassen {#adjust-text-layer-properties}

1. Selecteer in het scherm Sjabloonbasisbeginselen het tekstvak dat u wilt aanpassen.
1. Selecteer in het deelvenster Laageigenschappen een van de volgende opties:

   * **Tekst verkleinen (alleen Teksteditor v4.2)**  - Als u de tekst wilt aanpassen aan het tekstvak, selecteert u de optie om de tekst te verkleinen.

   * **Tekstomloop (alleen Teksteditor v4.2)**  - Selecteer een optie voor tekstomloop om op te geven of en hoe de tekst om moet lopen:

   * **Tekstomloop** : hiermee wordt de tekst zo ingesloten dat deze in een te klein, horizontaal tekstvak past.

   * **Geen tekstomloop**  - laat de tekst niet omlopen wanneer het tekstvak te klein horizontaal is en snijdt in plaats daarvan een gedeelte van de tekst af.

   * **NB Tekstomloop**  - (Niet-afbrekende omloop) Hiermee wordt de tekst in een tekstvak geplaatst en worden woorden niet afgebroken.

   * **Positie**  - Geeft de locatie van het tekstvak op het canvas aan.

   * **Opvulling**  - Hiermee voegt u marges toe of snijdt u de laagrechthoek bij. Geef het aantal pixels op dat u wilt toevoegen of verwijderen voor Links, Boven, Onder en Rechts. Voer positieve getallen in om een marge of negatieve getallen toe te voegen aan het uitsnijden.

### Tekstbroncode {#view-and-edit-text-source-code} weergeven en bewerken

De informatie op het tabblad Bron van de Teksteditor is ter referentie. Bewerk de tekst alleen als u bekend bent met het bewerken van broncode.

1. Dubbelklik in de lijst Lagen op de naam van het tekstvak met tekst die u wilt bewerken. De Teksteditor wordt geopend.
1. Als u de broncode voor de tekst wilt weergeven, klikt u op het tabblad **[!UICONTROL Source]** in de Teksteditor.
1. Bekijk of bewerk de tekst naar wens.

   De wijzigingen blijven intact als u heen en weer schakelt tussen de voorvertoning en de bronweergave.

1. Klik op **[!UICONTROL Apply]** om de bewerkingen te renderen.

## Werken met lagen {#working-with-layers}

Gebruik de lijst Lagen en het gebied Laageigenschappen om met lagen te werken. U kunt lagen opnieuw ordenen, de grootte en de positie van lagen wijzigen, lagen roteren en de achtergrondkleur, de voorgrondkleur, de dekking en de overvloeimodus van een laag bepalen.

U kunt ook de grootte van het canvas wijzigen, de achtergrondkleur kiezen en de instelling voor de dekking wijzigen.

### Lagen opnieuw ordenen {#reordering-layers}

Het wijzigen van de laagvolgorde kan van invloed zijn op de vormgeving, vooral wanneer er sprake is van transparantie of overdrukken. Bekijk een voorvertoning van het resultaat voordat u de wijzigingen doorvoert.

1. Gebruik een van de volgende technieken om de lagen in een sjabloon opnieuw te ordenen:

   * Selecteer een laag in de lijst Lagen. Klik vervolgens **[!UICONTROL Up]** of **[!UICONTROL Down]** zo vaak als nodig is om het op de juiste positie in de lijst te plaatsen.
   * Sleep een laag omhoog of omlaag in de lijst Lagen.

### De grootte en positie van lagen en het canvas wijzigen {#changing-the-size-and-position-of-layers-and-the-canvas}

Lagen moeten klein genoeg zijn om op het canvas te passen. U kunt de grootte van een laag of het canvas handmatig wijzigen of maatmetingen invoeren. U kunt de positie van een laag handmatig wijzigen of verschuivingsmetingen invoeren. U kunt een laag ook roteren.

>[!NOTE]
>
>Dynamic Media Classic raadt u aan een voorinstelling voor afbeeldingen te maken die de exacte grootte van uw sjabloon heeft. Als u de grootte van de voorinstelling Afbeelding afstemt op de sjabloongrootte, weet u zeker dat de uiteindelijke uitvoergrootte en de verscherpingsopties voor de sjabloon correct zijn ingesteld. Nadat u deze voorinstelling voor afbeelding hebt gemaakt, kunt u deze kiezen in het menu Voorinstelling toepassen op het scherm Sjabloonvoorvertoning. Het scherm toont u hoe het beeld eruit ziet wanneer het van de server wordt geleverd. Zie [Voorinstellingen voor afbeeldingen instellen](setting-image-presets.md#setting_up_image_presets).

* **De grootte van een laag**  wijzigen - Als u de grootte van een laag of het canvas wilt wijzigen, selecteert u de laag of het canvas in de lijst Lagen en gebruikt u een van de volgende technieken:

* **Grootte**  handmatig wijzigen - Selecteer en sleep een hoek van de laag of het canvas. Met tekstlagen kunt u ook een zijde van de laag slepen. Houd Shift ingedrukt terwijl u sleept om de grootte te wijzigen, maar de hoogte-breedteverhouding (de vorm) te behouden.

* **Metingen**  voor laaggrootte invoeren - Voer pixelmetingen in in de tekstvakken B (Breedte) en H (Hoogte) in het gebied Laageigenschappen.

U kunt een laag niet alleen vergroten of verkleinen, maar ook verkleinen. Voer hiertoe een opvullingsmeting in in het vak Links, Rechts, Boven en Onder in het gebied Laageigenschappen. Door opvulling wordt een marge aan de huidige laag toegevoegd die wordt verschoven ten opzichte van de omtrek van de basislaag. Opvulling is handig als u een slagschaduw of een effect Buitenste gloed toevoegt en u het effect beter zichtbaar wilt maken. Door opvulling wordt een laag groter en wordt de achtergrondkleur weergegeven in het uitgebreide gebied met opvulling. De basislaag verplaatst zichzelf ten opzichte van de nieuwe grootte van de laag. Als de huidige laag bijvoorbeeld is gecentreerd op de basislaag en u de linkerzijde van de laag uitbreidt, wordt deze verder naar rechts van de basislaag verplaatst.

* **De positie van een laag**  wijzigen - Als u de positie van een laag op het canvas wilt wijzigen, selecteert u de naam van de laag in de lijst Lagen en gebruikt u een van de volgende technieken:

* **Positie**  handmatig wijzigen - Verplaats de aanwijzer naar een laaggrens, maar niet naar een andere positie. Klik en sleep wanneer u de pijl met vier punten ziet.

* **Plaatsingsverschuivingsmetingen**  invoeren - Voer de X- en Y-verschuivingsmetingen in de tekstvakken X en Y in. Deze metingen vertegenwoordigen de x- en y-verschuiving van het ankerpunt in pixels.

* **Een laag**  roteren - In het vak Roteren wordt de hoek weergegeven waarop de laag is geroteerd. Als u een laag wilt roteren, selecteert u de naam van de laag in de lijst Lagen en gebruikt u een van de volgende technieken:

* **Handmatig roteren**  - De cursor verplaatsen naar, maar niet naar een hoek van de laag. Wanneer u de rotatiecursor ziet, sleept u de hoek van de laag. Houd Shift tijdens het slepen ingedrukt om in stappen van 15 graden te roteren.

* **Een gradenmeting**  invoeren - Voer het aantal graden in om de laag te roteren. de rotatie rechtsom is; Voer een negatief getal in om linksom te roteren.

**Een laag of een laageffect verbergen:**

U kunt een laag- of laageffect verbergen door op het oogpictogram naast de naam van een laag of effect te klikken. Verborgen lagen worden niet weergegeven in voorvertoningen of uitvoer. De laaggegevens worden niet verwijderd uit de URL. In plaats daarvan wordt `hide=1` toegevoegd aan de URL om te zien dat de laag verborgen is. Bijvoorbeeld:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### De achtergrondkleur, dekking en overvloeimodus {#determining-the-background-color-opacity-and-blend-mode} bepalen

Als u een achtergrondkleur, dekking en overvloeimodus voor een laag of het canvas wilt kiezen, selecteert u de laag of het canvas en gebruikt u de volgende technieken:

* **Voorgrondkleur**  - Klik  **[!UICONTROL Foreground Color]** en kies een kleurstaal om de kleur van de schaduw of gloed te wijzigen. U kunt ook een parameter color-value in het vak invoeren. De achtergrondkleur wordt alleen toegepast op lagen die transparantie gebruiken. Het is bijvoorbeeld van toepassing op een gedeeltelijk transparante laag in een prijstag of de achtergrond van een tekstveld. Lagen die bestaan uit een PSD-, TIFF- of PNG-afbeelding waarop transparantie is ingeschakeld, kunnen transparante achtergronden hebben.

* **Achtergrondkleur**  - Klik  **[!UICONTROL Background Color]** en kies een kleurstaal om de kleur van de opgevulde gebieden te wijzigen.

* **Dekking**  - Sleep de schuifregelaar Dekking om een laag doorzichtig te maken, zodat een deel van de onderliggende afbeelding zichtbaar wordt. De instelling van 100 procent is dekkend. 0 is transparant.

* **Overvloeimodus**  - Kies een optie om een van de overvloeimodi te simuleren die beschikbaar zijn in Photoshop. De opties zijn Normaal, Verspreiden, Lichter, Donkerder, Vermenigvuldigen en Scherm. Deze opties zijn beschikbaar voor lagen, niet voor het canvas.

## Schaduw- en gloedeffecten gebruiken op lagen {#using-shadow-and-glow-effects-on-layers}

U kunt een schaduw of gloed op een laag toepassen. De schaduw of gloed wordt toegepast op de omtrek van de laag en wordt naar binnen of naar buiten uitgebreid, afhankelijk van de optie voor schaduw of gloed die u kiest. Als uw sjabloon is gemaakt met een PSD-bestand met schaduw- en gloedeffecten, kunt u deze effecten aanpassen in Dynamic Media Classic.

Nadat u een schaduw- of gloedeffect hebt toegepast, kunt u de grootte, kleur, dekking en positie aanpassen in het gedeelte Laageigenschappen van het scherm Sjabloon.

### Schaduw- of gloedeffect toepassen op een laag {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Selecteer een laag in de lijst Lagen.
1. Selecteer het menu Effect toevoegen en kies een optie:

   * **Slagschaduw**  - Hiermee past u een schaduw toe op de onder- en rechterzijde van de laag.

   * **Schaduw**  binnen - Hiermee past u een schaduweffect toe binnen alle randen van de laag.

   * **Gloed**  buiten - Hiermee past u een gloedeffect toe rond alle randen van de laag.

   * **Gloed**  binnen - Hiermee past u een gloedeffect toe binnen alle randen van de laag.

Nadat u een effect hebt toegepast, wordt in de lijst Lagen een effectnaam weergegeven. Als u een effect wilt verwijderen, selecteert u de naam in de lijst Lagen en klikt u op **[!UICONTROL Delete]**.

>[!NOTE]
>
>Soms kunt u het effect van een slagschaduw of gloed buiten niet zien als de onderliggende laag niet groot genoeg is om deze weer te geven. Als u de schaduw of gloed niet kunt zien, kunt u overwegen waarden voor opvulling aan de laag toe te voegen of de laag opnieuw te ordenen. Zie [De grootte en positie van lagen en het canvas wijzigen](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) en [Lagen opnieuw ordenen](creating-template.md#reordering_layers).

### Een schaduw- of gloedeffect {#adjusting-a-shadow-or-glow-effect} aanpassen

Als u een schaduw- of gloedeffect wilt aanpassen, selecteert u eerst de naam van het effect in de lijst Lagen. Wijzig vervolgens de instellingen in het gedeelte Laageigenschappen van het scherm Sjabloon:

* **Kleur**  - Selecteer de knop Kleur en kies een kleurstaal om de kleur van de schaduw of gloed te wijzigen. U kunt ook een parameter color-value in het vak invoeren.

* **Dekking**  - Sleep de schuifregelaar om te bepalen hoe intens het effect is. Minder dekkende effecten zijn transparanter.

* **Overvloeimodus**  - Kies een optie om een van de overvloeimodi te simuleren die beschikbaar zijn in Photoshop. De opties zijn Normaal, Verspreiden, Lichter, Donkerder, Vermenigvuldigen en Scherm.

* **Grootte**  - Voer metingen in in het vak X en Y om het schaduweffect te vergroten of te verkleinen. Grootteopties zijn alleen beschikbaar voor binnenschaduwen en slagschaduwen.

* **Vergroten**  - Sleep de schuifregelaar om het effect naar binnen of naar buiten uit te breiden.

* **Vervagen**  - Sleep de schuifregelaar om doezelen aan de randen van het effect te bepalen. Effecten met meer vervaging zijn doezelder.

## Lagen maskeren {#masking-layers}

De lijst Lagen bevat een knop Masker die aangeeft hoe het masker of het alfakanaal van een laag wordt gebruikt. Met de knop Masker kunt u het effect van een achtergrondlaag toepassen op een bepaalde laag of op de gehele bovenliggende laag in de sjabloon. Selecteer een laag in de lijst Lagen en klik op **[!UICONTROL Mask]** om deze frames te doorlopen:

* De achtergrond van de laag is dekkend.
* De laaginhoud wordt omgekeerd en de achtergrond van de laag wordt gevuld met effen zwart.
* De achtergrond van de laag wordt gevuld met effen zwart.
