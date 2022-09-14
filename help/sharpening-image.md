---
title: Een afbeelding verscherpen
description: Leer hoe u een afbeelding verscherpt in Adobe Dynamic Media Classic.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2232'
ht-degree: 0%

---

# Een afbeelding verscherpen {#sharpening-an-image}

Verscherpen is een beeldbewerkingstechniek waarmee u de contouren van een digitale afbeelding duidelijker kunt maken. Bij het verscherpen wordt het contrast tussen de randpixels vergroot en wordt de overgang tussen donkere en lichte gebieden benadrukt. Door het verscherpen wordt het lokale contrast verhoogd en worden fijne details weergegeven. Er is geen strikte formule voor het correct verscherpen van alle afbeeldingen. Te weinig verscherping kan tot een zachte afbeelding leiden, maar te veel verscherpen voegt kransen, artefacten en ruis toe.

Adobe Dynamic Media Classic raadt u ten zeerste aan om voor alle afbeeldingen voorinstellingen voor afbeeldingen te gebruiken. Ze zorgen voor een uniforme grootte en verscherpen wordt toegepast op elke afbeelding die met een voorinstelling voor afbeeldingen wordt aangeroepen. Bovendien kunt u de verscherpingsparameters van een voorinstelling voor afbeeldingen gemakkelijk bewerken en wijzigen. De volgende keer dat u publiceert, krijgen alle afbeeldingen die met die voorinstelling worden aangeroepen de nieuwe waarden.

Adobe Dynamic Media Classic raadt ook aan verscherping toe te voegen aan Voorinstellingen viewer en vervolgens een viewer aan te roepen met die voorinstelling. Zo weet u zeker dat de beelden in uw kijkers scherp en aantrekkelijk zijn.

Of u nu Voorinstellingen afbeelding en Voorinstellingen viewer gebruikt of een andere methode voor verscherpen, de onderste regel is echter dat u de afbeeldingen moet verscherpen. Als u dat niet doet, kunnen uw afbeeldingen (en website) er zacht en vaag uitzien.

>[!NOTE]
>
>De opdrachten Verscherpen overschrijven de instellingen van de voorinstelling Afbeelding, inclusief de verscherpingseffecten. Met een voorinstelling voor afbeeldingen bepaalt u de grootte en opmaak van afbeeldingen die worden geleverd op Dynamic Media Image Servers. Adobe Dynamic Media Classic raadt u ten zeerste aan om Voorinstellingen voor afbeeldingen te gebruiken om alle afbeeldingen te leveren, zodat de afbeeldingen even groot en verscherpt worden. Nadat de verscherpingsinstellingen van een afzonderlijke afbeelding zijn gewijzigd, zijn de verscherpingsinstellingen van de voorinstelling voor afbeelding echter niet meer van toepassing op de afbeelding. Deze wordt geleverd zonder de verscherpingsinstellingen van de voorinstelling Afbeelding.

Het is vaak nodig om afbeeldingen te verscherpen. Adobe Dynamic Media Classic en Afbeeldingsservers bieden verschillende verscherpingsopties. Het is belangrijk dat u precies begrijpt wat verscherping doet met een afbeelding en hoeveel verscherping u nodig hebt. De meeste afbeeldingen moeten wat worden verscherpt, maar de vereiste hoeveelheid is afhankelijk van de afbeelding.

Met het verscherpen van afbeeldingen wordt het contrast van pixels vergroot, zodat randen scherper worden. Mensen zien dit verbeterde randcontrast als scherpte. Hoewel u een afbeelding gemakkelijk kunt verbeteren door verscherpingsfilters uit te voeren op een afbeelding, is het ook gemakkelijk om een afbeelding te veel te verscherpen.

Als u een afbeelding te veel verscherpt, krijgt u een halo-effect of een streep van de randlijnen.

U kunt de beste praktijken volgen om het scherpen van uw beelden in Adobe Dynamic Media Classic en op de Server van het Beeld van Dynamic Media te optimaliseren.

