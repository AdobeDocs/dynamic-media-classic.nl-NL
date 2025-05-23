---
title: Bestanden publiceren
description: Leer hoe u uw middelen publiceert naar Dynamic Media Image Servers.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 0%

---

# Bestanden publiceren{#publishing-files}

U publiceert uw middelen naar Dynamic Media Image Servers. U kunt elementen eenmalig publiceren of ervoor zorgen dat Adobe Dynamic Media Classic elementen volgens een terugkerend schema publiceert. Nadat uw activa worden gepubliceerd, zijn zij beschikbaar aan u voor levering. U kunt de URL-aanroepen van Adobe Dynamic Media Classic kopiëren en toevoegen aan uw website of toepassing.

Adobe Dynamic Media Classic ondersteunt nu de levering van alle afbeeldingen en video via HTTP/2. Er is dus een gepubliceerde URL of code voor insluiten beschikbaar voor de afbeelding of video die moet worden geïntegreerd met elke toepassing die een gehoste element accepteert. Dat gepubliceerde element gebruikt het HTTP/2-protocol om het te leveren. Deze leveringsmethode verbetert de manier waarop browsers en servers communiceren, waardoor u betere responstijd en laadtijden voor al uw Adobe Dynamic Media Classic-middelen krijgt. Zie [HTTP2 Veelgestelde vragen over inhoud](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/dynamic/http2).

## Publiceren na uploaden {#publish-after-uploading}

Activa in een gepubliceerde of niet-gepubliceerde status. Standaard worden alle elementen die u uploadt naar Adobe Dynamic Media Classic automatisch gemarkeerd voor publicatie.

