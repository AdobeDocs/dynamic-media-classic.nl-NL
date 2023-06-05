---
title: Elementen testen voordat ze openbaar worden gemaakt
description: Leer hoe u elementen in Adobe Dynamic Media Classic kunt testen voordat u ze openbaar maakt.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Elementen testen voordat ze openbaar worden gemaakt {#testing-assets-before-making-them-public}

Het veilige Testen helpt u een veilige testmilieu bepalen en een robuuste B2B oplossing bouwen, die op een configureerbare reeks IP adres en waaiers wordt gebaseerd. Met deze functionaliteit kunt u uw Adobe Dynamic Media Classic-implementaties afstemmen op de architectuur van uw contentbeheer en bedrijfssysteem.

Met Beveiligd testen kunt u een voorvertoning van de testversie van de website weergeven met niet-gepubliceerde inhoud.

Maak indien gewenst een testomgeving in plaats van elementen openbaar te maken, en wel om de volgende redenen:

* Geef een voorvertoning weer van websites voordat u deze openbaar maakt (website die wordt gefaseerd).
* Serve activa die beperkte toegang, zoals eCatalogi vereisen die prijzen in een B2B Webtoepassing tonen.
* Gebruik middelen achter een firewall als onderdeel van het systeem voor productinformatiebeheer, de toepassing van de klantenservice, de trainingssite enzovoort.

>[!NOTE]
>
>Beveiligd testen heeft geen invloed op de toegang tot Adobe Dynamic Media Classic. De beveiliging van Adobe Dynamic Media Classic blijft consistent en vereist de gebruikelijke aanmeldingsgegevens voor toegang tot Adobe Dynamic Media Classic en verwante webservices.

## Hoe Veilig testen werkt {#how-secure-testing-works}

De meeste bedrijven voeren hun Internet achter een firewall in werking. De toegang tot Internet is mogelijk door bepaalde routes en typisch door een beperkte waaier van openbare IP adressen.

Van uw collectief netwerk, kunt u uw openbaar IP adres uitvinden gebruikend websites zoals [https://www.whatismyip.com](https://www.whatismyip.com/) of vraag deze informatie aan bij uw IT-organisatie van uw bedrijf.

Met het Veilige Testen, vestigt Adobe Dynamic Media Classic een specifieke Server van het Beeld voor het opvoeren van milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd. De Beheerder van het Bedrijf van Adobe Dynamic Media Classic vormt de goedgekeurde lijst van IP adressen voor het Veilige Testen van hun bedrijf milieu.

Omdat de plaats van het originele verzoek moet worden bevestigd, wordt het verkeer van de Veilige Testende dienst niet verpletterd door een netwerk van de inhoudsdistributie zoals het openbare verkeer van de Server van het Beeld van Dynamic Media. Verzoeken naar de service Beveiligd testen hebben een iets hogere latentie dan de openbare Dynamic Media Image Servers.

Niet-gepubliceerde middelen zijn direct beschikbaar bij de services voor het beveiligen van tests, zonder dat ze hoeven te worden gepubliceerd. Op deze manier kunt u een voorvertoning uitvoeren voordat elementen worden gepubliceerd naar hun openbare afbeeldingsserver.

>[!NOTE]
>
>De veilige Testende diensten gebruiken de Server van de Catalogus die met een interne publicatiecontext wordt gevormd. Als uw bedrijf is geconfigureerd om te publiceren voor Secure Testing, worden geüploade middelen in Adobe Dynamic Media Classic daarom direct beschikbaar voor de services voor Beveiligd testen. Deze functionaliteit is van toepassing, ongeacht of de elementen zijn gemarkeerd voor publiceren tijdens het uploaden.

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
* Standaard Adobe Dynamic Media Classic-viewers met rijke media.
* Adobe Dynamic Media Classic OnDemand JSP-pagina&#39;s.
* Statische inhoud, zoals PDF-bestanden en progressief bediende video&#39;s.
* HTTP-videostreaming.
* Progressieve videostreaming.

De volgende elementtypen en -functies worden momenteel niet ondersteund:

* Zoeken in Adobe Dynamic Media Classic Info of eCatalog
* RTMP-videostreaming
* Web-to-print
* UGC-services (door de gebruiker gegenereerde inhoud)

>[!IMPORTANT]
>
>De ondersteuning voor nieuwe of bestaande UGC-vectorafbeeldingselementen in Adobe Dynamic Media Classic is afgelopen op 30 september 2021.

## De service Beveiligde tests testen {#testing-the-secure-testing-service}

Test de Secure Testing service zodat u zeker weet dat deze naar behoren functioneert.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Uw account voorbereiden

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Neem contact op met de klantenservice van Adobe en verzoek hen om Beveiligingstests op uw account in te schakelen.
1. Ga in Adobe Dynamic Media Classic op de Global Navigation Bar naar **[!UICONTROL Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**.
1. Op de pagina van de Server van het Beeld publiceren, in **[!UICONTROL Publish Context]** vervolgkeuzelijst, selecteert u **[!UICONTROL Test Image Serving]**.
1. Voor de Filter van het Adres van de Cliënt, selecteer **[!UICONTROL Add]**.
1. Schakel het selectievakje in zodat het adres is ingeschakeld en typ vervolgens een IP-adres en een netmasker in de desbetreffende tekstvelden.

   >[!NOTE]
   >
   >Als u één enkel IP adres en netto masker toevoegt, kan dat adres activavraag maken. Nochtans, zijn om het even welke andere IP adressen en netmaskers die u toevoegt niet toegestaan om activa te maken vraag. Als dusdanig, denk na onbruikbaar makend (draai weg) de controledoos in de stap hierboven om de capaciteit uit te zetten om een IP adres en een netto masker te specificeren. Zo effectief mogelijk maken *alles* IP adressen om activavraag te maken, en zij allen verschijnen.

1. Voer een van de volgende handelingen uit:
   * Herhaal de vorige twee stappen als u meer IP adressen moet toevoegen.
   * Ga door met de volgende stap.
1. Linksonder op de pagina Publiceren afbeeldingsserver selecteert u **[!UICONTROL Save]**
1. Upload de gewenste afbeeldingen naar uw Adobe Dynamic Media Classic-account.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Zorg ervoor dat sommige afbeeldingen zijn gemarkeerd voor publicatie en andere niet zijn gemarkeerd en verzend vervolgens de publicatietaak.

   Zie [Bestanden publiceren](publishing-files.md#publishing_files).

1. Bepaal de naam van uw Veilige het Testen dienst door te gaan **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.
1. Zoek op de pagina Algemene instellingen van toepassing de naam rechts van **[!UICONTROL Test Publish Context Server Name]**.

Neem contact op met de Adobe-service als de servernaam ontbreekt of als de URL&#39;s naar de server niet werken.

### Websitevariaties voorbereiden

U hebt twee variaties nodig van een website die de gepubliceerde en niet-gepubliceerde elementen koppelt:

* Openbare versie - Koppel elementen met behulp van uw traditionele Adobe Dynamic Media Classic URL-syntaxis.
* Versie Staging - Koppel elementen met dezelfde syntaxis, maar met de naam van de site voor Beveiligd testen.

### De tests uitvoeren

Voer de volgende tests uit:

1. Controleer of elementen zichtbaar zijn vanuit uw bedrijfsnetwerk.

   Vanuit het bedrijfsnetwerk dat door het eerder gedefinieerde IP-adresbereik wordt geïdentificeerd, worden in de testversie van de website alle afbeeldingen weergegeven, ongeacht of deze zijn gemarkeerd voor publicatie of niet. Zo kunt u testen zonder dat u per ongeluk afbeeldingen ter beschikking stelt voordat u een voorvertoning van goedkeuring of het product start.

   Bevestig dat in de openbare versie van uw site de gepubliceerde middelen worden weergegeven zoals die eerder met Adobe Dynamic Media Classic zijn gebruikt.

1. Van buiten uw bedrijfsnetwerk, verifieer dat nonpublished activa (d.w.z. unmarked voor publiceren) tegen derdetoegang worden beschermd.

   Heb toegang tot uw netwerk van buitenaf (zoals, van uw huiscomputer of over een 3G verbinding), dan verifieer dat de openbare versie van de plaats alle gepubliceerde activa maar geen van de niet gepubliceerde inhoud toont.

   Bevestig dat de het opvoeren versie geen activa toont omdat u tot de Veilige Testende dienst van een niet goedgekeurd IP adres toegang hebt.
