---
title: Elementen testen voordat ze openbaar worden gemaakt
seo-title: Elementen testen voordat ze openbaar worden gemaakt
description: 'null'
seo-description: Leer hoe u elementen kunt testen voordat u ze openbaar maakt.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 0%

---


# Elementen testen voordat ze openbaar worden gemaakt {#testing-assets-before-making-them-public}

Het veilige Testen helpt u een veilige testmilieu bepalen en een robuuste B2B oplossing bouwen, die op een configureerbare reeks IP adres en waaiers wordt gebaseerd. Deze functionaliteit laat u uw Dynamische Klassieke plaatsingen van Media met de architectuur van uw inhoudsbeheer en handelsplatform aanpassen.

Met Beveiligd testen kunt u een voorvertoning van de testversie van de website weergeven met niet-gepubliceerde inhoud.

U kunt liever een testomgeving maken in plaats van elementen openbaar te maken, en wel om de volgende redenen:

* Geef een voorvertoning weer van websites voordat u deze openbaar maakt (website die wordt gefaseerd).
* Serve activa die beperkte toegang, zoals eCatalogi vereisen die prijzen in een B2B Webtoepassing tonen.
* Gebruik middelen achter een firewall als onderdeel van het systeem voor productinformatiebeheer, de toepassing van de klantenservice, de trainingssite enzovoort.

>[!NOTE]
>
>Beveiligd testen heeft geen invloed op de toegang tot Dynamic Media Classic. Dynamic Media Classic blijft consistent en vereist de gebruikelijke referenties voor toegang tot Dynamic Media Classic en verwante webservices.

## Hoe Veilig testen werkt {#how-secure-testing-works}

De meeste bedrijven voeren hun Internet achter een firewall in werking. De toegang tot Internet is mogelijk door bepaalde routes en typisch door een beperkte waaier van openbare IP adressen.

Van uw collectief netwerk, kunt u uw openbare IP adres ontdekken gebruikend websites zoals https://whatismyip.com of om deze informatie van uw collectieve organisatie van IT verzoeken.

Met het Veilige Testen, leidt de Dynamische Klassiek van Media tot een specifieke Server van het Beeld voor het opvoeren van milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd. De dynamische Beheerder van het Bedrijf van Media Klassieke vormt de goedgekeurde lijst van IP adressen voor het Veilige Testen van hun bedrijf milieu.

Omdat de plaats van het originele verzoek moet worden bevestigd, wordt het verkeer van de Veilige Testende dienst niet verpletterd door een netwerk van de inhoudsdistributie zoals het openbare Dynamische verkeer van de Server van het Beeld van Media. Verzoeken naar de service Beveiligd testen kunnen een iets hogere latentie hebben dan de openbare Dynamic Media Image Servers.

Niet-gepubliceerde middelen zijn direct beschikbaar bij de services voor het beveiligen van tests, zonder dat ze hoeven te worden gepubliceerd. Op deze manier kunt u een voorvertoning uitvoeren voordat elementen worden gepubliceerd naar hun openbare afbeeldingsserver.

***opmerking **: Beveiligde testservices maken gebruik van de Catalogusserver die is geconfigureerd met een interne publicatiecontext. Daarom als uw bedrijf wordt gevormd om te publiceren om het Veilige Testen te beveiligen, me ervan bewust ben dat om het even welke geuploade activa in Dynamische Klassiek van Media onmiddellijk beschikbaar op de Veilige Testende diensten worden. Deze functionaliteit is van toepassing, ongeacht of de elementen zijn gemarkeerd voor publiceren tijdens het uploaden.*

De Secure Testing-services bieden momenteel ondersteuning voor de volgende typen middelen en functies:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Afbeeldingen.
* Vignettes (aanvragen van Server renderen).
* Serveraanvragen renderen (ondersteund, maar moet expliciet door de klant worden aangevraagd).
* Sets, inclusief afbeeldingssets, eCatalog, rendersets en mediasets.
* Standaard Dynamic Media Classic-rijke mediaviewers.
* Dynamic Media Classic OnDemand JSP-pagina&#39;s.
* Statische inhoud, zoals PDF-bestanden en progressief bediende video&#39;s.
* HTTP-videostreaming.
* Progressieve videostreaming.

De volgende elementtypen en -functies worden momenteel niet ondersteund:

* RTMP-videostreaming
* UGC-services
* Web-to-print
* Dynamische media Klassieke Info of eCatalog onderzoek

## De service Beveiligde tests testen {#testing-the-secure-testing-service}