Zie de klasse [Instant Publish Notice PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

Gebruik de volgende technieken om elementen te markeren voor publicatie:

* **[!UICONTROL Publish After Uploading]**: Selecteer onder aan op de pagina Uploaden de optie **[!UICONTROL Publish After Uploading]**. De standaardinstelling is een geselecteerde status.

* **[!UICONTROL Publish After Uploading]**: Selecteer in het dialoogvenster Taakopties **[!UICONTROL Publish After Uploading]**. De standaardinstelling is een geselecteerde status.

Sommige &quot;onderliggende&quot; elementen worden automatisch gemarkeerd voor publicatie wanneer hun ouders zijn gemarkeerd voor publicatie. Deze tabel bevat een lijst met onderliggende elementen die automatisch zijn gemarkeerd voor publicatie.

| Bovenliggend item (groep) | Onderliggende items (lid) |
| --- | --- |
| Afbeeldingssets | Afbeeldingen in de set. |
| Staalsets | Stalen in de set. |
| Sets draaien | Afbeeldingen in de set. |
| Sjablonen | Sjabloonbestanden, pagina&#39;s en afbeeldingen. |

Afgeleide afbeeldingen worden ook automatisch gemarkeerd voor publicatie wanneer de bovenliggende afbeeldingen worden gepubliceerd. Afgeleide afbeeldingen bevatten afbeeldingen die u hebt aangepast met opties voor het bewerken van afbeeldingen. U kunt deze afgeleide beelden in de Gedetailleerde Mening onder Bouwstijl &amp; Derivaten zien.

## Een publicatietaak maken {#creating-a-publish-job}

Maak een publicatietaak om elementen te publiceren die u naar Adobe Dynamic Media Classic-servers hebt geüpload, maar deze nog niet automatisch wilt publiceren. U kunt een eenmalige publicatietaak uitvoeren of taken plannen die regelmatig opnieuw worden uitgevoerd. Adobe Dynamic Media Classic biedt geavanceerde publicatieopties voor het publiceren naar specifieke servers en opties voor het opnieuw publiceren van middelen die al zijn gepubliceerd.

**Een publicatietaak maken:**

1. Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Publish]**.
1. Kies in het dialoogvenster Publiceren of u een eenmalige of terugkerende publicatietaak wilt uitvoeren.

   Zie [Een eenmalige publicatietaak maken](publishing-files.md#creating_a_one_time_publish_job) en [Een terugkerende publicatietaak maken](publishing-files.md#creating_a_recurring_publish_job).

1. Voer een taaknaam in.
1. Geef desgewenst de geavanceerde opties weer en kies deze opties.

   Zie [Geavanceerde publicatieopties](publishing-files.md#advanced_publish_options).

1. Selecteren **[!UICONTROL Submit Publish]**.

Adobe Dynamic Media Classic houdt publicatietaken bij op de pagina Jobs. U kunt publicatietaken op die pagina controleren.

>[!NOTE]
>
>Elementen die u opnieuw hebt gepubliceerd (en die u eerder hebt gepubliceerd) worden niet direct op uw website weergegeven vanwege het mechanisme voor webcaching op het CDN (Content Delivery Network). Zie [Hergepubliceerde elementen en CDN-vertragingen](publishing-files.md#republished_assets_and_cdn_delays).

### Een eenmalige publicatietaak maken {#creating-a-one-time-publish-job}

Maak een eenmalige publicatietaak door de optie **[!UICONTROL One-Time]** op de pagina Publiceren.

Als u wilt dat de publicatietaak later plaatsvindt, selecteert u op de pagina Publiceren de optie **[!UICONTROL One-Time]**. Selecteer in de vervolgkeuzelijst de optie **[!UICONTROL Schedule For Later]**. Gebruik de schuifregelaar Kalender en Tijd om een dag en tijd te selecteren waarop u de publicatietaak wilt uitvoeren.

### Een terugkerende publicatietaak maken {#creating-a-recurring-publish-job}

Een terugkerende publicatietaak maken door **[!UICONTROL Recurring]** op de pagina Publiceren.

Kies vervolgens de optie Herhalen van **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]**, of **[!UICONTROL Custom]** en geeft u op wanneer de publicatietaak moet worden herhaald. Adobe Dynamic Media Classic presenteert kalendergereedschappen voor het plannen van de terugkerende publicatietaak. U kunt de **[!UICONTROL Custom]** en voert u een regel in het tekstveld Regel in om een aangepast taakinterval te beschrijven.

Zie [Een aangepast tijdinterval voor uploaden of publiceren maken](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Terugkerende publiceer (en upload) banen zijn vermeld op de pagina van Banen. U kunt een geplande baan uitgeven of schrappen door naar het Geplande lusje van de pagina van Banen te gaan.

### Geavanceerde publicatieopties {#advanced-publish-options}

U kunt de Geavanceerde opties weergeven op de pagina Publiceren en deze opties kiezen voor het afhandelen van een publicatietaak:

* **[!UICONTROL Publish To]**: Als u elementen alleen naar een specifieke server wilt publiceren, kiest u een servertype.

* **[!UICONTROL Publish]**: Standaard publiceert Adobe Dynamic Media Classic alleen elementen die nieuw zijn en nog niet eerder zijn gepubliceerd (de optie Nieuw sinds laatste publicatie). U kunt echter **[!UICONTROL Full Publish]** dus u kunt ook elementen publiceren die zijn bijgewerkt of gewijzigd sinds ze voor het laatst zijn gepubliceerd. Selecteren **[!UICONTROL Full w/ Search Data]** als u een eCatalog publiceert en u lezers het door sleutelwoord wilt kunnen zoeken.

* **[!UICONTROL Run Job As]**: Kies een gebruikersnaam in de lijst. U kunt taken sorteren op gebruikersnaam op de pagina Taken. Als u een naam kiest, koppelt u een publicatietaak aan een gebruiker.

**[!UICONTROL HTTP Notification]**: Voer een URL in om volgende publicatietaken te activeren.

Zie [Een upload- of publicatietaak gebruiken als trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Een publicatietaak annuleren {#canceling-a-publish-job}

U kunt een publicatietaak die wordt uitgevoerd, annuleren. Bovendien als u een beheerder bent, kunt u een lopende het publiceren baan van de pagina van Banen van het bedrijf annuleren.

Als u een publicatietaak wilt annuleren, gaat u naar de pagina Taken en selecteert u **[!UICONTROL Cancel]**. Op het Geplande lusje van de pagina van Banen, kunt u een baan pauzeren of hervatten door het controlevakje in de Actieve kolom van de baan te schrappen of te selecteren.

>[!NOTE]
>
>Nadat u een publicatietaak hebt geannuleerd, verandert de status in &quot;stoppen&quot; totdat de taak een punt bereikt waarop deze veilig kan stoppen. Het kan enige tijd duren voordat een publicatietaak wordt gestopt als de taak bezig is gegevens uit de database op te halen.

## Elementen handmatig publiceren {#manually-publishing-assets}

U kunt afzonderlijke elementen handmatig publiceren in plaats van een publicatietaak te maken. Wanneer u sets publiceert, zoals een Afbeeldingsset of een Adaptieve videoset, worden de set (of &quot;bovenliggend item&quot;) en alle leden (of &quot;onderliggende items&quot;) binnen die set gepubliceerd.

Niet-gepubliceerde elementen worden in de gebruikersinterface aangeduid met een grijs, rond pictogram met een schuine streep erdoor (niet-gepubliceerde status), links van de naam van het element. Nadat een element is gepubliceerd, wordt het pictogram groen en heeft het een wit vinkje in het midden (gepubliceerde staat).

**Elementen handmatig publiceren:**

1. Voer een van de volgende handelingen uit:

   * Gebruik in de rasterweergave, lijstweergave of detailweergave de standaardmethoden voor het selecteren van bestanden om een of meer niet-gepubliceerde elementen te selecteren.

     Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Publish]**.

   * Selecteer in de rasterweergave, lijstweergave of detailweergave het grijze, ronde pictogram met een schuine streep erdoorheen, links van de naam van het element.

## Elementen handmatig verwijderen {#manually-unpublishing-assets}

U kunt afzonderlijke elementen handmatig verwijderen. Wanneer u de publicatie van sets, zoals een stalenset of een eCatalog, ongedaan maakt, wordt de set (of &quot;bovenliggend&quot;) zelf omgezet in een niet-gepubliceerde status. De leden (of &quot;kinderen&quot;) binnen die set worden echter niet beïnvloed, maar ze behouden hun bestaande gepubliceerde of niet-gepubliceerde status.

Gepubliceerde elementen worden in de gebruikersinterface aangeduid met een rond, groen pictogram met een wit vinkje in het midden (gepubliceerde status), links van de naam van het element. Nadat een element niet is gepubliceerd, wordt het pictogram grijs met een schuine streep erdoorheen (niet-gepubliceerde status).

**De publicatie van elementen handmatig ongedaan maken:**

1. Voer een van de volgende handelingen uit:

   * Selecteer een of meer gepubliceerde elementen in de rasterweergave, lijstweergave of detailweergave.

     Ga op de algemene navigatiebalk naar **[!UICONTROL File]** > **[!UICONTROL Unpublish]**.

   * Selecteer in de rasterweergave, de lijstweergave of de detailweergave het ronde groene vinkje links van de naam van het element.

## De publicatiegeschiedenis van een element ophalen {#getting-an-asset-s-publish-history}

De laatste datum waarop een element is gepubliceerd, wordt weergegeven in de gedetailleerde weergave boven in het deelvenster. U kunt meer details over de publicatiegeschiedenis krijgen door het paneel Geschiedenis &amp; Gepubliceerde Servers in de Gedetailleerde Mening te openen. Vanaf dat punt kunt u zien wanneer het middel is gepubliceerd en naar welke servers het is gepubliceerd.

## Hergepubliceerde elementen en CDN-vertragingen {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic-elementen worden gedistribueerd op het CDN (Content Delivery Network). CDN is een systeem van computerservers die samen samenwerken om inhoud, vooral grote media inhoud, aan eind te leveren - gebruikers. In het systeem CDN, wordt de inhoud van het Web opgeslagen in de geheime voorgeheugens van het Web over Internet (genoemd het netwerk van het randgeheime voorgeheugen). De inhoud van het Web wordt geleverd van de geheime voorgeheugens van het Web aan eind - gebruikers om voor snellere leveringen te maken.

De eerste keer iemand downloadt een Web-pagina, worden de activa geleverd aan een CDN het geheim voorgeheugenserver van het Web. Deze server slaat hen op zodat de volgende keer iemand in het zelfde gebied tot de Web-pagina toegang heeft, wordt de zelfde caching inhoud sneller geleverd. De inhoud wordt sneller geleverd, omdat deze zich dichter bij de eindgebruiker bevindt. CDN maakt snellere Web-pagina vertoningen. Het vermindert bandbreedteeisen op de centrale server omdat de inhoud van het netwerk van het randgeheime voorgeheugen, niet van een centrale server in elke instantie wordt geleverd.

Nieuw gepubliceerde Adobe Dynamic Media Classic-inhoud is direct beschikbaar voor de eindgebruiker en wordt snel in het Edge-cachenetwerk geplaatst. Nochtans, worden de onlangs opnieuw gepubliceerde inhoud, dat wil zeggen, de beelden die de zelfde namen hebben zoals beelden eerder aan een Server van het Beeld werden gepubliceerd, niet bijgewerkt op CDN tot tien uur. In plaats daarvan, zien de eindgebruikers wat in een geheime voorgeheugen van het Web op het netwerk CDN is. Daarom worden de opnieuw gepubliceerde Adobe Dynamic Media Classic-middelen tien uur lang niet weergegeven voor eindgebruikers.

Als u wilt dat de nieuw gepubliceerde afbeeldingselementen sneller beschikbaar zijn dan de vertraging van tien uur, kunt u webcaches op CDN leegmaken. Als u deze webcaches leegmaakt, wordt oude inhoud uit CDN-webcaches verwijderd en vervangen door de laatst gepubliceerde elementen.

Ga naar **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]**. Alle geselecteerde bestanden worden uit de cache verwijderd. Als er geen publiceerbare activa zijn, of als u geen bedrijfbeheerder bent, verwijdert uit CDN is de optie niet beschikbaar.

>[!MORELIKETHIS]
>
>* [Taakbestanden controleren](checking-job-files.md)
>* [Herhaalde taken bewerken, verwijderen, pauzeren en hervatten](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
