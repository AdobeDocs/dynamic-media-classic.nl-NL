---
title: "Snel starten: eCatalogs"
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
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '1437'
ht-degree: 0%

---

# Snel starten: eCatalogs{#quick-start-ecatalogs}

Een eCatalog is een digitale, webversie van drukmateriaal, bijvoorbeeld een catalogus, brochure, flyer, producthandleiding of reclamecirkel. Een eCatalog wordt getoond in een eCatalogKijker op een website. Deze viewer simuleert het lezen van afgedrukt materiaal.

Zie ook de volgende trainingsvideo&#39;s:

* [Snel starten 1: eCatalogi](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Snel starten 2: eCatalogi](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Afhankelijk van de instellingen die u kiest voor uw eCatalog, kunt u in de viewer het volgende doen:

* Zoek in de catalogus naar een trefwoord of trefwoorden. De zoekresultaten worden weergegeven als een lijst met miniaturen in een zoekvenster links in de catalogus. Elke aanklikbare miniatuur vertegenwoordigt een catalogusspread waar de gemarkeerde zoekterm is gevonden.

* Deel de catalogus via sociale media, download de catalogus om deze offline weer te geven en schakel Favorieten in om items te markeren die u snel wilt retourneren of druk de catalogus af.
* Navigeer in de catalogus met de inhoudsopgave of de weergave van het paginaraster. Selecteer de middelste rand van een pagina om de catalogus voor of achter de catalogus te plaatsen.
* Zoom in, zoom uit en pannen om items op een pagina te bekijken.
* Plaats de aanwijzer boven een paginagebied (de zogeheten Afbeeldingskaart), zodat u een pop-upvenster kunt zien met informatie over een item.
* Selecteer een paginagebied zodat er een nieuwe webpagina met meer informatie over een item wordt geopend.
* Schrijf een notitie en koppel deze aan een eCatalog-pagina.
* Tik op pictogrammen voor afbeeldingen met hyperlinks als u gerelateerde webpagina&#39;s of info-deelvensters in de context wilt starten.
* Gebruik gebaarinteracties, zoals vastzetten om in te zoomen en te veeggen om pagina&#39;s om te slaan.
* Zoeken op trefwoord voor objecten.

![De eCatalog zoals het aan gebruikers lijkt. A) Openingspagina van eCatalog. B)eCatalog is ingesteld op pagina 2.](/help/using/assets/ec_cat_viewer_popup.png)

Als u een eCatalog wilt maken, gebruikt u doorgaans PDF-bestanden met hoge resolutie die zijn gemaakt in Adobe Acrobat of een ander afdrukprogramma, maar u kunt ook een eCatalog maken op basis van afbeeldingsbestanden.

Als onderdeel van het maken van uw eCatalog kunt u pagina&#39;s of paginaspread in de gekozen volgorde rangschikken. U kunt ook declareren of u spreads met één pagina, spreads met twee pagina&#39;s of spreads met meerdere pagina&#39;s wilt. U kunt afbeeldingen met hyperlinks maken voor paginagebieden, zodat gebruikers bijvoorbeeld een gebied op de pagina kunnen selecteren en een nieuwe pagina op uw website kunnen openen. U kunt de het omvergooientekst beheren die gebruikend montages InfoPanel binnen het eCatalog scherm verschijnt. U kunt de eCatalogKijker ook vormen door van meer dan 100 verschillende configuratieopties te kiezen. U kunt de functies en de weergave van uw viewer aanpassen aan uw specifieke doelgroep.

