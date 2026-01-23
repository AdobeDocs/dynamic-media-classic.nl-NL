---
title: Een afbeelding verscherpen
description: Leer hoe u een afbeelding verscherpt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '2163'
ht-degree: 0%

---

# Een afbeelding verscherpen {#sharpening-an-image}

Verscherpen is een beeldbewerkingstechniek waarmee u de contouren van een digitale afbeelding duidelijker kunt maken. Bij het verscherpen wordt het contrast tussen de randpixels vergroot en wordt de overgang tussen donkere en lichte gebieden benadrukt. Door het verscherpen wordt het lokale contrast verhoogd en worden fijne details weergegeven. Er is geen strikte formule voor het correct verscherpen van alle afbeeldingen. Te weinig verscherping kan tot een zachte afbeelding leiden, maar te veel verscherpen voegt kransen, artefacten en ruis toe.

Adobe Dynamic Media Classic raadt u ten zeerste aan om voor alle afbeeldingen voorinstellingen voor afbeeldingen te gebruiken. Ze zorgen voor een uniforme grootte en verscherpen wordt toegepast op elke afbeelding die met een voorinstelling voor afbeeldingen wordt aangeroepen. Bovendien kunt u de verscherpingsparameters van een voorinstelling voor afbeeldingen gemakkelijk bewerken en wijzigen. De volgende keer dat u publiceert, krijgen alle afbeeldingen die met die voorinstelling worden aangeroepen de nieuwe waarden.

Adobe Dynamic Media Classic raadt ook aan verscherping toe te voegen aan Voorinstellingen viewer en vervolgens een viewer aan te roepen met die voorinstelling. Zo weet u zeker dat de afbeeldingen voor uw kijkers scherp en aantrekkelijk zijn.

Of u nu Voorinstellingen afbeelding en Voorinstellingen viewer gebruikt of een methode voor verscherpen, de onderste regel is echter dat u de afbeeldingen moet verscherpen. Als u dat niet doet, kunnen uw afbeeldingen (en website) er zacht en vaag uitzien.

>[!NOTE]
>
>De opdrachten Verscherpen overschrijven de instellingen van de voorinstelling Afbeelding, inclusief de verscherpingseffecten. Met een voorinstelling voor afbeeldingen bepaalt u de grootte en de opmaak van de afbeeldingen die worden geleverd op de dynamische mediageleveranciers. Adobe Dynamic Media Classic raadt u ten zeerste aan om Voorinstellingen voor afbeeldingen te gebruiken om alle afbeeldingen te leveren, zodat de afbeeldingen even groot en verscherpt worden. Nadat de verscherpingsinstellingen van een afzonderlijke afbeelding zijn gewijzigd, zijn de verscherpingsinstellingen van de voorinstelling voor afbeelding echter niet meer van toepassing op de afbeelding. Deze wordt geleverd zonder de verscherpingsinstellingen van de voorinstelling Afbeelding.

Het is vaak nodig om afbeeldingen te verscherpen. Adobe Dynamic Media Classic en Afbeeldingsservers bieden verschillende verscherpingsopties. Het is belangrijk dat u precies begrijpt wat verscherping doet met een afbeelding en hoeveel verscherping u nodig hebt. De meeste afbeeldingen moeten wat worden verscherpt, maar de vereiste hoeveelheid is afhankelijk van de afbeelding.

Met het verscherpen van afbeeldingen wordt het contrast van pixels vergroot, zodat randen scherper worden. Mensen zien dit verbeterde randcontrast als scherpte. Hoewel u een afbeelding gemakkelijk kunt verbeteren door verscherpingsfilters uit te voeren op een afbeelding, is het ook gemakkelijk om een afbeelding te veel te verscherpen.

Als u een afbeelding te veel verscherpt, ontstaat een halo-effect of een streep van de lijnen van de rand.

U kunt de beste werkwijzen volgen om de verscherping van uw afbeeldingen in Adobe Dynamic Media Classic en op Dynamic Media Image Server te optimaliseren.

Zie [ Beste praktijken voor het verscherpen van beelden in Adobe Dynamic Media Classic en op de Dynamische Server van het Beeld van Media ](/help/using/assets/s7_sharpening_images.pdf).

