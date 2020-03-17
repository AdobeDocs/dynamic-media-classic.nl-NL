---
title: Opties voor het bewerken van afbeeldingen tijdens het uploaden
seo-title: Opties voor het bewerken van afbeeldingen tijdens het uploaden
description: 'null'
seo-description: Meer informatie over de opties voor het bewerken van afbeeldingen die beschikbaar zijn op het moment van het uploaden.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
translation-type: tm+mt
source-git-commit: 917ba4469b5ef22e62c572f80008e470dccdebe4

---


# Opties voor het bewerken van afbeeldingen tijdens het uploaden{#image-editing-options-at-upload}

Wanneer u afbeeldingsbestanden uploadt, waaronder AI-, EPS- en PSD-bestanden, kunt u de volgende bewerkingen uitvoeren in het dialoogvenster Taakopties uploaden:

* Witruimte uitsnijden vanaf de rand van afbeeldingen.
* Handmatig uitsnijden vanaf de zijkanten van afbeeldingen.
* Kies een kleurprofiel.
* Maak een masker op basis van een uitknippad.
* Afbeeldingen verscherpen met onscherpe maskeropties
* Achtergrond uitnemen

Deze opties bevinden zich op het uploadscherm onder Opties voor het bewerken van afbeeldingen.

**Witruimte uitsnijden in afbeeldingen**

Als u pixels met witruimte automatisch wilt uitsnijden in een afbeelding, selecteert u het menu Uitsnijden en kiest u Bijsnijden. Kies vervolgens de volgende opties:

* **Wegsnijden op basis van** Kies of u wilt uitsnijden op basis van kleur of transparantie:

* **De optie Kleur** kiezen. Selecteer vervolgens in de vervolgkeuzelijst Hoek de hoek van de afbeelding met de kleur die het beste overeenkomt met de kleur voor de witruimte die u wilt uitsnijden.

* **Transparantie** Kies de optie Transparantie.

* **Tolerantie** Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven:

* **Bijsnijden op basis van kleur** Geef 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de afbeelding hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

* **Bijsnijden op basis van transparantie** Geef 0 op om alleen pixels bij te snijden als deze volledig transparant zijn; De cijfers dichter aan 1 staan voor meer transparantie.

**Handmatig uitsnijden vanaf de zijkanten van afbeeldingen**

Als u handmatig wilt uitsnijden aan weerszijden van een afbeelding, selecteert u het menu Uitsnijden en kiest u Handmatig. Voer vervolgens het aantal pixels in dat u aan elke zijde van de afbeelding wilt uitsnijden. Hoeveel van de afbeelding wordt uitgesneden, is afhankelijk van de ppi-instelling (pixels per inch) in het afbeeldingsbestand. Als de afbeelding bijvoorbeeld 150 ppi weergeeft en u 75 invoert in de tekstvakken Boven, Rechts, Onder en Links, wordt aan beide zijden een halve inch bijgesneden.

**Een kleurprofiel kiezen**

Kies een optie bij Kleurprofiel om een kleurruimte voor de afbeelding te selecteren:

