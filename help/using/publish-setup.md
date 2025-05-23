---
title: Publicatie-instelling
description: Met de instellingen voor Publicatie-instellingen kunt u bepalen hoe elementen standaard worden geleverd vanaf Adobe Dynamic Media Classic-servers naar websites of toepassingen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '2318'
ht-degree: 0%

---

# Publicatie-instelling {#publish-setup}

De pagina-instellingen voor Publicatie-instellingen bepalen hoe elementen standaard worden geleverd vanaf Adobe Dynamic Media Classic-servers naar websites of toepassingen. Als er geen instelling is opgegeven, levert de Adobe Dynamic Media Classic-server een element op basis van een standaardinstelling op een pagina Publicatie-instelling. Als u bijvoorbeeld een verzoek indient om een afbeelding te leveren die geen resolutiekenmerk bevat, wordt een afbeelding weergegeven met de standaardinstelling Objectresolutie op de pagina Afbeeldingsserver.

Beheerders kunnen de standaardinstellingen op de pagina&#39;s Afbeeldingsserver, Afbeeldingsrenderer en Vignet wijzigen om standaardinstellingen voor het leveren van elementen van servers in te stellen.

Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]**.

>[!NOTE]
>
>De pagina&#39;s van de Publish Opstelling zijn voor gebruik door ervaren ontwikkelaars en programmeurs van de Website. Adobe Dynamic Media Classic gaat ervan uit dat gebruikers die de instellingen op deze pagina&#39;s wijzigen, bekend zijn met Adobe Dynamic Media Classic, de normen en conventies voor HTTP-protocollen en de basistechnologie voor beeldbewerking.

## Afbeeldingsserver {#image-server}

De pagina van de Server van het Beeld vestigt standaardmontages voor het leveren van beelden van de Servers van het Beeld. De montages zijn beschikbaar in deze vijf categorieën (zie de pagina van de Server van het Beeld zelf voor gedetailleerde beschrijvingen van de montages).

Wijzig deze instellingen alleen met hulp van een Adobe Dynamic Media Classic-medewerker.

* **[!UICONTROL Catalog Management]**: Deze instellingen bepalen de interactie tussen Adobe Dynamic Media Classic en de catalogus. In tegenstelling tot de meeste servers van het Web, gaan de vraag van de Server URL van het Beeld van Dynamic Media naar manifest-of catalogusdossier eerder dan een beelddossier juist. Het catalogusbestand (dat niet moet worden verward met een eCatalog) bevat een lijst met alle inhoud die naar de afbeeldingsserver is gepubliceerd. Het bevat ook het pad naar elke afbeelding. Als u een Digimarc-id hebt, voert u uw gebruikersgegevens in het gedeelte Digimarc-gebruikersinfo in.

* **[!UICONTROL Request Attributes]**: Met deze instellingen worden limieten ingesteld voor afbeeldingen die van de server kunnen worden geleverd. Bijvoorbeeld de *maximum* **[!UICONTROL Reply Image Size Limit]** is **[!UICONTROL Width]** 5000 en **[!UICONTROL Height]** 5000.

* **[!UICONTROL Default Request Attributes]**: Deze instellingen hebben betrekking op de standaardweergave van afbeeldingen.

* **[!UICONTROL Common Thumbnail Attributes]**: Deze instellingen hebben betrekking op de standaardweergave en -uitlijning van miniatuurafbeeldingen.

* **[!UICONTROL Defaults for Catalog Fields]**: Deze instellingen hebben betrekking op de resolutie en het standaardtype miniatuur van afbeeldingen.

* **[!UICONTROL Color Management Attributes]**: Deze instellingen bepalen welke ICC-kleurprofielen worden gebruikt.

* **[!UICONTROL Compatibility Attributes]**: Met deze instelling kunnen alinea&#39;s met regelafstand en navolgende in tekstlagen op dezelfde manier worden behandeld als in versie 3.6 voor achterwaartse compatibiliteit.

