---
title: Publicatie-instelling
seo-title: Publicatie-instelling
description: 'null'
seo-description: De het schermmontages van de Publish Opstelling bepalen hoe de activa door gebrek van Dynamische servers van Media Classic aan websites of toepassingen worden geleverd.
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: df88ca77d3f9c40c59d796e6854942b93cef5729
workflow-type: tm+mt
source-wordcount: '2415'
ht-degree: 0%

---


# Publicatie-instelling {#publish-setup}

De het schermmontages van de Publish Opstelling bepalen hoe de activa door gebrek van Dynamische servers van Media Classic aan websites of toepassingen worden geleverd. Als er geen instelling is opgegeven, levert de Dynamic Media Classic-server een element volgens de standaardinstelling op een scherm Publish Setup. Bijvoorbeeld, een verzoek om een beeld te leveren dat geen resolutieattribuut omvat produceert een beeld met de StandaardResolutie die van Objecten op het scherm van de Server van het Beeld plaatsen.

Beheerders kunnen de standaardinstellingen wijzigen op de schermen Afbeeldingsserver, Afbeeldingsrenderer en Vignet om standaardinstellingen voor het leveren van elementen van servers in te stellen.

Als u de schermen Publicatie-instelling wilt openen, klikt u op Instellen > Toepassingsinstelling > Publicatie-instelling.

>[!NOTE]
>
>De schermen Publiceren van de Opstelling zijn voor gebruik door ervaren websiteontwikkelaars en programmeurs. Dynamic Media Classic gaat ervan uit dat gebruikers die instellingen op deze schermen wijzigen bekend zijn met Dynamic Media Classic, HTTP-protocolstandaarden en -conventies en de basistechnologie voor beeldbewerking.

## Afbeeldingsserver {#image-server}

Het scherm van de Server van het Beeld vestigt standaardmontages voor het leveren van beelden van beeldservers. De montages zijn beschikbaar in deze vijf categorieën (zie het scherm van de Server van het Beeld zelf voor gedetailleerde beschrijvingen van de montages).

Wijzig deze instellingen alleen met behulp van een persoon die Dynamic Media Classic ondersteunt.

**Catalogusbeheer** Deze instellingen bepalen hoe Dynamic Media Classic en de catalogus werken. In tegenstelling tot de meeste webservers gaan de URL-aanroepen van Dynamic Media Image Server naar een manifest- of catalogusbestand in plaats van naar het eigenlijke afbeeldingsbestand. Het catalogusbestand (dat niet moet worden verward met een eCatalog) bevat een lijst met alle inhoud die naar de afbeeldingsserver is gepubliceerd, samen met het pad naar elke afbeelding. Als u een Digimarc-id hebt, voert u uw gebruikersgegevens in het gedeelte Digimarc-gebruikersinfo in.

**Kenmerken** aanvragen Deze instellingen leggen limieten op aan afbeeldingen die van de server kunnen worden geleverd. Het *maximum* is bijvoorbeeld **[!UICONTROL Reply Image Size Limit]** 5000 en **[!UICONTROL Width]** **[!UICONTROL Height]** 5000.

**Standaardaanvraagkenmerken** Deze instellingen hebben betrekking op de standaardweergave van afbeeldingen.

**Algemene miniatuurkenmerken** Deze instellingen hebben betrekking op de standaardweergave en -uitlijning van miniatuurafbeeldingen.

**Standaardwaarden voor catalogusvelden** Deze instellingen hebben betrekking op de resolutie en het standaardminiatuurtype van afbeeldingen.

**Kenmerken** kleurbeheer Deze instellingen bepalen welke ICC-kleurprofielen worden gebruikt.

**Compatibiliteitskenmerken** Met deze instelling kunnen alinea&#39;s met regelafstand en navolgende in tekstlagen op dezelfde manier worden behandeld als in versie 3.6 voor achterwaartse compatibiliteit.

**Ondersteuning voor** lokalisatie Met deze instellingen kunt u meerdere locatiekenmerken beheren. U kunt hiermee ook een landinstellingenkaarttekenreeks opgeven, zodat u kunt definiëren welke talen u wilt ondersteunen voor de verschillende knopinfo in Viewers.

