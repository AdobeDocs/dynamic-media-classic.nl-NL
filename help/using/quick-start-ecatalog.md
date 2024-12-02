---
title: 'Snel starten: eCatalogs'
description: Een inleiding en Snel starten met eCatalogi om u te helpen snel aan de slag te gaan met eCatalog technieken in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1437'
ht-degree: 0%

---

# Snel starten: eCatalogs{#quick-start-ecatalogs}

Een eCatalog is een digitale, Web-versie van drukmateriaal-een catalogus, brochure, flyer, producthandleiding, of reclamecirkel, bijvoorbeeld. Een eCatalog wordt getoond in een eCatalogKijker op een Website. Deze viewer simuleert het lezen van afgedrukt materiaal.

Zie ook de volgende trainingsvideo&#39;s:

* [ Snelle start 1: eCatalogs ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [ Snelle start 2: eCatalogs ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Afhankelijk van de instellingen die u kiest voor uw eCatalog, kunt u in de viewer het volgende doen:

* Zoek in de catalogus naar een trefwoord of trefwoorden. De zoekresultaten worden weergegeven als een lijst met miniaturen in een zoekvenster links in de catalogus. Elke aanklikbare miniatuur vertegenwoordigt een catalogusspread waar de gemarkeerde zoekterm is gevonden.

* Deel de catalogus via sociale media, download de catalogus om deze offline weer te geven en schakel Favorieten in om items te markeren die u snel wilt retourneren of druk de catalogus af.
* Navigeer in de catalogus met de inhoudsopgave of de weergave van het paginaraster. Selecteer de middelste rand van een pagina om de catalogus voor of achter de catalogus te plaatsen.
* Zoom in, zoom uit en pannen om items op een pagina te bekijken.
* Plaats de aanwijzer boven een paginagebied (de zogeheten Afbeeldingskaart), zodat u een pop-upvenster kunt zien met informatie over een item.
* Selecteer een paginagebied zodat opent het een nieuwe Web-pagina met meer informatie over een punt.
* Schrijf een notitie en koppel deze aan een eCatalog-pagina.
* Tik op de pictogrammen Afbeelding met hyperlinks als u gerelateerde webpagina&#39;s of info-deelvensters in de context wilt starten.
* Gebruik gebaarinteracties, zoals vastzetten om in te zoomen en te veeggen om pagina&#39;s om te slaan.
* Zoeken op trefwoord voor objecten.

![ eCatalog aangezien het aan gebruikers verschijnt. A) Openingspagina van eCatalog. B)eCatalog werd aangezet aan pagina 2.](/help/using/assets/ec_cat_viewer_popup.png)

Als u een eCatalog wilt maken, gebruikt u doorgaans PDF-bestanden met hoge resolutie die zijn gemaakt in Adobe Acrobat of een ander afdrukprogramma, maar u kunt ook een eCatalog maken op basis van afbeeldingsbestanden.

Als onderdeel van het maken van uw eCatalog kunt u pagina&#39;s of paginaspread in de gekozen volgorde rangschikken. U kunt ook declareren of u spreads met één pagina, spreads met twee pagina&#39;s of spreads met meerdere pagina&#39;s wilt. U kunt afbeeldingen met hyperlinks maken voor paginagebieden, zodat gebruikers bijvoorbeeld een gebied op de pagina kunnen selecteren en een nieuwe pagina op uw website kunnen openen. U kunt de het omvergooientekst beheren die gebruikend montages InfoPanel binnen het eCatalog scherm verschijnt. U kunt de eCatalogKijker ook vormen door van meer dan 100 verschillende configuratieopties te kiezen. U kunt de functies en de weergave van uw viewer aanpassen aan uw specifieke doelgroep.

>[!NOTE]
>
>Als u Dynamic Media: Scene7-modus gebruikt en eCatalogs wilt gebruiken, bewerkt u de waarde `pdfbrochure` in CRXDE Lite. Ga hiervoor in Adobe Experience Manager naar **[!UICONTROL Tools]** > **[!UICONTROL General]** > **[!UICONTROL CRXDE Lite]** . Navigeer in de navigatiestructuur van het linkerdeelvenster naar `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf` .
>
>Selecteer in de rechterbenedenhoek van het tabblad **[!UICONTROL Properties]** de `jobParam` rij. Stel de waarde voor `pdfbrochure` in van `false` naar `true` . Zoals in `pdfbrochure=true`
>
>Selecteer **[!UICONTROL Save All]** in de linkerbovenhoek van de pagina CRXDE Lite.
>
>U kunt nu eCatalogs ontwerpen in Adobe Dynamic Media Classic.