* **Omzetten in sRGB** Omzetten in sRGB (standaard rood-groen blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

* **De oorspronkelijke kleurruimte** behouden

* **Kies Aangepast van > naar** om de menu&#39;s te openen, zodat u de optie Omzetten van en Omzetten in kleurruimte kunt kiezen. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar SPS hebt geüpload.

Zie [ICC-profielen](icc-profiles.md#icc_profiles).

**Maskers maken op basis van een uitknippad**

Selecteer Masker **maken van uitknippad** om een masker voor de afbeelding te maken op basis van de gegevens van het uitknippad. Deze optie is van toepassing op afbeeldingen die zijn gemaakt met beeldbewerkingstoepassingen waarin een uitknippad is gemaakt.

**Een afbeelding verscherpen met Masker verscherpen**

Met dit filter kunt u een verscherpingsfiltereffect op de uiteindelijke gedownsampelde afbeelding perfectioneren en zo de intensiteit van het effect, de straal van het effect (gemeten in pixels) en een drempel voor contrast instellen die wordt genegeerd.

Voor dit effect worden dezelfde opties gebruikt als voor het filter Onscherp masker van Photoshop. In tegenstelling tot wat de naam suggereert, is Onscherp masker een verscherpingsfilter.

Stel onder Onscherp masker de gewenste opties in. De instellingsopties worden in de volgende tabel beschreven:

| Onscherpe maskeropties | Beschrijving |
|--- |--- |
| Hoeveelheid | Hiermee bepaalt u de hoeveelheid contrast die wordt toegepast op de randpixels.<br><br>Beschouw het als de intensiteit van het effect. Het belangrijkste verschil tussen de waarden voor Onscherp masker in SPS en de waarden voor de hoeveelheid in Adobe Photoshop is dat Photoshop een bereik van 1% tot 500% heeft. In SPS is het waardebereik 0,0 tot 5,0. Een waarde van 5,0 in SPS is het ruwe equivalent van 500% in Photoshop; een waarde van 0,9 komt overeen met 90% enzovoort. |
| Straal | Hiermee bepaalt u de straal van het effect. <br><br>Het waardebereik is 0-250. Het effect wordt op alle pixels in een afbeelding uitgevoerd en wordt vanuit alle pixels in alle richtingen uitgestraald. De straal wordt gemeten in pixels. Als u bijvoorbeeld een vergelijkbaar verscherpingseffect wilt toepassen op een afbeelding van 2000 x 2000 pixels en een afbeelding van 500 x 500 pixels, stelt u een straal in van twee pixels op de afbeelding van 2000 x 2000 pixels en een straalwaarde van één pixel op de afbeelding van 500 x 500 pixels. Een hogere waarde wordt gebruikt voor een afbeelding met meer pixels. |
| Drempel | Drempel is een contrastbereik dat wordt genegeerd wanneer het filter Onscherp masker wordt toegepast. Dit is belangrijk, zodat er geen &#39;ruis&#39; wordt toegevoegd aan een afbeelding wanneer dit filter wordt gebruikt. Het waardebereik is 0-255. Dit is het aantal helderheidsstappen in een grijswaardenafbeelding. 0=zwart, 128=50% grijs en 255=wit.<br><br>Een drempelwaarde van 12 negeert bijvoorbeeld kleine variaties door de helderheid van de huidskleur om ruis te voorkomen, maar voegt toch randcontrast toe aan contrasterende gebieden, zoals waar de wimpers de huid raken.<br><br>Als u bijvoorbeeld een foto van iemands gezicht hebt, heeft het filter Onscherp masker invloed op de contrasterende delen van de afbeelding, zoals waar de wimpers en de huid elkaar raken om een duidelijk contrastgebied te maken en op de zachte huid zelf. Zelfs de meest vloeiende skin vertoont subtiele wijzigingen in helderheidswaarden. Als u geen drempelwaarde gebruikt, accentueert het filter deze subtiele veranderingen in huidpixel. Er wordt op zijn beurt een lawaai en een ongewenst effect gecreëerd terwijl het contrast op de wimpers wordt verhoogd, waardoor de scherpte wordt vergroot.<br><br>Om dit probleem te voorkomen, wordt een drempelwaarde geïntroduceerd die het filter vertelt om pixels te negeren die het contrast niet drastisch wijzigen, zoals een vloeiende skin. <br><br>Let op de structuur naast de ritssluiters in de afbeelding die u eerder hebt weergegeven. Ruis in de afbeelding wordt weergegeven omdat de drempelwaarden te laag waren om de ruis te onderdrukken. |
| Monochroom | Selecteer deze optie om de helderheid (intensiteit) van een afbeelding zonder scherp masker te wijzigen.<br><br>Schakel deze optie uit als u elke kleurcomponent afzonderlijk wilt ontscherpen. |

Zie ook Een afbeelding [](sharpening-image.md#sharpening_an_image)verscherpen.

Zie ook het [Verscherpen van beelden in het Publiceren Scene7 Systeem en op de Server](/help/assets/s7_sharpening_images.pdf)van het Beeld.

**Achtergrond uitnemen**

Met de achtergrond Uitnemen kunt u de achtergrond van een afbeelding automatisch verwijderen wanneer u de afbeelding uploadt. Deze techniek is nuttig om de aandacht op een bepaald voorwerp te vestigen en het van een drukke achtergrond te maken.

| Opties voor Achtergrond uitnemen | Beschrijving |
|:--- |:--- |
| Achtergrond uitnemen | Selecteer deze optie om de functie Achtergrond uitnemen en opties in te schakelen of in te schakelen. |
| Hoek | Vereist.<br><br>De hoek van de afbeelding die wordt gebruikt om de achtergrondkleur voor uitnemen te definiëren.<br><br>U kunt kiezen uit <b>Linksboven, Linksonder, Rechtsboven of Rechtsonder</b>. |
| Vulmethode | Vereist. <br><br>Hiermee regelt u de pixeltransparantie vanaf de locatie Hoek die u instelt.<br><br>U kunt kiezen uit de volgende vulmethoden: <ul><li><b>Vulling</b> overstroming - hiermee worden alle pixels transparant gemaakt die overeenkomen met de hoek die u hebt opgegeven en waarop u een koppeling hebt gemaakt.</li><li><b>Pixel</b> afstemmen - hiermee worden alle overeenkomende pixels transparant gemaakt, ongeacht de locatie van de pixels op de afbeelding.</li></ul> |
| Tolerantie | Optioneel.<br><br>Hiermee bepaalt u de toegestane hoeveelheid variatie in de overeenkomende pixelkleur op basis van de locatie van de hoek die u instelt.<br><br>Gebruik een waarde van 0,0 om de pixelkleuren exact overeen te laten komen of gebruik een waarde van 1,0 voor de grootste variatie. |

>[!MORELIKETHIS]
>
>* [Een afbeelding uitsnijden](cropping-image.md#cropping_an_image)

