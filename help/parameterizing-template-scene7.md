---
title: Een sjabloon in Dynamic Media Classic parametereren
seo-title: Een sjabloon in Dynamic Media Classic parametereren
description: 'null'
seo-description: Leer hoe u parameters kunt toewijzen aan een sjabloon in Dynamic Media Classic
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Een sjabloon in Dynamic Media Classic parametereren{#parameterizing-a-template-in-scene}

Nadat u een malplaatje van de Illustrator uploadt dat u als Dynamische Klassieke FXG van Media aan het het Publiceren Scene7 Systeem bewaarde, kunt u zijn veranderlijke elementen bepalen. Doe dit door veranderlijke elementen in het Publiceren van het Malplaatje te bepalen bouwen en de schermen van de Voorproef. Dynamic Media Classic biedt gereedschappen voor het definiëren van tekst- en objectparameters op lagen en hun respectievelijke eigenschappen. U kunt ook verschillende versies van een sjabloon maken.

Door het parameters toewijzen van een FXG-sjabloon kunt u de variabiliteit van tekst, afbeeldingen en afbeeldingen in de sjabloon aanpassen. U kunt bijvoorbeeld de parameters instellen voor een tekstregel, zodat eindgebruikers de tekst kunnen wijzigen via een webgebruikersinterface. U kunt lege tekstvelden definiëren als variabelen, zodat eindgebruikers deze velden kunnen vullen met gepersonaliseerde tekst. U kunt de attributen en de eigenschappen van ontwerpelementen in het Dynamische Publiceren van het Malplaatje van Media Klassieke het Publiceren van de Bouw van het Malplaatje ook parameters bepalen scherm.

>[!NOTE]
>
>Het is niet nodig om de sjabloon in Dynamic Media Classic te parameteren als u DOM-manipulatie wilt gebruiken.

## Parameters definiëren in FXG-sjablonen {#defining-parameters-in-fxg-templates}

Voer de volgende stappen uit in Dynamic Media Classic om parameters voor een FXG-sjabloon te definiëren:

1. Selecteer het FXG-bestand in het venster Bladeren.
1. Klik op **Samenstellen** en kies **Sjabloon publiceren** of klik op de knop **Bewerken** van het bestand.

   Het scherm Sjabloon publiceren wordt geopend.

1. Selecteer LRCo\FXG\Welcome_Summit_10 (FXG-bestand) en klik op **Samenstellen** > **Sjabloon publiceren**.</p>

   ![](assets/wp_fxg_edit.png)

1. Selecteer in het deelvenster Lagen van het scherm Sjabloon publiceren de laag met de elementen die u wilt parametereren.

   >[!NOTE]
   >
   >Klik op het oogpictogram in- en uitgeschakeld om te controleren of u het gewenste object selecteert.

1. Klik in het deelvenster Eigenschappen op een parameter in de kolom Naam (om de parameters van tekst te bepalen) of in de kolom Parameter (om de parameters van objecten te bepalen).

   * **Tekst** Klik in het tekstveld (schuif naar de onderkant van de lijst Eigenschappen om het te zoeken). Het dialoogvenster Parameters wordt weergegeven. Selecteer de tekst waarvan u de parameters wilt bepalen en klik op **Toevoegen**. U kunt meerdere parameters maken van dezelfde teksteigenschap door verschillende delen van de tekst te selecteren en parameters toe te voegen voor elk deel. Als u de naam van de parameter wilt wijzigen, klikt u erop, voert u een nieuwe naam in en klikt u op **Sluiten**.

   * **Objecten** Klik op een vak in de kolom Parameter. Het dialoogvenster Parameter bewerken wordt geopend. Voer een naam in en klik op **OK**.
   Als u meerdere kenmerken tegelijk met dezelfde waarde wilt aanpassen, gebruikt u voor elk kenmerk dezelfde parameternaam. Als uw sjabloon bijvoorbeeld een rechthoek en een ster heeft, kunt u `newcolor` als parameternaam voor elk SolidColor-kleurkenmerk typen. Wanneer u de `newcolor` waarde wijzigt, veranderen zowel de rechthoek als de ster in de nieuwe kleur.

1. Geef een standaardwaarde voor het kenmerk op in het veld Waarde of Gegevens. Stel alle eigenschappen voor het geselecteerde object in om de exacte weergave op te geven die u wilt.
1. (Optioneel) Herhaal stap 3 tot en met 5 voor alle objecten of lagen waarvan u de parameters wilt bepalen.
1. Klik op **Opslaan** of **Opslaan als**.
1. Klik op **Voorvertoning** om het venster FXG-voorvertoning te openen en bekijk de parameters die u met de standaardwaarden hebt gemaakt.

## Een object of laag in de FXG-sjabloon weergeven of verbergen {#show-or-hide-an-object-or-layer-in-the-fxg-template}

Verborgen objecten en lagen zijn niet zichtbaar in de voorvertoning of uitvoer, maar worden niet uit het bestand verwijderd. U kunt ze desgewenst weer zichtbaar maken. Zichtbaarheid is een kenmerk dat u kunt variëren. Als u op het oogpictogram klikt of als u dit pictogram uitschakelt, wordt de standaardwaarde voor de zichtbaarheid van een object of laag ingesteld.

1. Klik in het deelvenster Objecten op het oogpictogram naast de naam van een object of laag om het object of de laag in het bestand te verbergen.
1. Klik nogmaals om het object zichtbaar te maken.

## Verschillende versies van een sjabloon maken {#create-different-versions-of-a-template}

U kunt kenmerken bewerken om verschillende versies van de sjabloon te maken voor verschillende toepassingen.

Klik in het scherm Sjabloon publiceren op Opslaan als om het bestand op te slaan als een nieuwe FXG-sjabloon zonder de oorspronkelijke FXG-sjabloon te overschrijven.

## Tekst met omtrek gebruiken {#using-stroked-text}

Tekst met omtrek is een voorbeeld van hoe u kenmerken kunt parametereren. Dynamic Media Classic ondersteunt de volgende tekstfuncties met omtrek:

* Breedte van lijn
* Streekpatroon onderbroken
* Verschillende samenvoegstijlen
* Verschillende eindstijlen voor uiteinden
* Overdrukken van lijn
* Afzonderlijke kleurverwerking voor lijn, inclusief ondersteuning voor steunkleuren

In deze tabel worden de kenmerken beschreven die omlijnde tekst ondersteunen.

| Kenmerk | Beschrijving |
|--- |--- |
| s7:fill `<Boolean>`(alleen S7FXG) | Geeft aan of vulling is ingeschakeld voor tekst. De standaardwaarde is true. |
| s7:lijn `<Boolean>` (alleen S7FXG) | Geeft aan of lijn is ingeschakeld voor tekst. De standaardwaarde is false. |
| s7:dikte `<number>` (alleen S7FXG) | Hiermee bepaalt u de dikte van de lijn voor tekst in punten. De standaardwaarde is 1 punt. |
| s7:verbindingen `<string>` (verstek, rond, schuine kant) (alleen S7FXG) | Hiermee geeft u het type samenvoeging van de lijn op. De standaardwaarde is rond. |
| s7:uiteinden `<string>` (geen, rond, vierkant) (alleen S7FXG) | Hiermee geeft u het type uiteinde van de lijn op. De standaardwaarde is rond. |
| s7:miterLimit `<number>` (alleen S7FXG) | Hiermee bepaalt u de limiet van het verstek wanneer de verbinding verstek vormt voor de lijn. De standaardwaarde is 4. |
| s7:strokeOverprint `<Boolean>` (alleen S7FXG) | Hiermee geeft u aan of overdrukken is ingeschakeld voor de lijn. De standaardwaarde is false. |
| s7:strokeColorName (alleen S7FXG) | Hetzelfde als s7:colorName, behalve dat deze de naam van de kleur voor de streek definieert. |
| s7:strokeColorValue (alleen S7FXG) | Hetzelfde als s7:colorValue, maar definieert de waarde van de kleur die voor de streek wordt gebruikt. |
| s7:strokeColorSpace (alleen S7FXG) | Hetzelfde als s7:kleurruimte, behalve dat deze de kleurruimte van de streek definieert. |
| flm:dashPattern `<array>` (alleen S7FXG) | Standaard zijn er geen patronen voor de streepjes en tussenruimten. Dit kenmerk definieert het dash-/tussenruimtepatroon van de streek. De eerste waarde is het streepje van de lijn. Het tweede is de tussenruimte tussen de strepen. U kunt de array voor meerdere waarden op dezelfde manier uitbreiden, waarbij alternatieve waarden worden opgegeven als streepje en tussenruimte. |

## Verdraaide tekst gebruiken {#using-warped-text}

Met verdraaide tekst kunt u de vormgeving van tekst wijzigen met effecten zoals golf, vlag, uitrekken, enzovoort.

Verdraaide tekst wordt ondersteund voor RichText-objecten. Tekst kan verticaal of horizontaal zijn en kan punttekst, vlaktekst en padtekst zijn. Het volledige tekstobject moet zijn geselecteerd voordat verdraaide tekst kan worden toegepast.

Verdraaide tekst kan worden gemaakt in Adobe Illustrator.

Bij het verdraaien van tekst kunt u de volgende kenmerken instellen:

* Stijl
* Richting
* Buigen
* Horizontale vervorming
* Verticale vervorming

Elk kenmerk bevat een set waarden.

| Kenmerk | Waarden | Standaard |
|--- |--- |--- |
| Stijlen7:verdraaiingsstijl | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | none |
| Directions7:warpDirection | horizontaal verticaal | horizontaal |
| Bends7:warpBend | -1 t/m 1 | 0.5 |
| Horizontale vervorming7:warpHorizontalDistortion | -1 t/m 1 | 0 |
| Verticale vervormingen7:verdraaienVerticalDistortion | -1 t/m 1 | 0 |

>[!NOTE]
>
>Voor `inflate` en `fishEye`, heeft het veranderen van de `s7:warpDirection` vlag tussen horizontaal en verticaal geen effect op de output.

Raadpleeg de documentatie bij Adobe Illustrator voor meer informatie over het maken en gebruiken van verdraaide tekst.

>[!MORELIKETHIS]
>
>* [De eerste sjabloon maken in Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Bestanden uploaden voor Sjabloonpublicatie](upload-files-template-publishing.md#upload_files_for_template-publishing)

