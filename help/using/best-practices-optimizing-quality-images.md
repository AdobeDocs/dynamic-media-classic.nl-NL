---
title: Aanbevolen procedures voor het optimaliseren van de kwaliteit van uw afbeeldingen
description: Leer de beste werkwijzen voor het optimaliseren van de kwaliteit van uw afbeeldingen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Aanbevolen procedures voor het optimaliseren van de kwaliteit van uw afbeeldingen{#best-practices-for-optimizing-the-quality-of-your-images}

Het optimaliseren van de beeldkwaliteit kan een tijdrovend proces zijn omdat veel factoren bijdragen tot het renderen van acceptabele resultaten. Het resultaat is deels subjectief omdat individuen de beeldkwaliteit anders waarnemen. Gestructureerde experimenten zijn essentieel.

Adobe Dynamic Media Classic bevat meer dan 100 opdrachten voor het bedienen van afbeeldingen voor het instellen en optimaliseren van afbeeldingen en het renderen van resultaten. De volgende richtlijnen kunnen u helpen het proces stroomlijnen en goede resultaten snel bereiken gebruikend sommige essentiële bevelen en beste praktijken.

Zie ook [Slimme beeldverwerking](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

>[!TIP]
>
>Uitproberen en ontdekken wat de voordelen zijn van Dynamic Media-beeldmodifiers en Smart Imaging met Dynamic Media [_Opname_](https://snapshot.scene7.com/).
>
> Momentopname is een visueel demonstratieprogramma dat is ontworpen om de kracht van Dynamic Media te illustreren voor geoptimaliseerde en dynamische beeldlevering. Experimenteer met testafbeeldingen of Dynamic Media-URL&#39;s om visueel de uitvoer van verschillende Dynamic Media-afbeeldingsmodifiers en Smart Imaging-optimalisaties te bekijken voor:
>* Bestandsgrootte (met WebP en AVIF levering)
>* Netwerkbandbreedte
>* DPR (pixelverhouding apparaat)
>
>Als u wilt weten hoe eenvoudig het is om Momentopname te gebruiken, speelt u de opdracht [Video over momentopnamen](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot.html?lang=en) (3 minuten en 17 seconden).


## Aanbevolen werkwijzen voor afbeeldingsindeling (&amp;fmt=) {#best-practices-for-image-format-fmt}

* JPG of PNG zijn de beste keuze om afbeeldingen van goede kwaliteit en met beheerbare grootte en gewicht te leveren.
* Als er geen indelingsopdracht in de URL is opgegeven, wordt Dynamic Media Image Serving standaard ingesteld op JPG voor levering.
* JPG wordt met een verhouding van 10:1 gecomprimeerd en levert doorgaans kleinere afbeeldingsbestanden op. PNG wordt gecomprimeerd met een verhouding van ongeveer 2:1, behalve soms wanneer afbeeldingen een lege achtergrond bevatten. PNG-bestanden zijn doorgaans echter groter dan JPG-bestanden.
* JPG maakt gebruik van compressie met verlies. Dit betekent dat afbeeldingselementen (pixels) bij compressie verloren gaan. PNG gebruikt daarentegen compressie zonder verlies.
* JPG comprimeert foto&#39;s vaak met een betere beeldkwaliteit dan synthetische afbeeldingen met scherpe randen en contrast.
* Als uw afbeeldingen transparantie bevatten, gebruikt u PNG omdat JPG geen transparantie ondersteunt.

Als beste manier voor afbeeldingsindeling begint u met de meest gebruikelijke instelling `&fmt=JPG`.

## Aanbevolen werkwijzen voor afbeeldingsgrootte {#best-practices-for-image-size}

Het dynamisch verkleinen van de afbeeldingsgrootte is een van de meestvoorkomende taken die Dynamic Media Image Serving uitvoert. Hierbij moet u de grootte opgeven en desgewenst ook welke downsamplingmodus wordt gebruikt om de schaal van de afbeelding te verkleinen.

* Voor afbeeldingsgrootten is het gebruik van `&wid=<value>` en `&hei=<value>` of alleen `&hei=<value>`. Met deze parameters wordt de afbeeldingsbreedte automatisch ingesteld op basis van de hoogte-breedteverhouding.
* `&resMode=<value>` regelt het algoritme dat wordt gebruikt voor downsampling. Beginnen met `&resMode=sharp2`. Deze waarde biedt de beste afbeeldingskwaliteit. Tijdens het gebruik van de downsamplingwaarde `=bilin` is sneller, leidt dit vaak tot aliasing van artefacten.

U kunt het beste de afbeeldingsgrootte op de beste manier aanpassen `&wid=<value>&hei=<value>&resMode=sharp2` of `&hei=<value>&resMode=sharp2`

## Aanbevolen procedures voor verscherpen van afbeeldingen {#best-practices-for-image-sharpening}

Het verscherpen van afbeeldingen is het meest complexe aspect van het beheren van afbeeldingen op uw website en er worden veel fouten gemaakt. Neem de tijd om meer te weten te komen over hoe verscherpen en onscherp maskeren werken in Adobe Dynamic Media Classic door naar de volgende nuttige bronnen te verwijzen:

whitepaper over aanbevolen werkwijzen [Afbeeldingen verscherpen in Adobe Dynamic Media Classic en op afbeeldingsserver](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Met Adobe Dynamic Media Classic kunt u afbeeldingen verscherpen bij inname, bij levering of beide. Meestal verscherpt u afbeeldingen echter alleen met de ene of de andere methode, maar niet met beide. Wanneer u afbeeldingen verscherpt bij levering, op een URL, krijgt u doorgaans de beste resultaten.

U kunt twee methoden voor het verscherpen van afbeeldingen gebruiken:

* Eenvoudig verscherpen ( `&op_sharpen`) - Vergelijkbaar met het verscherpingsfilter dat in Photoshop wordt gebruikt, wordt bij eenvoudige verscherping de standaardverscherping toegepast op de uiteindelijke weergave van de afbeelding na dynamisch vergroten of verkleinen. Deze methode kan echter niet door de gebruiker worden geconfigureerd. De beste manier is niet om te gebruiken `&op_sharpen` tenzij dit vereist is.
* Onscherp maskeren ( `&op_USM`) - Onscherp maskeren is een industriestandaard filter voor verscherpen. U kunt afbeeldingen het beste verscherpen met onscherp maskeren volgens de onderstaande richtlijnen. Met Onscherp maskeren kunt u de volgende drie parameters instellen:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, sterkte van het effect.)
      * `radius` (0-250, breedte van de &#39;verscherpingslijnen&#39; die worden getekend rond het verscherpte object, zoals wordt gemeten in pixels.)

        Houd er rekening mee dat de parameters `radius` en `amount` tegen elkaar werken. Beperken `radius` kan worden gecompenseerd door `amount`. `Radius` Hiermee kunt u nauwkeuriger bepalen, aangezien bij een lagere waarde alleen de randpixels worden verscherpt, terwijl bij een hogere waarde een grotere groep pixels wordt verscherpt.

      * `threshold` (0-255, gevoeligheid van effect.)

        Deze parameter bepaalt hoe verschillend de verscherpte pixel van het omringende gebied moeten zijn alvorens zij als randpixel worden beschouwd en de filter scherpt hen. Met Drempel voorkomt u te veel verscherpte gebieden met vergelijkbare kleuren, zoals huidskleuren. Als u bijvoorbeeld een drempelwaarde van 12 instelt, worden kleine variaties in de helderheid van de huidskleur genegeerd om &#39;ruis&#39; te voorkomen, terwijl randcontrast wordt toegevoegd aan gebieden met hoog contrast, zoals waar de wimpers de huid raken.

        Voor meer informatie over hoe u deze drie parameters plaatst, met inbegrip van beste praktijken om met de filter te gebruiken, zie [Afbeeldingen verscherpen in Adobe Dynamic Media Classic en op afbeeldingsserver](/help/using/assets/s7_sharpening_images.pdf).

      * Met Adobe Dynamic Media Classic kunt u ook een vierde parameter instellen: monochroom ( `0,1`). Deze parameter bepaalt of onscherp maskeren wordt toegepast op elke kleurcomponent afzonderlijk met behulp van de waarde `0` of op de helderheid/intensiteit van de afbeelding met behulp van de waarde `1`.

Als beste praktijken, begin met de onscherpe parameter van de maskerstraal. De volgende instellingen voor Straal kunt u gebruiken:

* Website: 0,2-0,3 pixels
* Fotografisch afdrukken (250-300 ppi): 0,3-0,5 pixels
* Offsetdrukwerk (266-300 ppi): 0,7-1,0 pixels
* Afdrukken van canvas (150 ppi): 1,5-2,0 pixels

Verhoog de waarde geleidelijk van 1,75 naar 4. Als de verscherping nog steeds niet de gewenste manier is, vergroot u de straal met een decimaalteken en voer de hoeveelheid nogmaals uit van 1,75 naar 4. Herhaal deze bewerking zo nodig.

Laat de monochrome parameter-instelling op 0 staan.

## Aanbevolen werkwijzen voor JPEG-compressie (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Deze parameter bepaalt de coderingskwaliteit van de JPG. Een hogere waarde betekent een afbeelding van hogere kwaliteit, maar een groot bestand. Een lagere waarde betekent ook een afbeelding van lagere kwaliteit, maar een kleiner bestand. Het bereik voor deze parameter is 0-100.
* Stel de parameterwaarde niet in op 100 om te optimaliseren voor kwaliteit. Het verschil tussen een instelling van 90 of 95 en 100 is bijna onwaarneembaar, maar met 100 wordt het afbeeldingsbestand onnodig groter. Om de kwaliteit te optimaliseren maar te voorkomen dat afbeeldingsbestanden te groot worden, stelt u daarom de optie `qlt=` waarde 90 of 95.
* Als u wilt optimaliseren voor een kleine bestandsgrootte van de afbeelding, maar de afbeeldingskwaliteit op een aanvaardbaar niveau wilt houden, stelt u de optie `qlt=` waarde 80. Waarden lager dan 70 tot 75 resulteren in een aanzienlijke verslechtering van de beeldkwaliteit.
* Als beste praktijk, om in het midden te blijven, plaats `qlt=` waarde tot 85 om in het midden te blijven.
* De chromamarkering gebruiken in `qlt=`

   * De `qlt=` parameter heeft een tweede instelling waarmee u downsampling van RGB-chromaticiteit met de normale waarde kunt inschakelen `,0` (standaardwaarde) of schakel deze uit met de waarde `,1`.
   * Om het eenvoudig te houden, start u met RGB-chromaticiteitsdownsampling uitgeschakeld ( `,1`). Deze instelling resulteert doorgaans in een betere beeldkwaliteit, vooral bij synthetische afbeeldingen met veel scherpe randen en contrast.

Als beste praktijken voor het gebruik van de compressie van JPG `&qlt=85,0`.

## Aanbevolen werkwijzen voor JPEG vergroten/verkleinen (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

De parameter `jpegSize` Dit is handig als u wilt garanderen dat een afbeelding een bepaalde grootte niet overschrijdt voor levering aan apparaten met een beperkt geheugen.

* Deze parameter wordt ingesteld in kilobytes ( `jpegSize=<size_in_kilobytes>`). Hiermee wordt de maximaal toegestane grootte voor het leveren van de afbeelding gedefinieerd.
* `&jpegSize=` communiceert met de compressieparameter JPG `&qlt=`. Als de JPG reageert met de opgegeven JPG-compressieparameter ( `&qlt=`) niet hoger is dan `jpegSize` waarde, de afbeelding wordt geretourneerd met `&qlt=` zoals gedefinieerd. Anders, `&qlt=` wordt geleidelijk verkleind totdat de afbeelding past in de maximaal toegestane grootte, of totdat het systeem bepaalt dat de afbeelding niet past en een fout retourneert.

Stel `&jpegSize=` en voeg de parameter toe `&qlt=` als u JPG-afbeeldingen levert aan apparaten met een beperkt geheugen.

## Overzicht van best practices {#best-practices-summary}

U kunt het beste de volgende combinatie van parameters gebruiken om een hoge afbeeldingskwaliteit en een kleine bestandsgrootte te bereiken:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Deze combinatie van instellingen levert in de meeste gevallen uitstekende resultaten op.

Als de afbeelding verder moet worden geoptimaliseerd, kunt u de parameters voor verscherpen (onscherp maskeren) geleidelijk perfectioneren door te beginnen met een straal die is ingesteld op 0,2 of 0,3. Vervolgens verhoogt u geleidelijk het bedrag van 1,75 tot maximaal 4 (400% in Photoshop). Controleer of het gewenste resultaat is bereikt.

Als de verscherpingsresultaten nog steeds niet bevredigend zijn, vergroot u de straal in decimale stappen. Voor elke decimale toename start u de hoeveelheid opnieuw op bij 1,75 en verhoogt u deze geleidelijk tot 4. Herhaal dit proces totdat u het gewenste resultaat hebt bereikt. Terwijl de waarden hierboven een benadering zijn die creatieve studio&#39;s hebben bevestigd, herinner me dat u met andere waarden kunt beginnen en andere strategieën kunt volgen. Of de resultaten voor u bevredigend zijn of niet is een subjectieve kwestie, daarom is gestructureerde experimenten van essentieel belang.

Tijdens het experimenteren zijn de volgende algemene suggesties nuttig om uw workflow te optimaliseren:

* Probeer verschillende parameters in real-time uit en test ze rechtstreeks op een URL of met gebruik van de Adobe Dynamic Media Classic-functionaliteit voor het aanpassen van afbeeldingen. De laatste biedt real-time voorvertoningen voor aanpassingstransacties.
* U kunt het beste de opdrachten Dynamic Media Image Serving groeperen in een voorinstelling voor afbeeldingen. Een voorinstelling voor afbeeldingen bestaat in feite uit URL-opdrachtmacro&#39;s met aangepaste namen voor voorinstellingen, zoals `$thumb_low$` en `&product_high$`. Deze voorinstellingen worden aangeroepen door de naam van de aangepaste voorinstelling in een URL-pad. Met deze functionaliteit kunt u opdrachten en kwaliteitsinstellingen voor verschillende gebruikspatronen van afbeeldingen op uw website beheren en de totale lengte van URL&#39;s verkorten.
* Adobe Dynamic Media Classic biedt ook geavanceerdere manieren om de afbeeldingskwaliteit af te stemmen, zoals het toepassen van verscherping bij opname van afbeeldingen. Voor geavanceerd gebruik waarbij het verder afstemmen en optimaliseren van gerenderde resultaten een optie is, kan Adobe Professional Services u helpen met aangepaste inzichten en aanbevolen procedures.