U moet de service Beveiligd testen testen testen om te controleren of deze naar behoren werkt.

Opmerking: Als u geen IP&#39;s onder Opstelling > noemt publiceer Opstelling > de Server van het Beeld > de Dienst van het Beeld van de Test als u IP slechts toevoegt dat IP de activa zal kunnen roepen en geen andere IP zal worden toegestaan om de vraag te maken. Zolang er geen IP onder die sectie wordt vermeld worden alle IP&#39;s toegestaan om de vraag naar de activa te maken, en zij zullen verschijnen.

**Uw account voorbereiden**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Neem contact op met de technische ondersteuning en vraag of Secure Testing is ingeschakeld voor uw account.
1. Klik in Dynamic Media Classic op **Instellen** > **Publicatie-instelling** > **Afbeeldingsserver**.
1. Voor de Server van het Beeld publiceert pagina, in de Publish drop-down lijst van de Context, uitgezochte Beeld **Test Serving**.
1. Voor de Filter van het Adres van de Cliënt, voegt de klik **toe**.
1. Schakel het selectievakje in om het adres in te schakelen (inschakelen) en typ vervolgens een IP-adres en netmasker in de desbetreffende tekstvelden.

   >[!NOTE]
   >
   >Als u één enkel IP adres en netto masker toevoegt, kan dat adres activavraag maken. Nochtans, zijn om het even welke andere IP adressen en netmaskers die u toevoegt niet toegestaan om activa te maken vraag. Als dusdanig, kunt u willen overwegen onbruikbaar makend (draai uit) de controledoos in de stap hierboven om de capaciteit uit te zetten om een IP adres en een netto masker te specificeren. Het doen zo laat effectief *alle* IP adressen toe om activa vraag te maken, en zij zullen allen verschijnen.

1. Voer een van de volgende handelingen uit:
   * Herhaal de vorige twee stappen om meer IP adressen toe te voegen.
   * Ga door met de volgende stap.
1. Linksonder op de pagina Publiceren afbeeldingsserver klikt u op **Opslaan**
1. Upload de gewenste afbeeldingen naar uw Dynamic Media Classic-account.

   Zie Bestanden [uploaden](uploading-files.md#uploading_files).

1. Zorg ervoor dat sommige afbeeldingen zijn gemarkeerd voor publicatie en andere niet zijn gemarkeerd en verzend vervolgens de publicatietaak.

   Zie [Publiceren](publishing-files.md#publishing_files).

1. Bepaal de naam van uw Secure Testing service door te klikken op **Setup** > **Application Setup** > **General Settings**.
1. Voor de pagina van de Montages van de Toepassing Algemene, onder de groep van Servers, vind de naam rechts van de Naam **van de Server van de Context van de** Test Publish.

Neem contact op met de Adobe-service als de servernaam ontbreekt of als de URL&#39;s naar de server niet werken.

**Websitevariaties voorbereiden**

U hebt twee variaties nodig van een website die de gepubliceerde en niet-gepubliceerde elementen koppelt:

* Openbare versie - Koppel elementen met behulp van uw traditionele syntaxis voor de klassieke URL van Dynamic Media.
* Versie Staging - Koppel elementen met dezelfde syntaxis, maar met de naam van de site voor Beveiligd testen.

**De tests uitvoeren**

Voer de volgende tests uit:

1. Controleer of elementen zichtbaar zijn vanuit uw bedrijfsnetwerk.

   Van binnen het collectieve netwerk dat door de eerder bepaalde IP adreswaaier wordt geïdentificeerd, zou de het opvoeren versie van de website alle beelden moeten tonen, of duidelijk voor publicatie of niet. Zo kunt u testen zonder dat u per ongeluk afbeeldingen ter beschikking stelt voordat u een voorvertoning goedkeurt of het product start.

   Bevestig dat in de openbare versie van uw site gepubliceerde middelen worden weergegeven zoals die eerder met Dynamic Media Classic werden ervaren.

1. Van buiten uw bedrijfsnetwerk, verifieer dat nonpublished activa (d.w.z. unmarked voor publiceren) tegen derdetoegang worden beschermd.

   Heb toegang tot uw netwerk van buitenaf (zoals, van uw huiscomputer of over een 3G verbinding), dan verifieer dat de openbare versie van de plaats alle gepubliceerde activa maar geen van de niet gepubliceerde inhoud toont.

   Bevestig dat de het opvoeren versie geen activa toont omdat u tot de Veilige Testende dienst van een niet goedgekeurd IP adres toegang hebt.

