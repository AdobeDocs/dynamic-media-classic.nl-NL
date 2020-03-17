---
title: '"Snel starten: eCatalogs"'
seo-title: '"Snel starten: eCatalogs"'
description: 'null'
seo-description: Een inleiding en Snel Begin aan eCatalogi om u te helpen snel met eCatalog technieken opstaan en in werking stellen.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Snel starten: eCatalogs{#quick-start-ecatalogs}

Een eCatalog is een digitale, webversie van drukmateriaal, bijvoorbeeld een catalogus, brochure, flyer, producthandleiding of reclamecirkel. Een eCatalog wordt getoond in een eCatalogKijker op een website. Deze viewer simuleert het lezen van afgedrukt materiaal. Afhankelijk van de instellingen die u kiest voor uw eCatalog, kunt u in de viewer het volgende doen:

* Zoek in de catalogus naar een trefwoord of trefwoorden. De zoekresultaten worden weergegeven als een lijst met miniaturen in een zoekvenster links in de catalogus. Elke klikbare miniatuur vertegenwoordigt een catalogusspread waar de gemarkeerde zoekterm is gevonden.

* De catalogus delen via sociale media; de catalogus downloaden om offline te bekijken; Schakel Favorieten in om items te markeren waarnaar u snel wilt terugkeren of druk de catalogus af.
* Navigeer in de catalogus met de inhoudsopgave of de weergave van het paginaraster. Klik op de middelste rand van een pagina voor- of achteruit.
* Zoom in, zoom uit en pannen om items op een pagina te bekijken.
* Plaats de aanwijzer boven een paginagebied (de zogeheten Afbeeldingskaart) om een pop-upvenster weer te geven met informatie over een item.
* Klik op een paginagebied om een nieuwe webpagina met meer informatie over een item te openen.
* Schrijf een notitie en koppel deze aan een eCatalog-pagina.
* Tik op pictogrammen voor afbeeldingen met hyperlinks om gerelateerde webpagina&#39;s of info-deelvensters in de context te starten.
* Gebruik gebaarinteracties, zoals vastzetten om in te zoomen en te veeggen om pagina&#39;s om te slaan.
* Zoeken op trefwoord voor objecten.

![De eCatalog zoals het aan gebruikers kijkt. A) Openingspagina van eCatalog. B)eCatalog is ingesteld op pagina 2.](/help/assets/ec_cat_viewer_popup.png)

Voor het maken van een eCatalog gebruikt u meestal PDF-bestanden met een hoge resolutie die zijn gemaakt in Adobe® Acrobat® of een ander afdrukprogramma, maar u kunt ook een eCatalog maken van afbeeldingsbestanden.

Als onderdeel van het maken van uw eCatalog kunt u pagina&#39;s of paginaspread in de gekozen volgorde rangschikken. U kunt ook declareren of u spreads met één pagina, spreads met twee pagina&#39;s of spreads met meerdere pagina&#39;s wilt. U kunt afbeeldingen met hyperlinks maken voor paginagebieden, zodat gebruikers bijvoorbeeld op een gebied op de pagina kunnen klikken en een nieuwe pagina op uw website kunnen openen. U kunt de het omvergooientekst beheren die gebruikend montages InfoPanel binnen het eCatalog scherm verschijnt. U kunt de eCatalogKijker ook vormen door van meer dan 100 verschillende configuratieopties te kiezen. U kunt de functies en de weergave van uw viewer aanpassen aan uw specifieke doelgroep.

