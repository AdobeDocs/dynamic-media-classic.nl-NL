---
title: Toepassing instellen
description: Leer hoe u het toepassingsgebied van Adobe Dynamic Media Classic instelt en configureert.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10351'
ht-degree: 1%

---

# Toepassing instellen{#application-setup}

U kunt de pagina&#39;s van de Opstelling van de Toepassing gebruiken om Algemene Montages in te gaan, Vooraf ingestelde Beeld tot stand te brengen, Video het Coderen vooraf instelt, Kijker vooraf instelt, of standaardKijkers, en meta-gegevens te bepalen. U kunt Batchsetvoorinstellingen zodanig instellen dat het genereren van 2D-centrifuges (bijvoorbeeld), publicatie-instellingen en video-SEO-instellingen wordt geautomatiseerd.

>[!NOTE]
>
>Alleen Adobe Dynamic Media Classic-beheerders kunnen de instellingen wijzigen in Toepassingsinstellingen.

## Algemene instellingen {#general-settings}

Als u de pagina Algemene instellingen toepassing wilt openen, gaat u naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.

### Servers

Bij het maken van accounts verschaft Adobe Dynamic Media Classic automatisch de toegewezen servers voor uw bedrijf. Deze servers worden gebruikt om koorden URL voor uw Website en toepassingen te construeren. Deze URL-aanroepen gelden specifiek voor uw account.

Zie ook [De service Beveiligde tests testen](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Published Server Name]**: Deze server is de live CDN-server (Content Deliver Network) die wordt gebruikt in alle door het systeem gegenereerde URL-aanroepen die specifiek zijn voor uw account. Wijzig deze servernaam alleen als een technicus van de Adobe Dynamic Media Classic u hiervoor de instructie geeft.

* **[!UICONTROL Origin Server Name]**: Deze server wordt alleen gebruikt voor het testen van kwaliteitsborging. Wijzig deze servernaam alleen als een technicus van de Adobe Dynamic Media Classic u hiervoor de instructie geeft.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&Target Server Name]**: De doel&amp;URL testen, inclusief `.com`. Zie Integratie voor instructies over het verkrijgen van deze URL [!DNL Adobe Dynamic Media Classic] with [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS Streaming Server Name]**: De URL naar uw [!DNL Adobe Dynamic Media Classic] iOS-streamingserver. Deze server levert streaming video naar op iOS gebaseerde apparaten met behulp van het HTTP-protocol.

* **[!UICONTROL Progressive Video Server Name]**: De URL naar uw [!DNL Adobe Dynamic Media Classic] progressieve videoserver. Deze server levert progressieve video gebruikend het protocol van HTTP.