Zie ook [ het Verscherpen ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) trainingsvideo.

**om een beeld te verscherpen:**

Als u een afbeelding wilt verscherpen, selecteert u de rolloverknop **[!UICONTROL Edit]** en kiest u **[!UICONTROL Sharpen]** . U kunt de afbeelding ook openen in het deelvenster Bladeren in de gedetailleerde weergave en vervolgens **[!UICONTROL Sharpen]** selecteren. De pagina Scherpteditor wordt geopend met verscherpingsopdrachten. Kies de gewenste opdrachten en klik op **[!UICONTROL Save]** .

>[!NOTE]
>
>Voordat u een afbeelding verscherpt, kunt u het menu Voorinstelling toepassen selecteren en een voorinstelling voor afbeelding kiezen om te zien wat de verscherpingseffecten zijn. De verscherpingseffecten van een voorinstelling voor afbeeldingen zijn geschikt voor uw afbeelding. Het menu **[!UICONTROL Apply Preset]** bevindt zich onder aan de pagina Scherpteditor.

**het Verscherpen opties**

In de volgende tabel worden de verscherpingsopties voor de afbeeldingsserver weergegeven.

| Naam | URL-protocol | Waarden | Voorbeeld |
| --- | --- | --- | --- |
| Eenvoudig verscherpen | `op_sharpen` | `0` of `1` | `op_sharpen=1` |
| Modus Nieuwe pixels berekenen | `resMode` | `bilin` , `bicub` , `sharp2` , `trilin`<br><br>`bilin` : hiermee selecteert u de standaard bi-lineaire interpolatie. De snelste methode voor het berekenen van nieuwe pixels. Sommige aliasingartefacten zijn vaak opvallend.<br>`bicub`: hiermee selecteert u bi-cubische interpolatie. Meer CPU-intensief dan `bilin`, maar geeft scherpere beelden met minder merkbare aliasing artefacten.<br><br>`sharp2`: hiermee wordt een aangepaste Lanczos Windows®-functie geselecteerd als een interpolatiealgoritme. Het kan iets scherpere resultaten dan bi-cubisch tegen hogere kosten van CPU veroorzaken.<br><br>`trilin`: hiermee selecteert u een aangepaste trilineaire interpolatie, waarbij zowel een hogere als een lagere resolutie wordt gebruikt, indien beschikbaar. Wordt alleen aangeraden wanneer aliasing een probleem is. Hiermee verlaagt u de JPEG-formaten als gevolg van gereduceerde gegevens met hoge frequentie. | `resMode=sharp2` |
| Onscherp masker | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: filtersterktefactor (reëel 0...5) <br><br>`radius`: de straal van de filterkernel in pixel (reëel 0...250) <br><br>`threshold`: het niveau van de filterdrempel (geheel 0...255) <br><br>`monochrome` wordt geplaatst aan `0` aan unshark-masker elke kleurencomponent afzonderlijk, die aan `1` wordt geplaatst aan unsharp-masker helderheid beeld ness (intensiteit) | `op_usm=1,1,10,0` |

Selecteer het menu **[!UICONTROL Sharpening]** en kies een optie:

* **niets**: Maakt het scherpen onbruikbaar.

* **verscherpt**: stelt een eenvoudige het verscherpen pas op het dossier in werking nadat het resized. Dit filter lijkt op het filter &quot;Verscherpen&quot; in Adobe Photoshop en ondersteunt geen gebruikersparameters. Normaal gesproken gebruikt u dit filter of **[!UICONTROL Unsharp Mask]** , maar niet beide. Deze methode wordt als beste praktijk niet aanbevolen, maar kan helpen wazig worden compenseren. (URL: `op_sharpen`)

* **Onscherp Masker**: Laat u een het verscherpen filtereffect op het definitieve gedownsampelde beeld verfijnen. U kunt de intensiteit van het effect, de straal van het effect (gemeten in pixels) en een drempel voor contrast instellen die wordt genegeerd. Voor dit effect worden dezelfde opties gebruikt als voor het filter Onscherp masker in Photoshop. (URL: `op_usm`)

