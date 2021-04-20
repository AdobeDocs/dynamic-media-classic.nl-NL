---
title: Een afbeelding verscherpen
description: Leer hoe u een afbeelding verscherpt.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '2162'
ht-degree: 0%

---


# Een afbeelding {#sharpening-an-image} verscherpen

Verscherpen is een beeldbewerkingstechniek waarmee u de contouren van een digitale afbeelding duidelijker kunt maken. Bij het verscherpen wordt het contrast tussen de randpixels vergroot en wordt de overgang tussen donkere en lichte gebieden benadrukt. Door het verscherpen wordt het lokale contrast verhoogd en worden fijne details weergegeven. Er is geen strikte formule voor het correct verscherpen van alle afbeeldingen. Te weinig verscherping kan tot een zachte afbeelding leiden, maar te veel verscherpen voegt kransen, artefacten en ruis toe.

Dynamic Media Classic raadt u ten zeerste aan voorinstellingen voor afbeeldingen te gebruiken voor alle afbeeldingen. Op deze manier zorgt u voor een uniforme grootte en voor elke afbeelding die met een voorinstelling voor afbeeldingen wordt aangeroepen, is verscherping vereist. Bovendien kunt u de verscherpingsparameters van een voorinstelling voor afbeeldingen heel eenvoudig bewerken en wijzigen. De volgende keer dat u publiceert, krijgen alle afbeeldingen die met die voorinstelling worden aangeroepen de nieuwe waarden.

Dynamic Media Classic raadt ook aan verscherping toe te voegen aan Viewer-voorinstellingen en vervolgens een viewer aan te roepen met die voorinstelling. Dit zorgt ervoor dat de beelden binnen uw kijkers helder en aantrekkelijk zijn.

Of u nu Voorinstellingen afbeelding en Voorinstellingen viewer gebruikt of een andere methode voor verscherpen, de onderste regel is echter dat u de afbeeldingen moet verscherpen. Als u dat niet doet, kunnen uw afbeeldingen (en website) er zacht en vaag uitzien.

>[!NOTE]
>
>De opdrachten Verscherpen overschrijven de instellingen van de voorinstelling Afbeelding, inclusief de verscherpingseffecten. Met een voorinstelling voor afbeeldingen bepaalt u de grootte en opmaak van afbeeldingen die worden geleverd op Dynamic Media Image Servers. Dynamic Media Classic raadt u in hoge mate aan om voorinstellingen voor afbeeldingen te gebruiken om alle afbeeldingen te leveren, zodat de afbeeldingen op gelijke grootte worden geleverd en verscherpen. Nadat de verscherpingsinstellingen van een afzonderlijke afbeelding zijn gewijzigd, zijn de verscherpingsinstellingen van de voorinstelling voor afbeelding echter niet meer van toepassing op de afbeelding. Deze wordt geleverd zonder de verscherpingsinstellingen van de voorinstelling Afbeelding.

Het is vaak nodig om afbeeldingen te verscherpen. Dynamic Media Classic en Image Servers bieden verschillende verscherpingsopties. Het is belangrijk dat u precies begrijpt wat verscherping doet met een afbeelding en hoeveel verscherping u nodig hebt. De meeste afbeeldingen moeten wat worden verscherpt, maar de vereiste hoeveelheid is afhankelijk van de afbeelding.

Met het verscherpen van afbeeldingen wordt het contrast van pixels vergroot, zodat randen scherper worden. Mensen zien dit verbeterde randcontrast als scherpte. Hoewel u een afbeelding gemakkelijk kunt verbeteren door verscherpingsfilters uit te voeren op een afbeelding, is het ook gemakkelijk om een afbeelding te veel te verscherpen.

Als u een afbeelding te veel verscherpt, krijgt u een halo-effect of een streep van de randlijnen.

U kunt het beste de verscherping van uw afbeeldingen in Dynamic Media Classic en op Dynamic Media Image Server optimaliseren.