Zie [Aanbevolen procedures voor het verscherpen van afbeeldingen in Adobe Dynamic Media Classic en op Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

Zie ook [Verscherpen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) trainingsvideo.

**Een afbeelding verscherpen:**

Als u een afbeelding wilt verscherpen, selecteert u de rollover **[!UICONTROL Edit]** en kies **[!UICONTROL Sharpen]** of opent u deze in het deelvenster Bladeren in de gedetailleerde weergave en selecteert u vervolgens **[!UICONTROL Sharpen]**. De pagina Scherpteditor wordt geopend met verscherpingsopdrachten. Kies opdrachten en selecteer **[!UICONTROL Save]**.

>[!NOTE]
>
>Voordat u een afbeelding verscherpt, kunt u het menu Voorinstelling toepassen selecteren en een voorinstelling voor afbeelding kiezen om te zien wat de verscherpingseffecten zijn. De verscherpingseffecten van een voorinstelling voor afbeeldingen zijn geschikt voor uw afbeelding. De **[!UICONTROL Apply Preset]** onder aan de pagina van de Scherpteditor.

**Verscherpingsopties**

In de volgende tabel staan de verscherpingsopties voor de afbeeldingsserver.

| Naam | URL-protocol | Waarden | Voorbeeld |
| --- | --- | --- | --- |
| Eenvoudig verscherpen | `op_sharpen` | `0` of `1` | `op_sharpen=1` |
| Modus Nieuwe pixels berekenen | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`: Hiermee selecteert u de standaard bi-lineaire interpolatie. Snelste methode voor het berekenen van nieuwe monsters; sommige aliasingartefacten zijn vaak waarneembaar .<br>`bicub`: Selecteert bi-cubische interpolatie. Meer CPU-intensief dan bilin, maar geeft scherpere beelden met minder merkbare aliasing artefacten.<br><br>`sharp2`: Selecteert een gewijzigde functie Lanczos Windows® als interpolatiealgoritme. Dit levert iets scherpere resultaten op dan bi-cubisch tegen hogere CPU-kosten.<br><br>`trilin`: Hiermee selecteert u een aangepaste trilineaire interpolatie, waarbij zowel een hogere als een lagere resolutie wordt gebruikt, indien beschikbaar. Wordt alleen aanbevolen wanneer aliasing een probleem is. Hiermee verlaagt u de JPEG als gevolg van gereduceerde gegevens met hoge frequentie. | `resMode=sharp2` |
| Onscherp masker | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: filtersterktefactor (reëel 0...5)<br><br>`radius`: de straal van de filterkernel in pixel (echt 0...250) <br><br>`threshold`: filterdrempelniveau (int 0...255)<br><br>`monochrome`: instellen op `0` om elke kleurcomponent afzonderlijk onscherp te maskeren, ingesteld op `1` op helderheid (intensiteit) van afbeelding zonder scherp masker | `op_usm=1,1,10,0` |

Selecteer **[!UICONTROL Sharpening]** en kiest u een optie:

* **Geen** - Schakelt verscherpen uit.

* **Verscherpen** - Hiermee wordt een eenvoudige verscherpingscontrole uitgevoerd op het bestand nadat de grootte is gewijzigd. Dit filter lijkt op het filter &quot;Verscherpen&quot; in Adobe Photoshop en ondersteunt geen gebruikersparameters. Normaal gesproken gebruikt u dit filter of **[!UICONTROL Unsharp Mask]**, maar niet beide. Deze methode wordt als beste praktijk niet aanbevolen, maar kan helpen de vervaging te compenseren. (URL: `op_sharpen`)

* **Onscherp masker** - Hiermee kunt u een verscherpingsfiltereffect perfectioneren op de uiteindelijke gedownsampelde afbeelding. U kunt de intensiteit van het effect, de straal van het effect (gemeten in pixels) en een drempel voor het contrast instellen die wordt genegeerd. Voor dit effect worden dezelfde opties gebruikt als voor het filter Onscherp masker van Photoshop. (URL: `op_usm`)

Kies deze opties zodat u de verscherping kunt perfectioneren met Onscherp masker:

* **Hoeveelheid** - Hiermee bepaalt u de hoeveelheid contrast die wordt toegepast op de randpixels. De standaardwaarde is 0,0. Voor afbeeldingen met hoge resolutie kunt u de resolutie verhogen tot 5,0. Beschouw Hoeveelheid als een maat voor de filterintensiteit. De **[!UICONTROL Amount]** de instelling in Adobe Dynamic Media Classic is niet gelijk aan de instelling Hoeveelheid in Adobe Photoshop. Adobe Photoshop gebruikt een hoeveelheid tussen 1% en 500%, terwijl Adobe Dynamic Media Classic schaalt van 0,0 tot 5,0. (5,0 komt ongeveer overeen met 500% in Photoshop, 0,9 komt overeen met 90% enzovoort.)

* **Straal** - Hiermee bepaalt u het aantal pixels rondom de randpixels dat invloed heeft op de verscherping. Het effect wordt uitgevoerd op alle pixels in de afbeelding en wordt in alle richtingen uitgestraald.

De beste straalwaarde hangt van de grootte van het beeld af. Bij een lage waarde worden alleen de randpixels verscherpt. Met een hoge waarde wordt een grotere reeks pixels verscherpt.

Als u bijvoorbeeld een vergelijkbaar verscherpingseffect wilt toepassen op een afbeelding van 2000 x 2000 pixels en een afbeelding van 500 x 500 pixels, kunt u een straalwaarde van twee pixels instellen voor de afbeelding van 2000 x 2000 pixels. Stel vervolgens een straalwaarde in van één pixel in de afbeelding van 500 x 500 pixels (een hogere waarde voor een afbeelding met meer pixels).

* **Drempel** - Hiermee bepaalt u het contrastbereik dat moet worden genegeerd wanneer het filter Onscherp masker wordt toegepast. Met deze optie bepaalt u hoe verschillend de verscherpte pixels moeten zijn ten opzichte van het omringende gebied voordat ze als randpixels worden beschouwd en worden verscherpt.

Bij Drempel wordt een waarde tussen 0 en 255 gebruikt. Dit is het aantal helderheidsstappen in een grijswaardenafbeelding. 0=zwart, 128=50% grijs en 255=wit. Een drempelwaarde van 12 negeert bijvoorbeeld kleine variaties door de helderheid van de huidskleur, zodat er geen ruis wordt toegevoegd en er tegelijkertijd randcontrast wordt toegevoegd aan contrasterende gebieden, zoals waar de wimpers de huid raken.

Stel dat u een foto van iemands gezicht hebt. Het filter Onscherp masker beïnvloedt de gedeelten van de afbeelding met het meeste contrast en de zachte huid zelf. Zelfs de meest vloeiende skin vertoont subtiele wijzigingen in helderheidswaarden. Als u geen drempelwaarde gebruikt, accentueert het filter deze subtiele veranderingen in huidpixels, die tot een lawaaierig effect (waarschijnlijk ongewenst) leiden terwijl ook het contrast op de wimpers verhogen, die scherpte (waarschijnlijk wenselijk) verbeteren. U voorkomt dit door een drempelwaarde te gebruiken die het filter de opdracht geeft pixels te negeren die het contrast niet drastisch wijzigen, zoals een vloeiende skin. U voorkomt ruis of beperking van waarden in afbeeldingen met huidskleuren door bijvoorbeeld te experimenteren met **[!UICONTROL Threshold]** waarden twee tot en met 20. De standaardwaarde **[!UICONTROL Threshold]** Met de waarde 0 worden alle pixels in de afbeelding verscherpt.

* **Toepassen op** - Kies **[!UICONTROL Each Color]** als u de verscherping afzonderlijk wilt toepassen op elke kleurcomponent; kiezen **[!UICONTROL Brightness]** als u verscherping wilt toepassen op helderheidsgebieden van de afbeelding.

**Nieuwe pixels**

Selecteer **[!UICONTROL Resampling]** en kiest u een optie. Met deze opties verscherpt u de afbeelding wanneer deze wordt gedownsampled:

* **[!UICONTROL None]** - Schakelt resampling uit.

* **[!UICONTROL Bilinear]** - de snelste methode voor het berekenen van nieuwe monsters; er zijn enkele aliasingartefacten waarneembaar .

* **[!UICONTROL Bicubic]** - Verhoogt het CPU-gebruik op de afbeeldingsserver, maar geeft scherpere beelden met minder merkbare aliasing artefacten.

* **[!UICONTROL Sharpen2]** - Geeft iets scherpere resultaten dan **[!UICONTROL Bicubic]**, maar met nog hogere CPU-kosten op de Image Server.

* **[!UICONTROL Trilinear]** - gebruikt, indien beschikbaar, zowel hogere als lagere resoluties; wordt alleen aangeraden als aliasing een probleem is. Deze methode vermindert de grootte van JPEG als gevolg van gereduceerde gegevens met hoge frequentie.

**Voorinstellingen voor verscherpen en afbeeldingen**

U kunt alle drie verscherpingseffecten opnemen om het uiteindelijke resultaat te bereiken. Deze methode wordt echter niet aanbevolen. Adobe Dynamic Media Classic raadt u aan de verscherpingseffecten op te slaan als onderdeel van een voorinstelling voor afbeeldingen. Met Voorinstellingen voor afbeeldingen kunt u de meest gebruikte afbeeldingsmodifiers verpakken om een dynamisch vergroot/verkleind afbeelding te maken in een kleine tekstreeks. Een voorinstelling voor afbeeldingen bevat waarden voor de bestandsindeling (gewoonlijk JPEG voor het web), het aantal pixels en de verscherping van afbeeldingen. In plaats van de URL toe te voegen met elke afbeeldingsmodifier die u moet gebruiken om een bepaald type afbeeldingsgrootte te maken, maakt u een benoemde voorinstelling Afbeelding, zoals &quot;miniatuur&quot;. Configureer vervolgens de voorinstelling voor miniatuurafbeelding met de juiste grootte, bestandsindeling en verscherpingsopties. Roep de afbeelding aan met de naam Voorinstelling afbeelding. Met Voorinstellingen voor afbeelding wordt de lengte van de gehele URL ingekort. Deze twee URL&#39;s produceren dezelfde afbeelding van 350 x 350 JPEG met verscherping:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Voorinstellingen voor afbeeldingen kunnen op elk gewenst moment worden gewijzigd en bijgewerkt. U ziet de resultaten van een wijziging in een voorinstelling voor afbeeldingen nadat u deze hebt gepubliceerd en nadat de cache voor de URL is gewist.

Als u één voorinstelling gebruikt voor elke afbeelding in een groottecategorie, kan elke bedrijfsbeheerder de definitie van die voorinstelling voor afbeeldingen bijwerken, opnieuw publiceren en alle afbeeldingen met die indeling beïnvloeden, zonder webcode te wijzigen. U kunt het beste één voorinstelling voor afbeeldingen per unieke grootte op uw site gebruiken. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Image Presets]**. Selecteer vervolgens **[!UICONTROL Add]** of selecteer **[!UICONTROL Edit]** om een bestaande voorinstelling te wijzigen. Het enige vereiste veld is de naam van de voorinstelling zelf. Het wordt echter aanbevolen om in elke voorinstelling een mate van verscherping op te nemen.

**JPG-kwaliteit**

De opties voor Kwaliteit JPG bepalen het compressieniveau JPG:

* **JPG-kwaliteit** - Selecteer deze optie als u compressieniveaus en downsampling van chrominantie wilt instellen.

* **Schuifregelaar** - Hiermee bepaalt u het compressieniveau JPG. Deze instelling is van invloed op zowel de bestandsgrootte als de afbeeldingskwaliteit. De schaal van de kwaliteit van de JPG is 1-100.

* **Downsampling van JPG-chrominantie inschakelen** - Omdat het oog minder gevoelig is voor hoogfrequente kleurinformatie dan hoogfrequente luminantie, verdelen JPEG-afbeeldingen de afbeeldingsgegevens in luminantie en kleurcomponenten. Wanneer een JPEG-afbeelding wordt gecomprimeerd, blijft de luminantiecomponent op volledige resolutie staan, terwijl de kleurcomponenten worden gedownsampled door het gemiddelde te nemen van pixelgroepen. Door downsampling wordt het gegevensvolume met de helft of met een derde verminderd, zonder dat dit van invloed is op de waargenomen kwaliteit. Downsampling is niet van toepassing op grijswaardenafbeeldingen. Met deze techniek vermindert u de hoeveelheid compressie die handig is voor afbeeldingen met veel contrast (bijvoorbeeld afbeeldingen met overlappende tekst).

**Verscherpingsopties voor het hele bedrijf instellen**

Als u geen Vooraf ingesteld Beeld gebruikt of specifieke het scherpen protocollen van de Server van het Beeld langs het URL koord overgaat, dan wordt uw beeld niet verscherpt wanneer het wordt gedownsampled. Als dit gebrek aan verscherping optreedt, kunt u echter standaardwaarden voor verscherpen instellen en wordt elke afbeelding altijd wat verscherpt.

Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**. Als u de standaardmodus voor het berekenen van nieuwe pixels instelt op **[!UICONTROL Sharp2]** wordt de afbeelding altijd verscherpt wanneer het downsamplen wordt uitgevoerd.

**Verscherpen toevoegen aan viewervoorinstellingen**

Tenzij u wijzigingstoetsen voor verscherpende afbeeldingen toevoegt aan de voorinstelling, ziet de kleine afbeelding bij het laden er zacht uit, omdat deze is gedownsampled zodat deze in het viewervenster past zonder te worden verscherpt.

Met voorinstellingen voor viewers (zoals voorinstellingen voor afbeeldingen) kunt u veel opties centraliseren in één locatie, waaronder een keuze voor de skin- en vieweropties (zoals een knop Afdrukken of de snelheid van de zoomanimatie bepalen). Viewer-voorinstellingen bevinden zich in dezelfde sectie als Voorinstellingen afbeelding, onder **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Viewer Presets]**.

Zie [Viewer-voorinstellingen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) trainingsvideo.

De optie Modifiers bevindt zich onder de sectie Core Settings van alle voorinstellingen voor eCatalog, Centrifugeren en Aangepast zoomen Viewer. Door de URL-verscherpingsopdrachten toe te voegen aan het vak Modifiers, voegt u verscherping toe telkens wanneer de viewer wordt aangeroepen met de desbetreffende viewer-voorinstelling.

Als u de voorinstelling van de viewer wilt aanroepen, gebruikt u de `config=` in de URL van de viewer. Hier is een voorbeeld van het aanroepen van een Afbeeldingsset (schoenen) met een Viewer-voorinstelling (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

De voorinstelling wordt hier verscherpt en wijzigt de standaardskin van de viewer.

**Afbeeldingsspecifieke overschrijvingen maken**

De laatste en minst aanbevolen verscherpingsmethode is het per afbeelding verscherpen van overschrijvingen te maken. Met deze methode wordt de verscherping in een voorinstelling voor afbeeldingen overschreven door de eigen specifieke waarden. Deze methode negeert echter ook alle andere verscherpingsmethoden van elke gewenste grootte. Deze methode kan het beste worden gebruikt als bepaalde afbeeldingen niet met een hoge resolutie zijn opgeslagen en de waarden in de Voorinstellingen afbeelding te hoog zijn voor deze kleine afbeeldingen. In dit geval is er mogelijk enkele verscherping per afbeelding nodig.

Selecteer in Adobe Dynamic Media Classic een afbeelding en ga naar de Gedetailleerde weergave (door te dubbelklikken of door te drukken op **[!UICONTROL Detail View]** en selecteert u **[!UICONTROL Sharpen]**. Wijzig een parameter en selecteer vervolgens **[!UICONTROL Save]**. Dit proces vertelt de Server van het Beeld om deze het scherpen parameters eerder dan om het even welk bevel te gebruiken u in URL, zoals een het scherpen bepaling of Vooraf ingesteld Beeld roept. Zorg ervoor dat u publiceert om te zien dat de wijzigingen van kracht worden.