Kies deze opties zodat u de verscherping kunt perfectioneren met Onscherp masker:

* **Hoeveelheid**: Beheert de hoeveelheid contrast die op randpixel wordt toegepast. De standaardwaarde is 0,0. Voor afbeeldingen met een hoge resolutie kunt u de resolutie verhogen tot 5,0. Beschouw Hoeveelheid als een maat voor de filterintensiteit. De instelling **[!UICONTROL Amount]** in Adobe Dynamic Media Classic is niet gelijk aan de instelling Hoeveelheid in Adobe Photoshop. Adobe Photoshop gebruikt een hoeveelheid tussen 1% en 500%, terwijl Adobe Dynamic Media Classic schaalt van 0,0 tot 5,0. (5,0 komt ongeveer overeen met 500% in Photoshop, 0,9 komt overeen met 90% enzovoort.)

* **Straal**: Bepaalt het aantal pixel die de randpixel omringen die het scherpen beïnvloeden. Het effect wordt uitgevoerd op alle pixels in de afbeelding en wordt in alle richtingen uitgestraald.

De beste straalwaarde hangt van de grootte van het beeld af. Bij een lage waarde worden alleen de randpixels verscherpt. Met een hoge waarde wordt een grotere reeks pixels verscherpt.

Voor een vergelijkbaar verscherpingseffect voor een afbeelding van 2000 × 2000 pixels en een afbeelding van 500 × 500 pixels kunt u bijvoorbeeld een straalwaarde van twee pixels instellen voor de afbeelding van 2000 × 2000 pixels. Stel vervolgens een straalwaarde in van één pixel in de afbeelding van 500 × 500 pixels (een hogere waarde voor een afbeelding met meer pixels).

* **Drempel**: Bepaalt de waaier van contrast om te negeren wanneer de Unshark filter van het Masker wordt toegepast. Met deze optie bepaalt u hoe verschillend de verscherpte pixels moeten zijn ten opzichte van het omringende gebied voordat de randpixels worden verscherpt.

Bij Drempel wordt een waarde tussen 0 en 255 gebruikt. Dit is het aantal helderheidsstappen in een grijswaardenafbeelding. 0=zwart, 128=50% grijs en 255=wit Een drempelwaarde van 12 negeert bijvoorbeeld kleine variaties door de helderheid van de huidskleur. Hierbij wordt geen ruis toegevoegd, maar wordt wel randcontrast toegevoegd aan contrasterende gebieden, zoals waar de wimpers de huid raken.

Stel dat u een foto van iemands gezicht hebt. Het filter Onscherp masker beïnvloedt de gedeelten van de afbeelding met het meeste contrast en de vloeiende huid zelf. Zelfs de meest vloeiende skin vertoont subtiele wijzigingen in helderheidswaarden. Als u geen drempelwaarde gebruikt, accentueert het filter deze subtiele veranderingen in huidpixels, die tot een lawaaierig effect (waarschijnlijk ongewenst) leiden terwijl ook het contrast op de wimpers verhogen, die scherpte (waarschijnlijk wenselijk) verbeteren. U voorkomt dit door een drempelwaarde te gebruiken die het filter de opdracht geeft pixels te negeren die het contrast niet drastisch wijzigen, zoals een vloeiende skin. U voorkomt ruis of beperking van waarden in afbeeldingen met huidskleuren door bijvoorbeeld te experimenteren met **[!UICONTROL Threshold]** -waarden tussen twee en twintig. Met de standaardwaarde **[!UICONTROL Threshold]** 0 worden alle pixels in de afbeelding verscherpt.

* **is op** van toepassing: kies **[!UICONTROL Each Color]** als u het scherpen afzonderlijk op elke kleurencomponent wilt toepassen; kies **[!UICONTROL Brightness]** als u het scherpen op de gebieden van de beeldhelderheid wilt toepassen.

**opnieuw stalen nemend**

Selecteer het menu **[!UICONTROL Resampling]** en kies een optie. Met deze opties verscherpt u de afbeelding wanneer deze wordt gedownsampled:

* **[!UICONTROL None]**: schakelt het opnieuw berekenen van pixels uit.

