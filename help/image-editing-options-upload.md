---
title: Opties voor het bewerken van afbeeldingen tijdens het uploaden
description: Meer informatie over de opties voor het bewerken van afbeeldingen die beschikbaar zijn op het moment van het uploaden.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic, beheer van bedrijfsmiddelen
role: Business Practitioner
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Opties voor het bewerken van afbeeldingen tijdens het uploaden{#image-editing-options-at-upload}

Wanneer u afbeeldingsbestanden uploadt, waaronder AI-, EPS- en PSD-bestanden, kunt u de volgende bewerkingen uitvoeren in het dialoogvenster Taakopties uploaden:

* Witruimte uitsnijden vanaf de rand van afbeeldingen.
* Handmatig uitsnijden vanaf de zijkanten van afbeeldingen.
* Kies een kleurprofiel.
* Maak een masker op basis van een uitknippad.
* Afbeeldingen verscherpen met onscherpe maskeropties
* Achtergrond uitnemen

Deze opties vindt u op de pagina Uploaden onder Opties voor bewerken van afbeeldingen.

## Witruimte uitsnijden in afbeeldingen

Als u pixels met witruimte automatisch wilt uitsnijden in een afbeelding, selecteert u het menu Uitsnijden en kiest u Bijsnijden. Kies vervolgens de volgende opties:

* **Wegsnijden op basis van**  - Kies of u wilt uitsnijden op basis van kleur of transparantie:

* **Kleur**  - Kies de  **[!UICONTROL Color]** optie. Selecteer vervolgens in de vervolgkeuzelijst **[!UICONTROL Corner]** de hoek van de afbeelding met de kleur die het beste overeenkomt met de kleur voor de witruimte die u wilt uitsnijden.

* **Transparantie**  - Kies de optie Transparantie.

* **Tolerantie**  - Sleep de schuifregelaar om een tolerantie tussen 0 en 1 op te geven:

* **Bijsnijden op basis van kleur**  - Geef 0 op om alleen pixels bij te snijden als deze exact overeenkomen met de kleur die u in de hoek van de afbeelding hebt geselecteerd. De aantallen dichter aan 1 staan voor meer kleurenverschil toe.

* **Bijsnijden op basis van transparantie**  - Geef 0 op om pixels alleen uit te snijden als ze transparant zijn. De cijfers dichter aan 1 staan voor meer transparantie.

## Handmatig uitsnijden vanaf de zijkanten van afbeeldingen

Als u handmatig wilt uitsnijden aan weerszijden van een afbeelding, selecteert u het menu Uitsnijden en kiest u Handmatig. Voer vervolgens het aantal pixels in dat u aan elke zijde van de afbeelding wilt uitsnijden. Hoeveel van de afbeelding wordt uitgesneden, is afhankelijk van de ppi-instelling (pixels per inch) in het afbeeldingsbestand. Als de afbeelding bijvoorbeeld 150 ppi weergeeft en u 75 invoert in de tekstvakken Boven, Rechts, Onder en Links, wordt aan beide zijden een halve inch bijgesneden.

## Een kleurprofiel kiezen

Als u een kleurruimte voor de afbeelding wilt selecteren, kiest u een optie voor Kleurprofiel:

* **Omzetten in sRGB**  - Omzetten in sRGB (standaard rood-groen blauw). sRGB is de aanbevolen kleurruimte voor het weergeven van afbeeldingen op webpagina&#39;s.

* **Oorspronkelijke kleurruimte**  behouden - Behoudt de oorspronkelijke kleurruimte.

* **Aangepast van > naar**  - opent menu&#39;s zodat u een Omzetten van en Omzetten in kleurenruimte kunt kiezen. U kunt een standaard Photoshop-kleurruimte kiezen of een kleurruimte die u naar Dynamic Media Classic hebt geüpload.

Zie [ICC-profielen](icc-profiles.md#icc_profiles).

## Maskers maken op basis van een uitknippad

Als u een masker voor de afbeelding wilt maken op basis van de gegevens over het uitknippad, klikt u op **[!UICONTROL Create Mask From Clipping Path]**. Deze optie is van toepassing op afbeeldingen die zijn gemaakt met beeldbewerkingstoepassingen waarin een uitknippad is gemaakt.

## Een afbeelding verscherpen met Masker verscherpen

Met dit filter kunt u een verscherpingsfiltereffect op de uiteindelijke gedownsampelde afbeelding perfectioneren. Hiermee kunt u de intensiteit van het effect, de straal van het effect (gemeten in pixels) en een drempel voor het contrast instellen die wordt genegeerd.

Voor dit effect worden dezelfde opties gebruikt als voor het filter Onscherp masker van Photoshop. In tegenstelling tot wat de naam suggereert, is Onscherp masker een verscherpingsfilter.

Stel onder Onscherp masker de gewenste opties in. De instellingsopties worden in de volgende tabel beschreven:

| Onscherpe maskeropties | Beschrijving |
|--- |--- |
| Hoeveelheid | Hiermee bepaalt u de hoeveelheid contrast die wordt toegepast op de randpixels.<br><br>Beschouw het als de intensiteit van het effect. Het belangrijkste verschil tussen de waarden voor de hoeveelheid Unsharp Mask in Dynamic Media Classic en de waarden voor de hoeveelheid in Adobe Photoshop is dat Photoshop een bereik heeft van 1% tot 500%. In Dynamic Media Classic is het waardebereik 0,0 tot 5,0. Een waarde van 5,0 in Dynamic Media Classic is het ruwe equivalent van 500% in Photoshop; een waarde van 0,9 komt overeen met 90% enzovoort. |
| Straal | Hiermee bepaalt u de straal van het effect. <br><br>Het waardebereik is 0-250. Het effect wordt op alle pixels in een afbeelding uitgevoerd en wordt vanuit alle pixels in alle richtingen uitgestraald. De straal wordt gemeten in pixels. Als u bijvoorbeeld een vergelijkbaar verscherpingseffect wilt toepassen op een afbeelding van 2000 x 2000 pixels en een afbeelding van 500 x 500 pixels, stelt u een straal van twee pixels in voor de afbeelding van 2000 x 2000 pixels. Stel vervolgens een straalwaarde in van 1 pixel in de afbeelding van 500 x 500 pixels. Een hogere waarde wordt gebruikt voor een afbeelding met meer pixels. |
| Drempel | Drempel is een contrastbereik dat wordt genegeerd wanneer het filter Onscherp masker wordt toegepast. Dit effect is belangrijk, zodat er geen &#39;ruis&#39; wordt toegevoegd aan een afbeelding wanneer dit filter wordt gebruikt. Het waardebereik is 0-255. Dit is het aantal helderheidsstappen in een grijswaardenafbeelding. 0=zwart, 128=50% grijs en 255=wit.<br><br>Een drempelwaarde van 12 negeert bijvoorbeeld kleine variaties door de helderheid van de huidskleur om ruis te voorkomen, maar voegt toch randcontrast toe aan contrasterende gebieden, zoals waar de wimpers de huid raken.<br><br>Als u bijvoorbeeld een foto van iemands gezicht hebt, heeft het filter Onscherp masker invloed op de contrasterende gedeelten van de afbeelding. Bijvoorbeeld, waar wimpers en huid samenkomen om een duidelijk gebied van contrast tot stand te brengen, en de vlotte huid zelf. Zelfs de meest vloeiende skin vertoont subtiele wijzigingen in helderheidswaarden. Als u geen drempelwaarde gebruikt, accentueert het filter deze subtiele veranderingen in huidpixel. Er wordt op zijn beurt een lawaai en een ongewenst effect gecreëerd terwijl het contrast op de wimpers wordt verhoogd, waardoor de scherpte wordt vergroot.<br><br>Om dit probleem te voorkomen, wordt een drempelwaarde geïntroduceerd die het filter vertelt om pixels te negeren die het contrast niet drastisch wijzigen, zoals een vloeiende skin. <br><br>Let op de structuur naast de ritssluiters in de afbeelding die u eerder hebt weergegeven. Ruis in de afbeelding wordt weergegeven omdat de drempelwaarden te laag waren om de ruis te onderdrukken. |
| Monochroom | Selecteer deze optie om de helderheid (intensiteit) van een afbeelding zonder scherp masker te wijzigen.<br><br>Schakel deze optie uit als u elke kleurcomponent afzonderlijk wilt ontscherpen. |

Zie ook [Een afbeelding verscherpen](sharpening-image.md#sharpening_an_image).

Zie ook [Afbeeldingen verscherpen in Scene7 Publishing System en op Image Server](/help/assets/s7_sharpening_images.pdf).

## Achtergrond uitnemen

Met de achtergrond Uitnemen kunt u de achtergrond van een afbeelding automatisch verwijderen wanneer u de afbeelding uploadt. Deze techniek is nuttig om de aandacht op een bepaald voorwerp te vestigen en het van een drukke achtergrond te maken.

| Opties voor Achtergrond uitnemen | Beschrijving |
|:--- |:--- |
| Achtergrond uitnemen | Selecteer deze optie om de functie Achtergrond uitnemen en opties in te schakelen of in te schakelen. |
| Hoek | Vereist.<br><br>De hoek van de afbeelding die wordt gebruikt om de achtergrondkleur voor uitnemen te definiëren.<br><br>U kunt kiezen uit  <b>Linksboven, Linksonder, Rechtsboven of Rechtsonder</b>. |
| Vulmethode | Vereist. <br><br>Hiermee regelt u de pixeltransparantie vanaf de locatie Hoek die u instelt.<br><br>U kunt kiezen uit de volgende vulmethoden: <ul><li><b>Flood Fill</b>  - hiermee worden alle pixels transparant gemaakt die overeenkomen met de hoek die u hebt opgegeven en waarop de toepassing is aangesloten.</li><li><b>Pixel</b>  afstemmen: hiermee worden alle overeenkomende pixels transparant gemaakt, ongeacht de locatie van de pixels op de afbeelding.</li></ul> |
| Tolerantie | Optioneel.<br><br>Hiermee bepaalt u de toegestane hoeveelheid variatie in de overeenkomende pixelkleur op basis van de locatie van de hoek die u instelt.<br><br>Gebruik een waarde van 0,0 om de pixelkleuren exact overeen te laten komen of gebruik een waarde van 1,0 voor de grootste variatie. |

>[!MORELIKETHIS]
>
>* [Een afbeelding uitsnijden](cropping-image.md#cropping_an_image)

