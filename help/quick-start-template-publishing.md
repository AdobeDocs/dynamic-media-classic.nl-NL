---
title: '"Snel starten: Sjabloon publiceren"'
seo-title: '"Snel starten: Sjabloon publiceren"'
description: 'null'
seo-description: Een inleiding en Snel Begin aan het publiceren van het Malplaatje om u te helpen snel aan de slag gaan.
uuid: 101b6211-2421-4565-8635-944315a5c512
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 03671fc1-ce3b-4fae-ad1f-53c99abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Snel starten: Sjabloon publiceren{#quick-start-template-publishing}

Met de Adobe Dynamic Media Classic Web-to-Print kunt u professioneel gemerkte afdrukinhoud maken die uw klanten, klanten en medewerkers gemakkelijk kunnen aanpassen en aanpassen. U kunt de inhoud en merkidentiteit van uw bedrijf tijdens het publicatieproces behouden. Eindgebruikers kunnen de afdrukinhoud aanpassen, maar alleen het gedeelte van de inhoud dat u ze toestaat aan te passen. Persoonlijke stilstaande beelden, visitekaartjes, posters, wenskaarten, labels, cheques, geschenken, kleding, kalenders, plakboeken en fotoalbums zijn voorbeelden van aangepaste afdrukproducten die u kunt leveren. Ondernemingen kunnen een gemeenschappelijke merkidentiteit in hun handtekening handhaven die voor verschillende regio&#39;s, franchises, winkels, en bijkantoren kan worden aangepast.

U begint met het ontwerpen van een sjabloon in Adobe Illustrator. De sjabloon definieert zorgvuldig wat constant is en wat variabel is — de variabele componenten zijn de componenten die kunnen worden aangepast. Nadat bijvoorbeeld de parameters voor tekst in een Illustrator-bestand zijn ingesteld, kunnen eindgebruikers zelf tekst invoeren. Op dezelfde manier kan een achtergrondkleur, nadat deze is geparametriseerd als een variabele component, worden gewisseld voor een andere achtergrondkleur.

De dynamische Klassieke Media biedt twee werkschema&#39;s van het Publiceren van het Malplaatje, voor basisgebruiksgevallen en voor geavanceerde gebruiksgevallen aan. Basis-gebruikstoepassingen omvatten het maken van een ontwerp in Adobe Illustrator, het uploaden naar Dynamic Media Classic en het definiëren van variabele elementen met parameters in SPS. Gevallen van geavanceerd gebruik vereisen een uitvoerigere definitie van variabiliteit. Gevallen van geavanceerd gebruik omvatten het creëren van veranderlijke elementen in de Illustrator van Adobe, het uploaden van het dossier aan Dynamische Klassieke Media, en het direct manipuleren van die elementen op een niveau XML met URL vraag. Dit scenario wordt genoemd *`*DOM manipulation*`*.

>[!NOTE]
>
>Voor meer informatie over de Dynamische Klassieke Web-aan-druk werkschema&#39;s van Media, malplaatjeverwezenlijking, parameterization, DOM manipulatie, en meer, zie hier de Web-aan-Druk Gids van het Werkschema: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Download het ZIP-bestand naar uw lokale vaste schijf en extraheer de inhoud ervan (het dynamische document met zelfstudies voor Media Classic Web-To-PrintWorkflow en de zelfstudie).

**Snel starten**

In deze snelstartprocedure wordt de basisworkflow beschreven voor het gebruik van Illustrator-bestanden om aanpasbare afdrukproducten van hoge kwaliteit te maken.

**1. Uw Illustrator-bestand ontwerpen voor sjabloonpublicatie**

Ontwerp uw sjabloon in Illustrator. Als u de geavanceerde, DOM manipulatiemethode wilt gebruiken om uw malplaatje aan te passen, bepaal s7:elementIDs voor veranderlijke elementen in Illustrator.

Zie De [oorspronkelijke sjabloon maken in Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) en [DOM-bewerking](dom-manipulation.md#dom_manipulation).

**2. Zet uw malplaatje in Dynamische Klassieke FXG van Media om en upload het aan het Publiceren Scene7 Systeem**

Gebruikers van Adobe Creative Cloud kunnen de Adobe Illustrator-plug-in voor web-to-print gebruiken. Deze plug-in zet sjablonen om in Dynamic Media Classic FXG. Als een malplaatje doopvonten bevat, moeten de overeenkomstige doopvontdossiers aan het het Publiceren Scene7 Systeem worden geupload alvorens het FXG- dossier te uploaden.

Zie Bestanden [uploaden voor Sjabloonpublicatie](upload-files-template-publishing.md#upload_files_for_template_publishing).

**3. Parameters weergeven, definiëren of verfijnen in Dynamic Media Classic**

In de schermen van de Voorproef van het Publiceren van het Malplaatje en van de Bouwstijl, kunt u veranderlijke elementen bepalen en verfijnen via parameters, voorproef de resultaten, en test de resultaten. In deze schermen kunt u:

* Parameters maken en wijzigen.
* Geef standaardwaarden op voor parametereigenschappen en -kenmerken.
* Klik op URL kopiëren om de voorbeeld-URL naar het klembord te kopiëren en een voorvertoning van het resultaat weer te geven in een browservenster.

Zie Een sjabloon [parameteren in Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. De FXG-sjabloon publiceren**

Publiceer het bestand nadat u de parameters en kenmerken hebt gedefinieerd en getest. Als u uw FXG-sjabloon publiceert, wordt deze op de Dynamic Media Image Servers geplaatst en wordt de URL geactiveerd.

Zorg ervoor dat u alle afbeeldingen en lettertypen publiceert die aan de FXG-sjabloon zijn gekoppeld.

Zie FXG-sjablonen [publiceren](dom-manipulation.md#publish_fxg_templates).

**5. De URL ophalen**

Via zijn URL is de sjabloon nu gereed om in uw website te worden ingesloten, zodat eindgebruikers variabele inhoud kunnen aanpassen.

Zie Een FXG-sjabloon [koppelen aan een webpagina](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