* **[!UICONTROL Bilinear]**: de snelste methode voor het berekenen van nieuwe pixels. Er zijn enkele aliasingartefacten waarneembaar.

* **[!UICONTROL Bicubic]**: vergroot het CPU-gebruik op de afbeeldingsserver, maar geeft scherpere afbeeldingen met minder merkbare aliasing artefacten.

* **[!UICONTROL `Sharpen 2`]**: levert iets scherpere resultaten op dan **[!UICONTROL Bicubic]** , maar met nog hogere CPU-kosten voor de Image Server.

* **[!UICONTROL Trilinear]**: gebruikt, indien beschikbaar, zowel hogere als lagere resoluties. Wordt alleen aangeraden wanneer aliasing een probleem is. Met deze methode wordt de JPEG-grootte verminderd als gevolg van gereduceerde gegevens met hoge frequentie.

**Beeld stelt vooraf in en verscherpt**

U kunt alle drie verscherpingseffecten opnemen om het uiteindelijke resultaat te bereiken. Deze methode wordt echter niet aanbevolen. Adobe Dynamic Media Classic raadt u aan de verscherpingseffecten op te slaan als onderdeel van een voorinstelling voor afbeeldingen. Met Voorinstellingen voor afbeeldingen kunt u de meest gebruikte afbeeldingsmodifiers verpakken om een dynamisch vergroot/verkleind afbeelding te maken in een kleine tekstreeks. Een voorinstelling voor afbeeldingen bevat waarden voor de bestandsindeling (gewoonlijk JPEG voor het web), het aantal pixels en de verscherping van afbeeldingen. In plaats van de URL toe te voegen met elke afbeeldingsmodifier die u moet gebruiken om een bepaald type afbeeldingsgrootte te maken, maakt u een benoemde voorinstelling Afbeelding, bijvoorbeeld &quot;miniatuur&quot;. Configureer vervolgens de voorinstelling voor miniatuurafbeelding met de juiste grootte, bestandsindeling en verscherpingsopties. Roep de afbeelding aan met de naam Voorinstelling afbeelding. Met Voorinstellingen voor afbeelding wordt de lengte van de gehele URL ingekort. Deze twee URL&#39;s produceren dezelfde JPEG-afbeelding van 350 x 350 met verscherping:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Voorinstellingen voor afbeeldingen kunnen op elk gewenst moment worden gewijzigd en bijgewerkt. U ziet de resultaten van een wijziging in een voorinstelling voor afbeeldingen nadat u deze hebt gepubliceerd en nadat de cache voor de URL is gewist.

Als u één voorinstelling gebruikt voor elke afbeelding in een formaatcategorie, kan elke bedrijfsbeheerder de definitie van die voorinstelling voor afbeeldingen bijwerken. Vervolgens kunnen ze elke afbeelding opnieuw publiceren en beïnvloeden met die indeling. Alles zonder webcode te wijzigen. U kunt het beste één voorinstelling voor afbeeldingen per unieke grootte op uw site gebruiken. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Image Presets]** om een voorinstelling voor een afbeelding toe te voegen op de algemene navigatiebalk. Selecteer vervolgens **[!UICONTROL Add]** of selecteer **[!UICONTROL Edit]** om een bestaande voorinstelling te wijzigen. Het enige vereiste veld is de naam van de voorinstelling zelf. Het wordt echter aanbevolen om in elke voorinstelling een mate van verscherping op te nemen.

**Kwaliteit JPG**

Met de JPG-kwaliteitsopties bepaalt u het JPG-compressieniveau:

* **Kwaliteit van JPG**: Selecteer deze optie als u compressieniveaus en chrominantiedaling wilt controleren.

* **Schuif**: Bepaalt het de compressieniveau van JPG. Deze instelling is van invloed op zowel de bestandsgrootte als de afbeeldingskwaliteit. De kwaliteitsschaal van JPG is 1-100.

