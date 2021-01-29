---
title: Elementen testen voordat ze openbaar worden gemaakt
description: Leer hoe u elementen kunt testen voordat u ze openbaar maakt.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1096'
ht-degree: 0%

---


# Elementen testen voordat ze openbaar worden gemaakt {#testing-assets-before-making-them-public}

Het veilige Testen helpt u een veilige testmilieu bepalen en een robuuste B2B oplossing bouwen, die op een configureerbare reeks IP adres en waaiers wordt gebaseerd. Met deze functionaliteit kunt u uw Klassieke Dynamic Media-implementaties afstemmen op de architectuur van uw contentbeheer- en handelsplatform.

Met Beveiligd testen kunt u een voorvertoning van de testversie van de website weergeven met niet-gepubliceerde inhoud.

U kunt liever een testomgeving maken in plaats van elementen openbaar te maken, en wel om de volgende redenen:

* Geef een voorvertoning weer van websites voordat u deze openbaar maakt (website die wordt gefaseerd).
* Serve activa die beperkte toegang, zoals eCatalogi vereisen die prijzen in een B2B Webtoepassing tonen.
* Gebruik middelen achter een firewall als onderdeel van het systeem voor productinformatiebeheer, de toepassing van de klantenservice, de trainingssite enzovoort.

>[!NOTE]
>
>Beveiligd testen heeft geen invloed op de toegang tot Dynamic Media Classic. De Klassieke veiligheid van Dynamic Media blijft verenigbaar en vereist de gebruikelijke geloofsbrieven voor toegang tot de Klassieke van Dynamic Media en verwante Webdiensten.

## Hoe werkt Beveiligd testen {#how-secure-testing-works}

De meeste bedrijven voeren hun Internet achter een firewall in werking. De toegang tot Internet is mogelijk door bepaalde routes en typisch door een beperkte waaier van openbare IP adressen.

Van uw collectief netwerk, kunt u uw openbare IP adres ontdekken gebruikend websites zoals https://whatismyip.com of om deze informatie van uw collectieve organisatie van IT verzoeken.

Met het Veilige Testen, vestigt Dynamic Media Classic een specifieke server van het Beeld voor het opvoeren van milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd. De Klassieke Beheerder van het Bedrijf van Dynamic Media vormt de goedgekeurde lijst van IP adressen voor het Veilige Testen van hun bedrijf milieu.

Omdat de plaats van het originele verzoek moet worden bevestigd, wordt het verkeer van de Veilige Testende dienst niet verpletterd door een netwerk van de inhoudsdistributie zoals het openbare verkeer van de Server van het Beeld van Dynamic Media. Verzoeken naar de service Beveiligd testen kunnen een iets hogere latentie hebben dan de openbare Dynamic Media Image Servers.

Niet-gepubliceerde middelen zijn direct beschikbaar bij de services voor het beveiligen van tests, zonder dat ze hoeven te worden gepubliceerd. Op deze manier kunt u een voorvertoning uitvoeren voordat elementen worden gepubliceerd naar hun openbare afbeeldingsserver.

***opmerking **: Beveiligde testservices maken gebruik van de Catalogusserver die is geconfigureerd met een interne publicatiecontext. Als uw bedrijf is geconfigureerd om te publiceren voor Secure Testing, dient u er rekening mee te houden dat geüploade elementen in Dynamic Media Classic direct beschikbaar zijn voor de services voor Beveiligd testen. Deze functionaliteit is van toepassing, ongeacht of de elementen zijn gemarkeerd voor publiceren tijdens het uploaden.*

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
* Standaard Dynamic Media Classic rijke mediaviewers.
* Dynamic Media Classic OnDemand JSP-pagina&#39;s.
* Statische inhoud, zoals PDF-bestanden en progressief bediende video&#39;s.
* HTTP-videostreaming.
* Progressieve videostreaming.

De volgende elementtypen en -functies worden momenteel niet ondersteund:

* RTMP-videostreaming
* UGC-services
* Web-to-print
* Dynamic Media Klassieke Info of eCatalog zoeken

## De service Beveiligen testen {#testing-the-secure-testing-service} testen

U moet de service Beveiligd testen testen testen om te controleren of deze naar behoren werkt.

