---
title: Een PDF-document maken
seo-title: Een PDF-document maken
description: 'null'
seo-description: Leer hoe u een PDF-document maakt met behulp van het Web-to-Print-proces in Dynamic Media Classic.
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Een PDF-document maken {#creating-a-pdf-document}

De laatste stap in het Web-aan-Druk proces is het produceren van aangepaste PDF. Nadat eindgebruikers de sjabloon hebben aangepast met de webtoepassing die u hebt gemaakt, maken ze een definitief PDF-document. Deze uiteindelijke PDF wordt doorgaans naar een afdrukservicebureau verzonden voor professioneel afdrukken. Om ervoor te zorgen dat de uiteindelijke PDF goed wordt afgedrukt, gebruiken ontwikkelaars het juiste joboptions-bestand en stellen ze lettertypen, drukkermarkeringen en kleuren correct in.

## PDF-voorinstellingen instellen {#setting-up-pdf-presets}

Geef het PDF-compatibiliteitsniveau en de printerinstellingen op door een PDF-joboptions-bestand te maken en te uploaden naar de Dynamic Media Classic Server. U kunt bijvoorbeeld PDF/X-4-compatibele PDF-uitvoer selecteren (aanbevolen voor publicatieworkflows voor PDF-drukwerk). U kunt het joboptions-bestand maken in de ontwerpsoftware (zoals Adobe Illustrator) of in Acrobat. Neem altijd contact op met de printer. Deze kan u advies geven over de juiste instellingen voor de taakoptie voor de afdruktaak.

Zie de Help van Adobe Acrobat voor meer informatie over het maken van joboptions-bestanden en voor informatie over het maken van een joboptions-bestand in Acrobat.

Een joboptions-bestand maken in Illustrator:

1. Kies Bewerken > Adobe PDF-voorinstellingen.
1. Selecteer in het dialoogvenster de voorinstelling die u wilt gebruiken.

   De volgende instellingen voor taakopties worden ondersteund door Dynamic Media Classic:

   | Taakoptie | Beschrijving |
   |--- |--- |
   | Algemeen | <ul><li>Compatibiliteit </li><li>Compressie op objectniveau</li><li>Miniaturen insluiten</li><li>Optimaliseren voor snelle webweergave</li></ul> |
   | Afbeeldingen | <ul><li>Downsampling</li><li>Resolutie</li><li>Drempel</li><li>Compressie voor kleur, grijs en mono</li></ul> |
   | Lettertypen | <ul><li>Alle fonts insluiten (fonts worden standaard ingesloten)</li><li>OpenType-lettertypen insluiten</li><li>Subset maken van ingesloten lettertypen wanneer percentage gebruikte tekens kleiner is dan:</li><li>Altijd lijst insluiten</li><li>Nooit invoegen</li></ul> |
   | Kleur | <ul><li>Kleurstrategie (alleen labelen van afbeeldingen wordt behandeld als alles labelen)</li><li>Render-intentie document</li><li>Alleen de volgende werkruimten worden ondersteund voor 4.2.5. 4.3 zal u toestaan om het even welke klant te gebruiken verstrekt profiel dat aan IPS is geupload.</li><li>Als tussenoplossing kunt u de doelkleurruimte opgeven voor de illustratie waarnaar de standaardkleurprofielen voor het bedrijf moeten worden omgezet.</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB met coderingsbereik [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Platte XYZ</li><li>Lineaire ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8-bits</li><li>e-sYCC 8-bits</li></ul> |
   | Grijs | <ul><li>Grijsgamma 1,8</li><li>Grijsgamma 2,2</li><li>Puntverbreding 10%</li><li>Puntverbreding 15%</li><li>Puntverbreding 20%</li><li>Puntverbreding 25%</li><li>Puntverbreding 30%</li><li>sGray</li></ul> |
   | CMYK-waarden behouden voor gekalibreerde CMYK-kleurruimten |  |
   | Geavanceerd | OPI-opmerkingen behouden is altijd ingeschakeld |
   | Normen | Compatibiliteitsnorm |

   >[!NOTE]
   >
   >Dynamic Media Classic negeert de instellingen voor printermarkeringen in het joboptions-bestand. In plaats daarvan worden drukkermarkeringen geconfigureerd met de opdracht Dynamische media Klassieke URL.

1. Klik op Exporteren, geef een naam en locatie op en klik op Opslaan.
1. Upload het dossier van baanopties als activa aan het het Publiceren Scene7 Systeem.

   Gebruik het met uw gepubliceerde malplaatje door naar het in URL te verwijzen. Bijvoorbeeld:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## De PDF voorbereiden voor afdrukken {#preparing-the-pdf-for-print}

Voordat u de PDF voltooit voor afdrukken, moet u de richtlijnen in deze sectie volgen.

**Afbeeldingen**

Controleer of alle afbeeldingen in uw publicatietaak zijn geüpload naar de Dynamic Media Classic-server en gepubliceerd.

**Lettertypen**

Zorg ervoor dat alle lettertypen in de publicatietaak zijn geüpload naar de Dynamic Media Classic Server en gepubliceerd. Zorg ervoor dat u wettelijke rechten hebt om de lettertypen te hosten als u eindgebruikers wilt toestaan deze te wijzigen.

**Afbeeldingsresolutie (pixels per inch)**

De resolutie van bitmapafbeeldingen blijft behouden door de Dynamic Media Classic-server in gegenereerde PDF&#39;s die klaar zijn voor afdrukken. Met Dynamic Media Classic wordt de afbeeldingsresolutie indien nodig verhoogd. Voor optimale resultaten laat u de resolutie op de standaardwaarde (doorgaans 72 dpi) staan wanneer u een voorvertoning weergeeft op het web. De standaardresolutie voor alle afbeeldingen in uw bedrijf wordt ingesteld in het venster Publicatie-instellingen/afbeeldingsserver in de sectie Standaardafdrukresolutie. Hogere resoluties (zoals 300 dpi) kunnen leiden tot langere verwerkingstijd en dienen alleen te worden toegepast op een PDF die klaar is voor afdrukken. Gebruik de opdracht imageRes= in de URL om de standaardresolutie voor PDF-taken handmatig te overschrijven.

**Kleurbeheer**

In uw document en afbeeldingen kunnen grijswaarden-, CMYK-, benoemde steunkleuren-, RGB- of Lab-kleurmodellen worden gebruikt. Elk kleurenprofiel kan worden niet gekalibreerd of gekalibreerd door een ICC kleurenprofiel te gebruiken. Sluit het profiel in de gegenereerde PDF-bestand voor afdrukken in voor het beste resultaat. De dynamische Media Klassieke Server doet dit standaard. Controleer of alle vereiste kleurprofielen zijn geüpload naar het Dynamic Media Classic-platform. Controleer bij voorkeur of de kleurbeheeropties die in de ontwerptoepassing zijn ingesteld, overeenkomen met de opties die in de Dynamic Media Classic-server zijn ingesteld:

* **Instellingen voor kleurbeheer ontwerptoepassing:** Geef in de kleurinstellingen van de ontwerptoepassing (bijvoorbeeld Adobe Illustrator) de RGB- en CMYK-kleurprofielen op in de sectie Werkruimten.

* **Dynamische Klassieke instellingen voor kleurbeheer voor media:** De instellingen voor kleurbeheer in de ontwerptoepassing moeten doorgaans overeenkomen met de standaardkleurprofielen in de Dynamic Media Classic-server. U kunt deze instellingen vinden in het venster Publish Setup/Image Server.

## Drukkermarkeringen weergeven {#displaying-printer-marks}

U kunt voor een van deze gevallen een PDF maken:

* Een voltooid document
* Een tussentijds document, zoals een film of plaat, dat naar een drukker kan worden gestuurd voor productie

Een tussendocument kan aanvullende productie-inhoud bevatten, zoals afloopmarges, drukkermarkeringen enzovoort. Deze inhoud wordt meestal buiten de grenzen van de voltooide pagina weergegeven.

Alle markeringen die beschikbaar zijn in het scherm &quot;Drukkermarkeringen toevoegen&quot; in Acrobat, worden ondersteund. De drukkermarkeringen worden bestuurd met de `printerMark` parameter. De syntaxis is `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* snijtekens = 0|1
* aflooptekens = 0|1
* registratietekens = 0|1
* kleurenbalken = 0|1
* paginagegevens = 0|1
* style = Illustrator| IllustratorJ| QuarkXPress
* lijndikte = 0,125| 0,25| 0,50
* laag embed = 0|1

Wanneer u een document voorbereidt voor afdrukproductie, zijn mogelijk drukkermarkeringen nodig om de afdrukservice te helpen bij het uitlijnen van scheidingsfilms voor het maken van proefdrukken, het meten van film voor correcte kalibratie en inktdichtheid, het bijsnijden van film naar grootte, enzovoort. Drukkermarkeringen geven de grenzen van documentvakken aan, zoals bijsnijdvakken en afloopvakken. Productiegerelateerde inhoud kan het volgende omvatten:

* **Mediavak** De grenzen van het fysieke medium waarop de pagina wordt afgedrukt. Inhoud buiten het mediavak kan veilig worden verwijderd zonder dat dit van invloed is op de betekenis van het bestand.

* **Afloopvak** Het gebied waaraan de inhoud van de pagina wordt bijgesneden wanneer deze wordt uitgevoerd in een productieomgeving. Het afloopvak kan gebieden bevatten die nodig zijn om te voldoen aan de fysieke beperkingen van knip-, vouwings- en bijsnijdapparatuur. De standaardwaarde is het uitsnijdvak van de pagina.

* **Het bijsnijdvak** De gewenste afmetingen van de voltooide pagina na het bijsnijden. Het bijsnijdvak kan kleiner zijn dan het mediavak, zodat productiegebonden inhoud mogelijk is, zoals afdrukinstructies, snijtekens en kleurenbalken. De standaardwaarde is het uitsnijdvak van de pagina.

* **Illustratievak** De inhoud van de pagina die betekenis heeft (inclusief potentiële witruimte) zoals bedoeld door de maker van de pagina. De standaardwaarde is het uitsnijdvak van de pagina.

Met de opties in deze tabel kunt u de drukkermarkeringen weergeven die beschikbaar zijn in Adobe Illustrator, InDesign en Acrobat:

| Modifier/Values | Beschrijving |
|--- |--- |
| bleedMargin=top,left,bottom,right | Opgegeven in Acrobat met de optie Paginavakken instellen. Selecteer BleedBox en geef vervolgens de marges op met de optie Marge-instellingen.<br><br>Waarden geven de afstand aan tussen de boven-, linker-, onder- en rechterrand van de oorspronkelijke randen van de illustratie (het mediavak) en de binnenrand. Waarden (0-1000) worden opgegeven in punten.<br><br>Nieuwe hoogte=oorspronkelijke hoogte - (boven+onder)<br><br>Nieuwe breedte= oorspronkelijke breedte - (links+rechts) |
| mediaMargin=top,left,bottom,right | Opgegeven in Acrobat met de optie Paginavakken instellen. Pas het aangepaste paginaformaat aan onder de optie Paginaformaat wijzigen.<br><br>Waarden geven de afstand aan van de randen boven, links, onder en rechts ten opzichte van de oorspronkelijke randen van de illustratie (het mediavak) die naar buiten gaan. Waarden (0-1000) worden opgegeven in punten.<br><br>Nieuwe hoogte=boven+onder+oorspronkelijke<br><br>hoogteNieuwe breedte=boven+onder+oorspronkelijke<br><br>breedteDe nieuwe hoogte- en breedtewaarden bepalen de nieuwe paginagrootte van de gegenereerde PDF.<br><br>Wanneer een nieuw mediavak is gedefinieerd, moeten bij alle berekeningen van de bijsnijdmarge en de afloopmarge het nieuwe mediavak als de rand van de illustratie worden beschouwd. |
| trimMargin=top,left,bottom,right | Opgegeven in Acrobat met de optie Paginavakken instellen. Selecteer het Doos van de Verkleining, dan specificeer de marges met de optie van de Controles van de Marge.<br><br>Waarden geven de afstand aan tussen de boven-, linker-, onder- en rechterrand van de oorspronkelijke randen van de illustratie (het mediavak) en de binnenrand. Waarden (0-1000) worden opgegeven in punten.<br><br>Nieuwe hoogte=oorspronkelijke hoogte - (boven+onder)<br><br>Nieuwe breedte=oorspronkelijke breedte - (links+rechts) |
| printerMark= snijtekens, aflooptekens, registratietekens, kleurenbalken, paginagegevens, stijl, lijndikte, ingesloten laag | Waarden zijn als volgt:<br><br>snijtekens = 0,1 (standaardwaarde is 0)<br><br>aflooptekens = 0,1 (standaardwaarde is 0)<br><br>registratietekens = 0,1 (standaardwaarde is 0)<br><br>kleurenbalken = 0,1 (standaardwaarde is 0)<br><br>pagina-informatie = 0,1 (standaardwaarde is 0)<br><br>stijl = Default, InDesignJ1, InDesignJ2, Illustrator, illustratorJ; QuarkXPress (standaard is Standaard)<br><br>line weight= 0,125-0,2, beide waarden inclusief (standaard is 0,25)<br><br>ingesloten laag = 0, 1. Bij 1 wordt een nieuwe laag gemaakt die alle drukkermarkeringen bevat (standaard is 1)<br><br>Afhankelijk van de gebruikte stijl, worden de markeringen en kleurenbalken anders weergegeven en overeenkomen met de overeenkomstige stijlen die door Acrobat worden gebruikt. |

Let op het volgende over drukkermarkeringen:

* Wanneer u drukkermarkeringen opgeeft, kunt u afloopmarges, snijmarges en mediamarges opgeven via URL-oproepen. Als u drukkermarkeringen opgeeft zonder deze marges op te geven, worden deze markeringen buiten het zichtbare gebied van de gegenereerde PDF weergegeven. Bovendien overlappen de snijtekens en aflooptekens.
* Als u dezelfde margewaarden opgeeft voor de snijmarge en de afloopmarge, worden snijtekens en aflooptekens bij elkaar geplaatst als beide markeringen op 1 inch zijn ingesteld `&printerMark`.
* Als u fmt=swf/afbeeldingsindelingen opgeeft via URL-aanroepen, wordt de uitvoer zonder drukkermarkeringen of marges weergegeven, omdat deze functie specifiek is voor PDF-uitvoer.
* Wanneer u `&printerMark=`via de URL opgeeft, worden standaardwaarden gebruikt voor alle parameters. Als u `&printerMark=1` dit opgeeft, worden interne snijtekens ingesteld op 1 en worden standaardwaarden voor andere parameters gebruikt. Maar als u het element n op ON wilt instellen, moeten alle (n-1) parameters via URL worden opgegeven.
* Als u slechts één waarde opgeeft voor `&trimMargin`, `&bleedMargin`en `&mediaMargin` resulteert dit in het toepassen van die waarde op alle boven-, onder-, linker- en rechtermarges van de oorspronkelijke illustratie.
* Als u alleen de waarden voor de boven- en linkerzijde `&trimMargin`, `&bleedMargin`en `&mediaMargin` de bovenste waarde opgeeft, wordt de onderste waarde toegewezen en is de linkerwaarde gelijk aan de rechterwaarde.
* Als u de rechterwaarde niet opgeeft `&trimMargin`tot en met `&bleedMargin`en `&mediaMargin` als gevolg, wordt de linkerwaarde aan de rechterkant toegewezen.
* Voor een PDF met meerdere pagina&#39;s worden drukkermarkeringen/marges toegepast op alle pagina&#39;s (in Acrobat kunnen gebruikers paginabereiken selecteren voor drukkermarkeringen/marges).
* De uitvoer van een PDF met drukkermarkeringen/ingeschakelde marges komt exact overeen met die van Acrobat X, tenzij anders aangegeven.

Als u een PDF/X-4-compatibel PDF-bestand wilt maken via de &amp;joboption-optie in de URL, dient u rekening te houden met de beperkingen met betrekking tot drukkermarkeringen die zijn opgegeven in de PDF ISO_15930-7-2008.pdf:

* Elk paginaobject van een PDF-bestand bevat een MediaBox. Elk paginaobject in een bestand dat compatibel is met PDF/X-4, moet een TrimBox of een ArtBox bevatten, maar niet beide. De MediaBox kan door overerving worden omvat.
* Als de BleedBox aanwezig is, mag de ArtBox of de TrimBox zich niet buiten de grenzen van de BleedBox uitstrekken. Als de CropBox aanwezig is, mag geen van de ArtBox, de TrimBox of de BleedBox de grenzen van de CropBox overschrijden.
* De ArtBox, de TrimBox, de CropBox of de BleedBox mogen de grenzen van de MediaBox niet overschrijden.
* Voor bepaalde industriële praktijken moet de BleedBox worden gebruikt. Passende handelspraktijken moeten worden gevolgd.
* Het gebruik van de TrimBox wordt aanbevolen voor het gebruik van de ArtBox.
* Alle andere annotaties dan TrapNet- en PrinterMark-annotaties moeten een waarde hebben voor Rect dat volledig buiten de BleedBox ligt (of de TrimBox of de ArtBox als er geen BleedBox aanwezig is). Alle PrinterMark-annotaties moeten een waarde hebben voor Rect dat volledig buiten de TrimBox of ArtBox ligt. Een PDF/X-4-compatibele lezer kan annotaties volledig negeren, behalve PDF TrapNet-annotaties.
* Een rechthoek wordt als volledig buiten een selectiekader beschouwd als alle coördinaten van de rechthoek zich buiten het selectiekader of op de rand ervan bevinden en het snijpunt van de twee rechthoeken nul is.
* Als het ViewerPreferences-woordenboek de ViewArea, ViewClip, PrintArea of PrintClip toetsen bevat, heeft elk van deze toetsen de waarde MediaBox of (als er een BleedBox aanwezig is in alle paginaobjecten van het bestand) BleedBox.