* **laat de Downsampling van de Chrominantie van JPG** toe: Omdat het oog minder gevoelig aan high-frequency kleureninformatie dan high-frequency luminantie is, verdelen de beelden van JPEG beeldinformatie in helderheid en kleurencomponenten. Wanneer een JPEG-afbeelding wordt gecomprimeerd, blijft de luminantiecomponent op volledige resolutie staan, terwijl de kleurcomponenten worden gedownsampled door het gemiddelde te nemen van groepen pixels. Door downsampling wordt het gegevensvolume met de helft of met een derde verminderd, zonder dat dit van invloed is op de waargenomen kwaliteit. Downsampling is niet van toepassing op grijswaardenafbeeldingen. Met deze techniek vermindert u de hoeveelheid compressie die handig is voor afbeeldingen met veel contrast (bijvoorbeeld afbeeldingen met overlappende tekst).

**plaats bedrijf-brede het verscherpen opties**

Als u geen Vooraf ingesteld Beeld gebruikte of specifieke het scherpen protocollen van de Server van het Beeld langs het URL koord overging, dan komt geen verscherping van uw beeld voor wanneer gedownsampled. Als dit gebrek aan verscherping optreedt, kunt u echter standaardwaarden voor verscherpen instellen om ervoor te zorgen dat elke afbeelding altijd wat verscherpt wordt.

Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** om de standaard verscherpingsopties van uw bedrijf in te stellen. Als u de standaardmodus voor het berekenen van nieuwe pixels instelt op **`Sharp2`** , wordt de afbeelding altijd verscherpt wanneer het aantal pixels wordt verlaagd.

**voegt het scherpen aan Kijker toe stelt** vooraf in

Tenzij u wijzigingstoetsen voor verscherpende afbeeldingen hebt toegevoegd aan de voorinstelling, ziet de kleine afbeelding bij het laden er zacht uit, omdat deze is gedownsampled zodat deze in het viewervenster past zonder te worden verscherpt.

Met voorinstellingen voor viewers (zoals voorinstellingen voor afbeeldingen) kunt u veel opties centraliseren in één locatie, waaronder een keuze voor de skin- en vieweropties (zoals een knop Afdrukken of de snelheid van de zoomanimatie bepalen). Viewer Presets vindt u in dezelfde sectie als Voorinstellingen afbeelding onder **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Viewer Presets]** .

Zie [ Kijker vooraf instelt ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) opleidingsvideo.

De optie Modifiers bevindt zich onder de sectie Core Settings van alle voorinstellingen voor eCatalog, Centrifugeren en Aangepast zoomen Viewer. Door de URL-verscherpingsopdrachten toe te voegen aan het vak Modifiers, voegt u verscherping toe telkens wanneer de viewer wordt aangeroepen met die Viewer-voorinstelling.

Als u de voorinstelling van de viewer wilt aanroepen, gebruikt u de opdracht `config=` in de URL van de viewer. Hier is een voorbeeld van het roepen van een Reeks van het Beeld (schoenen) met een Vooraf ingestelde Kijker (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

De voorinstelling wordt hier verscherpt en wijzigt de standaardskin van de viewer.

**creeer beeld-specifieke treedt met voeten**

De laatste en minst aanbevolen verscherpingsmethode is het per afbeelding verscherpen van overschrijvingen te maken. Met deze methode wordt de verscherping in een voorinstelling voor afbeeldingen overschreven door de eigen specifieke waarden. Deze methode negeert echter ook alle andere verscherpingsmethoden van elke gewenste grootte. Deze methode kan het beste worden gebruikt als bepaalde afbeeldingen niet met een hoge resolutie zijn opgeslagen en de waarden in de Voorinstellingen afbeelding te hoog zijn voor deze kleine afbeeldingen. In dit geval is er mogelijk enkele verscherping per afbeelding nodig.

Selecteer in Adobe Dynamic Media Classic een willekeurige afbeelding, ga naar de detailweergave (door te dubbelklikken of op de knop **[!UICONTROL Detail View]** te drukken) en selecteer **[!UICONTROL Sharpen]** . Wijzig een parameter en selecteer vervolgens **[!UICONTROL Save]** . Dit proces vertelt de Server van het Beeld om deze het scherpen parameters eerder dan om het even welk bevel te gebruiken u in URL, zoals een het scherpen bepaling of Vooraf ingesteld Beeld roept. Zorg ervoor dat u publiceert om te zien dat de wijzigingen van kracht worden.
