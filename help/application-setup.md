---
title: Toepassing instellen
description: Leer hoe u het toepassingsgebied van Dynamic Media Classic instelt.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '10595'
ht-degree: 3%

---

# Toepassing instellen{#application-setup}

U kunt de pagina&#39;s van de Opstelling van de Toepassing gebruiken om algemene montages in te gaan, beeldvoorinstellingen, video het coderen vooraf instelt, kijkersvoorinstellingen, of standaardkijkers, en meta-gegevens te bepalen. U kunt voorinstellingen voor batchsets instellen om ook het genereren van 2D-centrifuges (bijvoorbeeld), publicatie-instellingen en video-SEO-instellingen te automatiseren.

>[!NOTE]
>
>Alleen Klassieke Dynamic Media-beheerders kunnen de instellingen op de pagina&#39;s voor het instellen van toepassingen wijzigen.

## Algemene instellingen {#general-settings}

Klik op **[!UICONTROL Setup > Application Setup > General Settings]** om de pagina Algemene instellingen toepassing te openen op de algemene navigatiebalk.

### Servers

Bij het maken van accounts biedt Dynamic Media Classic automatisch de toegewezen servers voor uw bedrijf. Deze servers worden gebruikt om URL-tekenreeksen voor uw website en toepassingen samen te stellen. Deze URL-aanroepen gelden specifiek voor uw account.