>[!NOTE]
>
>Als u in de Dynamic Media- Scene7-modus werkt en eCatalogi wilt gebruiken, bewerkt u de `pdfbrochure` waarde in CRXDE Lite. Ga hiervoor in Adobe Experience Manager naar **[!UICONTROL Tools]** > **[!UICONTROL General]** > **[!UICONTROL CRXDE Lite]**. Navigeer in de navigatiestructuur van het linkerdeelvenster naar `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>In de laag juiste ruit, in **[!UICONTROL Properties]** selecteert u de `jobParam` rij. Stel de waarde in voor `pdfbrochure` van `false` tot `true`. Als in `pdfbrochure=true`
>
>Selecteer in de linkerbovenhoek van de pagina CRXDE Lite de optie **[!UICONTROL Save All]**.
>
>U kunt nu eCatalogs ontwerpen in Adobe Dynamic Media Classic.

Deze eCatalog Quick Start is ontworpen om u te helpen snel aan de slag te gaan met eCatalogs. Voer stap 1 tot en met 7 uit. Na elke stap, is er een verwijzing naar een onderwerprubriek waar u meer informatie kunt vinden.

## 1. Upload de PDF-bestanden

Adobe PDF-bestanden zijn meestal de bron van een eCatalog. PDF-bestanden bevatten meestal CMYK-afbeeldingen, omdat ze moeten worden afgedrukt. Adobe Dynamic Media Classic detecteert deze afbeeldingen en zet deze om met een standaard CMYK-kleurprofiel. U moet echter wel een aangepast kleurprofiel uploaden en gebruiken.

Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Upload]** om PDF-bestanden of afbeeldingen voor uw eCatalog te uploaden. U kunt bestanden uploaden vanaf uw bureaublad of via FTP. FTP wordt aanbevolen als u veel bestanden of bestanden uploadt die groter zijn dan 100 MB.

Onder Opties voor PDF biedt het scherm Uploaden opties voor het uploaden van PDF-bestanden met de juiste resolutie en het corrigeren van de kleurruimte. Een resolutie van 150 pixels per inch wordt aanbevolen. U kunt de optie selecteren **[!UICONTROL Auto-Generate eCatalog]** om een eCatalog tot stand te brengen wanneer u een dossier van de PDF uploadt.

Zie [De PDF-bestanden uploaden](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Een eCatalog maken

Maak uw eCatalog door PDF of beelddossiers in het Browse Comité te selecteren. Selecteren **[!UICONTROL Build]** en kiest u **[!UICONTROL eCatalogs]**.

Op de pagina eCatalog, op **[!UICONTROL Order Pages]** selecteert u een lay-outoptie: **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]**, of **[!UICONTROL Custom]**. U kunt pagina&#39;s of spreads opnieuw rangschikken door deze te slepen of door in een grote eCatalog een paginanaam te kiezen in het menu Verplaatsen naar.

Als u pagina&#39;s wilt toevoegen, selecteert u een map in de elementenbibliotheek en sleept u vervolgens PDF- of afbeeldingsbestanden van de map naar het scherm Pagina&#39;s bestellen. In plaats van de standaardpaginanummers kunt u aangepaste paginanamen opgeven of een groot aantal paginanamen importeren.

Selecteren **[!UICONTROL Save]** voert u een naam in voor uw eCatalog, kiest u een Adobe Dynamic Media Classic-map om deze op te slaan en selecteert u **[!UICONTROL Save]**. Elke keer dat u de paginavolgorde wijzigt of uw eCatalog bewerkt, slaat u de wijzigingen op door **[!UICONTROL Save]**.

Zie [Een eCatalog maken](creating-ecatalog.md).

## 3. Afbeeldingen met hyperlinks maken

Afbeeldingen met hyperlinks voegen nog een aspect toe aan eCatalog-pagina&#39;s. Een afbeelding met hyperlinks is een gebied op een pagina dat meer informatie over een item bevat. Wanneer de kijkers de wijzer over een Kaart van het Beeld rollen, zien zij een beschrijving van het punt. Als u op een afbeelding met hyperlinks klikt, wordt een externe verwijzing geactiveerd waarmee een nieuwe webpagina wordt geopend waarin u meer kunt leren over een item.

Open het eCatalog-scherm om een afbeelding met hyperlinks te maken. Ga vervolgens naar de **[!UICONTROL Map Pages]** van het eCatalog-scherm en kader de kaart met het gereedschap Afbeelding met rechthoek of Veelhoekafbeelding met hyperlinks. U kunt de positie en de grootte van Afbeeldingen met hyperlinks aanpassen door kaartranden te slepen met het gereedschap Pannen.

Nadat u de Kaart van het Beeld kader, ga het URL adres in dat u wilt gaan wanneer u de Kaart van het Beeld selecteert. U kunt ook de rollover-tekst invoeren die wordt weergegeven wanneer u de aanwijzer over de Afbeeldingskaart beweegt.

Zie [ECatalog-afbeeldingen met hyperlinks maken](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Zie [Afbeeldingen met hyperlinks gebruiken om rijke media in een eCatalog in te sluiten](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

U kunt de tekst van de afbeeldingskaart instellen en beheren met de instellingen in het deelvenster Info in het eCatalog-scherm.

Zie [Inhoud van deelvenster Info in eCatalogs beheren](/help/using/info-panel-content-ecatalog.md).

## 4. Voorinstellingen eCatalog-viewer instellen

Eindgebruikers zien uw eCatalog in de eCatalogKijker. Beheerders kunnen de eCatalog-viewer configureren. U kunt de contourkleur wijzigen en een nieuwe skin selecteren om uw eCatalog van een merk te voorzien. Adobe Dynamic Media Classic wordt geleverd met verschillende &quot;best practices&quot;-voorinstellingen voor eCatalog Viewer. U kunt een van deze voorinstellingen kiezen voor de weergave van uw eCatalogs. Als beheerder kunt u ook zelf een voorinstelling voor een eCatalog-viewer maken.

Als u een voorinstelling voor een eCatalog-viewer wilt maken, selecteert u op de algemene navigatiebalk de optie **[!UICONTROL Setup]** en kies vervolgens **[!UICONTROL Viewer Presets]**. Selecteren **[!UICONTROL Add]** kiest u een platform en selecteert u vervolgens **[!UICONTROL eCatalog]** > **[!UICONTROL Viewer]**.

Zie [Voorinstellingen eCatalog-viewer instellen](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. E-catalogi voorvertonen in de eCatalog-viewer

De eCatalog Viewer-voorinstellingen bepalen de stijl en het gedrag van uw eCatalog-viewers.

Als u wilt weten hoe de eCatalog-viewer met voorinstellingen uw eCatalog weergeeft, selecteert u uw eCatalog in het deelvenster Bladeren en selecteert u **[!UICONTROL Preview]**. Het voorvertoningsscherm wordt geopend in de standaardviewer.

Let op de afdrukstand, het kleurenschema, hoe de besturingselementen voor het wijzigen van pagina&#39;s eruit zien en hoe de pagina&#39;s eruit zien wanneer ze worden omgedraaid.

Zie [Voorvertoning van eCatalogi weergeven in de eCatalog-viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. E-catalogus en bijbehorende PDF publiceren

Als u uw eCatalog en de bijbehorende PDF publiceert, wordt deze op Dynamic Media Image Servers geplaatst, zodat deze op uw website en toepassing kan worden geleverd. Als onderdeel van het publicatieproces activeert Adobe Dynamic Media Classic de URL-tekenreeks voor uw eCatalog. Gebruik deze URL om de eCatalog van de Servers van het Beeld van Dynamic Media aan uw website of toepassing te roepen.

Nadat u uw eCatalog en PDF voor publicatie in het deelvenster Bladeren hebt gemarkeerd, selecteert u de knop Publiceren op de algemene navigatiebalk om een publicatie te starten. Selecteer op de pagina Publiceren de optie **[!UICONTROL Submit Publish]**.

Zie [E-catalogi en bijbehorende PDF publiceren](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Een eCatalog aan een webpagina koppelen

Adobe Dynamic Media Classic activeert de URL-bijschrifttekenreeks die nodig is voor de weergave van uw eCatalog wanneer u deze publiceert naar Dynamic Media Image Servers. U kunt deze URL-tekenreeks kopiëren vanuit het voorvertoningsscherm en het deelvenster Bladeren (in de gedetailleerde weergave) door URL&#39;s te selecteren in het deelvenster. Nadat u de URL-tekenreeks hebt gekopieerd, is deze beschikbaar voor uw websites en toepassingen.

Werk samen met uw IT-team om de koppeling naar de eCatalog op de juiste plaats op uw webpagina te plaatsen. Wanneer gebruikers de koppeling selecteren, wordt de eCatalog-viewer weergegeven en kunnen gebruikers door de eCatalog bladeren.

Zie [Een eCatalog koppelen aan een webpagina](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