Als u bijvoorbeeld een nationaal merk bent dat in verschillende landen verkoopt, kunt u ervoor zorgen dat elk land zijn eigen landspecifieke viewer heeft. Voor deze functionaliteit geeft u een tekenreeks voor de landinstellingenkaart op. Vervolgens bewerkt u de knopinfo-tekst in de voorinstelling van een viewer door de vertaalde tekstreeksen toe te voegen voor de gewenste taal.

>[!NOTE]
> Als u Localization Support-opties wilt instellen, [gebruikt u de Admin Console om een ondersteuningscase te maken.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) In uw steungeval, verzoek opstelling hulp.

Zie **Overwegingen bij het instellen van lokalisatie van middelen** voor meer informatie over het instellen van [lokalisatieondersteuning](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Overwegingen bij het instellen van lokalisatie van middelen {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Als u Localization Support-opties wilt instellen in Dynamic Media Classic, zoals het veld Locale Map, [gebruikt u de Admin Console om een draagtas te maken.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) In uw steungeval, verzoek opstelling hulp.

Een algemene manier om Dynamic Media Classic te gebruiken, is het beheren van productafbeeldingen op websites voor e-handel. Internationale bedrijven staan voor de uitdaging dat activa voor soortgelijke producten er van land tot land anders uitzien. Doorgaans zijn de verschillen slechts voor een zeer klein deel van de media. Het aanpakken van dergelijke verschillen door alle activa voor elk van de landen te kopiëren en alleen de verschillen te overschrijven is een enorme inspanning en is in tegenspraak met de enkele master metaforen. Dergelijke verschillen voor activa kunnen, van landspecifieke video&#39;s met verschillende audiosporen, aan subtiele maar belangrijke verschillen in een machtskoord blijven dat met het product wordt gebruikt. De dynamische Klassieke Media gebruikt een basisraadplegingsmechanisme. U bepaalt een orde van activa achtervoegsels waarin de Server van het Beeld kijkt, beginnend bij de vereiste scène.

**Hoe middelen worden gelokaliseerd**

De landinstelling voor een IS-verzoek (Image Serving) wordt aangeduid met de volgende IS/IR-opdracht (Image Rendering):

`locale=`

Deze opdracht accepteert een tekenreeks met landinstellings-id (locId) die niet hoofdlettergevoelig is. De landinstellings-id is doorgaans een tekenreeks van 2-6 tekens die bestaat uit letters en &quot;_&quot;.

IS steunt willekeurige bedrukbare ASCII koorden.Het `locale=` bevel heeft een globaal werkingsgebied, betekenend dat het op het volledige verzoek, met inbegrip van alle genestelde verzoeken IS en AIR, referenced malplaatjes, en beeldlagen wordt toegepast. Meerdere landinstellingen per aanvraag, zoals een andere landinstelling voor elke laag, worden niet ondersteund. Het is echter denkbaar om expliciete overschrijvingen toe te staan in geneste verzoeken.

Indien `locale=` niet gespecificeerd, `attribute::DefaultLocale` wordt overgegaan tot de vertaalmotoren. Beperkte invoervalidatie wordt toegepast op de `locale=` waarde. Lege `locale=` waarden zijn toegestaan. Omdat `locale=` een globaal bereik heeft, wordt `attribute::DefaultLocale` dit verschaft door de hoofdcatalogus voor het gehele verzoek.

Enkele voordelen van het gebruik `locale=` en `attribute::DefaultLocale` omvatten het volgende:

* Inhoud delen voor meerdere landinstellingen.
* Toegang tot inhoud die specifiek is voor de landinstelling met behulp van generieke id&#39;s.
* Biedt flexibiliteit bij naamconventies en het beheer van landspecifieke inhoud, zoals het voorvoegsel van de landinstelling en het achtervoegsel, of taalspecifieke inhoud in een aparte catalogus.
* Rechtstreekse toegang tot landspecifieke versies ondersteunen.
* Samengevoegde objecten, zoals afbeeldingssets, kunnen algemene verwijzingen bevatten naar mogelijk landspecifieke inhoud.
* Ondersteunt alle inhoud die wordt beheerd door catalogi waarvoor lokalisatie nodig kan zijn, inclusief afbeeldingen, afbeeldingssets, vignetten, materialen en viewerconfiguratiegegevens.
* Minimaliseer veranderingen in het IPS gegevensbestand en IS duidelijke mechanismen.
* De steun voor statische inhoud zoals video&#39;s en huiden zal worden toegevoegd wanneer RFC IS-63 wordt uitgevoerd.
* De standaardlandinstelling kan worden geconfigureerd.

**Toepassingsscenario&#39;s**

| Toepassing | Scenario |
|--- |--- |
| Lokalisatie van viewers | Nadat de statische inhoudcatalogi worden uitgevoerd, wordt de localisatie gecontroleerd volledig met locale= parameter, die aan alle verzoeken wordt toegevoegd die aan IS worden gemaakt. Configuratierecords, skins, welkomstschermen, enzovoort, kunnen landspecifieke varianten hebben of niet. De correcte inhoud wordt verstrekt door IS zonder de kijker die moet weten welke inhoud wordt gelokaliseerd en wat zijn IDs is. |
| Afbeeldingen en video | Meerdere nationale bedrijven hebben vaak een combinatie van generieke en landspecifieke inhoud. Met dit mechanisme kan een verwijzing naar een beeld of een video algemeen zijn, en IS dient omhoog de landspecifieke inhoud als het beschikbaar is. |
| Afbeeldingssets en mediasets | De volledige afbeeldingsset kan voor sommige landinstellingen anders zijn, bijvoorbeeld wanneer een eCatalog volledig anders is, waarbij de vertaling van een generieke naar een landspecifieke afbeeldingsset die door de viewer wordt verwerkt. Meer algemeen kunnen afzonderlijke id&#39;s in een generieke set verwijzen naar gelokaliseerde inhoud. De meeste foto&#39;s van een apparaat kunnen bijvoorbeeld in alle talen hetzelfde zijn, behalve de foto van het bedieningspaneel. Deze id&#39;s worden automatisch vertaald. Het is dus niet nodig landspecifieke afbeeldingssets te genereren. |

**Locatie van middelen implementeren**

Dynamic Media Classic en Image Serving beschikken over een interface waarmee u afbeeldingen en statische inhoud kunt lokaliseren.

Zonder lokalisatie ziet een URL voor een afbeeldingsserver er als volgt uit:

`https://server/is/image/company/image`

Met localisatie voegt een URL van de Server van het Beeld de `locale=` parameter aan de weg, zoals in het volgende toe:

`https://server/is/image/company/image?locale=de_DE`

Na ontvangst van de http-aanroep door de Image Server wordt de `locale=` parameter geparseerd via het localeMap-veld in **Setup** > **Application Setup** > **Publish Setup** > **Image Server** > **** Localization Supportgroup.

Het veld Landinstelling kaart bevat een lijst met items die zijn gescheiden met het verticale balksymbool (|).

Elk item bestaat uit een door komma&#39;s gescheiden lijst met waarden. De eerste waarde is de zoekwaarde die door de `locale=` parameter wordt doorgegeven. De resterende waarden zijn achtervoegsels/vervangingswaarden die vervolgens worden geprobeerd totdat een bestaande afbeelding wordt weergegeven.

Of een achtervoegselwaarde of een vervangingswaarde wordt toegepast hangt van de Globale scène af die in **Opstelling** > de Opstelling **van de** Toepassing > **Publish Opstelling** > de Server **van het** Beeld > de **Groep van de Steun** van de Lokalisatie plaatst.

>[!NOTE]
>
>De instelling Globale landinstelling is momenteel alleen mogelijk wanneer u deze instelt via de API, niet binnen de Klassieke interface van dynamische media.

**Voorbeeld van achtervoegsel**

| URL | localeMap-id&#39;s | Resultaat |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Er is geen GlobalLocale gedefinieerd. De parameter de_DE voor landinstellingen komt overeen met de eerste vermelding in de localeMap. De eerste overeenkomstige waarde _DE wordt toegevoegd als achtervoegsel aan activa image_DE en een poging wordt gemaakt om het op de Server van het Beeld te vinden. Als deze op de server wordt gevonden, wordt deze geretourneerd. Anders wordt de tweede waarde &quot;&quot; gebruikt als achtervoegsel, waardoor de afbeelding zelf wordt geretourneerd. |

**Voorbeeld van vervanging**

| URL | GlobalLocale- en localeMap-id&#39;s | Resultaat |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | In het bovenstaande vervangingsvoorbeeld is GlobalLocale ingesteld op main. De parameter de_DE voor landinstellingen komt overeen met de eerste vermelding in de localeMap. De subtekenreeks van GlobalLocale wordt gevonden en vervangen door de eerste corresponderende waarde de in de localeMap: image-de-01. Als het op de Server van het Beeld wordt gevonden, is het teruggekeerd. Als dat niet het geval is, wordt de tweede waarde vervangen, wat resulteert in image-main-01. |

Als er geen landinstelling is gedefinieerd in de URL, gebruikt de afbeeldingsserver de DefaultLocale (indien deze is gedefinieerd) en past deze toe op de URL.

Als een onbekende of lege landinstellingsparameter wordt meegeleverd `locale=`, wordt de localeMap gescand voor de lege waarde &quot;beginnend met,&quot;. Het is belangrijk om dit te vormen zodat een standaardlandinstelling wordt toegepast voor onbekende landinstellingen.

**De standaardafbeelding**

De server van het Beeld probeert de opties voor de gevraagde scène, één na andere. Als er geen overeenkomst wordt gevonden, worden de landinstellingsopties toegepast op de defaultImage en wordt de overeenkomende versie geretourneerd. Daarom moet elke landinstelling een optie voor de afbeelding zonder lokalisatie bevatten, of moeten gelokaliseerde standaardafbeeldingsversies beschikbaar worden gemaakt in Dynamic Media Classic.

**Scenario&#39;s voor het zoeken van de localeMap**

Stel dat u de volgende landinstellingen wilt ondersteunen:

`en, en_us, en_uk, de, de_at, de_de, fr`

U wijst deze landinstellingen toe aan de achtervoegsels `_E`, `_G`en `_F`, voor Engels, Duits en Frans. Voor alle voorbeelden is de algemene id van de invoerafbeelding `myImg`.

*Standaardgedrag voor het zoeken naar de localeMap*

De landinstellings-id&#39;s worden toegewezen aan de corresponderende achtervoegsels. Als er geen landinstellings-specifieke id wordt gevonden in de catalogus, wordt de generieke id geprobeerd. Neem nota van de lege locSuffix waarden die aan generische identiteitskaart in kaart brengen

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | Uitvoer-id&#39;s waarnaar moet worden gezocht |
|--- |--- |
| en,en_us, en_uk | myImg_E, myImg |
| de,de_de,de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alle andere | - |

*De localeMap zoeken wanneer de landinstelling onbekend is*

U kunt onbekende landinstellingen toewijzen aan specifieke id&#39;s of aan generieke id&#39;s. Bij ons voorbeeld kunt u onbekende landinstellingen toewijzen aan de Engelse id&#39;s, of als deze niet bestaan, aan de generieke id&#39;s.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | Uitvoer-id&#39;s waarnaar moet worden gezocht |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Alle andere | myImg_E,myImg |

U zou ook een toegewezen locSuffix, zoals U, voor onbekende scènes kunnen hebben, en macht aan het standaardbeeld als geen `_U` bestaat, zoals in het volgende:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Of u kunt rechtstreeks een toewijzing maken aan de algemene id, zoals in het volgende voorbeeld:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*LocaleMap zoeken met behulp van een meerlaagse zoekopdracht*

Het is vaak wenselijk om landinstellingen, zoals Europees, Midden-Oosten en Noord-Amerika, te groeperen om regionale normen, zoals huidblootstelling, aan te pakken. U kunt dit effect bereiken met een zoekopdracht met meerdere lagen.

Stel dat u in dit voorbeeld verzamelingen wilt ondersteunen voor gebruik in het Westen en het Midden-Oosten. Beide verzamelingen zijn gebaseerd op de algemene afbeeldingsverzameling en voegen of wijzigen enkele afbeeldingen toe. Beide verzamelingen worden vervolgens verder verfijnd voor specifieke landinstellingen, zoals `m1, m2` voor twee varianten in het midden-oosten, en `w1, w2,` en `w3` voor drie westerse landinstellingen, behalve dat afbeeldingen worden gedeeld voor `w1` en `w3`. Onbekende landinstellingen worden alleen toegewezen aan de algemene verzameling en hebben geen toegang tot landspecifieke afbeeldingen. De kaart ziet er als volgt uit:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | Uitvoer-id&#39;s waarnaar moet worden gezocht |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Alle andere | mylmg |

*LocaleMap zoeken door te zoeken naar specifieke id&#39;s*

Sommige naamgevingsconventies voor afbeeldingen ondersteunen mogelijk geen algemene afbeeldings-id&#39;s. De generieke id&#39;s van het verzoek moeten worden toegewezen aan een specifieke id in de catalogus. Er kunnen zich echter gevallen voordoen waarin de exacte specifieke id niet bekend is.

Wanneer u het eerste voorbeeld als basis gebruikt, kunnen afbeeldingen voor alle talen achtervoegsels hebben `_1`, `_2`of `_3`. Afbeeldingen die specifiek zijn voor Franse landinstellingen, kunnen de achtervoegsels `_22` of het `_23` achtervoegsel hebben. En afbeeldingen die specifiek zijn voor Duitse landinstellingen kunnen achtervoegsels hebben `_470` of `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Uitvoer-id&#39;s waarnaar moet worden gezocht |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2, myImg_3 |
| Alle andere | myImg_1, myImg_2, myImg_3 |

**Belangrijke overwegingen bij het implementeren van lokalisatieondersteuning**

* De lokalisatie is beperkt tot op identiteitskaart-Gebaseerde activa vraag en kan niet op op weg-gebaseerde activa vraag worden gebruikt. Daarom wanneer het roepen van video&#39;s met scène, moet het als bedrijf/assetID worden geroepen; geen volledig pad naar de video. Dit betekent dat u geen rtmp met localisatie kunt gebruiken omdat die methode voor gebruik met weg-gebaseerde videovraag slechts is.
* U kunt geen Gemengde Reeks van Media gebruiken die één enkele video bevat wanneer localeMap actief is, anders ontbreekt de vraag aan de inhoud van de reeks. Als u dit probleem wilt verhelpen, kunt u één video toevoegen aan een adaptieve videoset. Voeg vervolgens de adaptieve videoret toe aan een gemengde mediaset.
* Bepaalde verzoeken zijn niet gelokaliseerd, zoals aanvragen voor de inhoud van een adaptieve videoret. Daarom als u van plan bent om de Aangepaste VideoReeksen met localisatie te gebruiken, zou u de Aangepaste VideoReeks binnen een Gemengde Reeks van Media moeten plaatsen. Dan, roep de reeks in een Gemengde kijker van Media met de `locale=` parameter.

## Renderer afbeelding {#image-renderer}

In het scherm Renderer afbeelding worden standaardinstellingen vastgelegd voor het leveren van afbeeldingssets op servers voor het renderen van afbeeldingen. De montages zijn beschikbaar in deze vijf categorieën (zie het scherm van de Server van het Beeld zelf voor gedetailleerde beschrijvingen van de montages):

**Catalogusbeheer** Deze instellingen bepalen hoe Dynamic Media Classic en het catalogusbestand communiceren. Dynamische media Klassieke de vraag van de Server URL van de Render wordt gemaakt aan de catalogus, die beurtelings roept om beelden van de server te leveren. Wijzig deze instellingen alleen met behulp van een persoon die Dynamic Media Classic ondersteunt.

**Sessiekenmerken** Deze instellingen stellen foutparameters, de URL voor relatieve afbeeldings-URL&#39;s en of objectoverlapping is toegestaan.

**Standaardmateriaalkenmerken** Deze instellingen stellen de standaardresolutie en verscherpingsinstellingen voor afbeeldingen in.

**Attributen** van reactieafbeelding Deze instellingen hebben betrekking op de standaardweergave van afbeeldingen.

**Kenmerken** kleurbeheer Deze instellingen hebben betrekking op de standaardkleurinstellingen van afbeeldingen.

## Vignet {#vignette}

Het scherm Vignet biedt instellingen om de standaardweergave van vignetten te bepalen (zie het scherm zelf voor gedetailleerde beschrijvingen van opties).