Deze eCatalog Quick Start is ontworpen om u te helpen snel aan de slag te gaan met eCatalogs. Voer stap 1 tot en met 7 uit. Na elke stap, is er een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

## 1. Upload de PDF-bestanden

Adobe PDF-bestanden zijn meestal de bron van een eCatalog. PDF-bestanden bevatten meestal CMYK-afbeeldingen, omdat ze moeten worden afgedrukt. Adobe Dynamic Media Classic detecteert deze afbeeldingen en zet deze om met een standaard CMYK-kleurprofiel. U moet echter wel een aangepast kleurprofiel uploaden en gebruiken.

Selecteer op de algemene navigatiebalk **[!UICONTROL Upload]** om PDF-bestanden of -afbeeldingen voor uw eCatalog te uploaden. U kunt bestanden uploaden vanaf uw bureaublad of via FTP. FTP wordt aanbevolen als u veel bestanden of bestanden uploadt die groter zijn dan 100 MB.

Onder Opties voor PDF biedt het scherm Uploaden opties voor het uploaden van PDF-bestanden met de juiste resolutie en het corrigeren van de kleurruimte. Een resolutie van 150 pixels per inch wordt aanbevolen. U kunt de optie **[!UICONTROL Auto-Generate eCatalog]** selecteren om een eCatalog tot stand te brengen wanneer u een dossier van de PDF uploadt.