Zie [Aanbevolen werkwijzen voor het verscherpen van afbeeldingen in Dynamic Media Classic en op Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**Een afbeelding verscherpen**

Als u een afbeelding wilt verscherpen, klikt u op de rollover **Bewerken** en kiest u Verscherpen. U kunt de afbeelding ook openen in het deelvenster Bladeren in de gedetailleerde weergave. Klik vervolgens op **Verscherpen**. Het scherm Scherm van de Redacteur van de Scherpte opent met het scherpen bevelen. Kies opdrachten en klik op **Opslaan**.

>[!NOTE]
>
>Voordat u een afbeelding verscherpt, kunt u het menu Voorinstelling toepassen selecteren en een voorinstelling voor afbeelding kiezen om te zien wat de verscherpingseffecten zijn. De verscherpingseffecten van een voorinstelling voor afbeeldingen kunnen geschikt zijn voor uw afbeelding. Het menu Voorinstelling toepassen bevindt zich onder aan het scherm van de Scherpteditor.

**Verscherpingsopties**

In de volgende tabel staan de verscherpingsopties voor de afbeeldingsserver.

| Naam | URL-protocol | Waarden | Voorbeeld |
|--- |--- |--- |--- |
| Eenvoudig verscherpen | op_scherpen | `0 | 1` | op_scherpen=1 |
| Modus Nieuwe pixels berekenen | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: Hiermee selecteert u de standaard bi-lineaire interpolatie. Snelste methode voor het berekenen van nieuwe monsters; sommige aliasingartefacten kunnen waarneembaar zijn.<br>bicub: Selecteert bi-cubische interpolatie. Meer CPU-intensief dan bilin, maar geeft scherpere beelden met minder merkbare aliasing artefacten.<br><br>scherp2: Selecteert een gewijzigde functie van het Venster Lanczos als interpolatiealgoritme. Dit levert mogelijk iets scherpere resultaten op dan bi-cubisch tegen hogere CPU-kosten.<br><br>triline: Hiermee selecteert u een aangepaste trilineaire interpolatie, waarbij zowel een hogere als een lagere resolutie wordt gebruikt, indien beschikbaar. Wordt alleen aanbevolen wanneer aliasing een probleem is. Hiermee verkleint u de JPEG-grootte door gereduceerde gegevens met hoge frequentie. | resMode=sharp2 |
| Onscherp masker | op_usm | hoeveelheid, straal, drempel, monochroom<br><br>hoeveelheid: filtersterktefactor (reëel 0...5)<br><br>radius: filterkerelstraal in pixels (reëel 0...250) <br><br>drempel: filterdrempelniveau (int 0...255)<br><br>monochroom: ingesteld op 0 voor afzonderlijk onscherp masker van elke kleurcomponent, ingesteld op 1 voor helderheid (intensiteit) van afbeelding zonder scherp masker. | op_usm=1,1,10,0 |

Selecteer het menu Verscherpen en kies een optie:

**** NoneDisables sharpening.

**** VerscherpenHiermee wordt een eenvoudige verscherpingscontrole uitgevoerd op het bestand nadat de grootte is gewijzigd. Dit is vergelijkbaar met het filter &quot;Verscherpen&quot; in Photoshop en ondersteunt geen gebruikersparameters. Normaal gesproken gebruikt u dit filter of Onscherp masker, maar niet beide. Deze methode wordt als beste praktijk niet aanbevolen, maar kan helpen de vervaging te compenseren. (URL: op_scherpen)

**Onscherp** maskerHiermee kunt u een verscherpingsfiltereffect perfectioneren voor de uiteindelijke gedownsampelde afbeelding. U kunt de intensiteit van het effect, de straal van het effect (gemeten in pixels) en een drempel voor het contrast instellen die wordt genegeerd. Voor dit effect worden dezelfde opties gebruikt als voor het filter Onscherp masker van Photoshop. (URL: op_usm)

Kies deze opties om de verscherping af te stemmen met Onscherp masker:

**** AmountHiermee bepaalt u de hoeveelheid contrast die op de randpixels wordt toegepast. De standaardwaarde is 0,0. Voor afbeeldingen met hoge resolutie kunt u de resolutie verhogen tot 5,0. Beschouw Hoeveelheid als een maat voor de filterintensiteit. Houd er rekening mee dat de instelling Bedrag in Dynamic Media Classic niet gelijk is aan de instelling Bedrag in Photoshop. Photoshop gebruikt een hoeveelheid tussen 1% en 500%, terwijl Dynamic Media Classic schaalt tussen 0,0 en 5,0. (5,0 komt ongeveer overeen met 500% in Photoshop, 0,9 komt overeen met 90% enzovoort.)

**** RadiusHiermee bepaalt u het aantal pixels rondom de randpixels dat invloed heeft op de verscherping. Het effect wordt uitgevoerd op alle pixels in de afbeelding en wordt in alle richtingen uitgestraald.

De beste straalwaarde hangt van de grootte van het beeld af. Bij een lage waarde worden alleen de randpixels verscherpt. Met een hoge waarde wordt een grotere reeks pixels verscherpt.

Voor een vergelijkbaar verscherpingseffect voor een afbeelding van 2000 x 2000 pixels en een afbeelding van 500 x 500 pixels, kunt u bijvoorbeeld een straalwaarde van twee pixels instellen voor de afbeelding van 2000 x 2000 pixels. Stel vervolgens een straalwaarde in van één pixel in de afbeelding van 500 x 500 pixels (een hogere waarde voor een afbeelding met meer pixels).

**** Drempel: hiermee bepaalt u het contrastbereik dat moet worden genegeerd wanneer het filter Onscherp masker wordt toegepast. Met deze optie bepaalt u hoe verschillend de verscherpte pixels moeten zijn ten opzichte van het omringende gebied voordat ze als randpixels worden beschouwd en worden verscherpt.

Bij Drempel wordt een waarde tussen 0 en 255 gebruikt. Dit is het aantal helderheidsstappen in een grijswaardenafbeelding. 0=zwart, 128=50% grijs en 255=wit. Een drempelwaarde van 12 negeert bijvoorbeeld kleine variaties door de helderheid van de huidskleur, zodat er geen ruis wordt toegevoegd en er tegelijkertijd randcontrast wordt toegevoegd aan contrasterende gebieden, zoals waar de wimpers de huid raken.

Stel dat u een foto van iemands gezicht hebt. Het filter Onscherp masker beïnvloedt de gedeelten van de afbeelding met het meeste contrast en de zachte huid zelf. Zelfs de meest vloeiende skin vertoont subtiele wijzigingen in helderheidswaarden. Als u geen drempelwaarde gebruikt, accentueert het filter deze subtiele veranderingen in huidpixels, die tot een lawaaierig effect (waarschijnlijk ongewenst) leiden terwijl ook het contrast op de wimpers verhogen, die scherpte (waarschijnlijk wenselijk) verbeteren. U voorkomt dit door een drempelwaarde te gebruiken die het filter de opdracht geeft pixels te negeren die het contrast niet drastisch wijzigen, zoals een vloeiende skin. Probeer te experimenteren met drempelwaarden tussen 2 en 20 om ruis of beperking toe te passen, bijvoorbeeld in afbeeldingen met huidskleuren. Met de standaardwaarde 0 voor Drempel worden alle pixels in de afbeelding verscherpt.

**Toepassen** opElke kleur kiezen om de verscherping afzonderlijk toe te passen op elke kleurcomponent. Kies Helderheid om toe te passen op verscherping op gebieden met helderheid van afbeelding.

**Nieuwe pixels**

Selecteer het menu Nieuwe pixels berekenen en kies een optie. Met deze opties verscherpt u de afbeelding wanneer deze wordt gedownsampled:

**** NoneHiermee schakelt u resampling uit.

**** BilineairDe snelste methode voor het berekenen van nieuwe monsters; er zijn enkele aliasingartefacten waarneembaar .

**** BicubicHiermee verhoogt u het CPU-gebruik op de Image Server, maar geeft u scherpere afbeeldingen met minder merkbare aliasing artefacten.

**Sharpen2** kan enigszins scherpere resultaten dan de Bicubische optie veroorzaken, maar aan nog hogere kosten cpu op de Server van het Beeld.

**** TrilinearGebruikt zowel hogere als lagere resoluties, indien beschikbaar; wordt alleen aangeraden als aliasing een probleem is. Met deze methode wordt de JPEG-grootte verminderd als gevolg van gereduceerde gegevens met een hoge frequentie.

**Voorinstellingen voor verscherpen en afbeeldingen**

U kunt alle drie de verscherpingseffecten mixen om het uiteindelijke resultaat te bereiken. Dit wordt echter niet aanbevolen. Dynamic Media Classic raadt u aan uw verscherpingseffecten op te slaan als onderdeel van een voorinstelling voor afbeeldingen. Met Voorinstellingen voor afbeeldingen kunt u de meestgebruikte afbeeldingswijzigingstoetsen verpakken om een dynamisch vergroot/verkleind afbeelding te maken in een kleine tekstreeks. Een voorinstelling voor afbeeldingen bevat waarden voor de bestandsindeling (meestal JPEG voor het web), het aantal pixels en de verscherping van afbeeldingen. In plaats van de URL toe te voegen met elke afbeeldingswijzigingstoets die nodig is om een bepaald type afbeelding te maken, maakt u een benoemde voorinstelling Afbeelding, zoals &quot;miniatuur&quot;. Configureer de voorinstelling voor miniatuurafbeelding met de juiste grootte, bestandsindeling en verscherpingsopties en roep de afbeelding vervolgens aan met de naam Voorinstelling afbeelding. Met Voorinstellingen voor afbeelding wordt de lengte van de gehele URL ingekort. Deze twee URL&#39;s produceren dezelfde JPEG-afbeelding van 350 x 350 met verscherping:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Voorinstellingen voor afbeeldingen kunnen op elk gewenst moment worden gewijzigd en bijgewerkt. Nadat u een afbeeldingsvoorinstelling hebt gepubliceerd en de cache voor de URL is gewist, ziet u de resultaten van een wijziging in de URL.

Als u één voorinstelling gebruikt voor elke afbeelding in een groottecategorie, kan elke bedrijfsbeheerder de definitie van die voorinstelling voor afbeeldingen bijwerken, opnieuw publiceren en alle afbeeldingen met die indeling beïnvloeden, zonder webcode te wijzigen. U kunt het beste één voorinstelling voor afbeeldingen per unieke grootte op uw site gebruiken. Als u een voorinstelling voor afbeeldingen wilt toevoegen, gaat u naar Instellingen > Toepassingsinstellingen > Voorinstellingen voor afbeeldingen. Voeg vervolgens een bestaande voorinstelling toe of bewerk deze. Het enige vereiste veld is de naam van de voorinstelling zelf. U moet echter in elke voorinstelling een mate van verscherping opnemen.

**JPG-kwaliteit**

De opties voor JPG-kwaliteit bepalen het compressieniveau voor JPG:

**JPG-** kwaliteitSelecteer deze optie als u compressieniveaus en downsampling van chrominantie wilt instellen.

**** SliderHiermee bepaalt u het compressieniveau voor JPG. Deze instelling is van invloed op zowel de bestandsgrootte als de afbeeldingskwaliteit. De JPG-kwaliteitsschaal is 1-100.

**JPG-chrominantiedownsampling inschakelen** Omdat het oog minder gevoelig is voor hoogfrequente kleurinformatie dan hoogfrequente luminantie, verdelen JPEG-afbeeldingen afbeeldingsgegevens in luminantie en kleurcomponenten. Wanneer een JPEG-afbeelding wordt gecomprimeerd, blijft de luminantiecomponent op volledige resolutie staan, terwijl de kleurcomponenten worden gedownsampled door het gemiddelde te nemen van groepen pixels. Door downsampling wordt het gegevensvolume met de helft of met een derde verminderd, zonder dat dit van invloed is op de waargenomen kwaliteit. Downsampling is niet van toepassing op grijswaardenafbeeldingen. Met deze techniek vermindert u de hoeveelheid compressie die handig is voor afbeeldingen met veel contrast (bijvoorbeeld afbeeldingen met overlappende tekst).

**Opties voor verscherpen in het hele bedrijf instellen**

Als u geen Vooraf ingesteld Beeld gebruikt of specifieke het scherpen protocollen van de Server van het Beeld langs het URL koord overgaat, dan wordt uw beeld niet verscherpt wanneer het wordt gedownsampled. Als dit gebeurt, kunt u echter wel standaardwaarden voor verscherpen instellen. Elke afbeelding wordt dan altijd wat verscherpt.

Ga naar Setup > Application Setup > Publish Setup > Image Server om de standaard verscherpingsopties van uw bedrijf in te stellen. Als u de standaardmodus voor het berekenen van nieuwe pixels instelt op Scherp2, wordt de afbeelding altijd verscherpt wanneer de pixels worden gedownsampled.

**Verscherpen toevoegen aan viewervoorinstellingen**

Tenzij u wijzigingstoetsen voor verscherpende afbeeldingen toevoegt aan de voorinstelling, ziet de kleine afbeelding bij het laden er zacht uit, omdat deze is gedownsampled zodat deze in het viewervenster past zonder te worden verscherpt.

In Dynamic Media Classic kunt u met Viewer-voorinstellingen (zoals voorinstellingen voor afbeeldingen) veel opties centraliseren in één locatie, waaronder opties voor skin en viewer (zoals een knop Afdrukken of de snelheid van de zoomanimatie bepalen). Voorinstellingen voor viewers bevinden zich in dezelfde sectie als Voorinstellingen afbeelding, onder Instellingen > Toepassingsinstellingen > Voorinstellingen voor viewer.

De optie Modifiers bevindt zich onder de sectie Core Settings van alle voorinstellingen voor eCatalog, Centrifugeren en Aangepast zoomen Viewer. Door de URL-verscherpingsopdrachten toe te voegen aan het vak Modifiers, voegt u verscherping toe telkens wanneer de viewer wordt aangeroepen met de desbetreffende viewer-voorinstelling.

Als u de voorinstelling Viewer wilt aanroepen, gebruikt u de opdracht config= op de URL van de viewer. Hier volgt een voorbeeld van het aanroepen van een Afbeeldingsset (schoenen) met een Viewer-voorinstelling (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

De voorinstelling wordt hier verscherpt en wijzigt de standaardskin van de viewer.

**Afbeeldingsspecifieke overschrijvingen maken**

De laatste en minst aanbevolen verscherpingsmethode is het per afbeelding verscherpen van overschrijvingen te maken. Hiermee wordt de verscherping in een voorinstelling voor afbeeldingen overschreven door de eigen specifieke waarden. Dit negeert echter alle andere verscherpingsmethoden van elke gewenste grootte. Deze methode kan het beste worden gebruikt als bepaalde afbeeldingen niet met een hoge resolutie zijn opgeslagen en de waarden in de Voorinstellingen afbeelding te hoog zijn voor deze kleine afbeeldingen. In dit geval is mogelijk enige verscherping per afbeelding nodig.

Selecteer in Dynamic Media Classic een willekeurige afbeelding, ga naar de detailweergave (door te dubbelklikken of op de knop Gedetailleerde weergave te drukken) en klik op Verscherpen. Wijzig een parameter en klik op Opslaan. Dit vertelt de Server van het Beeld om deze het scherpen parameters eerder dan om het even welk bevel te gebruiken u in URL, zoals een het scherpen bepaling of Vooraf ingesteld Beeld roept. U moet publiceren om te zien de veranderingen van kracht worden.