* **[!UICONTROL Localization Support]**: Met deze instellingen kunt u meerdere kenmerken voor de landinstelling beheren. U kunt hiermee ook een landinstellingenkaarttekenreeks opgeven, zodat u kunt definiëren welke talen u wilt ondersteunen voor de verschillende knopinfo in Viewers.

  Als u bijvoorbeeld een nationaal merk bent dat in verschillende landen verkoopt, kunt u ervoor zorgen dat elk land zijn eigen landspecifieke viewer heeft. U kunt deze functionaliteit uitvoeren door een tekenreeks voor de landinstellingenkaart op te geven. Vervolgens bewerkt u de knopinfo-tekst in de voorinstelling van een viewer. Voeg gewoon de vertaalde tekstreeksen toe voor de gewenste taal.

  >[!NOTE]
  > Voor het instellen van opties voor Localization Support [gebruik de Admin Console om een steungeval tot stand te brengen.](https://helpx.adobe.com/nl/enterprise/using/support-for-experience-cloud.html) In uw steungeval, verzoek opstelling hulp.

  Meer informatie over het instellen van **[!UICONTROL Localization Support]**, zie [Overwegingen bij het instellen van lokalisatie van middelen](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Overwegingen bij het instellen van lokalisatie van middelen {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Als u Localization Support-opties wilt instellen in Adobe Dynamic Media Classic, zoals het veld Locale Map, [gebruik de Admin Console om een steungeval tot stand te brengen.](https://helpx.adobe.com/nl/enterprise/using/support-for-experience-cloud.html) In uw steungeval, verzoek opstelling hulp.

Een algemene manier om Adobe Dynamic Media Classic te gebruiken is het beheren van productafbeeldingen op e-Commerce-websites. Internationale bedrijven staan voor de uitdaging dat activa voor soortgelijke producten er van land tot land anders uitzien. Meestal zijn de verschillen voor een paar delen van de totale media. Het aanpakken van dergelijke verschillen door alle activa voor elk van de landen te kopiëren en alleen de verschillen te overschrijven is een enorme inspanning en is in tegenspraak met de enkele primaire metaforen. Dergelijke verschillen voor activa kunnen, van landspecifieke video&#39;s met verschillende audiosporen, aan subtiele maar belangrijke verschillen in een machtskoord blijven dat met het product wordt gebruikt. Adobe Dynamic Media Classic gebruikt een basisopzoekmechanisme. U bepaalt een orde van activa achtervoegsels waarin de Server van het Beeld kijkt, beginnend bij de vereiste scène.

#### Hoe middelen worden gelokaliseerd

De landinstelling voor een IS-verzoek (Image Serving) wordt aangeduid met de volgende IS/IR-opdracht (Image Rendering):

`locale=`

Deze opdracht accepteert een landinstellings-id (locId)-tekenreeks die niet hoofdlettergevoelig is. De landinstellings-id is doorgaans een tekenreeks van 2-6 tekens die bestaat uit letters en &quot;`_`.&quot;

IS ondersteunt willekeurige afdrukbare ASCII-tekenreeksen. De `locale=` bevel heeft een globaal werkingsgebied, betekenend dat het op het volledige verzoek, met inbegrip van alle genestelde IS en verzoeken van AIR, referenced malplaatjes, en beeldlagen wordt toegepast. Meerdere landinstellingen per aanvraag, zoals een andere landinstelling voor elke laag, worden niet ondersteund. Het is echter denkbaar om expliciete overschrijvingen toe te staan in geneste verzoeken.

Indien `locale=` niet is opgegeven, `attribute::DefaultLocale` wordt doorgegeven aan de vertaalmachines. Beperkte invoervalidering wordt toegepast op de `locale=` waarde. Leeg `locale=` waarden zijn toegestaan. Omdat `locale=` een mondiaal toepassingsgebied heeft, `attribute::DefaultLocale` wordt verstrekt door de belangrijkste catalogus voor het volledige verzoek.

Enkele voordelen van het gebruik van `locale=` en `attribute::DefaultLocale` het volgende opnemen:

* Inhoud delen voor meerdere landinstellingen.
* Toegang tot inhoud die specifiek is voor de landinstelling met behulp van generieke id&#39;s.
* Biedt flexibiliteit bij naamconventies en het beheer van landspecifieke inhoud, zoals het voorvoegsel van de landinstelling en het achtervoegsel, of taalspecifieke inhoud in een aparte catalogus.
* Ondersteuning voor toegang tot landspecifieke versies.
* Samengevoegde objecten, zoals Afbeeldingssets, kunnen soms algemene verwijzingen naar mogelijk landspecifieke inhoud bevatten.
* Ondersteunt alle inhoud die wordt beheerd door catalogi die lokalisatie nodig hebben, inclusief afbeeldingen, afbeeldingssets, vignetten, materialen en viewerconfiguratierecords.
* Minimaliseer veranderingen in het IPS gegevensbestand en IS duidelijke mechanismen.
* De steun voor statische inhoud zoals video&#39;s en huiden wordt toegevoegd wanneer RFC IS-63 wordt uitgevoerd.
* De standaardlandinstelling kan worden geconfigureerd.

#### Toepassingsscenario&#39;s

| Toepassing | Scenario |
| --- | --- |
| Lokalisatie van viewer | Nadat de statische inhoudcatalogi worden uitgevoerd, wordt de localisatie gecontroleerd volledig met locale= parameter, die aan alle verzoeken wordt toegevoegd die aan IS worden gemaakt. Configuratierecords, skins, welkomstschermen, enzovoort, kunnen landspecifieke varianten hebben of niet. De correcte inhoud wordt verstrekt door IS zonder de kijker die moet weten welke inhoud wordt gelokaliseerd en wat zijn IDs is. |
| Afbeeldingen en video | Meerdere nationale bedrijven hebben vaak een combinatie van generieke en landspecifieke inhoud. Met dit mechanisme kan een verwijzing naar een beeld of een video algemeen zijn, en IS dient omhoog de landspecifieke inhoud als het beschikbaar is. |
| Afbeeldingssets en mediasets | De volledige afbeeldingsset kan voor sommige landinstellingen anders zijn, bijvoorbeeld wanneer een eCatalog anders is, waarbij de vertaling van een generieke naar een landspecifieke afbeeldingsset wordt verwerkt door de viewer. Meer algemeen, kunnen individuele IDs in een generische reeks naar inhoud verwijzen die gelokaliseerd is. De meeste foto&#39;s van een apparaat kunnen bijvoorbeeld in alle talen hetzelfde zijn, behalve de foto van het Configuratiescherm. IS automatisch id&#39;s vertalen, zodat er geen landspecifieke afbeeldingssets hoeven te worden gegenereerd. |

#### Middelen lokaliseren

Adobe Dynamic Media Classic en Image Serving beschikken over een interface waarmee u afbeeldingen en statische inhoud kunt lokaliseren.

Zonder lokalisatie ziet een URL voor een afbeeldingsserver er als volgt uit:

`https://server/is/image/company/image`

Met lokalisatie voegt een URL van een afbeeldingsserver de `locale=` parameter voor het pad, zoals hieronder:

`https://server/is/image/company/image?locale=de_DE`

Na ontvangst van de http-aanroep door de Image Server wordt de `locale=` parameter wordt geparseerd door de `localeMap` veld gevonden in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]** groep.

Het veld Landinstelling kaart bevat een lijst met items die zijn gescheiden met het verticale balksymbool (|).

Elk item bestaat uit een door komma&#39;s gescheiden lijst met waarden. De eerste waarde is de zoekwaarde die wordt doorgegeven via het dialoogvenster `locale=` parameter. De resterende waarden zijn achtervoegsels/vervangingswaarden die vervolgens worden geprobeerd totdat er een bestaande afbeelding ontstaat.

Of een achtervoegselwaarde of een vervangingswaarde wordt toegepast, is afhankelijk van de instelling voor de algemene landinstelling in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]** groep.

>[!NOTE]
>
>De instelling Globale landinstelling is alleen mogelijk wanneer u deze instelt via de API, niet binnen de Adobe Dynamic Media Classic-interface.

**Voorbeeld van achtervoegsel:**

| URL | localeMap-id&#39;s | Resultaat | Notities |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Er is geen GlobalLocale gedefinieerd. De parameter de_DE voor landinstellingen komt overeen met het eerste item in het dialoogvenster `localeMap`. De eerste overeenkomstige waarde _DE wordt toegevoegd als achtervoegsel aan activa image_DE en een poging wordt gemaakt om het op de Server van het Beeld te vinden. Als deze op de server wordt gevonden, wordt deze geretourneerd. Anders wordt de tweede waarde &quot;&quot; gebruikt als achtervoegsel, waardoor de afbeelding zelf wordt geretourneerd. |

**Voorbeeld van vervanging:**

| URL | `GlobalLocale` en `localeMap` ID&#39;s | Resultaat | Notities |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | In het bovenstaande vervangingsvoorbeeld is GlobalLocale ingesteld op main. De parameter de_DE voor landinstellingen komt overeen met het eerste item in het dialoogvenster `localeMap`. De subtekenreeks van GlobalLocale wordt gevonden en vervangen door de eerste overeenkomende waarde `de` in de `localeMap`: `image-de-01`. Indien gevonden op de Server van het Beeld, is het teruggekeerd. Zo niet, dan wordt de tweede waarde vervangen, wat resulteert in `image-main-01`. |

Als er geen landinstelling is gedefinieerd in de URL, gebruikt de afbeeldingsserver de DefaultLocale (indien deze is gedefinieerd) en past deze toe op de URL.

Als een onbekende of lege landinstellingsparameter wordt geleverd bij `locale=`en vervolgens de `localeMap` wordt gescand voor de lege waarde &quot;begint met.&quot; Het is belangrijk dat een standaardlandinstelling wordt toegepast voor onbekende landinstellingen.

#### Over defaultImage

De server van het Beeld probeert de opties voor de gevraagde scène, één na andere. Als er geen overeenkomst wordt gevonden, worden de landinstellingsopties toegepast op defaultImage en wordt de overeenkomende versie geretourneerd. Daarom moet elke landinstelling een optie voor de afbeelding zonder lokalisatie bevatten of moeten gelokaliseerde standaardafbeeldingsversies beschikbaar worden gesteld in Adobe Dynamic Media Classic.

#### Scenario&#39;s voor het zoeken van de localeMap

Stel dat u de volgende landinstellingen wilt ondersteunen:

`en, en_us, en_uk, de, de_at, de_de, fr`

U wijst deze landinstellingen toe aan de achtervoegsels `_E` (Engels), `_G` (Duits), en `_F` (Frans). Voor alle voorbeelden is de algemene id van de invoerafbeelding: `myImg`.

##### Standaardgedrag voor het zoeken naar de localeMap

De landinstellings-id&#39;s worden toegewezen aan de corresponderende achtervoegsels. Als er geen landinstellings-specifieke id wordt gevonden in de catalogus, wordt de generieke id geprobeerd. Noteer de lege locSuffix-waarden die aan de generieke id zijn toegewezen.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | Id&#39;s uitvoeren om te zoeken |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alle andere | : |

##### De localeMap zoeken wanneer de landinstelling onbekend is

U kunt onbekende landinstellingen toewijzen aan specifieke id&#39;s of aan generieke id&#39;s. U kunt bijvoorbeeld onbekende landinstellingen toewijzen aan de Engelse id&#39;s, of als deze niet bestaan, aan de algemene id&#39;s.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | Id&#39;s uitvoeren om te zoeken |
| --- | --- |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alle andere | myImg_E, myImg |

U kunt ook een toegewezen locSuffix, zoals U, gebruiken, alleen voor onbekende landinstellingen en de standaardafbeelding forceren als dit niet het geval is `_U` bestaat, zoals in het volgende voorbeeld:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Of u kunt rechtstreeks een toewijzing maken aan de algemene id, zoals in het volgende voorbeeld:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### De localeMap zoeken met behulp van een meerlaagse zoekopdracht

Het is vaak wenselijk om landinstellingen, zoals Europees, Midden-Oosten en Noord-Amerika, te groeperen om regionale normen, zoals huidblootstelling, aan te pakken. U kunt dit effect bereiken met een zoekopdracht met meerdere lagen.

Stel dat u verzamelingen wilt ondersteunen voor gebruik in het Westen en het Midden-Oosten. Beide verzamelingen zijn gebaseerd op de algemene afbeeldingsverzameling en voegen of wijzigen enkele afbeeldingen toe. Beide verzamelingen worden vervolgens verder verfijnd voor specifieke landinstellingen. Bijvoorbeeld: `m1, m2` voor twee varianten in het midden-oosten, en `w1, w2,` en `w3` voor drie westerse landinstellingen, behalve dat afbeeldingen worden gedeeld voor `w1` en `w3`. Onbekende landinstellingen worden alleen toegewezen aan de algemene verzameling en hebben geen toegang tot landspecifieke afbeeldingen. De kaart ziet er als volgt uit:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | Id&#39;s uitvoeren om te zoeken |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Alle andere | mylmg |

##### LocaleMap zoeken door te zoeken naar specifieke id&#39;s

Sommige naamgevingsconventies voor afbeeldingen ondersteunen geen algemene afbeeldings-id&#39;s. De generieke id&#39;s van het verzoek moeten worden toegewezen aan een specifieke id in de catalogus. Er zijn echter gevallen waarin de exacte specifieke id niet bekend is.

Wanneer het eerste voorbeeld als basis wordt gebruikt, kunnen afbeeldingen voor alle talen achtervoegsels hebben `_1`, `_2`, of `_3`. Afbeeldingen die specifiek zijn voor Franse landinstellingen, kunnen de achtervoegsels hebben `_22` of `_23` achtervoegsel. En afbeeldingen die specifiek zijn voor Duitse landinstellingen kunnen de achtervoegsels hebben `_470` of `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Id&#39;s uitvoeren om te zoeken |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2, myImg_3 |
| Alle andere | myImg_1, myImg_2, myImg_3 |

##### Belangrijke overwegingen bij het implementeren van lokalisatieondersteuning

* De lokalisatie is beperkt tot op identiteitskaart-Gebaseerde activa vraag en kan niet op op weg-gebaseerde activa vraag worden gebruikt. Wanneer u video&#39;s met een landinstelling aanroept, moet deze daarom worden aangeroepen als bedrijf/assetID; geen volledig pad naar de video. U kunt niet `RTMP` met lokalisatie omdat die methode alleen voor op paden gebaseerde videoaanroepen kan worden gebruikt.
* U kunt geen Gemengde Reeks van Media gebruiken die één enkele video bevat wanneer localeMap actief is, anders ontbreekt de vraag aan de inhoud van de reeks. U kunt dit probleem omzeilen door één video toe te voegen aan een adaptieve videoset. Voeg vervolgens de adaptieve videoret toe aan een gemengde mediaset.
* Bepaalde verzoeken zijn niet gelokaliseerd, zoals aanvragen voor de inhoud van een adaptieve videoret. Als u Adaptieve videosets dus wilt gebruiken met lokalisatie, plaatst u de adaptieve videoset in een gemengde mediaset. Vervolgens roept u de set aan in een gemengde mediasviewer met de `locale=` parameter.

## Renderer afbeelding {#image-renderer}

De pagina Renderer van het Beeld vestigt standaardmontages voor het leveren van de Reeksen van het Beeld van beeld-teruggevende servers. De montages zijn beschikbaar in deze vijf categorieën (zie de pagina van de Server van het Beeld zelf voor gedetailleerde beschrijvingen van de montages):

* **[!UICONTROL Catalog Management]**: Deze instellingen bepalen de interactie tussen Adobe Dynamic Media Classic en het catalogusbestand. Adobe Dynamic Media Classic Render Server URL-aanroepen worden uitgevoerd naar de catalogus, die op zijn beurt aanroepen om afbeeldingen van de server te leveren. Wijzig deze instellingen alleen met hulp van een Adobe Dynamic Media Classic-medewerker.

* **[!UICONTROL Session Attributes]**: Met deze instellingen worden foutparameters, de URL voor relatieve afbeeldings-URL&#39;s en of objectoverlapping is toegestaan.

* **[!UICONTROL Default Material Attributes]**: Met deze instellingen worden de standaardresolutie en verscherpingsinstellingen voor afbeeldingen ingesteld.

* **[!UICONTROL Response Image Attributes]**: Deze instellingen hebben betrekking op de standaardweergave van afbeeldingen.

* **[!UICONTROL Color Management Attributes]**: Deze instellingen hebben betrekking op de standaardkleurinstellingen van afbeeldingen.

## Vignet {#vignette}

De pagina Vignet biedt instellingen voor de standaardweergave van vignetten (zie de pagina zelf voor gedetailleerde beschrijvingen van opties).