Zie [ de dossiers van de PDF ](uploading-pdf-files.md#uploading_the_pdf_files) uploaden.

## 2. Een eCatalog maken

Maak uw eCatalog door PDF of beelddossiers in het Browse paneel te selecteren. Selecteer **[!UICONTROL Build]** en kies vervolgens **[!UICONTROL eCatalogs]** .

Selecteer op de pagina eCatalog op het tabblad **[!UICONTROL Order Pages]** een lay-outoptie: **[!UICONTROL 1 Up]** , **[!UICONTROL 2 Up]** of **[!UICONTROL Custom]** . U kunt pagina&#39;s of spreads opnieuw rangschikken door deze te slepen of door in een grote eCatalog een paginanaam te kiezen in het menu Verplaatsen naar.

Als u pagina&#39;s wilt toevoegen, selecteert u een map in de elementenbibliotheek en sleept u vervolgens PDF- of afbeeldingsbestanden van de map naar het scherm Pagina&#39;s bestellen. In plaats van de standaardpaginanummers kunt u aangepaste paginanamen opgeven of een groot aantal paginanamen importeren.

Selecteer **[!UICONTROL Save]**, voer een naam in voor uw eCatalog, kies een Adobe Dynamic Media Classic-map om deze op te slaan en selecteer **[!UICONTROL Save]** . Elke keer dat u de paginavolgorde wijzigt of uw eCatalog bewerkt, slaat u de wijzigingen op door **[!UICONTROL Save]** te selecteren.

Zie [ een eCatalog ](creating-ecatalog.md) creëren.

## 3. Afbeeldingen met hyperlinks maken

Afbeeldingen met hyperlinks voegen nog een aspect toe aan eCatalog-pagina&#39;s. Een afbeelding met hyperlinks is een gebied op een pagina dat meer informatie over een item bevat. Wanneer de kijkers de wijzer over een Kaart van het Beeld rollen, zien zij een beschrijving van het punt. Als u op een afbeelding met hyperlinks klikt, wordt een externe verwijzing geactiveerd die een nieuwe webpagina opent waarin u meer over een item kunt leren.

Open het eCatalog-scherm om een afbeelding met hyperlinks te maken. Ga vervolgens naar het tabblad **[!UICONTROL Map Pages]** van het eCatalog-scherm en kader de kaart met het gereedschap Afbeelding met rechthoek of Veelhoekafbeelding met hyperlinks. U kunt de positie en de grootte van Afbeeldingen met hyperlinks aanpassen door kaartranden te slepen met het gereedschap Pannen.

Nadat u de Kaart van het Beeld kader, ga het URL adres in dat u wilt gaan wanneer u de Kaart van het Beeld selecteert. U kunt ook de rollover-tekst invoeren die wordt weergegeven wanneer u de aanwijzer over de Afbeeldingskaart beweegt.

Zie [ ECatalogKaarten van het Beeld creëren ](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Zie [ Kaarten van het Beeld van het Gebruik om rijke media in een eCatalog ](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog) in te bedden.

U kunt de tekst van de Kaart van het Beeld opstelling en beheren gebruikend de montages van het Comité van Info in het eCatalog scherm.

Zie [ de inhoud van het Comité van Info in eCatalogs beheren ](/help/using/info-panel-content-ecatalog.md).

## 4. Voorinstellingen eCatalog-viewer instellen

Eindgebruikers zien uw eCatalog in de eCatalogKijker. Beheerders kunnen de eCatalog-viewer configureren. U kunt de contourkleur wijzigen en een nieuwe skin selecteren om uw eCatalog van een merk te voorzien. Adobe Dynamic Media Classic wordt geleverd met verschillende &quot;best practices&quot;-voorinstellingen voor eCatalog Viewer. U kunt een van deze voorinstellingen kiezen voor de weergave van uw eCatalogs. Als beheerder kunt u ook zelf een voorinstelling voor een eCatalog-viewer maken.

Als u een voorinstelling voor een eCatalog-viewer wilt maken, selecteert u **[!UICONTROL Setup]** op de algemene navigatiebalk en kiest u vervolgens **[!UICONTROL Viewer Presets]** . Selecteer **[!UICONTROL Add]** , kies een platform en selecteer vervolgens **[!UICONTROL eCatalog]** > **[!UICONTROL Viewer]** .

Zie [ Opstelling eCatalogKijker vooraf instelt ](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. E-catalogi voorvertonen in de eCatalog-viewer

De eCatalog Viewer-voorinstellingen bepalen de stijl en het gedrag van uw eCatalog-viewers.

Als u wilt weten hoe de eCatalog-viewer met voorinstellingen uw eCatalog weergeeft, selecteert u uw eCatalog in het deelvenster Bladeren en selecteert u vervolgens **[!UICONTROL Preview]** . Het voorvertoningsscherm wordt geopend in de standaardviewer.

Let op de afdrukstand, het kleurenschema, hoe de besturingselementen voor het wijzigen van pagina&#39;s eruit zien en hoe de pagina&#39;s eruit zien wanneer ze worden omgedraaid.

Zie [ eCatalogi van de Voorproef in de eCatalogKijker ](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publish eCatalog en bijbehorende PDF

Wanneer u uw eCatalog en de bijbehorende PDF publiceert, wordt deze op Dynamic Media Image Servers geplaatst, zodat deze aan uw website en toepassing kan worden geleverd. Als onderdeel van het publicatieproces activeert Adobe Dynamic Media Classic de URL-tekenreeks voor uw eCatalog. Gebruik deze URL om de eCatalog van de Servers van het Beeld van Dynamic Media aan uw Website of toepassing te roepen.

Nadat u uw eCatalog en PDF hebt gemarkeerd om te publiceren in het deelvenster Bladeren, selecteert u de Publish-knop op de algemene navigatiebalk om een publicatie te starten. Selecteer **[!UICONTROL Submit Publish]** op de pagina Publiceren.

Zie [ de eCatalogi van Publish en bijbehorende PDF ](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Koppel een eCatalog aan een Web-pagina

Adobe Dynamic Media Classic activeert de URL-bijschrifttekenreeks die nodig is voor de weergave van uw eCatalog wanneer u deze publiceert naar Dynamic Media Image Servers. U kunt deze URL-tekenreeks kopiëren vanuit het voorvertoningsscherm en het deelvenster Bladeren (in de gedetailleerde weergave) door URL&#39;s te selecteren in het deelvenster. Nadat u het koord URL kopieert, is het beschikbaar aan uw Websites en toepassingen.

Werk samen met uw IT-team om de koppeling naar de eCatalog op de juiste plaats in uw webpagina te plaatsen. Wanneer gebruikers de koppeling selecteren, wordt de eCatalog-viewer weergegeven en kunnen gebruikers door de eCatalog bladeren.

Zie [ Verbinding een eCatalog aan een Web-pagina ](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