Opmerking: Als u geen IP&#39;s noemt onder Setup > Publish Setup > Image Server > Test Image Service
als u IP slechts toevoegt dat IP de activa zal kunnen roepen en geen andere IP zal worden toegestaan om de vraag te maken. Zolang er geen IP onder die sectie wordt vermeld worden alle IP&#39;s toegestaan om de vraag naar de activa te maken, en zij zullen verschijnen.

**Uw account voorbereiden**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Neem contact op met de technische ondersteuning en vraag of Secure Testing is ingeschakeld voor uw account.
1. Klik in Dynamic Media Classic op **Setup** > **Publicatie-instelling** > **Afbeeldingsserver**.
1. Selecteer **Beeld testen dat** dient in de vervolgkeuzelijst Publicatie-context op de pagina Publiceren afbeeldingsserver.
1. Voor de Filter van het Adres van de Cliënt, klik **Add**.
1. Schakel het selectievakje in om het adres in te schakelen (inschakelen) en typ vervolgens een IP-adres en netmasker in de desbetreffende tekstvelden.

   >[!NOTE]
   >
   >Als u één enkel IP adres en netto masker toevoegt, kan dat adres activavraag maken. Nochtans, zijn om het even welke andere IP adressen en netmaskers die u toevoegt niet toegestaan om activa te maken vraag. Als dusdanig, kunt u willen overwegen onbruikbaar makend (draai uit) de controledoos in de stap hierboven om de capaciteit uit te zetten om een IP adres en een netto masker te specificeren. Het doen van dit laat effectief *alle* IP adressen toe om activa vraag te maken, en zij zullen allen verschijnen.

1. Voer een van de volgende handelingen uit:
   * Herhaal de vorige twee stappen om meer IP adressen toe te voegen.
   * Ga door met de volgende stap.
1. Linksonder op de pagina Publiceren afbeeldingsserver klikt u op **Opslaan**
1. Upload de gewenste afbeeldingen naar uw Dynamic Media Classic-account.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Zorg ervoor dat sommige afbeeldingen zijn gemarkeerd voor publicatie en andere niet zijn gemarkeerd en verzend vervolgens de publicatietaak.

   Zie [Publiceren](publishing-files.md#publishing_files).

1. Bepaal de naam van uw Secure Testing service door te klikken op **Setup** > **Application Setup** > **Algemene instellingen**.
1. Voor de pagina van de Montages van de Toepassing Algemene, onder de groep van Servers, vind de naam rechts van **de Naam van de Server van de Context van de Publicatie van de Test**.

Neem contact op met de Adobe-service als de servernaam ontbreekt of als de URL&#39;s naar de server niet werken.

**Websitevariaties voorbereiden**

U hebt twee variaties nodig van een website die de gepubliceerde en niet-gepubliceerde elementen koppelt:

* Openbare versie - Koppel elementen met behulp van uw traditionele Dynamic Media Classic URL-syntaxis.
* Versie Staging - Koppel elementen met dezelfde syntaxis, maar met de naam van de site voor Beveiligd testen.

**De tests uitvoeren**

Voer de volgende tests uit:

1. Controleer of elementen zichtbaar zijn vanuit uw bedrijfsnetwerk.

   Van binnen het collectieve netwerk dat door de eerder bepaalde IP adreswaaier wordt geïdentificeerd, zou de het opvoeren versie van de website alle beelden moeten tonen, of duidelijk voor publicatie of niet. Zo kunt u testen zonder dat u per ongeluk afbeeldingen ter beschikking stelt voordat u een voorvertoning goedkeurt of het product start.

   Bevestig dat in de openbare versie van uw site de gepubliceerde middelen worden weergegeven zoals die eerder met Dynamic Media Classic werden gebruikt.

1. Van buiten uw bedrijfsnetwerk, verifieer dat nonpublished activa (d.w.z. unmarked voor publiceren) tegen derdetoegang worden beschermd.

   Heb toegang tot uw netwerk van buitenaf (zoals, van uw huiscomputer of over een 3G verbinding), dan verifieer dat de openbare versie van de plaats alle gepubliceerde activa maar geen van de niet gepubliceerde inhoud toont.

   Bevestig dat de het opvoeren versie geen activa toont omdat u tot de Veilige Testende dienst van een niet goedgekeurd IP adres toegang hebt.

