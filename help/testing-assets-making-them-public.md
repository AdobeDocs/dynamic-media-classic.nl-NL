---
title: Elementen testen voordat ze openbaar worden gemaakt
seo-title: Elementen testen voordat ze openbaar worden gemaakt
description: 'null'
seo-description: Leer hoe u elementen kunt testen voordat u ze openbaar maakt.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

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
>Het Veilige Testen beïnvloedt geen toegang tot het het Publiceren Scene7 Systeem. De veiligheid van SPS blijft verenigbaar en vereist de gebruikelijke geloofsbrieven voor toegang tot SPS en verwante Webdiensten.

## Hoe Veilig testen werkt {#how-secure-testing-works}

De meeste bedrijven voeren hun Internet achter een firewall in werking. De toegang tot Internet is mogelijk door bepaalde routes en typisch door een beperkte waaier van openbare IP adressen.

Van uw collectief netwerk, kunt u uw openbare IP adres ontdekken gebruikend websites zoals https://whatismyip.com of om deze informatie van uw collectieve organisatie van IT verzoeken.

Met het Veilige Testen, leidt de Dynamische Klassiek van Media tot een specifieke Server van het Beeld voor het opvoeren van milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd. De dynamische Beheerder van het Bedrijf van Media Klassieke vormt de goedgekeurde lijst van IP adressen voor het Veilige Testen van hun bedrijf milieu.

Omdat de plaats van het originele verzoek moet worden bevestigd, wordt het verkeer van de Veilige Testende dienst niet verpletterd door een netwerk van de inhoudsdistributie zoals het openbare Dynamische verkeer van de Server van het Beeld van Media. Verzoeken naar de service Beveiligd testen kunnen een iets hogere latentie hebben dan de openbare Dynamic Media Image Servers.

Niet-gepubliceerde middelen zijn direct beschikbaar bij de services voor het beveiligen van tests, zonder dat ze hoeven te worden gepubliceerd. Op deze manier kunt u een voorvertoning uitvoeren voordat elementen worden gepubliceerd naar hun openbare afbeeldingsserver.

***opmerking **: Beveiligde testservices maken gebruik van de Catalogusserver die is geconfigureerd met een interne publicatiecontext. Daarom als uw bedrijf wordt gevormd om te publiceren om het Veilige Testen te beveiligen, ben zich ervan bewust dat om het even welke geuploade activa in het Publiceren Scene7 Systeem onmiddellijk beschikbaar op de Veilige Testende diensten worden. Deze functionaliteit is van toepassing, ongeacht of de elementen zijn gemarkeerd voor publiceren tijdens het uploaden.*

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

**Uw account voorbereiden**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Neem contact op met de technische ondersteuning en vraag of Secure Testing is ingeschakeld voor uw account.
1. In het Publiceren Scene7 Systeem, klik **Opstelling** > **Publish Opstelling** > de Server **van het** Beeld.
1. Voor de Server van het Beeld publiceert pagina, in de Publish drop-down lijst van de Context, uitgezochte Beeld **Test Serving**.
1. Voor de Filter van het Adres van de Cliënt, voegt de klik **toe**.
1. Schakel het selectievakje in om het adres in te schakelen (inschakelen) en typ vervolgens een IP-adres en netmasker in de desbetreffende tekstvelden.
1. Herhaal de vorige twee stappen om meer IP adressen toe te voegen. Anders gaat u door met de volgende stap.
1. Linksonder op de pagina Publiceren afbeeldingsserver klikt u op **Opslaan**
1. Upload de gewenste beelden aan uw Scene7 het Publiceren van de Rekening van het Systeem.

   Zie Bestanden [uploaden](uploading-files.md#uploading_files).

1. Zorg ervoor dat sommige afbeeldingen zijn gemarkeerd voor publicatie en andere niet zijn gemarkeerd en verzend vervolgens de publicatietaak.

   Zie [Publiceren](publishing-files.md#publishing_files).

1. Bepaal de naam van uw Secure Testing service door te klikken op **Setup** > **Application Setup** > **General Settings**.
1. Voor de pagina van de Montages van de Toepassing Algemene, onder de groep van Servers, vind de naam rechts van de Naam **van de Server van de Context van de** Test Publish.

Neem contact op met Technische ondersteuning als de servernaam ontbreekt of als URL&#39;s naar de server niet werken.

**Websitevariaties voorbereiden**

U hebt twee variaties nodig van een website die de gepubliceerde en niet-gepubliceerde elementen koppelt:

* Openbare versie: Elementen koppelen met behulp van de traditionele syntaxis van Dynamic Media Classic URL
* Staging versie: Elementen koppelen met dezelfde syntaxis, maar met de sitenaam voor Beveiligd testen

**De tests uitvoeren**

Voer de volgende tests uit:

1. Controleer of elementen zichtbaar zijn vanuit uw bedrijfsnetwerk.

   Van binnen het collectieve netwerk dat door de eerder bepaalde IP adreswaaier wordt geïdentificeerd, zou de het opvoeren versie van de website alle beelden moeten tonen, of duidelijk voor publicatie of niet. Zo kunt u testen zonder dat u per ongeluk afbeeldingen ter beschikking stelt voordat u een voorvertoning goedkeurt of het product start.

   Bevestig dat in de openbare versie van uw site gepubliceerde middelen worden weergegeven zoals die eerder met Dynamic Media Classic werden ervaren.

1. Van buiten uw bedrijfsnetwerk, verifieer dat nonpublished activa (d.w.z. unmarked voor publiceren) tegen derdetoegang worden beschermd.

   Heb toegang tot uw netwerk van buitenaf (zoals, van uw huiscomputer of over een 3G verbinding), dan verifieer dat de openbare versie van de plaats alle gepubliceerde activa maar geen van de niet gepubliceerde inhoud toont.

   Bevestig dat de het opvoeren versie geen activa toont omdat u tot de Veilige Testende dienst van een niet goedgekeurd IP adres toegang hebt.