* **[!UICONTROL Show URL for unpublished assets]**: Selecteer deze optie als u wilt [!DNL Adobe Dynamic Media Classic] om een URL weer te geven wanneer u een voorvertoning van een element weergeeft, gepubliceerd of niet. Als het element niet is gepubliceerd, werkt de URL niet. U kunt de URL echter ook gebruiken voor plannings- of organisatorische doeleinden.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN Invalidation Template]**: Geeft de sjabloon op die wordt gebruikt voor het ongeldig maken van de CDN-cache (Content Delivery Network).

  Stel dat u bijvoorbeeld een afbeeldings-URL invoert (inclusief Voorinstellingen of wijzigingstoetsen voor afbeeldingen) die verwijst naar `<ID>`in plaats van een specifieke afbeelding-id zoals in het volgende voorbeeld:

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  Als de sjabloon alleen bevat `<ID>`en vervolgens vult Adobe Dynamic Media Classic de `https://<server>/is/image`, waarbij `<server>` Dit is de naam van de Publishing Server die is gedefinieerd in Algemene instellingen.

  Het plaatsen van CDN ongeldig Malplaatje, selecteert een beeld genoemd Backpack_B, en gaat dan naar **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]** resulteert in volgende geproduceerde URL in CDN ongeldig maakt interface:

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  Selecteer in de keuzelijst URL de optie **[!UICONTROL Continue]** om het geheime voorgeheugen voor die specifieke beeldURL vraag te ontruimen. U kunt ook URL&#39;s toevoegen door deze in het vak URL-lijst te typen of te plakken. U hoeft de sjabloon niet vooraf in te stellen.

  Nadat u uw Malplaatje van de Invalidatie CDN hebt geselecteerd, en een ongeldig CDN verzoek gemaakt, duikt een indicator op in het gebruikersinterface. Het geeft u een schatting van hoe lang het duurt om het geheime voorgeheugen te ontruimen.

  Wanneer u op **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]**, wordt naar elke afbeelding verwezen in de opgeslagen sjabloon-URL als er meerdere afbeeldingen zijn geselecteerd in Dynamic Media Classic. Daarom kunt u CDN bepalen ongeldig Malplaatje dat van verwijzingen voorziet elke URL die op uw Website (zoals productdetail en onderzoeksresultaten) wordt voorzien. Wanneer u vervolgens een of meer afbeeldingen selecteert om uit de cache te worden verwijderd, vullen de URL&#39;s automatisch de interface in.

  Zie [Inhoud in cache plaatsen](dmc-platform-overview.md#content_caching).

  Zie [Hergepubliceerde elementen en CDN-vertragingen](publishing-files.md#republished_assets_and_cdn_delays).

### Bladeren

* **[!UICONTROL Show Projects]**: Hiermee bepaalt u of Projecten beschikbaar zijn als een manier om uw Adobe Dynamic Media Classic-middelen te organiseren. Zie [Uw werk organiseren met projecten](/help/using/organizing-projects.md).

* **[!UICONTROL Show Sample eVideo Content]**: Schakel de weergave van de inhoud van het eVideo-voorbeeld in of uit.

* **[!UICONTROL Show Generated Content]**: In mappen wordt de inhoud weergegeven die is gegenereerd op basis van een element. Wanneer een PDF-bestand bijvoorbeeld tijdens het uploaden wordt gerasterd, maakt Adobe Dynamic Media Classic één afbeelding voor elke pagina in de oorspronkelijke PDF. Als Gegenereerde inhoud tonen is geselecteerd, wordt elke gegenereerde afbeelding weergegeven wanneer de oorspronkelijke PDF wordt geüpload. Deze wordt samen met de PDF weergegeven in de map waarnaar de PDF is geüpload.

* **[!UICONTROL Show Encoded Videos]**: Standaard uitgeschakeld.

  U kunt in Adobe Dynamic Media Classic snel naar video&#39;s zoeken en deze zoeken zonder dat u door een groot aantal gecodeerde derivaten van dezelfde video hoeft te navigeren. Laat deze optie uitgeschakeld (standaard). Alleen de miniatuur Primaire video (de bronvideo die u hebt geüpload en gebruikt om de derivaten te maken) en de miniatuur &#39;Bovenliggende&#39; adaptieve videoset (die de &#39;onderliggende&#39; derivaten van de gecodeerde videoset bevat) worden weergegeven.

  U kunt echter wel toegang krijgen tot individuele gecodeerde video&#39;s via de primaire video of de adaptieve videoset. Dubbelklik hiertoe op de miniatuurafbeelding van de video om de gedetailleerde weergave te openen. Selecteer vervolgens **[!UICONTROL Encoded Videos]** in het rechterdeelvenster, zodat u toegang hebt tot alle &#39;onderliggende&#39; video&#39;s.

  U kunt ook naar **[!UICONTROL File]** > **[!UICONTROL Reprocess]** om meer gecodeerde &#39;onderliggende&#39; video&#39;s rechtstreeks vanuit een adaptieve videoset te maken. Adobe Dynamic Media Classic zoekt automatisch de &quot;bovenliggende&quot; primaire video van de adaptieve videoset en gebruikt die als de bronvideo voor transcodering. Wanneer u de nieuwe individuele gecodeerde video&#39;s opslaat, worden deze echter niet weergegeven wanneer u doorzoekt of bladert. Ze zijn echter nog steeds toegankelijk via het tabblad Gecodeerde video&#39;s in de gedetailleerde weergave.

  Zie [Video&#39;s uploaden en transcoderen](uploading-encoding-videos.md#uploading_and_encoding_videos).

  Als u wilt doorgaan met de mogelijkheid om toegang te krijgen tot al uw gecodeerde videoderivaten wanneer u doorzoekt en bladert, selecteert u **[!UICONTROL Show Encoded Videos]**.

  Het menu Build bevat bepaalde acties die alleen werken, of optioneel werken, met afzonderlijke video&#39;s. Deze functionaliteit maakt het noodzakelijk om alle gecodeerde videoderivaten te tonen die u kunt selecteren, ongeacht hoe u plaatst **[!UICONTROL Show Encoded Videos]**. De acties van de Bouwstijl die met voeten treden **[!UICONTROL Show Encoded Videos]** instellen, include **[!UICONTROL Adaptive Video Sets]**, en **[!UICONTROL eCatalogs]**.

  >[!NOTE]
  >
  >Als u Adobe Dynamic Media Classic niet hebt gebruikt om uw video-elementen te uploaden en te coderen, geeft Adobe Dynamic Media Classic al uw individuele gecodeerde video&#39;s weer, zelfs als deze optie is uitgeschakeld.

* **[!UICONTROL Show Refresh Subfolders Button]**: Schakel de weergave van de knop Submappen vernieuwen in of uit.

### Adobe Dynamic Media Classic FTP-account

* **[!UICONTROL Server]**: Hier wordt de FTP-accountserver weergegeven.

* **[!UICONTROL User Name]**: Hier wordt de gebruikersnaam van uw FTP-account weergegeven.

### Uploaden naar toepassing

Zie ook [Opties voor uploadtaken](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) trainingsvideo.

* **[!UICONTROL Overwrite Images]**: Adobe Dynamic Media Classic staat niet toe dat twee bestanden dezelfde naam hebben. De Adobe Dynamic Media Classic-id van elk item (de naam van de afbeelding min de extensie van de bestandsnaam) moet uniek zijn. Vanwege deze regel heeft het dialoogvenster Uploaden een optie Overschrijven. Het exacte effect van deze optie is afhankelijk van de opgegeven optie Afbeeldingen overschrijven. Met deze opties geeft u op hoe vervangende afbeeldingen worden geüpload: of ze de oorspronkelijke afbeeldingen vervangen of dubbele afbeeldingen worden. Dubbele afbeeldingen krijgen de naam &quot;-1&quot;. (De naam van bijvoorbeeld stoel.tif wordt gewijzigd in stoel-1.tif). Deze opties zijn van toepassing op afbeeldingen die naar een andere map zijn geüpload dan het origineel of afbeeldingen met een andere bestandsnaamextensie dan het origineel (zoals JPG, TIF of PNG). Zie [De optie Afbeeldingen overschrijven gebruiken](#using-the-overwrite-images-option).

   * **[!UICONTROL Overwrite in current folder, same base image name or extension]**: Deze optie is de strengste regel voor vervanging. Hiervoor moet u de vervangende afbeelding uploaden naar dezelfde map als het origineel en moet de vervangende afbeelding dezelfde bestandsnaamextensie hebben als het origineel. Als niet aan deze vereisten wordt voldaan, wordt een dubbel gecreeerd.

   * **[!UICONTROL Overwrite in current folder, same base asset name regardless of extension]**: Hiermee moet u de vervangende afbeelding uploaden naar dezelfde map als het origineel, maar de bestandsextensie kan afwijken van die van het origineel. bijvoorbeeld stoel.tif vervangt stoel.jpg.

   * **[!UICONTROL Overwrite in any folder, same base asset name or extension]**: Vereist dat de vervangende afbeelding dezelfde bestandsnaamextensie heeft als de oorspronkelijke afbeelding. bijvoorbeeld stoel.jpg moet stoel.jpg vervangen, niet stoel.tif). U kunt de vervangende afbeelding echter naar een andere map uploaden dan het origineel. De bijgewerkte afbeelding staat in de nieuwe map. Het bestand kan niet meer op de oorspronkelijke locatie worden gevonden

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]**: Deze optie is de meest inclusieve vervangingsregel. U kunt een vervangende afbeelding uploaden naar een andere map dan het origineel, een bestand met een andere bestandsnaamextensie uploaden en het oorspronkelijke bestand vervangen. Als het oorspronkelijke bestand zich in een andere map bevindt, bevindt de vervangende afbeelding zich in de nieuwe map waarnaar het is geüpload.

* **[!UICONTROL Retain Publish]**: Geeft aan of een vervangende afbeelding die naar Adobe Dynamic Media Classic is geüpload, de instelling Ready to Publish behoudt van de afbeelding die wordt vervangen. Of de instelling wordt opgegeven bij het uploaden.

* **[!UICONTROL Default Color Profiles]**: Hiermee geeft u de kleurprofielen op die worden toegepast als onderdeel van de standaardopties voor kleurprofielen bij het toevoegen van CMYK-afbeeldingen.

* **[!UICONTROL Default Upload Options]**: Hiermee opent u het dialoogvenster Taakopties uploaden, waarin u de standaardopties voor uploaden kunt opgeven. Zie voor informatie over deze opties [Uploadopties](/help/using/uploading-files.md#upload_options).

### Afbeeldingskaarteditor (naar toepassing)

* **[!UICONTROL Default Image Mapping HREF]**: Hiermee definieert u de standaard-URL die wordt gebruikt voor de HREF-kolom in afbeeldingstoewijzing. Deze URL is de standaard-URL die u ziet wanneer u afbeeldingen met hyperlinks maakt.

* **[!UICONTROL Default Image Mapping Template]**: Hiermee definieert u de standaard JavaScript voor de HREF-sjabloon in afbeeldingstoewijzing. U kunt hier een aangepaste code instellen die moet worden uitgevoerd wanneer u een afbeelding met hyperlinks selecteert.

### Overige instellingen (op toepassing)

* **[!UICONTROL Trash Can Clean Up Warnings]**: Elementen in de prullenbak worden automatisch binnen zeven dagen verwijderd. Selecteer &quot;E-mails verzenden voordat de prullenmand automatisch wordt verwijderd&quot; om meldingen te laten verzenden naar bedrijfsbeheerders wanneer elementen in de prullenmand vier dagen verwijderd zijn van definitieve verwijdering. Zie [De map Prullenmand beheren](/help/using/trash-folder.md).

## De optie Afbeeldingen overschrijven gebruiken {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic staat niet toe dat twee bestanden dezelfde naam hebben. De Adobe Dynamic Media Classic-id van elk item (de naam van de afbeelding min de extensie van de bestandsnaam) moet uniek zijn. Vanwege deze regel bevat het dialoogvenster Uploaden opties voor het overschrijven van afbeeldingen. Het exacte effect van deze optie is afhankelijk van een instelling voor de interne instellingen van Adobe Dynamic Media Classic van elk bedrijf.

Als u eerder afbeeldingen hebt geüpload en vervolgens de originele bestanden hebt gewijzigd (of deze hebt vervangen), bepaalt de gekozen optie Overschrijven hoe Adobe Dynamic Media Classic de afbeeldingen vervangt. Er wordt geen informatie over de afbeelding gewijzigd, maar de nieuwe afbeelding vervangt de oude. Als de map ook afbeeldingen bevat die nog niet in Adobe Dynamic Media Classic staan, worden deze afbeeldingen toegevoegd.

Gebruik deze optie als de geüploade afbeeldingen op een of andere manier zijn gewijzigd (de afbeelding is gewijzigd), maar de verwijzing naar de afbeelding ongewijzigd blijft. Overschrijven is ook handig bij het uploaden en rippen van Adobe®-PDF. Je kunt afstemmen hoe Adobe Dynamic Media Classic *rips* de afbeelding. U kunt ook de ICC-kleurprofielopties aanpassen in het dialoogvenster Uploaden en opnieuw uploaden met de functie Overschrijven.

De Adobe Dynamic Media Classic-id&#39;s die worden gebruikt om toegang te krijgen tot afbeeldingen van de productieservers, zijn afgeleid van de bestandsnamen van de afbeeldingen. Het gebruik van hoofdletters en kleine letters in de bestandsnaam is belangrijk, zowel voor de vervanging van bestaande bestanden als voor de Adobe Dynamic Media Classic-id&#39;s die worden gebruikt om de afbeelding te openen. Gebruik van bestandsnamen in hoofdletters en kleine letters is correct voordat u ze uploadt naar Adobe Dynamic Media Classic om te voorkomen dat Adobe Dynamic Media Classic-id&#39;s die alleen verschillen in hoofdletters en kleine letters voor dezelfde afbeelding.

Als u deze optie uitschakelt, worden alle afbeeldingen met dezelfde bestandsnamen als bestaande afbeeldingen behandeld als duplicaten en worden ze niet toegevoegd.

## Voorinstellingen afbeelding {#image-presets}

Het scherm Voorinstellingen afbeelding is bedoeld voor het maken en bewerken van voorinstellingen afbeelding. Met voorinstellingen voor afbeeldingen kan Adobe Dynamic Media Classic afbeeldingen dynamisch leveren in verschillende formaten dan in dezelfde primaire afbeelding. Elke voorinstelling voor afbeeldingen vertegenwoordigt een vooraf gedefinieerde verzameling opdrachten voor het vergroten of verkleinen en opmaken van afbeeldingen. Als u een voorinstelling voor afbeeldingen maakt, selecteert u een grootte voor de levering van de afbeelding. U kunt ook opmaakopdrachten selecteren, zodat de weergave van de afbeelding wordt geoptimaliseerd wanneer de afbeelding voor weergave wordt geleverd.

Beheerders kunnen voorinstellingen maken voor het exporteren van elementen. Gebruikers kunnen bij het exporteren van afbeeldingen een voorinstelling kiezen die de afbeeldingen opnieuw opmaakt volgens de specificaties die de beheerder heeft opgegeven.

Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.

Zie [Slimme beeldverwerking](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

### Voorinstellingen voor afbeeldingen maken en bewerken {#creating-and-editing-image-presets}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Maak een voorinstelling of begin met een bestaande voorinstelling:

   * **Een voorinstelling voor afbeeldingen maken**: Select **[!UICONTROL Add]**.
   * **Een voorinstelling voor afbeeldingen maken op basis van een bestaande voorinstelling**: Selecteer de voorinstelling Afbeelding die het meest lijkt op de voorinstelling die u wilt maken en selecteer **[!UICONTROL Edit]**.

1. Voer op de pagina Voorinstelling toevoegen (of bewerken) een naam in voor de voorinstelling.
1. Stel de gewenste voorinstellingsopties in.

   Zie [Voorinstellingsopties voor afbeelding](application-setup.md#image_preset_options).

1. Selecteren **[!UICONTROL Save]** of als u vanuit een bestaande voorinstelling bent begonnen, selecteert u **[!UICONTROL Save As]**.
1. Als u de voorinstelling wilt voorvertonen met uw eigen afbeelding, selecteert u **[!UICONTROL Browse]** en selecteert u vervolgens een afbeelding. Selecteer **[!UICONTROL Reset]**.

U kunt een Voorinstelling afbeelding bewerken door de naam ervan te selecteren in het scherm Voorinstellingen afbeelding en vervolgens **[!UICONTROL Edit]**. Als u een voorinstelling voor afbeeldingen wilt verwijderen, selecteert u deze en selecteert u vervolgens **[!UICONTROL Delete]**.

### Voorinstellingsopties voor afbeelding {#image-preset-options}

In het scherm Voorinstelling toevoegen en Voorinstelling bewerken vindt u de volgende opties voor het maken en bewerken van voorinstellingen voor afbeeldingen:

* **[!UICONTROL Preset Name]**: Voer een beschrijvende naam in zonder spaties. Als u gebruikers wilt helpen deze voorinstelling voor afbeeldingen te identificeren, neemt u de specificatie voor de afbeeldingsgrootte op in de naam.

* **[!UICONTROL Width and Height]**: Voer in pixels de grootte in waarmee de afbeelding wordt geleverd.

* **[!UICONTROL Format]**: Selecteer een indeling in het menu. Als u de indeling GIF, JPEG, PDF of TIFF kiest, zijn er meer opties beschikbaar:

   * Kwantiseringsopties voor kleur GIF

      * **[!UICONTROL Type]**: Selecteer Adaptief (standaard), Web of Mac. Als u **[!UICONTROL GIF With Alpha]**, is de optie Mac niet beschikbaar.

      * **[!UICONTROL Dither]**: Selecteer Onscherp of Uit.

      * **[!UICONTROL Number Of Colors]**: Sleep de schuifregelaar om 2-255 in te voeren.

      * **[!UICONTROL Color List]**: Voer een door komma&#39;s gescheiden lijst in. Voor wit, grijs en zwart voert u bijvoorbeeld de volgende gegevens in: `000000,888888,ffffff`.

   * JPEG-opties

      * **[!UICONTROL Quality]**: Hiermee bepaalt u het compressieniveau JPEG. Deze instelling is van invloed op zowel de bestandsgrootte als de afbeeldingskwaliteit. De schaal van de kwaliteit van de JPEG is 1-100.

      * **[!UICONTROL Enable JPG Chrominance Downsampling]**: Omdat het oog minder gevoelig is voor hoogfrequente kleurinformatie dan hoogfrequente luminantie, verdelen JPEG-afbeeldingen de afbeeldingsgegevens in luminantie en kleurcomponenten. Wanneer een JPEG-afbeelding wordt gecomprimeerd, blijft de luminantiecomponent op volledige resolutie staan, terwijl de kleurcomponenten worden gedownsampled door het gemiddelde te nemen van pixelgroepen. Door downsampling wordt het gegevensvolume met de helft of met een derde verminderd, zonder dat dit van invloed is op de waargenomen kwaliteit. Downsampling is niet van toepassing op grijswaardenafbeeldingen. Met deze techniek vermindert u de hoeveelheid compressie die handig is voor afbeeldingen met veel contrast (bijvoorbeeld afbeeldingen met overlappende tekst).

   * Opties voor PDF en TIFF

      * **[!UICONTROL Compression]**: Selecteer een compressiealgoritme.

* **[!UICONTROL Colorspace]**: Selecteer een kleurruimte.

* **[!UICONTROL Sharpening]**: Selecteer de optie Eenvoudig verscherpen inschakelen om een standaard verscherpingsfilter toe te passen op de afbeelding nadat alle schaling heeft plaatsgevonden. Verscherpen kan helpen de vervaging te compenseren die kan optreden wanneer u een afbeelding met een andere grootte weergeeft.

  Zie voor meer informatie over verscherpen, nieuwe beeldpixels berekenen en onscherp maskeren [Een afbeelding verscherpen](sharpening-image.md#sharpening_an_image). Zie ook [Verscherpen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) trainingsvideo.

* **[!UICONTROL Resample Mode]**: Selecteer een optie voor de modus Nieuwe pixels berekenen. Met deze opties verscherpt u de afbeelding wanneer deze wordt gedownsampled:

* **[!UICONTROL B-Linear]**: De snelste methode voor het berekenen van nieuwe pixels. Sommige aliasingartefacten zijn opvallend.

* **[!UICONTROL Bi-Cubic]**: Verhoogt het CPU-gebruik op de Image Server, maar geeft scherpere afbeeldingen met minder merkbare aliasing artefacten.

* **[!UICONTROL `Sharp 2`]**: Dit kan iets scherpere resultaten opleveren dan de optie Bi-Cubic, maar met nog hogere CPU-kosten op de afbeeldingsserver.

* **[!UICONTROL Tri-Linear]**: Hiermee gebruikt u zowel hogere als lagere resoluties, indien beschikbaar. Wordt alleen aangeraden als aliasing een probleem is. Deze methode vermindert de grootte van JPEG als gevolg van gereduceerde gegevens met hoge frequentie.

* **[!UICONTROL Unsharp Masking]**: Kies deze opties om de verscherping verder af te stemmen:

* **[!UICONTROL Amount]**: Hiermee bepaalt u de hoeveelheid contrast die wordt toegepast op de randpixels. De standaardwaarde is 1.0. Voor afbeeldingen met een hoge resolutie kunt u de resolutie verhogen tot 5,0. Beschouw Hoeveelheid als een maat voor de filterintensiteit.

* **[!UICONTROL Radius]**: Hiermee bepaalt u het aantal pixels rondom de randpixels dat invloed heeft op de verscherping. Voer voor afbeeldingen met een hoge resolutie een waarde in tussen 1 en 2. Met een lage waarde worden alleen de randpixels verscherpt; met een hoge waarde wordt een bredere reeks pixels verscherpt. De juiste waarde is afhankelijk van de grootte van de afbeelding.

* **[!UICONTROL Threshold]**: Hiermee bepaalt u het contrastbereik dat moet worden genegeerd wanneer het filter Onscherp masker wordt toegepast. Dat wil zeggen dat u hiermee kunt oplossen hoe verschillend de verscherpte pixels moeten zijn van het omringende gebied voordat ze als randpixels worden beschouwd en worden verscherpt. Experimenteer met waarden tussen `.02` en `0.2`. Met de standaardwaarde 6 worden alle pixels in de afbeelding verscherpt.

* **[!UICONTROL Color Space]**: Hiermee bepaalt u of de afbeelding de ruimte gebruikt waarin de afbeelding is gemaakt, meestal RGB (Origineel) of een luminantieruimte (Intensiteit).

* **[!UICONTROL Color]** Kies de volgende opties:

* **[!UICONTROL Output Color Profile]**: Select **[!UICONTROL Use Default]** of een van de ICC-kleurprofielen die beschikbaar zijn op de Adobe Dynamic Media Classic.

  Zie ook [ICC-profielen](icc-profiles.md#icc_profiles).

* **[!UICONTROL Rendering Intent]**: Selecteer een optie als u de standaard rendering intent van het kleurprofiel wilt overschrijven. Gebruik deze optie als een van de standaard-ICC-profielen de doelkleurruimte van een kleuromzetting is. Of dit profiel karakteriseert het uitvoerapparaat (printer of monitor) en de opgegeven rendering intent is geldig voor dit profiel.

* **[!UICONTROL Embed Profile]**: Selecteer deze optie als u deze afbeelding opent in Adobe® Photoshop®, wordt dit profiel gebruikt.

* **[!UICONTROL Print Resolution]**: Selecteer een resolutie voor het afdrukken van deze afbeelding; 72 pixels is de standaardinstelling.

* **[!UICONTROL URL Modifiers]**: Als u liever de URL-modifiers opgeeft die uw voorinstelling voor afbeeldingen definiëren in plaats van de instellingen, voert u hier de modifiers in.

* **[!UICONTROL Sample Image URL]**: Maakt een lijst van het &quot;ruwe&quot;koord URL dat de Server van het Beeld van Dynamic Media gebruikt om beelden met het Beeld te leveren vooraf instelt u toevoegt of uitgeeft. Deze URL-tekenreeks codeert alle indelingsinstellingen die u selecteert in het scherm Voorinstelling toevoegen of Voorinstelling bewerken.

### Een voorinstelling voor afbeeldingen bewerken, verwijderen of deactiveren {#editing-removing-or-deactivating-an-image-preset}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Selecteer in het scherm Voorinstellingen afbeelding een voorinstelling in de tabel en voer een van de volgende handelingen uit:

   * Selecteren **[!UICONTROL Edit]** en geeft u nieuwe opties op in het dialoogvenster Voorinstelling bewerken.
   * Selecteren **[!UICONTROL Delete]** om de voorinstelling uit de lijst te verwijderen.
   * Hef de selectie van **[!UICONTROL Active]** Schakel het selectievakje naast de naam van een voorinstelling in als u deze wilt verwijderen uit de volledige Adobe Dynamic Media Classic-gebruikersinterface voor MediaPortal-gebruikers.

## Aangepaste videovoorinstellingen activeren of deactiveren {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic biedt voorinstellingen voor adaptieve videocodering. Het is een primaire lijst met voorinstellingen die zowel 16:9 Adaptieve videovoorinstellingen als 4:3 Adaptieve videovoorinstellingen in één groep verenigt. Deze vooraf gedefinieerde voorinstellingen weerspiegelen de meest gangbare coderingsinstellingen en zijn geoptimaliseerd voor afspelen op mobiele doelapparaten, tablets en desktops.

Alleen coderingsvoorinstellingen voor Adaptieve video worden standaard geactiveerd (ingeschakeld of ingeschakeld). U kunt het desgewenst deactiveren. Inactieve adaptieve videovoorinstellingen worden niet als een selecteerbare optie weergegeven in de sectie eVideo van het dialoogvenster Taakopties uploaden.

Zie [Video&#39;s uploaden en coderen](uploading-encoding-videos.md#uploading_and_encoding_videos).

Zie ook [Videovoorinstellingen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) trainingsvideo.

**Aangepaste videovoorinstellingen activeren of deactiveren:**

1. Ga in de rechterbovenhoek van Adobe Dynamic Media Classic naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]**.
1. Schakel op de pagina Voorinstellingen adaptieve video het selectievakje naast de naam van een voorinstelling uit om de voorinstelling te verwijderen uit de lijst EVideo-opties in het dialoogvenster Taakopties uploaden.
1. Selecteren **[!UICONTROL Close]**.

## Videovoorinstellingen voor het coderen van videobestanden {#video-presets-for-encoding-video-files}

Als u een coderingsvoorinstelling wilt selecteren, selecteert u in de rechterbenedenhoek van de pagina Uploaden de optie **[!UICONTROL Job Options]**. Vouw de eVideo-opties uit in het dialoogvenster Taakopties uploaden en selecteer de gewenste voorinstellingen voor videocodering.

>[!NOTE]
>
>Met uitzondering van &quot;Adaptieve video&quot;, die standaard is ingeschakeld, kunt u niet alle andere voorinstellingen voor adaptieve video of enkele videocodering zien in het dialoogvenster Opties voor uploaden. Adobe Dynamic Media Classic-beheerders bepalen welke voorinstellingen voor videocodering worden weergegeven in het dialoogvenster Opties voor uploaden van taak.

* Selecteer een van de volgende voorinstellingen voor Adaptieve videocodering of enkele codering:

   * **[!UICONTROL 16:9 Adaptive Video]**: Maak video&#39;s met de hoogte-breedteverhouding 16:9 voor levering aan desktops, mobiele apparaten (iPhone, iPad, Android™) en tablets (iPad, Android™), geoptimaliseerd met de resolutie en bitsnelheid die het best overeenkomen met de verbindingssnelheid van de viewer.

   * **[!UICONTROL 4:3 Adaptive Video]**: Maak video&#39;s met de hoogte-breedteverhouding 4:3 voor levering aan desktops, mobiele apparaten (iPhone, iPad, Android™) en tablets (iPad, Android™), geoptimaliseerd met de resolutie en bitsnelheid die het best overeenkomen met de verbindingssnelheid van de viewer.

   * **[!UICONTROL Adaptive Video]**: Een voorinstelling voor één codering die met een willekeurige hoogte-breedteverhouding werkt voor het maken van video&#39;s voor levering op mobiele apparaten, tablets en desktops. Geüploade bronvideo&#39;s die met deze voorinstelling zijn gecodeerd, worden ingesteld met een vaste hoogte. De breedte wordt echter automatisch geschaald om de hoogte-breedteverhouding van de video te behouden.

     Deze flexibiliteit van een &#39;Automatisch schalen&#39; is standaard ook beschikbaar wanneer u uw eigen voorinstelling voor aangepaste videocodering maakt.

     Zie [Een voorinstelling voor videocodering toevoegen of bewerken](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Adaptive Video Encoding (16:9 or 4:3)]**: Maak zowel video&#39;s met de hoogte-breedteverhouding 16:9 als 4:3 voor levering aan desktops, mobiele apparaten (iPhone, iPad, Android™) en tablets (iPad, Android™). Alles geoptimaliseerd met de resolutie en bitsnelheid die het beste overeenkomen met de verbindingssnelheid van de viewer.

     Zie [Adaptieve videocodering (16:9 of 4:3), videovoorinstellingen](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Single Encoding Presets]**

     >[!NOTE]
     >
     >Als u video wilt leveren aan iPads, kunt u een voorinstelling voor mobiele codering of een voorinstelling voor tabletcodering selecteren. Tabletvoorinstellingen zijn speciaal ontworpen voor de iPad, meestal met een hogere resolutie en kwaliteit, zodat u kunt profiteren van de grotere schermgrootte en bandbreedteverbinding. Als u videobestanden wilt leveren die zijn gecodeerd met een voorinstelling voor tablets, moet u apparaatdetectiecode opnemen op uw mobiele site of toepassing. Deze code schakelt tussen een iPhone- of iPad-videobeleving, afhankelijk van het afspeelapparaat. Een mobiele voorinstelling kiezen voor het leveren van videobestanden naar de iPad is een eenvoudigere workflow. De reden hiervoor is dat u hetzelfde videobestand kunt gebruiken voor zowel iPhones als iPads. De kwaliteit wordt echter gestandaardiseerd aan de hand van de iPhone-ervaring met lagere resolutie.

      * Selecteer Naam of Grootte onder de groep Coderingsvoorinstellingen in de vervolgkeuzelijst Codering sorteren om voorinstellingen op naam of grootte te sorteren.
      * Selecteer een coderingsvoorinstelling op basis van de resolutiegrootte en de bandbreedte waarmee u de video wilt afspelen.
      * U kunt Adaptieve videocodering en een of meer coderingsvoorinstellingen per video selecteren. U kunt bijvoorbeeld een bestand coderen voor zowel desktop als mobiel in één uploadtaak.

Nadat u **[!UICONTROL Start Upload]**, wordt het oorspronkelijke primaire videobestand geüpload en worden gecodeerde bestanden gegenereerd vanuit het primaire bestand.

### Voorinstellingsopties voor codering {#about-encoding-preset-options}

De volgende parameters van de coderingsvoorinstellingsopties zijn beschikbaar:

* **[!UICONTROL Target connection speed]**: De verbindingssnelheid van de beoogde eindgebruiker.

* **[!UICONTROL Encoded file suffix]**: Het achtervoegsel dat voor identificatiedoeleinden aan het gecodeerde videobestand is gekoppeld.

* **[!UICONTROL Video bit rate (data rate)]**: De hoeveelheid gegevens die wordt gecodeerd om één seconde video af te spelen (in kilobits per seconde).

* **[!UICONTROL Pixel Width/Height]**: De breedte-afmetingen van de schermafbeelding, in pixels; de hoogte-afmetingen van de schermafbeelding (in pixels).

* **[!UICONTROL Frame per second (fps)]**: Het aantal frames, of stilstaande beelden, voor elke seconde van de video. In de Verenigde Staten en Japan wordt de meeste video opgenomen met een snelheid van 29,97 fps; in Europa en Azië (behalve Japan) wordt de meeste video opgenomen met een snelheid van 25 fps. De film is gemaakt met 24 fps.

* **[!UICONTROL Audio bit rate]**: De hoeveelheid gegevens die is gecodeerd om één seconde audio af te spelen, in kilobits per seconde.

In de volgende tabellen vindt u de aanbevolen werkwijzen voor het selecteren van videovoorinstellingen en de naamgevingsconventies die worden gebruikt om gecodeerde bestanden aan te wijzen.

### Adaptieve video (standaard) {#adaptive-video-default}

Een coderingsvoorinstelling die werkt met een willekeurige hoogte-breedteverhouding, zodat u video&#39;s kunt maken voor levering op mobiele apparaten, tablets en desktops. Geüploade bronvideo&#39;s die zijn gecodeerd met deze voorinstelling (de standaardinstelling en een aanbevolen werkwijze) worden ingesteld op een vaste hoogte terwijl de breedte automatisch wordt geschaald om de hoogte-breedteverhouding van de video te behouden.

**Adaptieve video (standaard)**

|  | Naam/knopinfotekst coderen van voorinstelling | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | FPS | Audiobitsnelheid (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Automatisch × 360, 800 Kbps | _Mobile_Auto×360p_800K | 800 | Automatisch×360 | Gelijk aan bron | 64 | Voor mobiele apparaten (iPhone, iPad, Android™) |
| 2 | Automatisch × 480, 1400 Kbps | _Tablet_Auto×480p_1400K | 1400 | Automatisch×480 | Gelijk aan bron | 96 | Voor tablets (iPad, Android™) |
| 3 | Automatisch × 720, 2600 Kbps | _Desktop_Auto×720p_2600K | 2600 | Automatisch×720 | Gelijk aan bron | 128 | Voor bureaublad |

### Voorinstellingen voor adaptieve videocodering (16:9 of 4:3) {#adaptive-video-encoding-or-video-presets}

Deze voorinstellingen voor adaptieve videocodering combineren een reeks afzonderlijke coderingsvoorinstellingen die automatisch voor u worden geselecteerd op basis van de hoogte-breedteverhouding van de video die u hebt geüpload. Als u bijvoorbeeld een 4:3-video uploadt, wordt deze automatisch gecodeerd met alle vijf voorinstellingen van 4:3 die zich in de lijst met primaire voorinstellingen in het dialoogvenster **Adaptieve videocodering (16:9 of 4:3)** -optie.

Zie voor informatie over parameters voor coderingsopties [Voorinstellingsopties voor codering](application-setup.md#about_encoding_preset_options).

**Voorinstellingen voor Adaptieve videocodering (16:9 of 4:3)**

|  | Naam/knopinfotekst coderen van voorinstelling | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | FPS | Audiobitsnelheid (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | Gelijk aan bron | 80 | Normale resolutie, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | Gelijk aan bron | 80 | Normale resolutie, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | Gelijk aan bron | 96 | Hoge resolutie, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | Gelijk aan bron | 96 | Hoge resolutie, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Gelijk aan bron | 128 | High-definition, breedbeeldscherm |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | Gelijk aan bron | 128 | High-definition |

### Voorinstellingen voor videocodering op bureaublad {#desktop-video-encoding-presets}

Voorinstellingen voor videocodering voor MP4 en OGV op bureaubladcomputers.

Zie voor informatie over parameters voor coderingsopties [De voorinstellingsopties voor codering](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2: audio-AAC, MP4-bestandsextensie**

|  | Naam/knopinfotekst coderen van voorinstelling | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | FPS | Audiobitsnelheid (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Gelijk aan bron | 64 | Lage breedbeeldresolutie |
| 2 | 16:9, 640 x 360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | Gelijk aan bron | 80 | Gemiddelde breedbeeldresolutie |
| 3 | 16:9, 800 x 450 (1.200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Gelijk aan bron | 128 | High-definition, breedbeeldscherm |
| 5 | 4:3, 320 x 240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | Gelijk aan bron | 64 | Lage resolutie |
| 6 | 4:3, 480 x 360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Gelijk aan bron | 80 | Normale resolutie |
| 7 | 4:3, 640 x 480 (1.200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640x480 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280x960 | Gelijk aan bron | 128 | High-definition |

**OGG Theora Vorbis: OGV-bestandsextensie**

|  | Naam/knopinfotekst coderen van voorinstelling | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videogegevenssnelheid (Kbps) | Breedte/Hoogte (pixels) | FPS | Audiobitsnelheid (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Gelijk aan bron | 64 | Lage breedbeeldresolutie |
| 2 | 16:9, 640 x 360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | Gelijk aan bron | 80 | Gemiddelde breedbeeldresolutie |
| 3 | 16:9, 800 x 450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | Gelijk aan bron | 128 | High-definition, breedbeeldscherm |
| 5 | 4:3, 320 x 240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | Gelijk aan bron | 64 | Lage resolutie |
| 6 | 4:3, 480 x 360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Gelijk aan bron | 80 | Normale resolutie |
| 7 | 4:3, 640x480 (1.200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | Gelijk aan bron | 96 | Gemiddelde resolutie |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | Gelijk aan bron | 128 | High-definition |

### Voorinstellingen voor mobiele videocodering {#mobile-video-encoding-presets}

Hetzelfde als bron-fps. Voorinstellingen voor videocodering voor mobiele iPhone-, iPad- en Android™-apparaten.

Zie voor informatie over parameters voor coderingsopties [De voorinstellingsopties voor codering](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1: Audio AAC, MP4-bestandsextensie**

|  | Naam/knopinfotekst coderen van voorinstelling | Doelverbindingssnelheid (Kbps) | Achtervoegsel van gecodeerd bestand | Videobitsnelheid (Kbps) | Pixelbreedte/-hoogte | FPS | Audiobitsnelheid (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, mobiel (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 2 | 16:9, 512 x 288, mobiel (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 3 | 16:9, 512 x 288, mobiel (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Gelijk aan bron | 80 | Normale resolutie, Wi-Fi |
| 4 | 16:9, 512 x 288, mobiel (1000 Kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | Gelijk aan bron | 80 | Hoge resolutie, Wi-Fi |
| 5 | 16:9, 512 x 288, mobiel (1200 Kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | Gelijk aan bron | 96 | Hoge resolutie, Wi-Fi |
| 6 | 4:3, 384 x 288, mobiel (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Gelijk aan bron | 64 | Lage resolutie, 3G |
| 7 | 4:3, 384 x 288, mobiel (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | Gelijk aan bron | 64 | Normale resolutie, 3G |
| 8 | 4:3, 448 x 336, mobiel (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Gelijk aan bron | 80 | Normale resolutie, Wi-Fi |
| 9 | 4:3, 448 x 336, mobiel (1000 Kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | Gelijk aan bron | 80 | Hoge resolutie, Wi-Fi |
| 10 | 4:3, 448 x 336, mobiel (1200 Kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | Gelijk aan bron | 96 | Hoge resolutie, Wi-Fi |

## Voorinstellingen viewer {#viewer-presets}

>[!NOTE]
>
>**Eindbericht voor Flash Viewers**: Met ingang van 31 januari 2017 heeft Adobe Dynamic Media Classic officieel de ondersteuning van het viewerplatform voor Flash beëindigd.

A *Voorinstelling viewer* is een verzameling instellingen die bepalen hoe gebruikers rich-media-elementen op hun computerschermen en mobiele apparaten weergeven. Als beheerder kunt u Viewer-voorinstellingen maken. Er zijn instellingen beschikbaar voor een array met viewerconfiguratieopties. U kunt bijvoorbeeld de weergavegrootte, het zoomgedrag, de kleurenschema&#39;s, de randen en de lettertypen van de viewer wijzigen.

U kunt het beste Adobe Dynamic Media Classic HTML5-videoviewers gebruiken. De voorinstellingen die worden gebruikt in HTML5-videoviewers zijn robuuste videospelers.

Door het volgende te combineren in één speler:

* De mogelijkheid om de afspeelcomponenten te ontwerpen met behulp van HTML5 en CSS.
* Afspelen ingesloten hebben.
* Gebruik adaptieve en progressieve streaming afhankelijk van de browsermogelijkheden.

U vergroot het bereik van uw rijke media-inhoud tot gebruikers op het bureaublad, het tablet en het mobiele apparaat en zorgt voor een gestroomlijnde videobeleving.

Zie [Informatie over HTML5-viewers](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) in de Adobe Viewers Reference Guide.

Zie [Compatibiliteitsmatrix voor Adobe Dynamic Media Classic Viewer-voorinstellingen](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Zie [Tips en trucs: De HTML5-videoviewer gebruiken](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Afhankelijk van de viewer kunt u communityfuncties toevoegen. De communautaire eigenschappen omvatten een Embed knoop, E-mail knoop, de knoop van de Verbinding, en de knoop van de Plaats van het Bezoek. Met deze knoppen kunnen mensen die de viewers gebruiken de viewer delen met anderen of de Adobe Dynamic Media Classic-website openen.

Zie ook [Voorbeelden van Adobe Viewers Reference Library](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Viewer-ondersteuning voor responsieve webpagina&#39;s {#viewer-support-for-responsive-designed-web-pages}

Verschillende webpagina&#39;s hebben verschillende behoeften. Soms wilt u een Web-pagina die een verbinding verstrekt die de HTML5 Kijker in een afzonderlijk browser venster opent. In andere gevallen moet u de HTML5 Viewer rechtstreeks insluiten op de hostpagina. In het laatste geval heeft de webpagina waarschijnlijk een statische lay-out. Of de interface reageert op een ander scherm en wordt op verschillende apparaten of voor verschillende venstergrootten van de browser anders weergegeven. Om aan deze behoeften te voldoen, steunen de HTML5 Viewers die met Adobe Dynamic Media Classic zowel statische Web-pagina&#39;s als responsieve Web-pagina&#39;s komen.

Voor meer informatie over hoe te om ontvankelijke kijkers op uw Web-pagina&#39;s in te bedden, zie [De bibliotheek met responsieve afbeeldingen](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api), [Responsieve afbeeldingsbibliotheek gebruiken](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api), en [Command reference: Command attributes](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library).

### Voorinstellingstypen voor viewer {#viewer-preset-types}

Beheerders kunnen de volgende typen voorinstellingen voor viewers maken en aanpassen:

* **[!UICONTROL eCatalog Viewer]**: Hiermee simuleert u het lezen van een afgedrukte catalogus. U kunt van pagina naar pagina gaan, in- en uitzoomen op items op een pagina, Afbeeldingen met hyperlinks gebruiken om meer informatie over items op de pagina weer te geven of de catalogus doorzoeken. U kunt ook een deelvenster Info opnemen om gedetailleerde informatie weer te geven en een item waaraan een afbeelding is toegewezen als het kaartgebied een geldig kenmerk rollover_key heeft. Als u een deelvenster Info wilt opnemen, geeft u een URL voor de Informatieserver op in het deelvenster Instellingen van het deelvenster Info van het voorinstellingenvenster van de eCatalog Viewer.

* **[!UICONTROL Swatch Set Viewer]**: Hiermee geeft u een afbeelding weer in een andere kleur, in een ander materiaal, in een andere structuur, in een andere afwerking of in een andere structuur. Gebruikers selecteren een miniatuur om de variaties in de afbeelding te zien.

* **[!UICONTROL Mixed Media Set Viewer]**: geeft verschillende typen media weer in één viewer. U kunt staalsets, centrifuges, afbeeldingen en video&#39;s opnemen. U kunt tabbladen instellen voor verschillende typen inhoud, zoals een tabblad voor Afbeeldingssets en een tabblad voor video&#39;s. Voor video&#39;s die worden afgespeeld vanuit een gemengde mediaset, wordt een standaard Video-viewer gebruikt met een tijdlijn en videobesturingselementen, zoals Stoppen, Pauzeren, Terugspoelen en Afspelen. Wanneer u een voorinstelling voor een gemengde mediaset voor de viewer instelt, geeft u op welke viewers u wilt gebruiken voor de verschillende typen elementen in de gemengde mediaset. U kunt ook de rasterviewer of de Carousel Viewer gebruiken om een gemengde mediaset weer te geven.

* **[!UICONTROL Spin Set Viewer]**: Deze modus biedt meerdere weergaven van een afbeelding, zodat gebruikers het object kunnen draaien om de verschillende zijden en hoeken te bekijken.

* **Video Viewer**: Hiermee geeft u video&#39;s weer met de resolutieafmetingen van het bronbestand of een aangepaste grootte. Adobe Dynamic Media Classic wordt geleverd met veel vooraf gedefinieerde Viewer-voorinstellingen voor het afspelen van video. Als u een beheerder bent, kunt u aangepaste Video Viewer-voorinstellingen maken. Er zijn meer dan 12 verschillende instellingen voor het configureren van de Video Viewer. U kunt het volgende configureren:

   * size
   * voor- en achtergrondkleur
   * besturingselementen voor video en audio
   * voortgangsbalk
   * user-interface skin
   * sociale kenmerken
   * en Help

* **[!UICONTROL Zoom Viewers]**: Biedt een keuze uit drie typen zoomviewers:

* **[!UICONTROL Zoom Viewer]**: Hiermee kunnen gebruikers inzoomen op het gebied door het te selecteren. Ze kunnen besturingselementen selecteren om in te zoomen, uit te zoomen en de standaardgrootte van de afbeelding te herstellen.

* **[!UICONTROL Zoom Viewer: Fly-out]**: geeft een tweede afbeelding van het ingezoomde gebied weer naast de oorspronkelijke afbeelding. Er zijn geen besturingselementen om te gebruiken. Gebruikers verplaatsen de selectie over het gebied dat ze willen weergeven.

Houd er bij het bepalen van het totale bandbreedtegebruik voor deze viewer rekening mee dat zowel de hoofdafbeelding als de vervolgafbeelding in de viewer worden weergegeven. De grootte van de vervolgafbeelding wordt bepaald door de grootte van de hoofdafbeelding (breedte en hoogte van werkgebied) en de zoomfactor. Als u wilt voorkomen dat het flyout-bestand te groot wordt, brengt u de volgende twee waarden met elkaar in evenwicht: als u een grote hoofdafbeeldingsgrootte hebt, verlaagt u de waarde voor Zoomfactor. (De breedte en hoogte van de Flyout bepalen de grootte van het wegvliegvenster, maar niet de grootte van het vliegend beeld dat aan de kijker wordt gediend.)

Als de hoofdafbeelding bijvoorbeeld 350 x 350 pixels groot is, met een zoomfactor van 3, is de resulterende uitvliegafbeelding 1050 x 1050 pixels. Als de hoofdafbeeldingsgrootte 300 x 300 pixels is, met een zoomfactor van 4, is de vervolgafbeelding 1200 x 1200 pixels. Afhankelijk van de kwaliteitsinstelling JPEG (aanbevolen instellingen liggen tussen 80 en 90), kunt u de bestandsgrootte aanzienlijk verkleinen. De aanbevolen zoomfactoren zijn 2,5 tot 4, afhankelijk van de grootte van de hoofdafbeelding.

### Compatibiliteitsmatrix voor Adobe Dynamic Media Classic Viewer-voorinstellingen {#scene-viewer-preset-compatibility-matrix}

**Eindbericht voor Flash Viewers**: Met ingang van 31 januari 2017 heeft Adobe Dynamic Media Classic officieel de ondersteuning van het viewerplatform voor Flash beëindigd.

In de volgende tabel worden de momenteel beschikbare Adobe Dynamic Media Classic Viewer-voorinstellingen weergegeven. In de tabel wordt ook aangegeven of de viewer compatibel is met mobiele en desktopapparaten en welke technologie voor elke viewer wordt gebruikt.

Zie ook [Voorbeelden van Adobe Viewers Reference Library](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Voor informatie over ondersteunde webbrowsers en besturingssysteemversies voor Viewers kunt u de Opmerkingen bij de release van Viewers bekijken.

Zie [Opmerkingen bij de release Adobe Viewers](https://experienceleague.adobe.com/nl/docs/dynamic-media-developer-resources).

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Zoomviewers |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML 5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML 5 | X | X | X | X | X |
| Universal_HTML5_Zoomen_donker | HTML 5 | X | X | X | X | X |
| Universal_HTML5_Zoomen_licht | HTML 5 | X | X | X | X | X |


|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Afbeeldingssetviewers |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML 5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_donker | HTML 5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML 5 | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Viewers voor stalensets |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML 5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_black | HTML 5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML 5 | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog-viewers |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Bevat ondersteuning voor sociale media en zoeken naar catalogi.) | HTML 5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Inclusief ondersteuning voor sociale media en zoeken naar catalogi.) | HTML 5 | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Weergaven draaien |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_donker | HTML 5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML 5 | X | X | X | X | X |

**eVideo-viewers**

Adobe Dynamic Media Classic ondersteunt het afspelen van mobiele video voor MP4 H.264-video.

* U kunt de apparaten van BlackBerry® vinden die dit videoformaat bij het volgende steunen: [Ondersteunde video-indelingen op BlackBerry®](https://developers.blackberry.com/us/en)
* U kunt ook de volgende Windows®-apparaten vinden die deze video-indeling ondersteunen: [Ondersteunde video-indelingen op Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet | BlackBerry® Smartphone | Windows®-telefoon |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Inclusief ondersteuning voor ondertiteling.) Zie [Beste praktijken: Het gebruiken van de Universele HTML5 Videokijker.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML 5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Inclusief ondersteuning voor ondertiteling en sociale media.) | HTML 5 | X | X | X | X | X | X | X |

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Gemengde mediasetviewers |  |  |  |  |  |  |
| Universal_HTML5_GemengdMedia_donker | HTML 5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML 5 | X | X | X | X | X |

### Ondersteunde matrix voor bewegingen voor mobiele viewers {#supported-mobile-viewers-gestures-matrix}

In de volgende tabel worden de bewegingen van de mobiele viewer weergegeven die worden ondersteund op iOS-, Android™ 2.x- en Android™ 3.x-apparaten.

|  | Viewertechnologie | Desktop | Apple iPhone | Apple iPad | Android™-smartphone | Android™-tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Afbeeldingssetviewers |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML 5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_donker | HTML 5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML 5 | X | X | X | X | X |

### Het scherm Viewer Preset {#about-the-viewer-preset-screen}

Maak en beheer Viewer Presets op het scherm Viewer Presets. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

Het scherm Voorinstellingen viewer bevat gereedschappen voor de volgende taken:

* **Een voorinstelling toevoegen**: Select **[!UICONTROL Add]** en maakt u keuzen in het dialoogvenster Voorinstelling viewer toevoegen.

      Zie [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).
  
* **Een voorinstelling bewerken**: Selecteer een voorinstelling en selecteer **[!UICONTROL Edit]**.

      Zie [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).
  
* **Een voorinstelling verwijderen**: Selecteer een voorinstelling en selecteer **[!UICONTROL Delete]**.

* **Een voorinstelling exporteren**: Selecteer een HTML5 Viewer-voorinstelling. Klik vervolgens op **[!UICONTROL Export]** om de viewerskin te downloaden, zodat u deze kunt gebruiken als basis voor het maken en toevoegen van een andere Viewer-voorinstelling.

      Zie [Een HTML5 Viewer-voorinstelling exporteren](application-setup.md#exporting_an_html5_viewer_preset).
  
* **De voorinstellingenlijst van de viewer filteren**: Gebruik deze gereedschappen om de lijst te filteren:

      * Open de vervolgkeuzelijst **Actief/Inactief** en selecteer een optie om actieve voorinstellingen, inactieve voorinstellingen of alle voorinstellingen weer te geven.
      * Open de vervolgkeuzelijst **Viewer** en selecteer een optie om alleen bepaalde viewers weer te geven. Selecteren **[!UICONTROL All Viewers]** om alle viewers weer te geven.
  
* **Voorinstellingen sorteren**: Selecteer een kolomkop (**[!UICONTROL Active]**, **[!UICONTROL Type]**, **[!UICONTROL Preset]**, of **[!UICONTROL Platform]**) om de lijst in een kolom te sorteren. Selecteer nogmaals een kolomkop om de lijst in aflopende (of oplopende) volgorde te sorteren.

* **Voorinstellingen activeren en deactiveren**: Selecteer een voorinstelling en selecteer vervolgens de optie Actief, zodat u deze kunt activeren of deactiveren.

      Zie [Viewer Presets activeren of deactiveren](application-setup.md#activating_or_deactivating_viewer_presets).
  
>[!NOTE]
>
>Selecteren **[!UICONTROL Preview]** aan de rechterkant van de pagina Voorinstellingen viewer, zodat u kunt zien hoe een element eruitziet in de door u geselecteerde voorinstelling voor viewers. Als u een ander element wilt zien, selecteert u **[!UICONTROL Browse]** op de pagina Voorinstellingen viewer en selecteer een ander element in het dialoogvenster Voorvertoning van element selecteren.

### Viewer-voorinstellingen toevoegen en bewerken {#adding-and-editing-viewer-presets}

Naast het toevoegen van Kijker vooraf instelt door te gebruiken **[!UICONTROL Add]** in de gebruikersinterface kunt u ook **[!UICONTROL Export]** om een Viewer-voorinstelling toe te voegen. U exporteert gewoon een bestaande HTML5 Viewer-voorinstelling en gebruikt deze als basis voor de nieuwe voorinstelling.

Zie [Voorinstelling HTML5-viewer exporteren](application-setup.md#exporting_an_html5_viewer_preset).

Zie ook [Voorinstellingen viewer](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) trainingsvideo.

**Viewer-voorinstellingen toevoegen en bewerken:**

1. Ga in de rechterbovenhoek van Adobe Dynamic Media Classic naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

   U kunt filteren op de lijst met voorinstellingen. Als u bijvoorbeeld alleen voorinstellingen voor videoviewers wilt weergeven, selecteert u Video-viewer in het vervolgkeuzemenu Viewers op de werkbalk direct boven de tabel.

1. Voeg op de pagina Voorinstellingen viewer de voorinstelling Viewer toe of bewerk deze in het scherm Voorinstellingen viewer.

   * **Toevoegen**: Selecteer op de werkbalk **[!UICONTROL Add]**. Selecteer een platform in het dialoogvenster Voorinstelling viewer toevoegen en selecteer een type rich-media-element.

         Selecteren **[!UICONTROL Save As]** wanneer u klaar bent met het maken van de voorinstelling Viewer.
     
   * **Toevoegen door te beginnen met een bestaande viewervoorinstelling**: Selecteer in de tabel een voorinstelling voor de video-viewer en selecteer **[!UICONTROL Edit]** op de werkbalk.

         Selecteer **&#x200B; nadat u de video-viewer opnieuw hebt geconfigureerd[!UICONTROL Save As]** om de voorinstelling op te slaan onder een andere naam in het tekstveld Naam voorinstelling.
     
   * **Bewerken**: Selecteer een bestaande Viewer-voorinstelling en selecteer **[!UICONTROL Edit]**.

1. Typ of bewerk de naam van de voorinstelling in het veld Naam voorinstelling op de pagina Viewer configureren.
1. Stel de overige gewenste opties in.

   >[!NOTE]
   >
   >Selecteren **[!UICONTROL Same As Source]** zodat u de grootte van de video-viewer automatisch kunt aanpassen aan de grootte van de resolutie van de gecodeerde video zelf. Als u deze optie selecteert, kunt u de breedte van het werkgebied en de hoogte van het werkgebied niet invoeren. In plaats daarvan komen deze opties uit de video zelf. Als u **[!UICONTROL Same As Source]**, stelt u de optie Grootte marge in om de afmetingen van de skin buiten het afspeelgebied van de video weer te geven. Deze margegrootte is de pixelhoogte en -breedte van de videobesturingselementen. U kunt de volgende afbeelding gebruiken om de margegrootten te bepalen die u wilt gebruiken.*

   ![Margeconfiguratie van videoviewer](assets/vs_video_viewer_configure_margin.png)

1. Voer een van de volgende handelingen uit:

   * Selecteren **[!UICONTROL Save As]** als u een Viewer-voorinstelling hebt toegevoegd door te beginnen met een bestaande voorinstelling.
   * Selecteren **[!UICONTROL Save]** als u een voorinstelling voor de viewer hebt toegevoegd of bewerkt.

### Een voorinstelling voor een HTML5-viewer exporteren {#exporting-an-html-viewer-preset}

U kunt een bestaande voorinstelling voor de HTML5-viewer exporteren en deze gebruiken als basis voor het maken van een HTML5-viewervoorinstelling. Deze exportoptie is handig omdat u de viewer niet helemaal opnieuw hoeft te maken. In plaats daarvan exporteert u een voorinstelling die er zo uitziet en zich dicht bij u gedraagt. Vervolgens kunt u deze voorinstelling als uitgangspunt gebruiken om ontwerpaanpassingen aan te brengen.

Alle standaard CSS-bestanden met een voorinstelling voor een buitenverpakking in Adobe Dynamic Media Classic gebruiken relatieve paden die dienen als basis voor afbeeldingen die verwijzen naar elementen op `Scene7SharedAssets`. Hieronder ziet u bijvoorbeeld een relatief pad naar een afbeeldingselement in een CSS-bestand met voorinstellingen voor viewers op

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Als u echter CSS-bestanden van de viewer host op uw eigen site, moet u deze relatieve paden naar afbeeldingen oplossen door in uw eigen omgeving een expliciet pad naar de afbeeldingsserver te gebruiken. Als u bijvoorbeeld het relatieve pad boven een expliciet pad hebt bijgewerkt, ziet het er als volgt uit: `https://s7d1.scene7.com` is de directe weg aan uw Server van het Beeld: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Een HTML5 Viewer-voorinstelling exporteren:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Selecteer in de tweede vervolgkeuzelijst links op de werkbalk Voorinstellingen viewer de optie **[!UICONTROL HTML5]**.
1. Selecteer in de derde vervolgkeuzelijst aan de linkerkant de optie **[!UICONTROL All Viewers]**.
1. Selecteer de Viewer-voorinstelling die u als basis voor een nieuwe HTML5 Viewer-voorinstelling wilt gebruiken.
1. Selecteer in de werkbalk de optie **[!UICONTROL Export]**.
1. In het dialoogvenster Geselecteerde elementen exporteren selecteert u **[!UICONTROL Submit Export]**.

   Na het exporteren krijgt u een CSS-bestand. Download en decomprimeer het bestand.

1. Open het CSS-bestand in een CSS-editor, breng de wijzigingen aan en sla het bestand op.
1. Upload het CSS-bestand naar Adobe Dynamic Media Classic.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Publiceer het CSS-bestand naar de Dynamic Media Image Server.

   Zie [Bestanden publiceren](publishing-files.md#publishing_files).

1. Voeg de nieuwe voorinstelling voor de viewer op de gebruikelijke wijze toe. Selecteer het CSS-bestand van de viewer dat u hebt geüpload.

   Zie [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).

### Viewer-voorinstellingen activeren of deactiveren {#activating-or-deactivating-viewer-presets}

Als u een URL wilt maken voor het weergeven van elementen, openen gebruikers de vervolgkeuzelijst Voorinstellingen in het dialoogvenster Voorvertoning, selecteert u een voorinstelling voor de viewer en selecteert u **[!UICONTROL Copy URL]** (zie [De URL van een voorinstelling voor viewers kopiëren](application-setup.md#copying_the_url_of_a_viewer_preset)). Deze lijst Voorinstellingen bevat voorinstellingen voor viewers die beheerders toevoegen en beheren in het scherm Voorinstellingen viewer. Alle actieve voorinstellingen voor de eCatalog-viewer worden bijvoorbeeld weergegeven in de vervolgkeuzelijst Voorinstellingen in het dialoogvenster Voorvertoning wanneer een gebruiker een voorvertoning van een eCatalog weergeeft.

Tenzij u de Viewer-voorinstellingen in het scherm Voorinstellingen viewer deactiveert, kan de vervolgkeuzelijst Voorinstellingen in het dialoogvenster Voorvertoning vol raken.

**Viewer-voorinstellingen activeren of deactiveren:**

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Schakel op de pagina Voorinstellingen viewer de optie **[!UICONTROL Active]** opties om Viewer-voorinstellingen te activeren of te deactiveren.

### De URL van een voorinstelling voor viewers kopiëren {#copying-the-url-of-a-viewer-preset}

Nadat u een element hebt gepubliceerd, kunt u een URL kopiëren voor het weergeven van het element met de instellingen uit een voorinstelling voor de viewer.

De URL wordt naar het klembord gekopieerd. U kunt het zonodig in de code van HTML van uw Web-pagina, mobiel apparaat, of toepassing gebruiken.

**De URL van een voorinstelling voor viewers kopiëren:**

1. Selecteer het element in het deelvenster Bladeren.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteren **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer in de URL&#39;s en het deelvenster Code insluiten aan de rechterkant de optie **[!UICONTROL Copy URL]** rechts van de gewenste viewer.
   * Selecteren **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Copy URL]**.

   * Selecteren **[!UICONTROL List View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens rechts van de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Copy URL]**.

   * Selecteren **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Copy URL]**.

### De insluitcode van een viewervoorinstelling kopiëren {#copying-the-embed-code-of-a-viewer-preset}

Met de functie Code insluiten kunt u de viewercode voor de geselecteerde Viewer-voorinstelling controleren. U kunt de code aan het klembord ook kopiëren zodat kunt u het in uw Web-pagina&#39;s voor plaatsing van de kijker kleven.

U mag de code niet bewerken in het dialoogvenster Code insluiten.

**De insluitcode van een voorinstelling voor de viewer kopiëren:**

1. Selecteer het element in het deelvenster Bladeren van element.
1. Voer boven het deelvenster Asset Browse een van de volgende handelingen uit aan de rechterkant van de werkbalk:

   * Selecteren **[!UICONTROL Grid View]**. Dubbelklik in het deelvenster Asset Browse op één element om dit te openen in de gedetailleerde weergave. Selecteer in het deelvenster URL&#39;s aan de rechterkant de optie **[!UICONTROL Embed Code]**.
   * Selecteren **[!UICONTROL Grid View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens onder de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Embed Code]**.

   * Selecteren **[!UICONTROL List View]**. Selecteer in het deelvenster Asset Browse één element en ga vervolgens rechts van de miniatuurafbeelding naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Embed Code]**.

   * Selecteren **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, of **[!UICONTROL Detail View]**. Ga op dezelfde werkbalk naar **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Selecteer in de pagina Viewer List onder de kolom Acties van de tabel de optie **[!UICONTROL Embed Code]**.

1. Selecteer in het dialoogvenster Code insluiten **[!UICONTROL Copy to Clipboard]**.
1. Selecteren **[!UICONTROL Close]**.

## Standaardviewers configureren {#configure-default-viewers}

Met Standaardviewers kunt u de standaardviewer configureren die aan een element is gekoppeld wanneer u Voorvertoning in Adobe Dynamic Media Classic gebruikt. U kunt de standaardvoorbeeldervaring instellen voor de volgende elementtypen:

* Afbeelding
* Video
* SpinSet
* Catalogus
* ImageSet
* SwatchSet
* MediaSet

**Standaardviewers configureren:**

1. Selecteer in de vervolgkeuzelijst Instellen de optie **[!UICONTROL Application Setup]**.
1. Ga in het venster Setup (Instellingen) in het linkerdeelvenster naar **[!UICONTROL Application Setup]** > **[!UICONTROL Viewers]**
1. Selecteren **[!UICONTROL Default Viewers]**.
1. Selecteer in het venster Standaardviewers in de vervolgkeuzelijst voor elk elementtype de viewer die u aan de voorvertoning van het element wilt koppelen.
1. Selecteer in de rechterbenedenhoek van het venster Standaardviewers de optie **[!UICONTROL Save Settings]**.
1. Selecteer in de rechterbenedenhoek van het venster Instellen de optie **[!UICONTROL Close]** om terug te keren naar het venster Middelen.

## Weergaven metagegevens {#metadata-views}

*Metagegevens* is gestandaardiseerde informatie over een actief. U kunt metagegevens gebruiken om uw workflow te stroomlijnen, uw elementen te ordenen en het zoeken te verbeteren. Adobe Dynamic Media Classic ondersteunt de IPTC-standaard (International Press Telecommunications Council) en de XMP (Extensible metadata Platform). Voordat gebruikers metagegevens over een element weergeven of invoeren in de gedetailleerde weergave, kunnen ze het menu Weergaven metagegevens openen. Hiervanaf kunnen ze de set metagegevensvelden selecteren die ze willen bekijken of gebruiken om het element te beschrijven.

Adobe Dynamic Media Classic wordt geleverd met vooraf gedefinieerde weergaven van metagegevens en beheerders kunnen hun eigen weergaven van metagegevens maken, zodat gebruikers kunnen kiezen wanneer ze metagegevens invoeren.

### Een metagegevensweergave maken {#creating-a-metadata-view}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Selecteren **[!UICONTROL Add]**.
1. Typ een naam voor de weergave in het tekstveld Naam voorinstelling.
1. (Optioneel) Schakel **[!UICONTROL Make Default]** om van deze weergave de weergave te maken die gebruikers zien wanneer zij het deelvenster Metagegevens openen in de gedetailleerde weergave.
1. (Optioneel) Selecteer **[!UICONTROL Include UDF]** om door de gebruiker gedefinieerde velden op te nemen in de weergave. Door gebruiker gedefinieerde velden staan boven aan het deelvenster Metagegevens in de gedetailleerde weergave.
1. Selecteer de velden die u voor de weergave wilt gebruiken (selecteer **[!UICONTROL Select All]** om alle velden te selecteren).
1. Selecteren **[!UICONTROL Save]**.

   De geselecteerde categorieën en velden voor de weergave worden weergegeven in het deelvenster Voorbeeld.

### Weergaven van metagegevens beheren {#managing-metadata-views}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Voer een van de volgende handelingen uit:

   * Als u een voorvertoning van een weergave wilt weergeven, selecteert u deze. De velden in de weergave worden weergegeven in het deelvenster Voorvertoning.
   * Als u een weergave wilt bewerken, selecteert u deze en selecteert u vervolgens **[!UICONTROL Edit]**. Schakel vervolgens veldnamen in of uit in het deelvenster Voorvertoning en selecteer de optie **[!UICONTROL Include UDF]** -optie.
   * Als u een weergave wilt verwijderen, selecteert u deze en selecteert u vervolgens **[!UICONTROL Delete]**.
   * Als u een weergave als standaard wilt instellen, selecteert u deze en selecteert u vervolgens **[!UICONTROL Make Default]**. De standaardweergave is de weergave die gebruikers zien wanneer ze elementen openen in de gedetailleerde weergave en naar het deelvenster Metagegevens gaan.

## Voorinstellingen metagegevens {#metadata-presets}

Met voorinstellingen voor metagegevens kunnen beheerders de metagegevens beheren die aan elementen zijn toegewezen. In de Gedetailleerde weergave kan een gebruiker metagegevens over een element invoeren in velden die voor dat doel zijn opgegeven. Een gebruiker kan bijvoorbeeld een naam, copyrightbeschrijving en adres van de eigenaar invoeren. Om ervoor te zorgen dat gebruikers deze informatie correct en volledig invoeren, kunt u Voorinstellingen voor metagegevens maken. Als u een metagegevensvoorinstelling kiest in de gedetailleerde weergave, worden metagegevensvelden gevuld met vooraf gedefinieerde waarden. Zo worden automatisch een naam, copyrightbeschrijving en adres van de eigenaar ingevoerd.

Maak een voorinstelling voor metagegevens voor elke set waarden voor metagegevens die gebruikers automatisch moeten kunnen invoeren in de gedetailleerde weergave om een element te beschrijven.

### Een metagegevensvoorinstelling maken of bewerken {#creating-or-editing-a-metadata-preset}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Voer een van de volgende handelingen uit in het scherm Metagegevensvoorinstellingen:

   * Selecteer **[!UICONTROL Add]**. Typ een naam voor de voorinstelling in het tekstveld Naam sjabloon metagegevens. Selecteren **[!UICONTROL Metadata Views]** en selecteert u vervolgens een weergave in de vervolgkeuzelijst (zie [Weergaven metagegevens](application-setup.md#metadata_views)).
   * Als u een bestaande voorinstelling wilt bewerken, selecteert u de voorinstelling in de lijst Voorinstellingen metagegevens en selecteert u vervolgens **[!UICONTROL Edit]**.

1. Vouw de koppen uit die u in de voorinstelling wilt opnemen en voer waarden in in de verschillende velden die u in de voorinstelling wilt opnemen.
1. Selecteren **[!UICONTROL Save]**.

   De geselecteerde categorieën en velden voor de voorinstelling worden weergegeven in het deelvenster Voorvertoning.

### Metagegevensvoorinstellingen beheren {#managing-metadata-presets}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Voer een van de volgende handelingen uit:

   * Selecteer de voorinstelling waarvan u een voorvertoning wilt weergeven als u een voorinstelling wilt weergeven. De vooraf ingestelde informatie (categorieën en velden) wordt weergegeven in het voorvertoningsscherm.
   * Als u een voorinstelling wilt verwijderen, selecteert u de voorinstelling en selecteert u **[!UICONTROL Delete]**.

## Door gebruiker gedefinieerde velden {#user-defined-fields}

Een beheerder van Media Portal of een Beheerder van het Bedrijf kan douane, user-defined meta-gegevensgebieden tot stand brengen. Met aangepaste velden kunt u elementen ordenen in Adobe Dynamic Media Classic. U kunt de velden desgewenst als Actief markeren. Als deze optie is ingeschakeld, worden de namen van deze aangepaste metagegevensvelden weergegeven in het deelvenster Metagegevens in de gedetailleerde weergave. Gebruikers kunnen informatie invoeren in door de gebruiker gedefinieerde metagegevensvelden om elementen te beschrijven. Gebruikers kunnen ook een door de gebruiker gedefinieerd metagegevensveld als criterium gebruiken bij zoekopdrachten.

Een effectief gebruik van door de gebruiker gedefinieerde metagegevensvelden is het vertragen van de activeringstijd van een element voor een specifieke opstart of verkoop. U definieert een veld voor activering op basis van het type *Datum*. Vervolgens gebruikt u de **[!UICONTROL Metadata]** in de gedetailleerde weergave of **[!UICONTROL File]** > **[!UICONTROL Edit Info]** kunt u opgeven wanneer het element wordt geactiveerd. Adobe Dynamic Media Classic controleert de gepubliceerde status van een middel en de publicatiegeschiedenis. Als deze niet binnen de activeringstijd valt, wordt de publicatiestatus &#39;&#39;Niet gepubliceerd&#39;&#39; weergegeven.

>[!NOTE]
>
>Als u wilt dat door de gebruiker gedefinieerde velden worden weergegeven in het deelvenster Metagegevens in de gedetailleerde weergave, neemt u door de gebruiker gedefinieerde velden op in de weergave Metagegevens. Selecteer in het scherm Weergaven metagegevens de optie Inclusief UDF (door de gebruiker gedefinieerde velden). Zie voor meer informatie [Weergaven metagegevens](application-setup.md#metadata_views).

>[!NOTE]
>
>Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** en selecteer vervolgens **[!UICONTROL Include UDFs in Search]**. Zie [Persoonlijke instelling](personal-setup.md#personal_setup).

### Een door de gebruiker gedefinieerd metagegevensveld maken {#creating-a-user-defined-metadata-field}

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.
1. Selecteren **[!UICONTROL Add]**
1. Stel in het dialoogvenster Aangepast veld de gewenste opties in.

   * **[!UICONTROL Name]**: Voer een naam in voor het metagegevensveld.

   * **[!UICONTROL Type]**: Selecteer een optie waarmee het type informatie wordt gedefinieerd dat gebruikers kunnen invoeren in het metagegevensveld:

   * **[!UICONTROL String]**: Een tekstreeks.

   * **[!UICONTROL Int]**: Een geheel getal.

   * **[!UICONTROL Float]**: Een drijvende-kommagetal.

   * **[!UICONTROL Yes/No]**: Een Booleaanse waarde ja/nee.

   * **[!UICONTROL Date]**: Een datum. De notatie DD-MM-JJJJ wordt geaccepteerd.

   * **[!UICONTROL Filename]**: De naam van een bestand.

   * **[!UICONTROL Color]**: De naam van een kleur.

   * **[!UICONTROL Dimension]**: De breedte en hoogte van het element.

   * **[!UICONTROL Untyped]**: Voor achterwaartse compatibiliteit. Selecteer deze optie niet.

   * **[!UICONTROL Default Value]**: Optioneel. Voer de waarde in die gebruikers waarschijnlijk in het veld invoeren. De waarde die u invoert, wordt de standaardwaarde voor het veld dat u maakt.

   * **[!UICONTROL Applies To]**: Optioneel. Selecteer een elementtype als u het metagegevensveld alleen wilt toepassen op een bepaald type element.

     >[!NOTE]
     >
     >Selecteer een **[!UICONTROL Applies To]** zorgvuldig te wijzigen, omdat u de **[!UICONTROL Applies To]** nadat u een door de gebruiker gedefinieerd veld hebt gemaakt. Met Adobe Dynamic Media Classic kunt u de naam, het type en de standaardwaarde van een door de gebruiker gedefinieerd veld bewerken, maar niet de **[!UICONTROL Applies To]** instellen. *

1. Selecteren **[!UICONTROL Save]** als u klaar bent met het maken van het metagegevensveld.

### Door de gebruiker gedefinieerde velden beheren {#manage-user-defined-fields}

Het scherm Door gebruiker gedefinieerde velden bevat opdrachten voor het beheer van aangepaste, door de gebruiker gedefinieerde metagegevensvelden.

Alleen een beheerder van het Media Portal of een bedrijfsbeheerder kan door de gebruiker gedefinieerde velden beheren.

Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.

* **Een veld bewerken**: Selecteer het veld en selecteer vervolgens **[!UICONTROL Edit]**.

* **Een veld verwijderen**: Selecteer het veld en selecteer vervolgens **[!UICONTROL Delete]**.

* **Veld activeren**: Schakel de optie **[!UICONTROL Active]** naast de naam van een veld. Als u in een rol van het bedrijfbeleid bent, wordt deze optie niet getoond. Omdat deze optie met MediaPortal verwant is, moet u (draai) selecteren toont de Eigenschappen MediaPortal in Persoonlijke Opstelling om de geactiveerde gebieden te zien.

## Bestanden optimaliseren {#optimize-files}

Wanneer u bestanden uploadt naar de Adobe Dynamic Media Classic, worden deze geoptimaliseerd voor opslag en publicatie. Als het uploadproces wordt onderbroken, kunnen sommige afbeeldingen echter niet worden geoptimaliseerd. In dit geval wordt het bericht &quot;Afbeelding nog niet geoptimaliseerd&quot; weergegeven. U kunt deze bestanden echter optimaliseren als u een beheerder bent.

Adobe Dynamic Media Classic doorzoekt uw bestanden en optimaliseert alleen de afbeeldingen die nog niet volledig zijn geoptimaliseerd.

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** en selecteer vervolgens **[!UICONTROL Optimize Files]**.
1. Geef informatie op voor de optimalisatietaak en selecteer **[!UICONTROL Submit]**.

   Als u met meer dan één bedrijf werkt, optimaliseer dossiers die tot verschillende bedrijven afzonderlijk behoren.

## Voorinstellingen batchset {#batch-set-presets}

Gebruik de voorinstellingen Batch-set, zodat u automatisch afbeeldingssets of centrifuges kunt maken terwijl er een taak wordt uitgevoerd om elementen te uploaden naar Adobe Dynamic Media Classic.

De beheerders van het bedrijf bepalen eerst noemende overeenkomsten voor de activa die zij in een reeks willen groeperen. Vervolgens kunt u een voorinstelling Batch-set maken om naar deze afbeeldingen te verwijzen. Elke voorinstelling is een op zichzelf staande verzameling instructies met een unieke naam die definieert hoe de set moet worden samengesteld met afbeeldingen die overeenkomen met de gedefinieerde naamgevingsconventies in het vooraf ingestelde recept.

Alle actieve voorinstellingen voor batchsets voor een bedrijf worden weergegeven in het dialoogvenster Optie taak uploaden, zodat u kunt opgeven welke voorinstelling u wilt toepassen tijdens elke uploadsessie. Bedrijfsbeheerders zien alle actieve en inactieve voorinstellingen voor batchsets. Wanneer u bestanden uploadt, maakt Adobe Dynamic Media Classic automatisch een set met alle bestanden die overeenkomen met de gedefinieerde naamgevingsconventie in de actieve voorinstellingen.

### Standaardnaam {#default-naming}

De beheerder van het Bedrijf leidt tot een standaard noemende overeenkomst die in om het even welk Recipe van de Vooraf ingestelde Reeks van de Partij wordt gebruikt. De standaardnaamgevingsconventie die is geselecteerd in de definitie van Voorinstelling Batch kan alles zijn wat uw bedrijf nodig heeft om sets voor alle websites in batch te genereren. Er wordt een voorinstelling Batch-set gemaakt waarin de standaardnaamgevingsconventie wordt gebruikt die u definieert. U kunt zo vele Voorinstellingen Batch van de Reeks met afwisselende, douane noemende overeenkomsten tot stand brengen nodig voor een bepaalde reeks inhoud in gevallen waar er een uitzondering op het bedrijf-bepaalde gebrek het noemen is.

U hoeft geen standaardnaamgevingsconventie in te stellen als u de functie Voorinstelling batch instellen wilt gebruiken. Nochtans, adviseert de beste praktijken van de Adobe dat u een standaardnoemende overeenkomst gebruikt om zo vele elementen van uw noemende overeenkomst te bepalen die u in een reeks wilt groeperen. Zo kunt u het maken van Batch-sets stroomlijnen.

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**.
1. Selecteren **[!UICONTROL View Form]** of **[!UICONTROL View Code]** om op te geven hoe u informatie over elk element wilt weergeven en invoeren.

   U kunt de **[!UICONTROL View Code]** Schakel het selectievakje in om de waarde van de reguliere expressie naast de formulierselecties weer te geven. U kunt deze waarden invoeren of wijzigen om de elementen van de naamgevingsconventie te definiëren, als de formulierweergave u beperkt om welke reden dan ook. Als uw waarden niet kunnen worden geparseerd in de formulierweergave, worden de formuliervelden inactief.

   >[!NOTE]
   >
   >De-geactiveerde formuliervelden geven geen ongeldige reguliere expressie aan. Er is geen validatie die aangeeft dat de reguliere expressies juist zijn. U ziet de resultaten van de reguliere expressie die u bouwt voor elk element na de resultaatregel. De volledige reguliere expressie wordt onder aan de pagina weergegeven.

1. Vouw indien nodig elk element uit en voer de naamgevingsconventies in die u wilt gebruiken.
1. Selecteer zo nodig **[!UICONTROL Add]** om een andere naamgevingsconventie voor een element toe te voegen. Of selecteer **[!UICONTROL Remove]** om een naamgevingsconventie voor een element te verwijderen.
1. Selecteren **[!UICONTROL Save As]** en typ een naam voor de voorinstelling. Of selecteer **[!UICONTROL Save]** als u een bestaande voorinstelling bewerkt.

U kunt ook Code weergeven gebruiken zonder formuliervelden. In deze weergave maakt u uw definities van de naamgevingsconventie volledig met behulp van reguliere expressies.

Er zijn twee elementen beschikbaar voor definitie, Identieke en Basisnaam. Dit zijn alle elementen die u voor een naamgevingsconventie hebt gedefinieerd. Zij kunnen helpen het deel van de overeenkomst identificeren dat wordt gebruikt om de reeks te noemen waarin zij bevat. De individuele noemende overeenkomst van een bedrijf kon één of meerdere lijnen van definitie voor elk van deze elementen gebruiken. U kunt zoveel regels gebruiken voor uw unieke definitie en deze groeperen in afzonderlijke elementen, zoals voor hoofdafbeelding, kleurelement, alternatief weergaveelement en staalelement.

### Een voorinstelling voor een batchset maken {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic gebruikt Voorinstellingen voor batchsets om elementen die veel voorkomende informatie of inhoud delen, te ordenen in sets afbeeldingen die worden weergegeven in viewers. De recepten voor voorinstellingen batch-set worden automatisch uitgevoerd naast de taken voor het importeren van elementen die u in Adobe Dynamic Media Classic plant.

Met Voorinstelling Batch-set kunt u uw voorinstellingen voor Batch-sets maken, bewerken en beheren. U kunt zo veel voorinstellingen maken als nodig is om alle taken voor het opnemen van elementen die u nodig hebt, te kunnen uitvoeren. Er zijn twee vormen van de Reeks van de Partij vooraf ingestelde definities: één voor een standaard noemende overeenkomst die u hebt opstelling, en één voor douane-noemende overeenkomsten die u bij de vlucht creeert.

U kunt de methode van het vormgebied gebruiken om een Vooraf ingestelde Batch te bepalen of de codemethode, die u regelmatige uitdrukkingen laat gebruiken. Als in **[!UICONTROL Default Naming]**, kunt u **[!UICONTROL Code View]** tegelijkertijd definieert u in de formulierweergave en gebruikt u reguliere expressies om uw definities samen te stellen. U kunt ook de optie voor het uitsluitend gebruiken van de ene weergave of de andere uitschakelen.

Zie ook [Een voorinstelling voor een batch-set maken voor het automatisch genereren van een 2D-centrifugeset](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

Zie ook [2D-centrifugeset](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) trainingsvideo.

**Een voorinstelling voor een batchset maken:**

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, zoals ingesteld in de rechterbovenhoek van de pagina Details, is de standaardweergave.
1. Selecteer in het deelvenster Lijst met voorinstellingen de optie **[!UICONTROL Add]** om de definitievelden in het paneel van Details op de rechterkant van de pagina te activeren.
1. Typ in het veld Naam voorinstelling in het deelvenster Details een naam voor de voorinstelling.
1. Selecteer een type voorinstelling in het keuzemenu Type batch.

   Selecteer **[!UICONTROL Multi-Axis Spin Set]** in de vervolgkeuzelijst Type batch.

1. Voer een van de volgende handelingen uit:

   * Als u een standaardnaamgevingsconventie gebruikt die u eerder hebt ingesteld onder **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**, uitbreiden **[!UICONTROL Asset Naming Conventions]** en selecteer vervolgens in de vervolgkeuzelijst Bestandsnaamgeving de optie **[!UICONTROL Default]**.
   * Als u een naamgevingsconventie wilt definiëren terwijl u de voorinstelling instelt, vouwt u **[!UICONTROL Asset Naming Conventions]** en selecteer vervolgens in de vervolgkeuzelijst Bestandsnaamgeving de optie **[!UICONTROL Custom]**.

1. Definieer bij Volgorde de volgorde voor de afbeeldingen nadat de set in Adobe Dynamic Media Classic is gegroepeerd. Uw elementen worden standaard alfanumeriek geordend. U kunt echter een door komma&#39;s gescheiden lijst met reguliere expressies gebruiken om de volgorde te definiëren.
1. Geef bij Naamgeving instellen en Creatieconcept het achtervoegsel of het voorvoegsel op voor de basisnaam die u in de Naamgevingsconventie voor middelen hebt gedefinieerd. Definieer ook waar de afbeeldingsset wordt gemaakt in de Adobe Dynamic Media Classic-mapstructuur.

   Als u grote aantallen reeksen van het Beeld bepaalt, houd deze reeksen gescheiden van de omslagen die de activa zelf bevatten. Vele klanten creëren een omslag van de Reeksen van het Beeld en richten de toepassing om Geproduceerde reeksen van de Partij hier te plaatsen.

1. Selecteren **[!UICONTROL Save]** in het deelvenster Details.

### Een voorinstelling voor een batch-set maken voor het automatisch genereren van een 2D-centrifugeset {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

U kunt het Type Batch gebruiken **Draaiset met meerdere assen** om een &quot;recept&quot; te maken dat het genereren van 2D-centrifuges automatiseert. Bij het groeperen van afbeeldingen worden de reguliere expressies Rij en Kolom gebruikt, zodat de afbeeldingselementen op de juiste wijze worden uitgelijnd op de corresponderende locatie in de multidimensionale array.

Zie ook [Een voorinstelling voor een batchset maken](application-setup.md#creating_a_batch_set_preset).

Er is geen minimum of maximum aantal rijen of kolommen dat u in een reeks van de Rotatie moet hebben meerdere assen.

Stel dat u bijvoorbeeld een reeks met meerdere assen, genaamd *spin-2dspin*. U hebt een reeks afbeeldingen in de reeks met draaien die drie rijen bevatten, met 12 afbeeldingen per rij. De afbeeldingen krijgen de volgende naam:

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

![Batchsetrecept](assets/se_batch_set_recipe.png)

De groepering voor het gedeelde element naamdeel van de reeks van de Rotatie wordt toegevoegd aan het gebied van de Gelijke (zoals benadrukt). Het variabele gedeelte van de elementnaam die de rij en kolom bevat, wordt toegevoegd aan respectievelijk de velden Rij en Kolom.

Wanneer de centrifugeerset wordt geüpload en gepubliceerd, activeert u de naam van het 2D-centrifugesetrecept dat onder **[!UICONTROL Batch Set Presets]** in het dialoogvenster Taakopties uploaden.

**Een voorinstelling voor een batch-set maken voor het automatisch genereren van een 2D-reeks voor draaien:**

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, zoals ingesteld in de rechterbovenhoek van de pagina Details, is de standaardweergave.
1. Selecteer in het deelvenster Lijst met voorinstellingen de optie **[!UICONTROL Add]** om de definitievelden in het paneel van Details aan de rechterkant van de pagina te activeren.
1. Typ in het veld Naam voorinstelling in het deelvenster Details een naam voor de voorinstelling.
1. Selecteer in de vervolgkeuzelijst Type batch de optie **[!UICONTROL Asset Set]**.
1. Selecteer in de vervolgkeuzelijst Subtype de optie **[!UICONTROL Multi-Axis Spin Set]**.
1. Uitbreiden **[!UICONTROL Asset Naming Conventions]** en selecteer vervolgens in de vervolgkeuzelijst Bestandsnaamgeving de optie **[!UICONTROL Custom]**.
1. Gebruik de **[!UICONTROL Match]** en eventueel **[!UICONTROL Base Name]** kenmerken om een reguliere expressie te definiëren voor de naamgeving van afbeeldingselementen waaruit de groepering bestaat.

   De reguliere expressie Letterlijke overeenkomst kan er bijvoorbeeld als volgt uitzien:

   `(\w+)-\w+-\w+`

1. Uitbreiden **[!UICONTROL Row Column Position]** en definieert u vervolgens de naamindeling voor de positie van het afbeeldingselement binnen de 2D-array met spellingsets.

   Gebruik het haakje om de rij- of kolompositie in de bestandsnaam in te sluiten.

   Voor de reguliere expressie van uw rij kan deze er bijvoorbeeld als volgt uitzien:

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
   >Als de combinatie van reguliere expressies in rijen en kolommen de positie van het element binnen de multidimensionale Spin-set-array niet kan bepalen, wordt dat element niet aan de set toegevoegd. Er is een fout geregistreerd.

1. Geef bij Naamgeving instellen en Creatieconcept het achtervoegsel of het voorvoegsel op voor de basisnaam die u in de Naamgevingsconventie voor middelen hebt gedefinieerd. Definieer ook waar de afbeeldingsset wordt gemaakt in de Adobe Dynamic Media Classic-mapstructuur.

   Als u grote aantallen reeksen van het Beeld bepaalt, houd deze reeksen gescheiden van de omslagen die de activa zelf bevatten. Vele klanten creëren een omslag van de Reeksen van het Beeld en richten de toepassing om Geproduceerde reeksen van de Partij hier te plaatsen.

1. Selecteren **[!UICONTROL Save]** in het deelvenster Details.
1. Upload en publiceer de centrifugeset op de gebruikelijke wijze. Zorg ervoor dat u de naam van de 2D-centrifugeset activeert in het dialoogvenster Opties voor laden van taak, onder Voorinstellingen voor batchset.

>[!MORELIKETHIS]
>
>* [Een voorvertoning van een element weergeven](previewing-asset.md#previewing_an_asset)
>* [Voorinstellingen afbeelding instellen](setting-image-presets.md#setting_up_image_presets)
>* [Metagegevens weergeven, toevoegen en exporteren](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Taakbestanden controleren](checking-job-files.md#checking_job_files)
