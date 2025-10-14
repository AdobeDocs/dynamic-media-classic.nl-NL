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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# Aanbevolen procedures voor het optimaliseren van de kwaliteit van uw afbeeldingen{#best-practices-for-optimizing-the-quality-of-your-images}

Het optimaliseren van de afbeeldingskwaliteit kan veel tijd in beslag nemen. Veel factoren dragen bij tot het renderen van acceptabele resultaten. Het resultaat is deels subjectief omdat individuen de beeldkwaliteit anders waarnemen. Gestructureerde experimenten zijn essentieel.

Adobe Dynamic Media Classic bevat meer dan 100 opdrachten voor het bedienen van afbeeldingen voor het instellen en optimaliseren van afbeeldingen en het renderen van resultaten. De volgende richtlijnen kunnen u helpen het proces stroomlijnen en goede resultaten snel bereiken gebruikend sommige essentiële bevelen en beste praktijken.

Zie ook [&#x200B; Slimme beeldvorming &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Probeer uit en ontdek de voordelen van Dynamische het beeldbepalingen van Media en Slim Beeld, gebruikend Dynamische Momentopname van Media [__ &#x200B;](https://snapshot.scene7.com/).
>
> Momentopname is een visueel demonstratieprogramma dat is ontworpen om de kracht van dynamische media te illustreren voor geoptimaliseerde en dynamische beeldlevering. Experimenteer met testafbeeldingen of dynamische media-URL&#39;s, zodat u visueel de uitvoer van verschillende dynamische media-afbeeldingsmodifiers en slimme afbeeldingsoptimalisaties kunt bekijken voor het volgende:
>
>* Bestandsgrootte (met WebP en AVIF levering)
>* Netwerkbandbreedte
>* DPR (Pixelverhouding apparaat)
>
>Om te leren hoe gemakkelijk het Momentopname moet gebruiken, speel de [&#x200B; video van de de opleidingsopleiding van de Momentopname &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 minuten en 17 seconden).


## Aanbevolen werkwijzen voor afbeeldingsindeling (&amp;fmt=) {#best-practices-for-image-format-fmt}

* JPG of PNG zijn de beste keuze om afbeeldingen van goede kwaliteit en met beheerbare grootte en gewicht te leveren.
* Als er geen indelingsopdracht in de URL wordt opgegeven, wordt standaard JPG ingeschakeld voor levering.
* JPG comprimeert met een verhouding van 10 :1 en produceert doorgaans kleinere afbeeldingsbestanden. PNG perst bij een verhouding van ongeveer 2 :1 samen, behalve soms wanneer de beelden een lege achtergrond bevatten. PNG-bestanden zijn doorgaans echter groter dan JPG-bestanden.
* JPG maakt gebruik van compressie met verlies. Dit betekent dat afbeeldingselementen (pixels) bij compressie verloren gaan. PNG daarentegen maakt gebruik van compressie zonder verlies.
* In JPG worden foto&#39;s vaak gecomprimeerd met een hogere kwaliteit dan synthetische afbeeldingen met scherpe randen en contrast.
* Als uw afbeeldingen transparantie bevatten, gebruikt u PNG omdat JPG geen transparantie ondersteunt.

U kunt het beste de afbeeldingsindeling gebruiken door eerst de meest gebruikelijke instelling te gebruiken `&fmt=JPG` .

## Aanbevolen werkwijzen voor afbeeldingsgrootte {#best-practices-for-image-size}

Dynamisch verkleinen van de afbeeldingsgrootte is een van de meest voorkomende taken die Dynamic Media Image Serving uitvoert. Hierbij moet u de grootte opgeven en eventueel opgeven in welke downsamplingmodus de afbeelding moet worden gedownsampled.

* Voor het instellen van de afbeeldingsgrootte kunt u het beste en het meest rechtse `&wid=<value>` en `&hei=<value>` of alleen `&hei=<value>` gebruiken. Met deze parameters wordt de afbeeldingsbreedte automatisch ingesteld op basis van de hoogte-breedteverhouding.
* `&resMode=<value>` bepaalt de algoritme die wordt gebruikt voor downsampling. Begin met `&resMode=sharp2` . Deze waarde biedt de beste afbeeldingskwaliteit. Terwijl het gebruiken van de downsampling waarde `=bilin` sneller is, resulteert het vaak in aliasing van artefacten.

U kunt het beste `&wid=<value>&hei=<value>&resMode=sharp2` of `&hei=<value>&resMode=sharp2` gebruiken om de afbeeldingsgrootte aan te passen

## Aanbevolen procedures voor verscherpen van afbeeldingen {#best-practices-for-image-sharpening}

Het verscherpen van afbeeldingen is het meest complexe aspect van het beheren van afbeeldingen op uw website en er worden veel fouten gemaakt. Neem de tijd om meer te weten te komen over hoe verscherpen en onscherp maskeren werken in Adobe Dynamic Media Classic door naar de volgende nuttige bronnen te verwijzen:

Het Witboek van beste praktijken [&#x200B; verscherpt beelden in Adobe Dynamic Media Classic en op de Server van het Beeld &#x200B;](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Met Adobe Dynamic Media Classic kunt u afbeeldingen verscherpen bij inname, bij levering of beide. Meestal verscherpt u afbeeldingen echter alleen met de ene of de andere methode, maar niet met beide. Wanneer u afbeeldingen verscherpt bij levering, op een URL, krijgt u doorgaans de beste resultaten.

U kunt twee methoden voor het verscherpen van afbeeldingen gebruiken:

* Eenvoudig verscherpen ( `&op_sharpen` ): net als het verscherpingsfilter in Photoshop wordt bij eenvoudige verscherping de standaardverscherping toegepast op de uiteindelijke weergave van de afbeelding na dynamisch vergroten of verkleinen. Deze methode kan echter niet door de gebruiker worden geconfigureerd. U kunt het gebruik van `&op_sharpen` het beste voorkomen, tenzij dat nodig is.
* Onscherp maskeren ( `&op_USM` ): Onscherp maskeren is een industriestandaard filter voor verscherpen. U kunt afbeeldingen het beste verscherpen met onscherp maskeren volgens de onderstaande richtlijnen. Met Onscherp maskeren kunt u de volgende drie parameters instellen:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, sterkte van het effect.)
      * `radius` (0-250, breedte van de &#39;verscherpingslijnen&#39; die rond het verscherpte object zijn getekend, zoals gemeten in pixels.)

        Onthoud dat de parameters `radius` en `amount` tegen elkaar werken. Vermindering van `radius` kan worden gecompenseerd door het verhogen van `amount` . Met `Radius` kunt u nauwkeuriger bepalen, aangezien bij een lagere waarde alleen de randpixels worden verscherpt, terwijl bij een hogere waarde een grotere groep pixels wordt verscherpt.

      * `threshold` (0-255, gevoeligheid van effect.)

        Deze parameter bepaalt hoe verschillend de verscherpte pixel van het omringende gebied moeten zijn alvorens zij als randpixel worden beschouwd en de filter scherpt hen. Met Drempel voorkomt u te veel verscherpte gebieden met vergelijkbare kleuren, zoals huidskleuren. Als u bijvoorbeeld een drempelwaarde van 12 instelt, worden kleine variaties in de helderheid van de huidskleur genegeerd om &#39;ruis&#39; te voorkomen, terwijl randcontrast wordt toegevoegd aan gebieden met hoog contrast, zoals waar de wimpers de huid raken.

        Voor meer informatie over hoe u deze drie parameters plaatst, met inbegrip van beste praktijken om met de filter te gebruiken, zie [&#x200B; scherp beelden in Adobe Dynamic Media Classic en op de Server van het Beeld &#x200B;](/help/using/assets/s7_sharpening_images.pdf).

      * Met Adobe Dynamic Media Classic kunt u ook een vierde parameter beheren: monochroom ( `0,1`). Deze parameter bepaalt of onscherp maskeren wordt toegepast op elke kleurcomponent afzonderlijk met de waarde `0` of op de helderheid/intensiteit van de afbeelding met de waarde `1` .

Als beste praktijken, begin met de onscherpe parameter van de maskerstraal. De volgende instellingen voor Straal kunt u gebruiken:

* Website: 0.2-0.3 pixels
* Fotografisch afdrukken (250-300 ppi): 0,3-0,5 pixels
* Offsetdrukwerk (266-300 ppi): 0,7-1,0 pixels
* Afdrukken van canvas (150 ppi): 1,5-2,0 pixels

Verhoog de waarde geleidelijk van 1,75 naar 4. Als de verscherping nog steeds niet de gewenste manier is, vergroot u de straal met een decimaalteken en voer de hoeveelheid nogmaals uit van 1,75 naar 4. Herhaal deze bewerking zo nodig.

Laat de monochrome parameter-instelling op 0 staan.

## Aanbevolen procedures voor JPEG-compressie (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Deze parameter bepaalt de coderingskwaliteit van JPG. Een hogere waarde betekent een afbeelding van hogere kwaliteit, maar een groot bestand. Een lagere waarde betekent een afbeelding van lagere kwaliteit, maar een kleiner bestand. Het bereik voor deze parameter is 0-100.
* Stel de parameterwaarde niet in op 100 om te optimaliseren voor kwaliteit. Het verschil tussen een instelling van 90 of 95 en 100 is bijna onwaarneembaar. Toch vergroot 100 onnodig de grootte van het afbeeldingsbestand. Stel de waarde `qlt=` daarom in op 90 of 95 om de kwaliteit te optimaliseren, maar te voorkomen dat afbeeldingsbestanden te groot worden.
* Als u wilt optimaliseren voor een kleine bestandsgrootte van de afbeelding, maar de afbeeldingskwaliteit op een acceptabel niveau wilt houden, stelt u de `qlt=` -waarde in op 80. Waarden lager dan 70 tot 75 resulteren in een aanzienlijke verslechtering van de beeldkwaliteit.
* Als beste manier om in het midden te blijven, stelt u de `qlt=` -waarde in op 85 om in het midden te blijven.
* De chromamarkering gebruiken in `qlt=`

   * De parameter `qlt=` heeft een tweede instelling waarmee u het downsamplen van RGB-kleuren kunt inschakelen met de normale waarde `,0` (standaardwaarde) of uitschakelen met de waarde `,1` .
   * Om het eenvoudig te houden, start u met RGB-chromaticiteitsdownsampling uitgeschakeld ( `,1` ). Deze instelling resulteert doorgaans in een betere beeldkwaliteit, vooral bij synthetische afbeeldingen met veel scherpe randen en contrast.

U kunt het beste `&qlt=85,0` gebruiken voor JPG-compressie.

## Best practices voor JPEG-grootte (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

De parameter `jpegSize` is handig als u wilt garanderen dat een afbeelding een bepaalde grootte niet overschrijdt voor levering aan apparaten met een beperkt geheugen.

* Deze parameter wordt ingesteld in kilobytes ( `jpegSize=<size_in_kilobytes>`). Hiermee wordt de maximaal toegestane grootte voor het leveren van de afbeelding gedefinieerd.
* `&jpegSize=` heeft invloed op de JPG-compressieparameter `&qlt=` . Als de JPG-reactie met de opgegeven JPG-compressieparameter ( `&qlt=` ) de `jpegSize` -waarde niet overschrijdt, wordt de afbeelding geretourneerd met `&qlt=` zoals gedefinieerd. Anders wordt `&qlt=` geleidelijk verkleind totdat de afbeelding past in de maximaal toegestane grootte. Of, totdat het systeem bepaalt dat het niet past en een fout retourneert.

U kunt het beste `&jpegSize=` instellen en de parameter `&qlt=` toevoegen als u JPG-afbeeldingen levert aan apparaten met beperkt geheugen.

## Overzicht van best practices {#best-practices-summary}

U kunt het beste een hoge afbeeldingskwaliteit en een kleine bestandsgrootte bereiken door de volgende combinatie van parameters te gebruiken:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Deze combinatie van instellingen levert in de meeste gevallen uitstekende resultaten op.

Als de afbeelding verder moet worden geoptimaliseerd, kunt u de parameters voor verscherpen (onscherp maskeren) geleidelijk perfectioneren door te beginnen met een straal die is ingesteld op 0,2 of 0,3. Vervolgens verhoogt u geleidelijk het bedrag van 1,75 tot maximaal 4 (400% in Photoshop). Controleer of het gewenste resultaat is bereikt.

Als de verscherpingsresultaten nog steeds niet bevredigend zijn, vergroot u de straal in decimale stappen. Voor elke decimale toename start u de hoeveelheid opnieuw op bij 1,75 en verhoogt u deze geleidelijk tot 4. Herhaal dit proces totdat u het gewenste resultaat hebt bereikt. Terwijl de waarden hierboven een benadering zijn die creatieve studio&#39;s hebben bevestigd, herinner me dat u met andere waarden kunt beginnen en andere strategieën kunt volgen. Of de resultaten voor u bevredigend zijn of niet is een subjectieve kwestie, daarom is gestructureerde experimenten van essentieel belang.

Tijdens het experimenteren zijn de volgende algemene suggesties nuttig om uw workflow te optimaliseren:

* Probeer verschillende parameters in real-time uit en test ze rechtstreeks op een URL of met gebruik van de Adobe Dynamic Media Classic-functionaliteit voor het aanpassen van afbeeldingen. De laatste biedt real-time voorvertoningen voor aanpassingstransacties.
* Houd er rekening mee dat u de opdrachten Dynamisch mediabeeld dat dienen in een voorinstelling voor afbeeldingen kunt groeperen. Een voorinstelling voor afbeeldingen bestaat in feite uit URL-opdrachtmacro&#39;s met aangepaste namen voor voorinstellingen, zoals `$thumb_low$` en `&product_high$` . De naam van de aangepaste voorinstelling in een URL-pad roept deze voorinstellingen aan. Met deze functionaliteit kunt u opdrachten en kwaliteitsinstellingen voor verschillende gebruikspatronen van afbeeldingen op uw website beheren en de totale lengte van URL&#39;s verkorten.
* Adobe Dynamic Media Classic biedt ook geavanceerdere manieren om de afbeeldingskwaliteit af te stemmen, zoals het toepassen van verscherping bij opname van afbeeldingen. Voor geavanceerd gebruik waarbij het verder afstemmen en optimaliseren van gerenderde resultaten een optie is, kan Adobe Professional Services u helpen met aangepaste insight en aanbevolen procedures.