Zie ook [De service Beveiligd testen testen](testing-assets-making-them-public.md#testing_the_secure_testing_service) testen.

* **Gepubliceerde servernaam**  - Deze server is de CDN-server (Live Content Deliver Network) die wordt gebruikt in alle door het systeem gegenereerde URL-aanroepen die specifiek zijn voor uw account. Wijzig deze servernaam alleen als een technicus van Dynamic Media Classic u hiervoor instructies heeft gegeven.

* **Naam**  oorspronkelijke server - Deze server wordt alleen gebruikt voor het testen van de kwaliteit. Wijzig deze servernaam alleen als een Dynamic Media Classic-supporttechnicus hiervoor instructies heeft gegeven.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by a Dynamic Media Classic support technician. -->

* **&amp;Naam**  testserver - uw test&amp;doel-URL, tot en met .com. Zie [!DNL Dynamic Media Classic] integreren met [!DNL Adobe Target Standard/Premium] voor instructies over het verkrijgen van deze URL.

<!-- **Test Publish Context Server Name** -->

* **iOS-streamingservernaam** : de URL naar uw  [!DNL Dynamic Media Classic] iOS-streamingserver. Deze server levert streaming video aan op iOS gebaseerde apparaten gebruikend het protocol van HTTP.

* **Naam**  van progressieve videoserver: de URL naar uw  [!DNL Dynamic Media Classic] progressieve videoserver. Deze server levert progressieve video gebruikend het protocol van HTTP.

* **URL tonen voor niet-gepubliceerde elementen**   [!DNL Dynamic Media Classic]  - Selecteer deze optie als u een URL wilt weergeven wanneer u een voorbeeld van een element weergeeft, ongeacht of het is gepubliceerd of niet. Als het element niet is gepubliceerd, werkt de URL niet. U kunt de URL echter ook gebruiken voor plannings- of organisatorische doeleinden.

<!-- **Allow AIR install** Select this option to allow users to download Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Dynamic Media Classic AIR. Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **CDN-validatiesjabloon**  - Geeft de sjabloon op die wordt gebruikt voor het ongeldig maken van de CDN-cache (Content Delivery Network).

   Stel bijvoorbeeld dat u een URL voor een afbeelding (inclusief voorinstellingen of modifiers voor afbeeldingen) opgeeft die verwijst naar `<ID>`, in plaats van een specifieke afbeeldings-id zoals in het volgende voorbeeld:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Als de sjabloon alleen `<ID>` bevat, vult Dynamic Media Classic `https://<server>/is/image` in, waarbij `<server>` de naam van de publicatieserver is die is gedefinieerd in Algemene instellingen.

   Het plaatsen van CDN maakt Malplaatje ongeldig, die een beeld genoemd Backpack_B selecteert, en dan het klikken **Dossier** > **ongeldig CDN** resulteert in volgende geproduceerde URL in CDN ongeldig maakt interface:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   Klik in de keuzelijst URL op **[!UICONTROL Continue]** om de cache voor die specifieke URL-aanroep van de afbeelding te wissen. U kunt ook URL&#39;s toevoegen door deze in het vak URL-lijst te typen of te plakken; u hoeft de sjabloon niet vooraf in te stellen.

   Nadat u uw Malplaatje van de Invalidatie CDN hebt geselecteerd, en een ongeldig CDN verzoek gemaakt, duikt een indicator op in het gebruikersinterface. Het geeft u een schatting van hoe lang het duurt om het geheime voorgeheugen te ontruimen.

   Als er meerdere afbeeldingen zijn geselecteerd in Dynamic Media Classic wanneer u op **Bestand** > **CDN** ongeldig maken klikt, wordt naar elke afbeelding verwezen in de opgeslagen sjabloon-URL. Daarom kunt u CDN bepalen ongeldig Malplaatje dat van verwijzingen voorziet elke URL die op uw Website (zoals productdetail en onderzoeksresultaten) wordt voorzien. Wanneer u vervolgens een of meer afbeeldingen selecteert om ongeldig te worden gemaakt door het cachegeheugen, vullen de URL&#39;s automatisch de interface in.

   Zie [Inhoud in cache plaatsen](dmc-platform-overview.md#content_caching).

   Zie [Opnieuw gepubliceerde elementen en CDN-vertragingen](publishing-files.md#republished_assets_and_cdn_delays).

### Bladeren

* **Projecten**  tonen - Hiermee bepaalt u of Projecten beschikbaar zijn om uw Klassieke Dynamic Media-middelen te organiseren. Zie Uw werk organiseren met Projecten.

* **Voorbeeldvideo-inhoud**  tonen - De weergave van eVideo-voorbeeldinhoud in- of uitschakelen.

* **Gegenereerde inhoud**  weergeven - In mappen geeft u de inhoud weer die uit een element is gegenereerd. Als een PDF-bestand bijvoorbeeld tijdens het uploaden wordt gerasterd, maakt Dynamic Media Classic één afbeelding voor elke pagina in de oorspronkelijke PDF. Als Gegenereerde inhoud tonen is geselecteerd, wordt elke afbeelding die tijdens het uploaden van de oorspronkelijke PDF is gegenereerd, samen met de PDF weergegeven in de map waarnaar de PDF is geüpload.

* **Gecodeerde video&#39;s**  tonen - Deze optie is standaard uitgeschakeld.

   Als u snel naar video&#39;s in Dynamic Media Classic wilt zoeken en deze wilt zoeken zonder door een groot aantal gecodeerde derivaten van dezelfde video te hoeven navigeren, schakelt u deze optie uit (standaard). Alleen de Master Video-miniatuur, de bronvideo die u hebt geüpload en gebruikt om alle afgeleiden te maken, en de bovenliggende Adaptive Video Set-miniatuur, die alle onderliggende afgeleiden van de gecodeerde videoset bevat, worden weergegeven in de gebruikersinterface.

   U kunt echter wel toegang krijgen tot individuele gecodeerde video&#39;s uit de Master video of de adaptieve videoset. Dubbelklik hiertoe op de miniatuurafbeelding van de video om de gedetailleerde weergave te openen. Klik vervolgens op **[!UICONTROL Encoded Videos]** in het rechterdeelvenster om alle onderliggende video&#39;s te openen.

   U kunt **[!UICONTROL File]** > **[!UICONTROL Reprocess]** ook gebruiken om meer gecodeerde &quot;kindvideo&quot;video&#39;s direct van een Aangepaste VideoReeks tot stand te brengen. Dynamic Media Classic zoekt automatisch de &quot;bovenliggende&quot; Master video van de adaptieve videoset en gebruikt die als de bronvideo voor transcodering. Wanneer u de nieuwe individuele gecodeerde video&#39;s opslaat, worden deze echter niet weergegeven wanneer u doorzoekt of bladert. Ze zijn echter nog steeds toegankelijk via het tabblad Gecodeerde video&#39;s in de gedetailleerde weergave.

   Zie [Video uploaden en transcoderen](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Selecteer **Gecodeerde video&#39;s tonen** om door te gaan met de mogelijkheid om toegang te krijgen tot al uw gecodeerde videomateriaal wanneer u doorbladert.

   Er zijn bepaalde acties in het menu Opbouwen die alleen werken, of optioneel werken, met afzonderlijke video&#39;s. Deze functionaliteit maakt het noodzakelijk om alle gecodeerde videoderivaten te tonen die u kunt selecteren, ongeacht hoe u **Gecodeerde Video&#39;s tonen** plaatst. De acties van de Bouwstijl die de **Show Gecodeerde Video&#39;s** plaatsen met voeten treden omvatten **Aangepaste VideoReeksen**, en **eCatalogs**.

   >[!NOTE]
   >
   >Als u Dynamic Media Classic niet hebt gebruikt om uw video-elementen te uploaden en te coderen, toont Dynamic Media Classic al uw individuele gecodeerde video&#39;s, zelfs als deze optie is uitgeschakeld.

* **Knop**  Submappen vernieuwen tonen - De weergave van de knop Submappen vernieuwen in- of uitschakelen.

### Dynamic Media Classic FTP-account

* **Server**  - Geeft uw FTP-accountserver weer.

* **Gebruikersnaam**  - Hier wordt de gebruikersnaam van uw FTP-account weergegeven.

### Uploaden naar toepassing

* **Afbeeldingen**  overschrijven - Dynamic Media Classic staat niet toe dat twee bestanden dezelfde naam hebben. De klassieke Dynamic Media-id van elk item (de naam van de afbeelding min de extensie van de bestandsnaam) moet uniek zijn. Vanwege deze regel heeft het dialoogvenster Uploaden een optie Overschrijven. Het exacte effect van deze optie is afhankelijk van de opgegeven optie Afbeeldingen overschrijven. Met deze opties geeft u op hoe vervangende afbeeldingen worden geüpload: of ze de oorspronkelijke afbeeldingen vervangen of dubbele afbeeldingen worden. Dubbele afbeeldingen krijgen de naam &quot;-1&quot;. (De naam van bijvoorbeeld stoel.tif wordt gewijzigd in stoel-1.tif). Deze opties zijn van toepassing op afbeeldingen die naar een andere map zijn geüpload dan het origineel of afbeeldingen met een andere bestandsnaamextensie dan het origineel (zoals JPG, TIF of PNG). (Zie De optie Afbeeldingen overschrijven gebruiken.)

   * **Overschrijven in huidige map, dezelfde naam/extensie**  voor basisafbeelding - Deze optie is de strengste regel voor vervanging. Hiervoor moet u de vervangende afbeelding uploaden naar dezelfde map als het origineel en moet de vervangende afbeelding dezelfde bestandsnaamextensie hebben als het origineel. Als niet aan deze vereisten wordt voldaan, wordt een dubbel gecreeerd.

   * **Overschrijven in de huidige map, dezelfde naam van het basiselement, ongeacht de extensie** . U moet de vervangende afbeelding uploaden naar dezelfde map als het origineel, maar de extensie van de bestandsnaam kan afwijken van het origineel. bijvoorbeeld stoel.tif vervangt stoel.jpg.

   * **Overschrijven in een map, dezelfde naam/extensie**  voor basiselementen - Vereist dat de vervangende afbeelding dezelfde bestandsnaamextensie heeft als de oorspronkelijke afbeelding (bijvoorbeeld stoel.jpg moet stoel.jpg vervangen, niet stoel.tif). U kunt de vervangende afbeelding echter naar een andere map uploaden dan het origineel. De bijgewerkte afbeelding staat in de nieuwe map; kan het bestand niet meer vinden op de oorspronkelijke locatie

   * **Overschrijven in elke map, dezelfde naam van het basiselement ongeacht de extensie**  - Deze optie is de meest inclusieve vervangingsregel. U kunt een vervangende afbeelding uploaden naar een andere map dan het origineel, een bestand met een andere bestandsnaamextensie uploaden en het oorspronkelijke bestand vervangen. Als het oorspronkelijke bestand zich in een andere map bevindt, bevindt de vervangende afbeelding zich in de nieuwe map waarnaar het is geüpload.

* **Publiceren**  behouden - Geeft aan of een vervangende afbeelding die naar Dynamic Media Classic is geüpload de instelling Klaar voor publicatie behoudt van de afbeelding die deze vervangt, of dat de instelling bij het uploaden wordt opgegeven.

* **Standaardkleurprofielen**  - Hiermee geeft u de kleurprofielen op die worden toegepast als onderdeel van de standaardopties voor kleurprofiel wanneer u CMYK-afbeeldingen toevoegt.

* **Standaardopties**  voor uploaden - Hiermee opent u het dialoogvenster Opties voor uploaden. Hier kunt u de standaardopties voor uploaden opgeven. Zie Opties voor uploaden voor informatie over deze opties.

### Afbeeldingskaarteditor, naar toepassing

* **HREF**  - Hiermee definieert u de standaard-URL die wordt gebruikt voor de href-kolom voor afbeeldingstoewijzing. Deze URL is de standaard-URL die u ziet wanneer u Afbeeldingen met hyperlinks maakt.

* **Standaardsjabloon voor afbeelding toewijzen**  - Definieert de standaard JavaScript™ voor de href-sjabloon voor afbeeldingstoewijzing. U kunt hier aangepaste code instellen die wordt uitgevoerd wanneer u op een afbeelding met hyperlinks klikt.

### Overige instellingen, naar toepassing

* **Prullenbak kan waarschuwingen**  opruimen - Elementen in de prullenmand worden automatisch binnen zeven dagen verwijderd. Selecteer &quot;E-mails verzenden voordat de prullenmand automatisch wordt verwijderd&quot; als u wilt dat meldingen worden verzonden naar bedrijfsbeheerders wanneer elementen in de prullenmand vier dagen verwijderd zijn van definitieve verwijdering. Zie De map Prullenbak beheren.

## De optie Afbeeldingen overschrijven gebruiken {#using-the-overwrite-images-option}

In Dynamic Media Classic kunnen twee bestanden niet dezelfde naam hebben. De klassieke Dynamic Media-id van elk item (de naam van de afbeelding min de extensie van de bestandsnaam) moet uniek zijn. Vanwege deze regel bevat het dialoogvenster Uploaden opties voor het overschrijven van afbeeldingen. Het exacte effect van deze optie is afhankelijk van een instelling voor de Classic Internal Settings van elk bedrijf.

Als u eerder afbeeldingen hebt geüpload en vervolgens de originele bestanden hebt gewijzigd (of deze hebt vervangen), bepaalt de gekozen optie Overschrijven hoe de afbeeldingen worden vervangen door Dynamic Media Classic. Er wordt geen informatie over de afbeelding gewijzigd, maar de oude wordt vervangen door de nieuwe afbeelding. Als de map ook afbeeldingen bevat die nog niet in Dynamic Media Classic staan, worden deze afbeeldingen toegevoegd.

Gebruik deze optie als de afbeeldingen die u hebt geüpload op een of andere manier zijn gewijzigd (de afbeelding is gewijzigd), maar de verwijzing naar de afbeelding ongewijzigd blijft. Overschrijven is ook handig bij het uploaden en rippen van Adobe® PDF&#39;s. Als u wilt instellen hoe de afbeelding in Dynamic Media Classic *wordt bijgesneden, past u de ICC-kleurprofielopties in het dialoogvenster Uploaden aan en uploadt u deze opnieuw met de functie Overschrijven.*

De klassieke Dynamic Media-id&#39;s die worden gebruikt om toegang te krijgen tot afbeeldingen van de productieservers, zijn afgeleid van de bestandsnamen van de afbeeldingen. Het gebruik van hoofdletters en kleine letters in de bestandsnaam is belangrijk, zowel voor de vervanging van bestaande bestanden als voor de klassieke Dynamic Media-id&#39;s die worden gebruikt om de afbeelding te openen. Zorg ervoor dat het gebruik van hoofdletters en kleine letters in bestandsnamen correct is voordat u bestanden uploadt naar Dynamic Media Classic. Op deze manier voorkomt u dat klassieke Dynamic Media-id&#39;s die alleen verschillen in hoofdletters en kleine letters voor dezelfde afbeelding.

Als u deze optie uitschakelt, worden alle afbeeldingen met dezelfde bestandsnamen als bestaande afbeeldingen behandeld als duplicaten en worden ze niet toegevoegd.

## Voorinstellingen afbeelding {#image-presets}

Het scherm Voorinstellingen afbeelding is bedoeld voor het maken en bewerken van voorinstellingen afbeelding. Met voorinstellingen voor afbeeldingen kan Dynamic Media Classic afbeeldingen dynamisch leveren in verschillende formaten van dezelfde master afbeelding. Elke voorinstelling voor afbeeldingen vertegenwoordigt een vooraf gedefinieerde verzameling opdrachten voor het vergroten of verkleinen en opmaken van afbeeldingen. Wanneer u een voorinstelling voor afbeeldingen maakt, kiest u een grootte voor het leveren van de afbeelding. U kiest ook opmaakopdrachten, zodat de weergave van de afbeelding wordt geoptimaliseerd wanneer de afbeelding wordt geleverd voor weergave.

Beheerders kunnen voorinstellingen maken voor het exporteren van elementen. Gebruikers kunnen bij het exporteren van afbeeldingen een voorinstelling kiezen. Hiermee worden de afbeeldingen ook opnieuw opgemaakt volgens de specificaties die de beheerder heeft opgegeven.

Als u het scherm Voorinstelling afbeelding wilt openen, klikt u op **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** op de algemene navigatiebalk.

Zie [Slimme beeldverwerking](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Voorinstellingen voor afbeeldingen maken en bewerken {#creating-and-editing-image-presets}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Maak een voorinstelling of begin met een bestaande voorinstelling:

   * **Een voorinstelling**  voor afbeeldingen maken - klik  **[!UICONTROL Add]**.
   * **Een voorinstelling voor afbeeldingen maken op basis van een bestaande voorinstelling** . Selecteer de voorinstelling voor afbeeldingen die het meest lijkt op de voorinstelling die u wilt maken en klik op  **[!UICONTROL Edit]**.

1. Voer op de pagina Voorinstelling toevoegen (of bewerken) een naam in voor de voorinstelling.
1. Stel de gewenste voorinstellingsopties in.

   Zie [Opties voor voorinstellingen afbeelding](application-setup.md#image_preset_options).

1. Klik **[!UICONTROL Save]**, of als u van bestaande vooraf ingesteld begonnen bent, klik **[!UICONTROL Save As]**.
1. Als u een voorvertoning van de voorinstelling met uw eigen afbeelding wilt weergeven, klikt u op **[!UICONTROL Browse]** en selecteert u een afbeelding. Klik op **[!UICONTROL Reset]** om een voorvertoning weer te geven met de standaardafbeelding.

U kunt een Voorinstelling afbeelding bewerken door de naam ervan te selecteren in het scherm Voorinstellingen afbeelding en vervolgens op Bewerken te klikken. Als u een voorinstelling voor afbeeldingen wilt verwijderen, selecteert u deze en klikt u op Verwijderen.

### Voorinstellingsopties voor afbeelding {#image-preset-options}

In het scherm Voorinstelling toevoegen en Voorinstelling bewerken vindt u de volgende opties voor het maken en bewerken van voorinstellingen voor afbeeldingen:

* **Naam**  voorinstelling - Voer een beschrijvende naam in zonder spaties. Als u gebruikers wilt helpen deze voorinstelling voor afbeeldingen te identificeren, neemt u de specificatie voor de afbeeldingsgrootte op in de naam.

* **Breedte en Hoogte**  - Voer in pixels de grootte in waarmee de afbeelding wordt geleverd.

* **Indeling**  - Kies een indeling in het menu. Als u de indeling GIF, JPEG, PDF of TIFF kiest, zijn er meer opties beschikbaar:

   * Kwantiseringsopties GIF-kleur

      * **Type**  - Kies Adaptief (de standaardinstelling), Web of Macintosh. Als u GIF met alfa kiest, is de optie Macintosh niet beschikbaar.

      * **Dithering**  - Kies Onscherp of Uit.

      * **Aantal kleuren**  - Sleep de schuifregelaar om 2-255 in te voeren.

      * **Kleurenlijst**  - Voer een lijst met door komma&#39;s gescheiden waarden in. Voer voor wit, grijs en zwart bijvoorbeeld 000000,888888,ffffffff in.
   * JPEG-opties

      * **Kwaliteit**  - Hiermee bepaalt u het compressieniveau JPEG. Deze instelling is van invloed op zowel de bestandsgrootte als de afbeeldingskwaliteit. De JPEG-kwaliteitsschaal is 1-100.

      * **Downsampling**  van JPG-chrominantie inschakelen - Omdat het oog minder gevoelig is voor hoogfrequente kleurinformatie dan hoogfrequente luminantie, verdelen JPEG-afbeeldingen afbeeldingsgegevens in luminantie en kleurcomponenten. Wanneer een JPEG-afbeelding wordt gecomprimeerd, blijft de luminantiecomponent op volledige resolutie staan, terwijl de kleurcomponenten worden gedownsampled door het gemiddelde te nemen van groepen pixels. Door downsampling wordt het gegevensvolume met de helft of met een derde verminderd, zonder dat dit van invloed is op de waargenomen kwaliteit. Downsampling is niet van toepassing op grijswaardenafbeeldingen. Met deze techniek vermindert u de hoeveelheid compressie die handig is voor afbeeldingen met veel contrast (bijvoorbeeld afbeeldingen met overlappende tekst).
   * Opties voor PDF en TIFF

      * **Compressie**  - Kies een compressiealgoritme.



* **Kleurruimte**  - Kies een kleurruimte.

* **Verscherpen**  - Selecteer de optie Eenvoudig verscherpen inschakelen om een basisfilter voor verscherpen toe te passen op de afbeelding nadat alle schaling heeft plaatsgevonden. Verscherpen kan helpen de vervaging te compenseren die kan optreden wanneer u een afbeelding met een andere grootte weergeeft.

   Zie [Een afbeelding verscherpen](sharpening-image.md#sharpening_an_image) voor meer informatie over verscherpen, modi voor opnieuw berekenen en onscherp maskeren.

* **Modus**  Nieuw voorbeeld - kies een optie voor de modus Nieuw voorbeeld. Met deze opties verscherpt u de afbeelding wanneer deze wordt gedownsampled:

* **B-Lineair** : de snelste methode voor het berekenen van nieuwe monsters; er zijn enkele aliasingartefacten waarneembaar .

* **Bi-Cubic**  - Verhoogt het gebruik van cpu op de Server van het Beeld, maar produceert scherpere beelden met minder merkbare aliasing artefacten.

* **Sharp2**  - kan enigszins scherpere resultaten dan de bi-Cubische optie veroorzaken, maar aan nog hogere kosten cpu op de Server van het Beeld.

* **Drielineair**  - Gebruikt zowel hogere als lagere resoluties, indien beschikbaar; wordt alleen aangeraden als aliasing een probleem is. Met deze methode wordt de JPEG-grootte verminderd als gevolg van gereduceerde gegevens met een hoge frequentie.

* **Onscherp maskeren**  - Kies deze opties om de verscherping af te stemmen:

* **Hoeveelheid**  - Hiermee bepaalt u de hoeveelheid contrast die wordt toegepast op de randpixels. De standaardwaarde is 1.0. Voor afbeeldingen met hoge resolutie kunt u de resolutie verhogen tot 5,0. Beschouw Hoeveelheid als een maat voor de filterintensiteit.

* **Straal**  - Hiermee bepaalt u het aantal pixels rond de randpixels dat invloed heeft op de verscherping. Voer voor afbeeldingen met een hoge resolutie een waarde in tussen 1 en 2. Bij een lage waarde worden alleen de randpixels verscherpt. met een hoge waarde wordt een grotere reeks pixels verscherpt . De juiste waarde is afhankelijk van de grootte van de afbeelding.

* **Drempel**  - Hiermee bepaalt u het contrastbereik dat moet worden genegeerd wanneer het filter Onscherp masker wordt toegepast. Met andere woorden, met deze optie bepaalt u hoe verschillend de verscherpte pixels moeten zijn van het omringende gebied voordat ze als randpixels worden beschouwd en worden verscherpt. Experimenteer met waarden tussen 0,02 en 0,2 om ruis te voorkomen. Met de standaardwaarde 6 worden alle pixels in de afbeelding verscherpt.

* **Kleurruimte**  - Hiermee wordt bepaald of de afbeelding de ruimte gebruikt waarin de afbeelding is gemaakt, meestal RGB (Origineel) of een luminantieruimte (Intensiteit).

* **** KleurKies de volgende opties:

* **Uitvoerkleurprofiel**  - Selecteer Standaard gebruiken of een van de ICC-kleurprofielen die beschikbaar zijn in de Dynamic Media Classic.

   Zie ook [ICC-profielen](icc-profiles.md#icc_profiles).

* **Render-** intentieSelecteer een optie als u de standaard rendering intent van het kleurprofiel wilt overschrijven. Gebruik deze optie als een van de standaard-ICC-profielen de doelkleurruimte van een kleurconversie is, een uitvoerapparaat (printer of monitor) door dit profiel wordt gekarakteriseerd en de opgegeven render-intentie geldig is voor dit profiel.

* **Profiel** insluitenSelecteer deze optie zodat dit profiel wordt gebruikt als u deze afbeelding opent in Adobe® Photoshop®.

* **AfdrukresolutieKies een** resolutie voor het afdrukken van deze afbeelding. 72 pixels is de standaardinstelling.

* **URL-** modifiersAls u liever de URL-modifiers opgeeft die uw voorinstelling voor afbeeldingen definiëren in plaats van de instellingen, voert u hier de modifiers in.

* **Voorbeeldafbeelding** URLList de &quot;raw&quot; URL-tekenreeks die de Dynamic Media Image Server gebruikt om afbeeldingen te leveren met de voorinstelling voor afbeeldingen die u toevoegt of bewerkt. Deze URL-tekenreeks codeert alle indelingsinstellingen die u selecteert in het scherm Voorinstelling toevoegen of Voorinstelling bewerken.

### Een afbeeldingsvoorinstelling bewerken, verwijderen of deactiveren {#editing-removing-or-deactivating-an-image-preset}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Selecteer in het scherm Voorinstellingen afbeelding een voorinstelling in de tabel en voer een van de volgende handelingen uit:

   * Klik op **[!UICONTROL Edit]** en geef nieuwe opties op in het dialoogvenster Voorinstelling bewerken.
   * Klik op **[!UICONTROL Delete]** om de voorinstelling uit de lijst te verwijderen.
   * Schakel het selectievakje **[!UICONTROL Active]** naast de naam van een voorinstelling uit als u deze wilt verwijderen uit de volledige Dynamic Media Classic-gebruikersinterface voor MediaPortal-gebruikers.

## Aangepaste videovoorinstellingen activeren of deactiveren {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic biedt voorinstellingen voor adaptieve videocodering. Het is een master lijst met voorinstellingen die zowel voorinstellingen voor 16:9 adaptieve video als voor 4:3 adaptieve video in één groep verenigt. Deze vooraf gedefinieerde voorinstellingen weerspiegelen de meest gangbare coderingsinstellingen en zijn geoptimaliseerd voor afspelen op mobiele doelapparaten, tablets en desktops.

Alleen coderingsvoorinstellingen voor Adaptieve video worden standaard geactiveerd (ingeschakeld of ingeschakeld). U kunt het desgewenst deactiveren. Inactieve adaptieve videovoorinstellingen worden niet als een selecteerbare optie weergegeven in de sectie eVideo van het dialoogvenster Taakopties uploaden.

Zie [Video&#39;s uploaden en coderen](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Aangepaste videovoorinstellingen activeren of deactiveren:**

1. Klik in de rechterbovenhoek van Dynamic Media Classic op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]**.
1. Schakel op de pagina Voorinstellingen adaptieve video het selectievakje naast de naam van een voorinstelling uit om de voorinstelling te verwijderen uit de lijst EVideo-opties in het dialoogvenster Taakopties uploaden.
1. Klik op **[!UICONTROL Close]**.

## Videovoorinstellingen voor het coderen van videobestanden {#video-presets-for-encoding-video-files}

Als u een coderingsvoorinstelling wilt kiezen, klikt u rechtsonder op de pagina Uploaden op Taakopties. Vouw de eVideo-opties in het dialoogvenster Taakopties uploaden uit en kies de gewenste voorinstellingen voor videocodering.

>[!NOTE]
>
>Met uitzondering van &quot;Adaptieve video&quot;, die standaard is ingeschakeld, kunt u niet alle andere aangepaste video- of videocoderingsvoorinstellingen in het dialoogvenster Opties voor uploaden zien. Dynamic Media Klassieke beheerders bepalen welke voorinstellingen voor videocodering zichtbaar zijn in het dialoogvenster Taakopties uploaden.

* Kies een van de volgende adaptieve videocodering of voorinstellingen voor één codering:

   * **16:9 Adaptieve video**  - Maak video&#39;s met een hoogte-breedteverhouding van 16:9 voor levering aan desktops, mobiele apparaten (iPhone, iPad, Android™) en tablets (iPad, Android™), geoptimaliseerd met de resolutie en bitsnelheid die het best overeenkomen met de verbindingssnelheid van de viewer.

   * **4:3 Adaptieve video**  - Maak video&#39;s met een hoogte-breedteverhouding van 4:3 voor levering aan desktops, mobiele apparaten (iPhone, iPad, Android™) en tablets (iPad, Android™), geoptimaliseerd met de resolutie en bitsnelheid die het best overeenkomen met de verbindingssnelheid van de viewer.

   * **Adaptieve video** : één coderingsvoorinstelling die met een willekeurige hoogte-breedteverhouding werkt om video&#39;s te maken voor levering op mobiele apparaten, tablets en desktops. Geüploade bronvideo&#39;s die met deze voorinstelling zijn gecodeerd, worden ingesteld met een vaste hoogte. De breedte wordt echter automatisch geschaald om de hoogte-breedteverhouding van de video te behouden.

      Deze flexibiliteit van een &#39;Automatisch schalen&#39; is standaard ook beschikbaar wanneer u uw eigen voorinstelling voor aangepaste videocodering maakt.

      Zie [Een voorinstelling voor videocodering toevoegen of bewerken](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **Adaptieve videocodering (16:9 of 4:3)**  - Maak video&#39;s met de hoogte-breedteverhouding 16:9 en 4:3 voor levering aan desktops, mobiele apparaten (iPhone, iPad, Android™) en tablets (iPad, Android™). Alles geoptimaliseerd met de resolutie en bitsnelheid die het beste overeenkomen met de verbindingssnelheid van de viewer.

      Zie [Aangepaste videocodering (16:9 of 4:3) voor videovoorinstellingen](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **Enkele coderingsvoorinstellingen**

      >[!NOTE]
      >
      >Als u video wilt leveren aan iPads, kunt u een voorinstelling voor mobiele codering of een voorinstelling voor tabletcodering kiezen. Tabletvoorinstellingen zijn speciaal ontworpen voor de iPad, meestal met een hogere resolutie en kwaliteit, zodat u kunt profiteren van de grotere schermgrootte en bandbreedteverbinding. Als u videobestanden wilt leveren die zijn gecodeerd met een voorinstelling voor tablets, moet u apparaatdetectiecode opnemen op uw mobiele site of toepassing. Deze code schakelt tussen een iPhone- of iPad-videobeleving, afhankelijk van het afspeelapparaat. Een mobiele voorinstelling kiezen voor het leveren van videobestanden naar de iPad is een eenvoudigere workflow. De reden hiervoor is dat u hetzelfde videobestand kunt gebruiken voor zowel iPhones als iPads. De kwaliteit wordt echter gestandaardiseerd op basis van de lagere resolutie van de iPhone-ervaring.

      * Selecteer Naam of Grootte onder de groep Coderingsvoorinstellingen in de vervolgkeuzelijst Codering sorteren als u voorinstellingen op naam of grootte wilt sorteren.
      * Kies een coderingsvoorinstelling op basis van de resolutiegrootte en de bandbreedte waarmee u de video wilt afspelen.
      * U kunt Adaptieve videocodering en een of meer coderingsvoorinstellingen per video selecteren. U kunt bijvoorbeeld een bestand coderen voor zowel desktop als mobiel in één uploadtaak.

Nadat u op **[!UICONTROL Start Upload]** hebt geklikt, wordt het originele master videobestand geüpload en worden gecodeerde bestanden gegenereerd vanuit het master bestand.

### Voorinstellingsopties voor codering {#about-encoding-preset-options}

De volgende parameters van de coderingsvoorinstellingsopties zijn beschikbaar:

* **Doelverbindingssnelheid**  - De internetverbindingssnelheid van de beoogde eindgebruiker.

* **Achtervoegsel**  van gecodeerd bestand: het achtervoegsel dat voor identificatiedoeleinden aan het gecodeerde videobestand wordt gekoppeld.

* **Videobitsnelheid (gegevenssnelheid)**  - De hoeveelheid gegevens die wordt gecodeerd om één seconde video af te spelen (in kilobits per seconde).

* **Pixelbreedte/-hoogte** : de breedte-afmetingen van de schermafbeelding, in pixels; de hoogte-afmetingen van de schermafbeelding (in pixels).

* **Frame per seconde (fps)**  - Het aantal frames of stilstaande beelden voor elke seconde van de video. In de Verenigde Staten en Japan wordt de meeste video opgenomen bij 29,97 fps. in Europa en Azië (met uitzondering van Japan) wordt de meeste video opgenomen met 25 fps. Film wordt opgenomen bij 24 fps.

* **Audiobitsnelheid** : de hoeveelheid gegevens die is gecodeerd om één seconde audio af te spelen, in kilobits per seconde.

In de volgende tabellen vindt u de aanbevolen werkwijzen voor het selecteren van videovoorinstellingen en de naamgevingsconventies die worden gebruikt om gecodeerde bestanden aan te wijzen.

### Adaptieve video (standaard) {#adaptive-video-default}

Een coderingsvoorinstelling die werkt met een willekeurige hoogte-breedteverhouding, zodat u video&#39;s kunt maken voor levering op mobiele apparaten, tablets en computers. Geüploade bronvideo&#39;s die zijn gecodeerd met deze voorinstelling (de standaardinstelling en de aanbevolen procedure) worden ingesteld op een vaste hoogte terwijl de breedte automatisch wordt geschaald om de hoogte-breedteverhouding van de video te behouden.

**Adaptieve video (standaard)**

|  | Naam/knopinfotekst coderen | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | Fps | Audiobitsnelheid (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Automatisch x 360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | Gelijk aan bron | 64 | Voor mobiele apparaten (iPhone, iPad, Android™) |
| 2 | Automatisch x 480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | Gelijk aan bron | 96 | Voor tablet (iPad, Android™) |
| 1 | Automatische x 720, 2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | Gelijk aan bron | 128 | Voor bureaublad |

### Adaptieve videocodering (16:9 of 4:3), videovoorinstellingen {#adaptive-video-encoding-or-video-presets}

Deze aangepaste videocoderingsvoorinstellingen combineren een reeks afzonderlijke coderingsvoorinstellingen die automatisch voor u worden geselecteerd op basis van de hoogte-breedteverhouding van de video die u hebt geüpload. Als u bijvoorbeeld een 4:3-video uploadt, wordt deze automatisch gecodeerd met alle vijf voorinstellingen van 4:3 die zich in de lijst met master voorinstellingen bevinden in de optie **Adaptieve videocodering (16:9 of 4:3)**.

Zie [Informatie over coderingsvoorinstellingsopties](application-setup.md#about_encoding_preset_options) voor informatie over parameters voor coderingsopties.

**Voorinstellingen voor Adaptieve videocodering (16:9 of 4:3)**

|  | Naam/knopinfotekst coderen | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | Fps | Audiobitsnelheid (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9, 512 x 288, mobiel (iPhone, iPad, Android™), (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 2 | 4:3, 384 x 288 px, mobiel (iPhone, iPad, Android™), (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 1 | 16:9, 512 x 288, mobiel (iPhone, iPad, Android™), (600 Kbps) | 700 | _Mobile_512x288_600K | 800 | 512x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 4 | 4:3, 384 x 288, mobiel (iPhone, iPad, Android™), (600 Kbps) | 700 | _Mobile_384x288_600 | 800 | 384x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 5 | 16:9, 640 x 360, tablet (iPad, Android™), (800 Kbps) | 900 | _iPad_640x360_800K | 800 | 640x360 | Gelijk aan bron | 80 | Normale resolutie, WiFi |
| 6 | 4:3, 640x480, tablet (iPad, Android™), (800 Kbps) | 900 | _iPad_640x480_800K | 800 | 640x480 | Gelijk aan bron | 80 | Normale resolutie, WiFi |
| 7 | 16:9, 768 x 432, tablet (iPad, Android™), (1200 Kbps) | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | Gelijk aan bron | 96 | Hoge resolutie, WiFi |
| 8 | 4:3, 768 x 576, tablet (iPad, Android™), (1200 Kbps) | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | Gelijk aan bron | 96 | Hoge resolutie, WiFi |
| 9 | 16:9, 1280x720, desktop, (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Gelijk aan bron | 128 | High-definition, breedbeeldscherm |
| 10 | 4:3, 1280x960, desktop, (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | Gelijk aan bron | 128 | High-definition |

### Voorinstellingen voor videocodering op bureaublad {#desktop-video-encoding-presets}

Voorinstellingen voor videocodering voor MP4 en OGV op bureaubladcomputers.

Zie [Informatie over de coderingsvoorinstellingsopties](application-setup.md#about_encoding_preset_options) voor informatie over parameters voor coderingsopties.

**H264 Main 3.2 - Audio AAC, MP4-bestandsextensie**

|  | Naam/knopinfotekst coderen | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | Fps | Audiobitsnelheid (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Gelijk aan bron | 64 | Lage breedbeeldresolutie |
| 2 | 16:9, 640 x 360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | Gelijk aan bron | 80 | Gemiddelde breedbeeldresolutie |
| 1 | 16:9, 800 x 450 (1.200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Gelijk aan bron | 128 | High-definition, breedbeeldscherm |
| 5 | 4:3, 320 x 240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | Gelijk aan bron | 64 | Lage resolutie |
| 6 | 4:3, 480 x 360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Gelijk aan bron | 80 | Normale resolutie |
| 7 | 4:3, 640 x 480 (1.200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640x480 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280x960 | Gelijk aan bron | 128 | High-definition |

**OGG Theora Vorbis - OGV-bestandsextensie**

|  | Naam/knopinfotekst coderen | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | Fps | Audiobitsnelheid (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Gelijk aan bron | 64 | Lage breedbeeldresolutie |
| 2 | 16:9, 640 x 360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | Gelijk aan bron | 80 | Gemiddelde breedbeeldresolutie |
| 1 | 16:9, 800 x 450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | Gelijk aan bron | 128 | High-definition, breedbeeldscherm |
| 5 | 4:3, 320 x 240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | Gelijk aan bron | 64 | Lage resolutie |
| 6 | 4:3, 480 x 360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Gelijk aan bron | 80 | Normale resolutie |
| 7 | 4:3, 640x480 (1.200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | Gelijk aan bron | 128 | High-definition |

### Voorinstellingen voor mobiele videocodering {#mobile-video-encoding-presets}

Hetzelfde als bron-fps. Voorinstellingen voor videocodering voor mobiele iPhone-, iPad- en Android™-apparaten.

Zie [Informatie over de coderingsvoorinstellingsopties](application-setup.md#about_encoding_preset_options) voor informatie over parameters voor coderingsopties.

**H264 Baseline 2.1 - Audio AAC, MP4-bestandsextensie**

|  | Naam/knopinfotekst coderen | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videobitsnelheid (Kbps) | Pixelbreedte/-hoogte | Fps | Audiobitsnelheid (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, mobiel (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 2 | 16:9, 512 x 288, mobiel (600 Kbps) | 700 | _Mobile_512x288_600K | 800 | 512x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 1 | 16:9, 512 x 288, mobiel (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Gelijk aan bron | 80 | Normale resolutie, Wi-Fi |
| 4 | 16:9, 512 x 288, mobiel (1000 Kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | Gelijk aan bron | 80 | Hoge resolutie, Wi-Fi |
| 5 | 16:9, 512 x 288, mobiel (1200 Kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | Gelijk aan bron | 96 | Hoge resolutie, Wi-Fi |
| 6 | 4:3, 384 x 288, mobiel (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 7 | 4:3, 384 x 288, mobiel (600 Kbps) | 700 | _Mobile_384x288_600K | 800 | 384x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 8 | 4:3, 448 x 336, mobiel (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Gelijk aan bron | 80 | Normale resolutie, Wi-Fi |
| 9 | 4:3, 448 x 336, mobiel (1000 Kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | Gelijk aan bron | 80 | Hoge resolutie, Wi-Fi |
| 10 | 4:3, 448 x 336, mobiel (1200 Kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | Gelijk aan bron | 96 | Hoge resolutie, Wi-Fi |

## Voorinstellingen viewer {#viewer-presets}

>[!NOTE]
>
>**Flash Viewers End-of-Life Notice**  - Vanaf 31 januari 2017 wordt de Klassieke ondersteuning van Adobe Dynamic Media Classic officieel beëindigd voor het Flash-viewerplatform.

Een *Voorinstelling voor viewer* is een verzameling instellingen die bepalen hoe gebruikers rich-media-elementen weergeven op hun computerschermen en mobiele apparaten. Als beheerder kunt u Viewer-voorinstellingen maken. Er zijn instellingen beschikbaar voor een array met viewerconfiguratieopties. U kunt bijvoorbeeld de weergavegrootte, het zoomgedrag, de kleurenschema&#39;s, de randen en de lettertypen van de viewer wijzigen.

U kunt het beste Dynamic Media Classic HTML5-videoviewers gebruiken. De voorinstellingen die worden gebruikt in HTML5-videoviewers zijn robuuste videospelers. Door de combinatie in één speler van de capaciteit om de playbackcomponenten te ontwerpen gebruikend HTML5 en CSS, ingebedde playback te hebben, en adaptieve en progressieve het stromen te gebruiken afhankelijk van het vermogen van browser, breidt u het bereik van uw rijke media inhoud tot Desktop, tablet, en mobiele gebruikers uit, en verzekert een gestroomlijnde videoervaring.

Zie [Informatie over HTML5 Viewers](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) in de handleiding van de Referentie voor Adobe Viewers.

Zie [Dynamic Media Classic Viewer Preset-compatibiliteitsmatrix](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Zie [Beste werkwijzen: De HTML5 Video-viewer](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) gebruiken.

Afhankelijk van de viewer kunt u communityfuncties toevoegen. De communautaire eigenschappen omvatten een Embed knoop, E-mail knoop, de knoop van de Verbinding, en de knoop van de Plaats van het Bezoek. Met deze knoppen kunnen gebruikers die de viewer gebruiken de viewer delen met anderen of de klassieke Dynamic Media-website openen.

Zie ook [Adobe Viewers Reference Library Examples](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Viewer-ondersteuning voor responsieve webpagina&#39;s {#viewer-support-for-responsive-designed-web-pages}

Verschillende webpagina&#39;s hebben verschillende behoeften. Soms wilt u een webpagina met een koppeling waarmee de HTML5 Viewer wordt geopend in een apart browservenster. In andere gevallen moet de HTML5 Viewer rechtstreeks worden ingesloten op de hostpagina. In het laatste geval heeft de webpagina waarschijnlijk een statische indeling. Of de interface reageert op de toepassing en wordt anders weergegeven op verschillende apparaten of voor verschillende venstergrootten in de browser. Om aan deze behoeften te voldoen, ondersteunen de HTML5 Viewers die bij Dynamic Media Classic worden geleverd zowel statische webpagina&#39;s als responsieve webpagina&#39;s.

Zie [Informatie over responsieve afbeeldingsbibliotheek](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [Responsieve afbeeldingsbibliotheek gebruiken](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api) en [Command reference - Command attributes](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library) voor meer informatie over het insluiten van responsieve viewers op uw webpagina&#39;s.

### Voorinstellingstypen voor viewer {#viewer-preset-types}

Beheerders kunnen de volgende typen voorinstellingen voor viewers maken en aanpassen:

* **eCatalog Viewer** : hiermee simuleert u het lezen van een afgedrukte catalogus. U kunt van pagina naar pagina gaan, in- en uitzoomen op items op een pagina, afbeeldingen met hyperlinks gebruiken om meer informatie over items op de pagina weer te geven of de catalogus doorzoeken. U kunt ook een deelvenster Info opnemen om gedetailleerde informatie weer te geven en een item waaraan een afbeelding is toegewezen als het kaartgebied een geldig kenmerk rollover_key heeft. Als u een deelvenster Info wilt opnemen, geeft u een URL voor de Informatieserver op in het deelvenster Instellingen van het deelvenster Info van het voorinstellingenvenster van de eCatalog Viewer.

* **Staalsetviewer**  - Hiermee geeft u een afbeelding weer in een andere kleur, in een ander materiaal, in een andere structuur, in een andere afwerking of in een andere structuur. Gebruikers klikken op een miniatuur om de variaties in de afbeelding te zien.

* **Gemengde Media Set Viewer**  - Verschillende typen media worden in één viewer weergegeven. U kunt staalsets, centrifuges, afbeeldingen en video&#39;s opnemen. U kunt tabbladen instellen voor verschillende typen inhoud, zoals een tabblad voor afbeeldingssets en een tabblad voor video&#39;s. Video&#39;s die worden afgespeeld via een gemengde mediaset maken gebruik van een standaardvideoviewer met een tijdlijn en videobesturingselementen, zoals Stoppen, Pauzeren, Terugspoelen en Afspelen. Wanneer u een voorinstelling voor een gemengde mediaset maakt, geeft u op welke viewers u wilt gebruiken voor de verschillende typen elementen in de gemengde mediaset. U kunt ook de rasterviewer of de Carousel-viewer gebruiken om een gemengde mediaset weer te geven.

* **Spin Set Viewer**  - Biedt meerdere weergaven van een afbeelding, zodat gebruikers het object kunnen draaien om de verschillende zijden en hoeken te bekijken.

* **Video-viewer** : geeft video&#39;s weer met de resolutieafmetingen van het bronbestand of een aangepaste grootte. Dynamic Media Classic wordt geleverd met veel vooraf gedefinieerde voorinstellingen voor viewers voor het afspelen van video. Als u een beheerder bent, kunt u aangepaste voorinstellingen voor de video-viewer maken. Er zijn meer dan een dozijn verschillende instellingen voor het configureren van de video-viewer. U kunt de grootte, de voor- en achtergrondkleur, video- en audiobesturingselementen, de voortgangsbalk, de skin van de gebruikersinterface, de sociale functies en de Help configureren.

* **Zoomviewers**  - Hier kunt u kiezen uit drie typen zoomviewers:

* **Zoomviewer**  - Hiermee kunnen gebruikers inzoomen op het gebied door erop te klikken. Ze kunnen op besturingselementen klikken om in te zoomen, uit te zoomen en de standaardgrootte van de afbeelding te herstellen.

* **Zoomviewer: Uitvliegen**  - Geeft een tweede afbeelding weer van het ingezoomde gebied naast de oorspronkelijke afbeelding. Er zijn geen besturingselementen om te gebruiken. Gebruikers verplaatsen de selectie over het gebied dat ze willen weergeven.

Houd er bij het bepalen van het totale bandbreedtegebruik voor deze viewer rekening mee dat zowel de hoofdafbeelding als de vervolgafbeelding in de viewer worden weergegeven. De grootte van de vervolgafbeelding wordt bepaald door de grootte van de hoofdafbeelding (breedte en hoogte van werkgebied) en de zoomfactor. Als u wilt voorkomen dat de flyout-bestandsgrootte te groot wordt, brengt u de volgende twee waarden met elkaar in evenwicht: Als u een grote hoofdafbeeldingsgrootte hebt, verlaagt u de waarde voor Zoomfactor. (De breedte en hoogte van de Flyout bepalen de grootte van het wegvliegvenster, maar niet de grootte van het vliegend beeld dat aan de kijker wordt gediend.)

Als de hoofdafbeelding bijvoorbeeld 350 x 350 pixels groot is, met een zoomfactor van 3, is de resulterende uitvliegafbeelding 1050 x 1050 pixels. Als de hoofdafbeeldingsgrootte 300 x 300 pixels is, met een zoomfactor van 4, is de vervolgafbeelding 1200 x 1200 pixels. Afhankelijk van de kwaliteitsinstelling voor JPEG (de aanbevolen instellingen liggen tussen 80 en 90), kunt u de bestandsgrootte aanzienlijk verkleinen. De aanbevolen zoomfactoren zijn 2,5 tot 4, afhankelijk van de grootte van de hoofdafbeelding.

### Dynamic Media Classic Viewer Preset-compatibiliteitsmatrix {#scene-viewer-preset-compatibility-matrix}

**Eindbericht** voor Flash-viewers: Met ingang van 31 januari 2017 is de officiële ondersteuning voor het Flash-viewerplatform door Adobe Dynamic Media Classic beëindigd.

In de volgende tabel worden de momenteel beschikbare Dynamic Media Classic Viewer-voorinstellingen weergegeven. In de tabel wordt ook aangegeven of de viewer compatibel is met mobiele en desktopapparaten en welke technologie voor elke viewer wordt gebruikt.

Zie ook [Adobe Viewers Reference Library Examples](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Voor informatie over ondersteunde webbrowsers en besturingssysteemversies voor Viewers kunt u de Opmerkingen bij de release Viewers bekijken.

Zie [Opmerkingen bij de release Adobe Viewers Reference](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Zoomviewers |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_Donkerder | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Afbeeldingssetviewers |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_donker | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Viewers voor stalensets |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_donker | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog-viewers |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Bevat ondersteuning voor sociale media en zoeken naar catalogi.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Inclusief ondersteuning voor sociale media en zoeken naar catalogi.) | HTML5 | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Weergaven draaien |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_donker | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo-viewers**

Dynamic Media Classic ondersteunt het afspelen van mobiele video voor MP4 H.264-video.

* U kunt de apparaten van BlackBerry® vinden die dit videoformaat bij het volgende steunen: [Ondersteunde video-indelingen op BlackBerry®](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* U kunt ook de volgende Windows®-apparaten vinden die deze video-indeling ondersteunen: [Ondersteunde video-indelingen op Windows® Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet | BlackBerry® Smartphone | Windows®-telefoon |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(biedt ondersteuning voor ondertiteling met gesloten deuren) Zie [Beste werkwijzen: De Universal HTML5 Video Viewer gebruiken.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Inclusief ondersteuning voor ondertiteling en sociale media.) | HTML5 | X | X | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Gemengde mediasetviewers |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_donker | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Ondersteunde matrix voor bewegingen voor mobiele viewers {#supported-mobile-viewers-gestures-matrix}

In de volgende tabel worden de bewegingen van de mobiele viewer weergegeven die worden ondersteund op iOS-, Android™ 2.x- en Android™ 3.x-apparaten.

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Afbeeldingssetviewers |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_donker | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Het scherm Voorinstellingen van viewer {#about-the-viewer-preset-screen}

Maak en beheer Viewer Presets op het scherm Viewer Presets. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** om dit scherm te openen.

Het scherm Voorinstellingen viewer bevat gereedschappen voor de volgende taken:

* **Een voorinstelling**  toevoegen - Klik  **[!UICONTROL Add]** en maak keuzen in het dialoogvenster Voorinstelling viewer toevoegen.

       Zie [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).
   
* **Een voorinstelling**  bewerken - Selecteer een voorinstelling en klik op  **[!UICONTROL Edit]**.

       Zie [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).
   
* **Een voorinstelling**  verwijderen - Selecteer een voorinstelling en klik op  **[!UICONTROL Delete]**.

* **Een voorinstelling**  exporteren - Selecteer een voorinstelling voor een HTML5-viewer en klik  **[!UICONTROL Export]** om de viewerskin te downloaden, zodat u deze kunt gebruiken als basis voor het maken en toevoegen van een andere voorinstelling voor de viewer.

       Zie [Een voorinstelling voor een HTML5-viewer exporteren](application-setup.md#exporting_an_html5_viewer_preset).
   
* **Filteren van de lijst met**  voorinstellingen voor viewer - Gebruik deze gereedschappen om de lijst te filteren:

       * Open de vervolgkeuzelijst **Actief/Inactief** en kies een optie om actieve voorinstellingen, inactieve voorinstellingen of alle voorinstellingen weer te geven.
       * Open de vervolgkeuzelijst **Viewer** en kies een optie om alleen bepaalde viewers weer te geven. Kies **[!UICONTROL All Viewers]** om alle viewers weer te geven.
   
* **Voorinstellingen**  sorteren - Klik op een kolomkop (**[!UICONTROL Active]**,  **[!UICONTROL Type]**,  **[!UICONTROL Preset]** of  **[!UICONTROL Platform]**) om de lijst in een kolom te sorteren. Klik nogmaals op een kolomkop om de lijst in aflopende (of oplopende) volgorde te sorteren.

* **Voorinstellingen**  activeren en deactiveren: selecteer een voorinstelling en klik op de optie Actief om deze te activeren of te deactiveren.

       Zie [Viewer-voorinstellingen activeren of deactiveren](application-setup.md#activating_or_deactivating_viewer_presets).
   
>[!NOTE]
>
>Klik op **[!UICONTROL Preview]** aan de rechterkant van de pagina Voorinstellingen viewer om te zien hoe een element eruitziet in de door u geselecteerde voorinstelling voor viewers. Als u een ander element wilt zien, klikt u op **[!UICONTROL Browse]** op de pagina Voorinstellingen viewer en selecteert u een ander element in het dialoogvenster Voorvertoning van element selecteren.

### Viewer-voorinstellingen toevoegen en bewerken {#adding-and-editing-viewer-presets}

Naast het toevoegen van voorinstellingen voor viewers met **[!UICONTROL Add]** in de gebruikersinterface, kunt u ook **[!UICONTROL Export]** gebruiken om een voorinstelling voor viewers toe te voegen. U exporteert gewoon een bestaande voorinstelling voor een HTML5-viewer en gebruikt deze als basis voor de nieuwe voorinstelling.

Zie [Een HTML5 Viewer-voorinstelling exporteren](application-setup.md#exporting_an_html5_viewer_preset).

**Viewer-voorinstellingen toevoegen en bewerken:**

1. Klik in de rechterbovenhoek van Dynamic Media Classic op **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

   U kunt filteren op de lijst met voorinstellingen. Als u bijvoorbeeld alleen voorinstellingen voor videoviewers wilt weergeven, selecteert u Video-viewer in het vervolgkeuzemenu Viewers op de werkbalk direct boven de tabel.

1. Voeg op de pagina Voorinstellingen viewer de voorinstelling Viewer toe of bewerk deze in het scherm Voorinstellingen viewer.

   * **Toevoegen** - Klik op de werkbalk  **[!UICONTROL Add]**. Kies een platform in het dialoogvenster Voorinstelling viewer toevoegen en kies een type rich-media-element.

          Klik op **[!UICONTROL Save As]** wanneer u klaar bent met het maken van de voorinstelling Viewer.
      
   * **Als u een voorinstelling**  voor de viewer toevoegt, begint u met een bestaande voorinstelling voor de viewer. Selecteer in de tabel een voorinstelling voor de video-viewer en klik op Bewerken op de werkbalk.

          Nadat u de video-viewer opnieuw hebt geconfigureerd, klikt u op **[!UICONTROL Save As]** om de voorinstelling op te slaan onder een andere naam in het tekstveld Naam voorinstelling.
      
   * **Bewerken**  - Selecteer een bestaande voorinstelling voor de viewer en klik op  **[!UICONTROL Edit]**.

1. Voer in het scherm Viewer configureren de naam van de voorinstelling in het veld Naam voorinstelling in of bewerk deze.
1. Stel de overige gewenste opties in.

   >[!NOTE]
   >
   >Klik op **[!UICONTROL Same As Source]** om de grootte van de video-viewer automatisch in te stellen op de resolutiegrootte van de gecodeerde video zelf. Als u deze optie kiest, kunt u de breedte van het werkgebied en de hoogte van het werkgebied niet invoeren. In plaats daarvan komen deze opties uit de video zelf. Als u Gelijk aan Bron kiest, plaats de optie van de Grootte van de Marge om op de huidafmetingen buiten het videoplaybackgebied te wijzen. Deze margegrootte is de pixelhoogte en -breedte van de videobesturingselementen. U kunt de volgende illustratie gebruiken om u te helpen de margegrootten bepalen die u wilt gebruiken.*

   ![Margeconfiguratie van videoviewer](assets/vs_video_viewer_configure_margin.png)

1. Voer een van de volgende handelingen uit:

   * Klik **[!UICONTROL Save As]** als u een Viewer-voorinstelling hebt toegevoegd door te beginnen met een bestaande voorinstelling.
   * Klik op **[!UICONTROL Save]** als u een Viewer-voorinstelling hebt toegevoegd of bewerkt.

### Een voorinstelling voor een HTML5-viewer exporteren {#exporting-an-html-viewer-preset}

U kunt een bestaande HTML5 Viewer-voorinstelling exporteren en gebruiken als basis voor het maken van een HTML5 Viewer-voorinstelling. Deze exportoptie is handig omdat u de viewer niet helemaal opnieuw hoeft te maken. In plaats daarvan exporteert u een voorinstelling die er zo uitziet en zich dicht bij u gedraagt. Vervolgens kunt u deze voorinstelling als uitgangspunt gebruiken om ontwerpaanpassingen aan te brengen.

Alle standaard, out-of-box vooraf ingestelde CSS-bestanden van de viewer in Dynamic Media Classic gebruiken relatieve afbeeldingspaden die verwijzen naar elementen op `Scene7SharedAssets`. Hier volgt bijvoorbeeld een relatief pad naar een afbeeldingselement in een CSS-bestand met een Viewer-voorinstelling op

`Scene7SharedAsset`:  `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Als u echter CSS-bestanden van de viewer op uw eigen site host, moet u deze relatieve paden naar afbeeldingen omzetten door in uw eigen omgeving een expliciet pad naar de afbeeldingsserver te gebruiken. Als u het relatieve pad boven naar een expliciet pad wilt bijwerken, ziet het er als volgt uit: `https://s7d1.scene7.com` is het directe pad naar de afbeeldingsserver: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Een voorinstelling voor een HTML5-viewer exporteren:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Selecteer **[!UICONTROL HTML5]** in de tweede vervolgkeuzelijst links op de werkbalk Voorinstellingen viewer.
1. Selecteer **[!UICONTROL All Viewers]** in de derde vervolgkeuzelijst links.
1. Selecteer de viewervoorinstelling die u als basis voor een nieuwe HTML5 Viewer-voorinstelling wilt gebruiken.
1. Klik op **[!UICONTROL Export]** op de werkbalk.
1. Klik in het dialoogvenster Geselecteerde elementen exporteren op **[!UICONTROL Submit Export]**.

   Na het exporteren krijgt u een CSS-bestand. Download en decomprimeer het bestand.

1. Open het CSS-bestand in een CSS-editor, breng de wijzigingen aan en sla het bestand op.
1. Upload het CSS-bestand naar Dynamic Media Classic.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Publiceer het CSS-bestand naar de Dynamic Media Image Server.

   Zie [Bestanden publiceren](publishing-files.md#publishing_files).

1. Voeg de nieuwe viewervoorinstelling zoals gewoonlijk toe. Selecteer het CSS-bestand van de viewer dat u hebt geüpload.

   Zie [Voorinstellingen voor viewers toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).

### Viewer-voorinstellingen activeren of deactiveren {#activating-or-deactivating-viewer-presets}

Als u een URL wilt maken voor het weergeven van elementen, opent u de vervolgkeuzelijst Voorinstellingen in het dialoogvenster Voorvertoning, selecteert u een voorinstelling voor de viewer en klikt u op URL kopiëren (zie [De URL van een voorinstelling voor de viewer kopiëren](application-setup.md#copying_the_url_of_a_viewer_preset)). Deze lijst met voorinstellingen bevat voorinstellingen voor viewers die beheerders toevoegen en beheren in het scherm Voorinstellingen viewer. Alle actieve voorinstellingen voor de eCatalog-viewer worden bijvoorbeeld weergegeven in de vervolgkeuzelijst Voorinstellingen in het dialoogvenster Voorvertoning wanneer een gebruiker een voorvertoning van een eCatalog weergeeft.

Tenzij u de Viewer-voorinstellingen in het scherm Voorinstellingen viewer deactiveert, kan de vervolgkeuzelijst Voorinstellingen in het dialoogvenster Voorvertoning vol raken.

**Viewer-voorinstellingen activeren of deactiveren:**

1. Kies **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Schakel op de pagina Voorinstellingen viewer de optie **[!UICONTROL Active]** in of uit om Voorinstellingen viewer te activeren of deactiveren.

### De URL van een viewervoorinstelling kopiëren {#copying-the-url-of-a-viewer-preset}

Nadat u een element hebt gepubliceerd, kunt u een URL kopiëren voor het weergeven van het element met de instellingen uit een voorinstelling voor de viewer.

De URL wordt naar het klembord gekopieerd. U kunt deze desgewenst gebruiken in de HTML-code van uw webpagina, mobiel apparaat of toepassing.

**De URL van een voorinstelling voor de viewer kopiëren:**

1. Selecteer het element in het deelvenster Bladeren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik in de URL&#39;s en het deelvenster Code insluiten rechts van de gewenste viewer op **[!UICONTROL Copy URL]**.
   * Klik op **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en klik vervolgens onder de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Klik op **[!UICONTROL Copy URL]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik op **[!UICONTROL List View]**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   Klik op **[!UICONTROL Copy URL]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Klik op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** op dezelfde werkbalk.
   Klik op **[!UICONTROL Copy URL]** onder de kolom Handelingen van de tabel in de Viewer List.

### De insluitcode van een viewervoorinstelling kopiëren {#copying-the-embed-code-of-a-viewer-preset}

Met de functie Code insluiten kunt u de viewercode voor de geselecteerde Viewer-voorinstelling controleren. U kunt de code ook naar het klembord kopiëren, zodat u de code op uw webpagina&#39;s kunt plakken en de viewer kunt implementeren.

Het bewerken van de code is niet toegestaan in het dialoogvenster Code insluiten.

**De insluitcode van een voorinstelling voor de viewer kopiëren:**

1. Selecteer het element in het deelvenster Bladeren van element.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Klik op **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Klik in het deelvenster URL&#39;s aan de rechterkant op **[!UICONTROL Embed Code]**.
   * Klik op **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en klik vervolgens onder de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Klik op **[!UICONTROL Embed Code]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik op **[!UICONTROL List View]**. Selecteer één element in het deelvenster Asset Browse en klik vervolgens rechts van de miniatuurafbeelding op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   Klik op **[!UICONTROL Embed Code]** onder de kolom Handelingen van de tabel in de Viewer List.

   * Klik **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Klik op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** op dezelfde werkbalk.
   Klik op **[!UICONTROL Embed Code]** onder de kolom Handelingen van de tabel in de Viewer List.

1. Klik in het dialoogvenster Code insluiten op **[!UICONTROL Copy to Clipboard]**.
1. Klik op **[!UICONTROL Close]**.

## Standaardviewers configureren {#configuring-default-viewers}

U kunt Standaardviewers gebruiken om de standaardviewer te configureren die aan een element is gekoppeld wanneer u Voorvertoning in Dynamic Media Classic gebruikt. U kunt de standaardvoorbeeldervaring instellen voor de volgende elementtypen:

* Afbeelding
* Video
* SpinSet
* Catalogus
* ImageSet
* SwatchSet
* MediaSet

**Standaardviewers configureren:**

1. Klik in de vervolgkeuzelijst Setup op **[!UICONTROL Application Setup]**.
1. Vouw **[!UICONTROL Application Setup]** > **[!UICONTROL Viewers]** in het venster Setup (Instellingen) in het linkerdeelvenster uit
1. Klik op **[!UICONTROL Default Viewers]**.
1. Selecteer in het venster Standaardviewers in de vervolgkeuzelijst voor elk type element de viewer die u aan de voorvertoning van het element wilt koppelen.
1. Klik in de rechterbenedenhoek van het venster Standaardviewers op **[!UICONTROL Save Settings]**.
1. Klik in de rechterbenedenhoek van het venster Setup op **[!UICONTROL Close]** om terug te keren naar het venster Asset.

## Weergaven metagegevens {#metadata-views}

** Metadatais gestandaardiseerde informatie over een middel. U kunt metagegevens gebruiken om uw workflow te stroomlijnen, uw elementen te ordenen en het zoeken te verbeteren. Dynamic Media Classic biedt ondersteuning voor de IPTC-standaard (International Press Telecommunications Council) en de XMP-standaard (Extensible Metadata Platform). Voordat gebruikers metagegevens over een element weergeven of invoeren in de gedetailleerde weergave, kunnen ze het menu Weergaven metagegevens openen. Van daaruit kunnen ze de set metagegevensvelden kiezen die ze willen bekijken of gebruiken om het element te beschrijven.

Dynamic Media Classic wordt geleverd met vooraf gedefinieerde weergaven van metagegevens en beheerders kunnen hun eigen weergaven van metagegevens maken, zodat gebruikers kunnen kiezen wanneer ze metagegevens invoeren.

### Een metagegevensweergave maken {#creating-a-metadata-view}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Klik op **[!UICONTROL Add]**.
1. Typ een naam voor de weergave in het tekstveld Naam voorinstelling.
1. (Optioneel) Schakel **[!UICONTROL Make Default]** in om van deze weergave de weergave te maken die gebruikers zien wanneer zij het deelvenster Metagegevens openen in de gedetailleerde weergave.
1. (Optioneel) Selecteer **[!UICONTROL Include UDF]** om door de gebruiker gedefinieerde velden op te nemen in de weergave. Door gebruiker gedefinieerde velden staan boven aan het deelvenster Metagegevens in de gedetailleerde weergave.
1. Selecteer de velden die u voor de weergave wilt gebruiken (klik op **[!UICONTROL Select All]** om alle velden te selecteren).
1. Klik op **[!UICONTROL Save]**.

   De geselecteerde categorieën en velden voor de weergave worden weergegeven in het deelvenster Voorbeeld.

### Weergaven van metagegevens beheren {#managing-metadata-views}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Voer een van de volgende handelingen uit:

   * Als u een voorvertoning van een weergave wilt weergeven, selecteert u deze. De velden in de weergave worden weergegeven in het deelvenster Voorvertoning.
   * Als u een weergave wilt bewerken, selecteert u de weergave en klikt u op **[!UICONTROL Edit]**. Schakel vervolgens veldnamen in of uit in het deelvenster Voorvertoning en selecteer of hef de selectie van de optie **[!UICONTROL Include UDF]** op.
   * Als u een weergave wilt verwijderen, selecteert u deze en klikt u op **[!UICONTROL Delete]**.
   * Als u een weergave als standaard wilt instellen, selecteert u deze en klikt u op **[!UICONTROL Make Default]**. De standaardweergave is de weergave die gebruikers zien wanneer zij elementen openen in de gedetailleerde weergave en naar het deelvenster Metagegevens gaan.

## Voorinstellingen metagegevens {#metadata-presets}

Met voorinstellingen voor metagegevens kunnen beheerders metagegevens beheren die aan elementen zijn toegewezen. In de gedetailleerde weergave kan een gebruiker metagegevens over een element invoeren in velden die voor dat doel zijn opgegeven. Een gebruiker kan bijvoorbeeld een naam, copyrightbeschrijving en adres van de eigenaar invoeren. Om ervoor te zorgen dat gebruikers deze informatie correct en volledig invoeren, kunt u Voorinstellingen voor metagegevens maken. Als u een metagegevensvoorinstelling kiest in de gedetailleerde weergave, worden metagegevensvelden gevuld met vooraf gedefinieerde waarden. Zo worden automatisch een naam, copyrightbeschrijving en adres van de eigenaar ingevoerd.

Maak een voorinstelling voor metagegevens voor elke set waarden voor metagegevens die gebruikers automatisch moeten kunnen invoeren in de gedetailleerde weergave om een element te beschrijven.

### Een metagegevensvoorinstelling maken of bewerken {#creating-or-editing-a-metadata-preset}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Voer een van de volgende handelingen uit in het scherm Metagegevensvoorinstellingen:

   * Als u een voorinstelling wilt maken, klikt u op **[!UICONTROL Add]**. Typ in het tekstveld Naam van metagegevenssjabloon een naam voor de voorinstelling en klik vervolgens op **[!UICONTROL Metadata Views]** en kies een weergave in de vervolgkeuzelijst (zie [Weergaven van metagegevens](application-setup.md#metadata_views)).
   * Als u een bestaande voorinstelling wilt bewerken, selecteert u de voorinstelling in de lijst Voorinstellingen metagegevens en klikt u op **[!UICONTROL Edit]**.

1. Vouw de koppen die u in de voorinstelling wilt opnemen uit en voer waarden in in de verschillende velden die u in de voorinstelling wilt opnemen.
1. Klik op **[!UICONTROL Save]**.

   De geselecteerde categorieën en velden voor de voorinstelling worden weergegeven in het deelvenster Voorvertoning.

### Voorinstellingen metagegevens beheren {#managing-metadata-presets}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Voer een van de volgende handelingen uit:

   * Selecteer de voorinstelling die u wilt voorvertonen om een voorvertoning van de voorinstelling weer te geven. De vooraf ingestelde informatie (categorieën en velden) wordt weergegeven in het voorvertoningsscherm.
   * Als u een voorinstelling wilt verwijderen, selecteert u de voorinstelling en klikt u op **[!UICONTROL Delete]**.

## Door gebruiker gedefinieerde velden {#user-defined-fields}

Een beheerder van Media Portal of een Beheerder van het Bedrijf kan douane, user-defined meta-gegevensgebieden tot stand brengen. Met aangepaste velden kunt u elementen ordenen in Dynamic Media Classic. U kunt de velden desgewenst als Actief markeren. Als deze optie is ingeschakeld, worden de namen van deze aangepaste metagegevensvelden weergegeven in het deelvenster Metagegevens in de gedetailleerde weergave. Gebruikers kunnen informatie invoeren in door de gebruiker gedefinieerde metagegevensvelden om elementen te beschrijven. Gebruikers kunnen ook een door de gebruiker gedefinieerd metagegevensveld als criterium gebruiken bij zoekopdrachten.

Een effectief gebruik van door de gebruiker gedefinieerde metagegevensvelden is het vertragen van de activeringstijd van een element voor een specifieke opstart of verkoop. U definieert een veld &quot;activation&quot; op basis van het type *Date*. Vervolgens kunt u met het deelvenster **[!UICONTROL Metadata]** in de gedetailleerde weergave of **[!UICONTROL File]** > **[!UICONTROL Edit Info]** opgeven wanneer het element wordt geactiveerd. Dynamic Media Classic controleert de publicatiestatus van een element en de publicatiegeschiedenis. Als de publicatie niet binnen de activeringstijd valt, wordt de status Niet gepubliceerd weergegeven.

>[!NOTE]
>
>Als u wilt dat door de gebruiker gedefinieerde velden worden weergegeven in het deelvenster Metagegevens in de gedetailleerde weergave, neemt u door de gebruiker gedefinieerde velden op in de weergave Metagegevens. Selecteer in het scherm Weergaven metagegevens de optie Inclusief UDF (door de gebruiker gedefinieerde velden). Zie [Weergaven van metagegevens](application-setup.md#metadata_views) voor meer informatie.

>[!NOTE]
>
>Als u wilt zoeken naar elementen met behulp van aangepaste, door de gebruiker gedefinieerde velden, klikt u op **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** en selecteert u **[!UICONTROL Include UDFs in Search]**. Zie [Persoonlijke installatie](personal-setup.md#personal_setup).

### Een door de gebruiker gedefinieerd metagegevensveld maken {#creating-a-user-defined-metadata-field}

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.
1. Klik op **[!UICONTROL Add]**
1. Stel in het dialoogvenster Aangepast veld de gewenste opties in.

   * **Naam**  - Voer een naam in voor het metagegevensveld.

   * **Type**  - Kies een optie waarmee het type gegevens wordt gedefinieerd dat gebruikers kunnen invoeren in het metagegevensveld:

   * **Tekenreeks**  - Een tekstreeks.

   * **Int**  - Een geheel getal.

   * **Float**  - Een drijvende-kommagetal.

   * **Ja/Nee**  - Een Booleaanse waarde ja/nee.

   * **Datum**  - Een datum. De notatie DD-MM-JJJJ wordt geaccepteerd.

   * **Bestandsnaam** : de naam van een bestand.

   * **Kleur**  - De naam van een kleur.

   * **Dimension**  - De breedte en hoogte van het element.

   * **Niet getypt**  - Voor achterwaartse compatibiliteit. Selecteer deze optie niet.

   * **Standaardwaarde**  - Voer desgewenst de waarde in die gebruikers waarschijnlijk in het veld invoeren. De waarde die u invoert, wordt de standaardwaarde voor het veld dat u maakt.

   * **Kies desgewenst een elementtype als u het metagegevensveld alleen op een bepaald type element wilt toepassen** .

      >[!NOTE]
      >
      >Kies zorgvuldig een optie **[!UICONTROL Applies To]** omdat u de optie **[!UICONTROL Applies To]** niet kunt wijzigen nadat u een door de gebruiker gedefinieerd veld hebt gemaakt. Met Dynamic Media Classic kunt u de naam, het type en de standaardwaarde van een door de gebruiker gedefinieerd veld bewerken, maar niet de instelling **[!UICONTROL Applies To]**. *

1. Klik **[!UICONTROL Save]** wanneer u klaar bent met het creëren van het meta-gegevensgebied.

### Door de gebruiker gedefinieerde velden beheren {#manage-user-defined-fields}

Het scherm Door gebruiker gedefinieerde velden bevat opdrachten voor het beheer van aangepaste, door de gebruiker gedefinieerde metagegevensvelden.

Alleen een beheerder van het Media Portal of een bedrijfsbeheerder kan door de gebruiker gedefinieerde velden beheren.

Als u dit scherm wilt openen, klikt u op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.

* **Een veld**  bewerken - Selecteer het veld en klik op  **[!UICONTROL Edit]**.

* **Een veld**  verwijderen: selecteer het veld en klik op  **[!UICONTROL Delete]**.

* **Veld**  activeren - Klik om de  **[!UICONTROL Active]** optie naast de naam van een veld in of uit te schakelen. Als u in een rol van het bedrijfbeleid bent, wordt deze optie niet getoond. Omdat deze optie met MediaPortal verwant is, moet u (draai) Eigenschappen MediaPortal in Persoonlijke Opstelling tonen selecteren om de activerende gebieden te zien.

## Bestanden optimaliseren {#optimize-files}

Wanneer u bestanden uploadt naar de Dynamic Media Classic, worden deze geoptimaliseerd voor opslag en publicatie. Als het uploadproces wordt onderbroken, kunnen sommige afbeeldingen echter niet worden geoptimaliseerd. In dit geval wordt het bericht &quot;Afbeelding nog niet geoptimaliseerd&quot; weergegeven. U kunt deze bestanden echter optimaliseren als u een beheerder bent.

Dynamic Media Classic doorzoekt uw bestanden en optimaliseert alleen de afbeeldingen die nog niet volledig zijn geoptimaliseerd.

1. Kies **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** en selecteer **[!UICONTROL Optimize Files]**.
1. Voer informatie in voor de optimalisatietaak en klik op **[!UICONTROL Submit]**.

   Als u met meer dan één bedrijf werkt, optimaliseer dossiers die tot verschillende bedrijven afzonderlijk behoren.

## Voorinstellingen batchset {#batch-set-presets}

Met de voorinstellingen voor batchsets kunt u automatisch afbeeldingssets of centrifuges maken terwijl een taak wordt uitgevoerd om elementen te uploaden naar Dynamic Media Classic.

De beheerders van het bedrijf bepalen eerst noemende overeenkomsten voor de activa die zij in een reeks willen groeperen. Vervolgens kunt u een voorinstelling voor een batch-set maken om naar deze afbeeldingen te verwijzen. Elke voorinstelling is een op zichzelf staande verzameling instructies met een unieke naam die definieert hoe de set moet worden samengesteld met afbeeldingen die overeenkomen met de gedefinieerde naamgevingsconventies in het vooraf ingestelde recept.

Alle actieve voorinstellingen voor batchsets voor een bedrijf worden weergegeven in het dialoogvenster Taakoptie uploaden, zodat u kunt opgeven welke voorinstelling u wilt toepassen tijdens elke uploadsessie. Bedrijfsbeheerders zien alle actieve en inactieve voorinstellingen voor batchsets. Wanneer u bestanden uploadt, maakt Dynamic Media Classic automatisch een set met alle bestanden die overeenkomen met de gedefinieerde naamgevingsconventie in de actieve voorinstellingen.

### Standaardnaam {#default-naming}

De bedrijfsbeheerder maakt een standaardnaamgevingsconventie die wordt gebruikt in elk recept voor een voorinstelling voor batchsets. De standaardnaamgevingsconventie die is geselecteerd in de definitie van de voorinstelling voor batch-sets, kan alle code zijn die uw bedrijf nodig heeft om sets voor alle websites in batch te genereren. Er wordt een voorinstelling voor een batch-set gemaakt waarin de standaardnaamgevingsconventie wordt gebruikt die u definieert. U kunt zo veel voorinstellingen Batch-set maken met alternatieve, aangepaste naamconventies die nodig zijn voor een bepaalde set inhoud als er een uitzondering is op de standaardnaamgeving die door het bedrijf is gedefinieerd.

U hoeft geen standaardnaamgevingsconventie in te stellen als u de functie voor voorinstellingen voor batchsets wilt gebruiken. Nochtans, adviseert de beste praktijken van de Adobe dat u een standaardnoemende overeenkomst gebruikt om zo vele elementen van uw noemende overeenkomst te bepalen die u in een reeks wilt groeperen. Zo kunt u het maken van batchsets stroomlijnen.

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**.
1. Selecteer **[!UICONTROL View Form]** of **[!UICONTROL View Code]** om op te geven hoe u informatie over elke asset wilt weergeven en invoeren.

   U kunt het selectievakje **[!UICONTROL View Code]** inschakelen om de waarde van de reguliere expressie naast de formulierselecties weer te geven. U kunt deze waarden invoeren of wijzigen om de elementen van de naamgevingsconventie te definiëren, als de formulierweergave u beperkt om welke reden dan ook. Als uw waarden niet kunnen worden geparseerd in de formulierweergave, worden de formuliervelden inactief.

   >[!NOTE]
   >
   >De-geactiveerde formuliervelden geven geen ongeldige reguliere expressie aan. Er is geen validatie die aangeeft dat de reguliere expressies juist zijn. U zult resultaten van de regelmatige uitdrukking zien u voor elk element na de resultaatlijn bouwt. De volledige reguliere expressie wordt onder aan de pagina weergegeven.

1. Vouw indien nodig elk element uit en voer de naamgevingsconventies in die u wilt gebruiken.
1. Klik zo nodig op **[!UICONTROL Add]** om een andere naamgevingsconventie voor een element toe te voegen. Of klik **[!UICONTROL Remove]** om een noemende overeenkomst voor een element te schrappen.
1. Klik op **[!UICONTROL Save As]** en typ een naam voor de voorinstelling. Of klik **[!UICONTROL Save]** als u een bestaande voorinstelling bewerkt.

U kunt ook Code weergeven gebruiken zonder formuliervelden. In deze weergave maakt u uw definities van de naamgevingsconventie volledig met behulp van reguliere expressies.

Er zijn twee elementen beschikbaar voor definitie, Identieke en Basisnaam. Met deze velden kunt u alle elementen van een naamgevingsconventie definiëren en het gedeelte van de conventie identificeren dat wordt gebruikt voor de naamgeving van de set waarin deze elementen zich bevinden. De individuele noemende overeenkomst van een bedrijf kon één of meerdere lijnen van definitie voor elk van deze elementen gebruiken. U kunt zo vele lijnen voor uw unieke definitie gebruiken en hen groeperen in verschillende elementen, zoals voor HoofdBeeld, het element van de Kleur, het element van de Afwisselende Mening, en het element van het Monster.

### Een voorinstelling voor een batchset maken {#creating-a-batch-set-preset}

Dynamic Media Classic gebruikt voorinstellingen voor batchsets om elementen die veel voorkomende informatie of inhoud bevatten, te ordenen in sets afbeeldingen die worden weergegeven in viewers. De vooraf ingestelde batchrecepten worden automatisch uitgevoerd naast de importtaken voor elementen die u in Dynamic Media Classic plant.

Met Voorinstelling Batchset kunt u voorinstellingen voor batchsets maken, bewerken en beheren. U kunt zoveel voorinstellingen voor batchsets maken als nodig zijn om alle taken voor het opnemen van elementen die u nodig hebt, te kunnen uitvoeren. Er zijn twee vormen van vooraf ingestelde batch-definities: een voor een standaardnaamgevingsconventie die u hebt ingesteld en een conventie voor aangepaste naamgevingsconventies die u direct maakt.

U kunt de methode voor formuliervelden gebruiken om een voorinstelling voor een batchset te definiëren of de methode voor code, waarmee u reguliere expressies kunt gebruiken. Net als bij Standaardnaam kunt u de codeweergave kiezen terwijl u in de formulierweergave definieert en reguliere expressies gebruikt om uw definities samen te stellen. U kunt ook de optie voor het uitsluitend gebruiken van de ene weergave of de andere uitschakelen.

Zie ook [Een voorinstelling voor een batchset maken voor het automatisch genereren van een 2D-reeks voor draaien](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Een voorinstelling voor een batch-set maken:**

1. Klik op **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, zoals ingesteld in de rechterbovenhoek van de pagina Details, is de standaardweergave.
1. Klik in het deelvenster Lijst met voorinstellingen op **[!UICONTROL Add]** om de definitievelden te activeren in het deelvenster Details aan de rechterkant van de pagina.
1. Typ in het veld Naam voorinstelling in het deelvenster Details een naam voor de voorinstelling.
1. Selecteer een type voorinstelling in het keuzemenu Type batch.

   Als u automatisch een 2D-centrifugeset wilt genereren, selecteert u **[!UICONTROL Multi-Axis Spin Set]** in de vervolgkeuzelijst Type batch-set.

1. Voer een van de volgende handelingen uit:

   * Als u een standaardnaamgevingsconventie gebruikt die u eerder hebt ingesteld onder **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**, vouwt u **[!UICONTROL Asset Naming Conventions]** uit en klikt u vervolgens in de vervolgkeuzelijst Bestandsnaamgeving op **[!UICONTROL Default]**.
   * Als u een naamgevingsconventie wilt definiëren terwijl u de voorinstelling instelt, vouwt u **[!UICONTROL Asset Naming Conventions]** uit en klikt u vervolgens in de vervolgkeuzelijst Bestandsnaamgeving op **[!UICONTROL Custom]**.

1. Definieer bij Volgorde de volgorde voor de afbeeldingen nadat de set is gegroepeerd in Dynamic Media Classic. Uw elementen worden standaard alfanumeriek geordend. U kunt echter een door komma&#39;s gescheiden lijst met reguliere expressies gebruiken om de volgorde te definiëren.
1. Geef bij Naamgeving instellen en Creatieconcept het achtervoegsel of het voorvoegsel op van de basisnaam die u in de Naamgevingsconventie voor middelen hebt gedefinieerd. Definieer ook waar de afbeeldingsset wordt gemaakt in de Classic-mapstructuur van Dynamic Media.

   Als u grote aantallen afbeeldingssets definieert, moet u deze sets gescheiden houden van de mappen die de elementen zelf bevatten. Vele klanten creëren een omslag van de Reeksen van het Beeld en leiden de toepassing om partij te plaatsen geproduceerde reeksen hier.

1. Klik **[!UICONTROL Save]** in het paneel van Details.

### Een voorinstelling voor een batch-set maken voor het automatisch genereren van een 2D-reeks voor draaien {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

U kunt het Type van Type van Reeks **Meerassige Reeks** gebruiken om een &quot;recept&quot;tot stand te brengen dat de generatie van 2D Reeksen van de Draai automatiseert. Bij het groeperen van afbeeldingen worden de reguliere expressies Rij en Kolom gebruikt, zodat de afbeeldingselementen op de juiste wijze worden uitgelijnd op de corresponderende locatie in de multidimensionale array.

Zie ook [Een voorinstelling voor een batchset maken](application-setup.md#creating_a_batch_set_preset).

Er is geen minimum- of maximumaantal rijen of kolommen dat u in een centrifugeerset moet hebben.

Als voorbeeld, veronderstel u een multi-as goot reeks genoemd *spin-2dspin* wilt tot stand brengen. U hebt een set afbeeldingen met een set centrifuges die drie rijen bevatten, met 12 afbeeldingen per rij. De afbeeldingen krijgen de volgende naam:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Met deze informatie kunt u het recept voor Type batch-set als volgt maken:

![](assets/se_batch_set_recipe.png)

De groepering voor het gedeelde element naamdeel van de spinset wordt toegevoegd aan het veld Overeenkomst (zoals gemarkeerd). Het variabele gedeelte van de naam van de asset met de rij en kolom wordt toegevoegd aan respectievelijk de velden Rij en Kolom.

Wanneer de Spin-set wordt geüpload en gepubliceerd, activeert u de naam van het recept voor de 2D-centrifugeset dat onder **[!UICONTROL Batch Set Presets]** wordt weergegeven in het dialoogvenster Opties voor uploaden van taak.

**Een voorinstelling voor een batch-set maken voor het automatisch genereren van een 2D-reeks voor draaien:**

1. Kies **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, zoals ingesteld in de rechterbovenhoek van de pagina Details, is de standaardweergave.
1. Klik in het deelvenster Lijst met voorinstellingen op **[!UICONTROL Add]** om de definitievelden te activeren in het deelvenster Details rechts op de pagina.
1. Typ in het veld Naam voorinstelling in het deelvenster Details een naam voor de voorinstelling.
1. Selecteer in het vervolgkeuzemenu Batchsettype de optie **[!UICONTROL Asset Set]**.
1. Selecteer **[!UICONTROL Multi-Axis Spin Set]** in de vervolgkeuzelijst Subtype.
1. Vouw **[!UICONTROL Asset Naming Conventions]** uit en klik vervolgens in de vervolgkeuzelijst Bestandsnaamgeving op **[!UICONTROL Custom]**.
1. Gebruik de kenmerken **[!UICONTROL Match]** en (optioneel) **[!UICONTROL Base Name]** om een reguliere expressie te definiëren voor de naamgeving van afbeeldingsassets waaruit de groepering bestaat.

   De reguliere expressie Letterlijke overeenkomst kan er bijvoorbeeld als volgt uitzien:

   `(\w+)-\w+-\w+`

1. Vouw **[!UICONTROL Row Column Position]** uit en definieer vervolgens de naamnotatie voor de positie van het afbeeldingselement binnen de 2D-array met spellingsets.

   Gebruik het haakje om de rij- of kolompositie in de bestandsnaam in te sluiten.

   Voor uw reguliere rijexpressie zou deze er bijvoorbeeld als volgt kunnen uitzien:

   `\w+-R([0-9]+)-\w+`

   of

   `\w+-(\d+)-\w+`

   Voor de reguliere kolomexpressie kan deze er als volgt uitzien:

   `\w+-\w+-C([0-9]+)`

   of

   `\w+-\w+-C(\d+)`

   Onthoud dat deze expressies slechts voorbeelden zijn. U kunt uw reguliere expressie maken op een manier die aan uw wensen voldoet.

   >[!NOTE]
   >
   >Als de combinatie van reguliere rij- en kolomexpressies de positie van het element binnen de multidimensionale spin-set-array niet kan bepalen, wordt dat element niet aan de set toegevoegd en wordt een fout geregistreerd.

1. Geef bij Naamgeving instellen en Creatieconcept het achtervoegsel of het voorvoegsel op van de basisnaam die u in de Naamgevingsconventie voor middelen hebt gedefinieerd. Definieer ook waar de afbeeldingsset wordt gemaakt in de Classic-mapstructuur van Dynamic Media.

   Als u grote aantallen afbeeldingssets definieert, moet u deze sets gescheiden houden van de mappen die de elementen zelf bevatten. Vele klanten creëren een omslag van de Reeksen van het Beeld en leiden de toepassing om partij te plaatsen geproduceerde reeksen hier.

1. Klik **[!UICONTROL Save]** in het paneel van Details.
1. Upload en publiceer de centrifugeerset op de gebruikelijke manier. Zorg ervoor dat u de naam van de 2D-centrifugeset activeert in het dialoogvenster Opties voor laden van taak, onder Voorinstellingen voor batchset.

>[!MORELIKETHIS]
>
>* [Een voorvertoning van een element weergeven](previewing-asset.md#previewing_an_asset)
* [Voorinstellingen afbeelding instellen](setting-image-presets.md#setting_up_image_presets)
* [Metagegevens weergeven, toevoegen en exporteren](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Taakbestanden controleren](checking-job-files.md#checking_job_files)