>[!NOTE]
>
>Als u een gebruiker van de wijze AEM Dynamische Media - Scene7 bent en eCatalogs wilt gebruiken, zult u de `pdfbrochure` waarde in CRXDE Lite moeten uitgeven. Klik hiertoe in AEM op **[!UICONTROL Tools > General > CRXDE Lite]**. Navigeer in de navigatiestructuur van het linkerdeelvenster naar `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
Selecteer de **[!UICONTROL Properties]** rij in het rechterondervenster op het `jobParam` tabblad. Stel de waarde in voor `pdfbrochure` van `false` naar `true`. Zoals `pdfbrochure=true`in de upper-left hoek van de pagina van CRXDE Lite, klik **[!UICONTROL Save All]**.
U kunt nu eCatalogs in SPS ontwerpen.

**Snel starten**

Deze eCatalog Quick Start is ontworpen om u te helpen snel aan de slag te gaan met eCatalogs. Voer stap 1 tot en met 7 uit. Na elke stap is een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

**1. De PDF-bestanden uploaden**

Adobe PDF-bestanden zijn meestal de bron van een eCatalog. PDF-bestanden bevatten meestal CMYK-afbeeldingen, omdat ze moeten worden afgedrukt. Het het Publiceren Scene7 Systeem ontdekt deze beelden en zet hen om gebruikend een standaard CMYK kleurenprofiel. Het is echter mogelijk dat u een aangepast kleurprofiel moet uploaden en gebruiken.

Klik op Uploaden op de algemene navigatiebalk om PDF-bestanden of -afbeeldingen voor uw eCatalog te uploaden. U kunt bestanden uploaden vanaf uw bureaublad of via FTP; FTP wordt aanbevolen als u veel bestanden of bestanden van meer dan 100 MB uploadt.

Onder PDF-opties biedt het scherm Uploaden opties voor het uploaden van PDF-bestanden met de juiste resolutie en het corrigeren van de kleurruimte. Een resolutie van 150 pixels per inch wordt aanbevolen. U kunt de optie eCatalog automatisch genereren selecteren om een eCatalog tot stand te brengen wanneer u een Pdf- dossier uploadt.

Zie PDF-bestanden [uploaden](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Een eCatalog maken**

Maak uw eCatalog door PDF of beelddossiers in het Browse Comité te selecteren, dan de knoop van de Bouwstijl te klikken en eCatalogs te kiezen. Het eCatalog-scherm wordt geopend.

Selecteer op het tabblad Order Pages een knop Indeling (1 omhoog, 2 omhoog of Aangepast) om te kiezen of u enkele, dubbele of aangepaste paginapreads wilt gebruiken. U kunt pagina&#39;s of spreads opnieuw rangschikken door deze te slepen of door in een grote eCatalog een paginanaam te kiezen in het menu Verplaatsen naar.

Als u pagina&#39;s wilt toevoegen, selecteert u een map in de elementenbibliotheek en sleept u PDF- of afbeeldingsbestanden van de map naar het scherm Pagina&#39;s bestellen. In plaats van de standaardpaginanummers kunt u aangepaste paginanamen opgeven of een groot aantal paginanamen importeren.

Klik **[!UICONTROL Save]**, ga een naam voor uw eCatalog in, kies een omslag SPS voor het opslaan, en klik **[!UICONTROL Save]**. Elke keer dat u de paginavolgorde wijzigt of uw eCatalog bewerkt, slaat u de wijzigingen op door op **[!UICONTROL Save]** te klikken.

Zie [Een eCatalog](creating-ecatalog.md)maken.

**3. Afbeeldingskaarten maken**

Afbeeldingskaarten voegen een andere dimensie toe aan eCatalog-pagina&#39;s. Een afbeelding met hyperlinks is een gebied op een pagina dat meer informatie over een item bevat. Wanneer de kijkers de wijzer over een Kaart van het Beeld rollen, zien zij een beschrijving van het punt. Als u op een afbeelding met hyperlinks klikt, wordt een externe verwijzing geactiveerd waarmee een nieuwe webpagina wordt geopend waarin u meer kunt leren over een item.

Open het eCatalog-scherm om een afbeelding met hyperlinks te maken. Ga vervolgens naar het **[!UICONTROL Map Pages]** tabblad van het eCatalog-scherm en teken de kaart met het gereedschap Afbeelding met rechthoek of het gereedschap Veelhoekafbeelding met hyperlinks. U kunt de positie en de grootte van Afbeeldingen met hyperlinks aanpassen door kaartranden te slepen met het gereedschap Pannen.

Nadat u de Kaart van het Beeld tekent, ga het URL adres in dat u wilt gaan wanneer u de Kaart van het Beeld klikt. U kunt ook de rollover-tekst invoeren die wordt weergegeven wanneer u de aanwijzer over de Afbeeldingskaart beweegt.

Zie Afbeeldingen met hyperlinks [maken](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)in eCatalog.

Zie [Afbeeldingen met hyperlinks gebruiken om rijke media in een eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)in te sluiten.

U kunt de tekst van de afbeeldingskaart instellen en beheren met de instellingen in het deelvenster Info in het eCatalog-scherm.

Zie Inhoud [van deelvenster Info](info-panel-content.md#managing-info-panel-content)beheren.

**4. Voorinstellingen eCatalog-viewer instellen**

Eindgebruikers zien uw eCatalog in de eCatalogKijker. Beheerders kunnen de eCatalog-viewer configureren. U kunt de contourkleur wijzigen en een nieuwe skin selecteren om uw eCatalog van een merk te voorzien. Dynamic Media Classic wordt geleverd met verschillende voorinstellingen voor de eCatalog-viewer met &#39;best practices&#39;. U kunt een van deze voorinstellingen kiezen voor de weergave van uw eCatalogs. Als beheerder kunt u ook zelf een voorinstelling voor een eCatalog-viewer maken.

Als u een voorinstelling voor een eCatalog-viewer wilt maken, klikt u op de algemene navigatiebalk **[!UICONTROL Setup]** en kiest u **[!UICONTROL Viewer Presets]**. Klik vervolgens op **[!UICONTROL Add]** een platform en klik op **[!UICONTROL eCatalog > Viewer]**.

Zie Voorinstellingen voor eCatalog-viewer [instellen](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

**5. Voorvertoning van eCatalogi weergeven in de eCatalog-viewer**

De eCatalog Viewer-voorinstellingen bepalen de stijl en het gedrag van uw eCatalog-viewers.

Als u wilt weten hoe de eCatalog-viewer met voorinstellingen uw eCatalog weergeeft, selecteert u de eCatalog in het deelvenster Bladeren en klikt u op **[!UICONTROL Preview]**. Het voorvertoningsscherm wordt geopend in de standaardviewer.

Let op de afdrukstand, het kleurenschema, hoe de besturingselementen voor het wijzigen van pagina&#39;s eruit zien en hoe de pagina&#39;s eruit zien wanneer ze worden omgedraaid.

Zie Een [voorbeeld van eCatalogi weergeven in de eCatalog-viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. ECatalog en bijbehorende PDF&#39;s publiceren**

Als u uw eCatalog en de bijbehorende PDF publiceert, wordt deze op Dynamic Media Image Servers geplaatst, zodat deze op uw website en toepassing kan worden geleverd. Als deel van het het publiceren proces, activeert het het Publiceren Scene7 Systeem het koord URL voor uw eCatalog. Gebruik deze URL om de eCatalog van Dynamische Servers van het Beeld van Media aan uw website of toepassing te roepen.

Nadat u uw eCatalog en PDF hebt gemarkeerd voor publicatie in het deelvenster Bladeren, selecteert u de knop Publiceren op de algemene navigatiebalk om een publicatie te starten. Klik in het scherm Publiceren op **[!UICONTROL Start Publish]**.

Zie E-catalogi en bijbehorende PDF&#39;s [publiceren](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. Een eCatalog koppelen aan een webpagina**

Dynamic Media Classic activeert de URL-bijschrifttekenreeks die nodig is voor de weergave van uw eCatalog wanneer u deze publiceert naar Dynamic Media Image Servers. U kunt deze URL-tekenreeks kopiëren vanuit het voorvertoningsscherm en het deelvenster Bladeren (in de gedetailleerde weergave) door URL&#39;s te selecteren in het deelvenster. Nadat u de URL-tekenreeks hebt gekopieerd, is deze beschikbaar voor uw websites en toepassingen.

Werk samen met uw IT-team om de koppeling naar de eCatalog op de juiste plaats op uw webpagina te plaatsen. Wanneer gebruikers op de koppeling klikken, wordt de eCatalog-viewer weergegeven en kunnen gebruikers door uw eCatalog bladeren.

Zie Een eCatalog [koppelen aan een webpagina](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
