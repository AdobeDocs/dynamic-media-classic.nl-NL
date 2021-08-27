---
title: Taakbestanden controleren
description: Leer hoe u taakbestanden kunt controleren in Adobe Dynamic Media Classic.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1532'
ht-degree: 0%

---

# Taakbestanden controleren{#checking-job-files}

Als u het uploaden van bestanden naar de Adobe Dynamic Media Classic wilt controleren en bestanden wilt publiceren naar Adobe Dynamic Media Classic-servers, biedt Adobe Dynamic Media Classic de pagina Taken. U kunt het uploaden en publiceren banen op de pagina van Banen herzien, de status van banen controleren, en het annuleren van het publiceren banen van deze pagina. U kunt ook uploads en publicatietaken plannen.

Wanneer u elementen uploadt, wordt een draaiend pictogram weergegeven naast het menu Taken. Dit geeft aan dat een taak wordt uitgevoerd en dat het aantal bestanden in uitvoering is. U kunt het pictogram selecteren om meer informatie over de actieve taak weer te geven.

>[!NOTE]
>
>Een lijst met onlangs gepubliceerde taken is ook beschikbaar op de pagina Recente activiteiten. Selecteer **[!UICONTROL Recent]** op de globale bar van de Navigatie.

## De pagina Taken {#about-the-jobs-page}

Selecteer **[!UICONTROL Jobs]** op de Globale bar van de Navigatie zodat opent de pagina van Banen. Standaard worden taken weergegeven die beginnen met de meest recente.

Taken worden in de volgende categorieën op het tabblad Historie van de pagina Taken vermeld:

* **[!UICONTROL Job Type]** - Een pictogram geeft het taaktype aan: Uploaden en publiceren zijn de meest voorkomende taaktypen.

* **[!UICONTROL Job Name]** - De naam van de taak. De naam bevat het door de gebruiker ingevoerde gedeelte van de naam en de datum en tijd.

* **[!UICONTROL Started]** - Wanneer de taak is gestart.

* **[!UICONTROL Total]** - Het aantal overgedragen bestanden.

* **[!UICONTROL W (warnings)]** - Het aantal waarschuwingen in de taak (indien aanwezig). Waarschuwingen geven problemen aan met de taak die geen invloed hadden op de algehele voltooiing van de taak. Deze waarschuwingen kunnen meestal worden genegeerd omdat ze worden gerapporteerd over verborgen bestanden. `.DS_store`-bestanden (Macintosh) en Thumbs.db-bestanden (Windows®) bevatten bijvoorbeeld informatie over het weergeven van afbeeldingsbestanden voor gebruikers. Waarschuwingsgegevens voor deze bestanden kunnen echter worden genegeerd omdat ze geen betrekking hebben op de manier waarop deze bestanden worden gebruikt in Adobe Dynamic Media Classic. U kunt dubbelklikken op een taaknaam voor gedetailleerde informatie over waarschuwingen.

* **[!UICONTROL E (errors)]** - Hier wordt het aantal eventuele fouten in de taak weergegeven. U kunt dubbelklikken op een taaknaam voor gedetailleerde informatie over fouten.

* **[!UICONTROL Duration]** - Hoe lang duurde het om de taak te voltooien.

* **[!UICONTROL Status]** - Geeft de status van de taak weer.

* **[!UICONTROL Destination]** - Voor uploadtaken: de bedrijfsnaam en de map waarnaar de bestanden zijn geüpload. Deze categorie is niet van toepassing op publicatietaken.

* **[!UICONTROL Submitted By]** - Lijsten die de elementen hebben geüpload.

>[!NOTE]
>
>U kunt publicatie- en uploadtaken tijdens de uitvoering annuleren door op de knop **[!UICONTROL Cancel]** naast de voortgangsbalk te klikken.

## Weergaven wijzigen op de pagina Taken {#changing-views-on-the-jobs-page}

Gebruik deze technieken om taken te sorteren of uw weergave van het tabblad Historie van de pagina Taken te wijzigen:

* **[!UICONTROL Sorting]** - Selecteer een kolomnaam om de lijst op een bepaalde kolom te sorteren. U kunt de schakelaar naast de kolomnaam selecteren om in dalende of stijgende orde te sorteren.

* **[!UICONTROL Date Range]** - Selecteer het  **[!UICONTROL Date Range]** menu en kies een optie om de lijst met taken te beperken tot de huidige datum, de vorige week of de vorige maand. Selecteer **[!UICONTROL Custom Date Range]** en voer een specifiek datumbereik in.

* **[!UICONTROL Job Type]** - Selecteer het  **[!UICONTROL Job Type]** menu en kies  **[!UICONTROL Publish]** of verklein de lijst  **[!UICONTROL Upload]** om taken te publiceren of te uploaden. Selecteer **[!UICONTROL All]** om beide typen taken weer te geven.

* **[!UICONTROL Show]** - Ga naar  **[!UICONTROL Show]** >  **[!UICONTROL My Jobs]** of  **[!UICONTROL Show]** >  **[!UICONTROL All Jobs]** om de lijst te beperken tot taken die u hebt besteld of taken die door mensen in uw bedrijf zijn besteld.

## Een rapport met taakdetails weergeven, kopiëren of afdrukken {#viewing-copying-or-printing-a-job-details-report}

Dubbelklik op de naam van een rapport op de pagina Taken zodat de pagina Taakdetails wordt geopend. Deze pagina bevat een samenvattingsrapport over de bestanden in de taak. Selecteer **[!UICONTROL View Detail]** zodat kunt u de Klassieke identiteitskaart van Adobe Dynamic Media van een ingang, bestemmingspad, en statusinformatie zien. Als u een PDF- of PostScript-bestand hebt geüpload waarvoor fonts nodig zijn die niet beschikbaar zijn in Adobe Dynamic Media Classic, worden de ontbrekende fonts weergegeven in het rapport.

U kunt deze gegevens naar het klembord kopiëren.

1. Dubbelklik op de naam van een rapport op de pagina Taken.
1. Selecteer **[!UICONTROL View Detail]** op de pagina Taakdetails om een gedetailleerd rapport over een item op te halen.
1. Selecteer **[!UICONTROL Copy to Clipboard]**.

## Herhalende upload- en publicatietaken verwerken {#handling-recurring-upload-and-publish-jobs}

Het terugkomen upload en publiceer banen die u op Upload en publiceer pagina&#39;s creeert zijn vermeld op het Geplande lusje van de pagina van Banen. U kunt terugkerende taken op het geplande tabblad bewerken en verwijderen.

Selecteer de knoop van Banen op de Globale bar van de Navigatie en, op de pagina van Banen, selecteer **[!UICONTROL Scheduled]** tabel zodat kunt u terugkomende banen uitgeven en schrappen.

>[!NOTE]
>
>U kunt de takenlijst op het **[!UICONTROL Scheduled]** lusje met **[!UICONTROL Job Type]** en **[!UICONTROL Show]** menu&#39;s filtreren. Selecteer een taaktype zodat u de lijst kunt beperken tot het publiceren van taken van een specifiek type. Selecteer een optie **[!UICONTROL Show]** als u de banen wilt tonen u of banen creeerde door iedereen in uw bedrijf.

### Herhaalde taken bewerken, verwijderen, pauzeren en hervatten {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selecteer een terugkomende baan op de pagina van Banen en volg deze instructies als u het wilt uitgeven of schrappen:

* **Een terugkerende taak**  bewerken - Selecteer de  **[!UICONTROL Edit]** knop en voer planningsinformatie in het dialoogvenster Geplande taak bewerken in. Als u wilt dat de taak met een interval van uw keuze opnieuw wordt uitgevoerd, gaat u naar **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**.

Zie [Een aangepaste upload- of publiceertaaktijdinterval maken](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Een terugkerende taak**  verwijderen - Selecteer de  **[!UICONTROL Delete]** knop.

* **Een terugkerende taak**  onderbreken (en hervatten) - Schakel in de kolom Actief het selectievakje uit om een taak te pauzeren. Schakel een selectievakje in om een gepauzeerde taak te hervatten.

### Een aangepast tijdinterval voor uploaden of publiceren maken {#creating-a-custom-upload-or-publish-job-time-interval}

Als u een aangepast tijdinterval wilt maken voor een upload (via FTP) of een publicatietaak, gaat u op de pagina Uploaden of Publiceren naar **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**. Dan ga aantallen en vervangingen in het vakje van de Regel in beschrijvend een tijdinterval voor uploaden of publiceer banen om opnieuw te komen.

De syntaxis voor het beschrijven van aangepaste upload en publicatietijdintervallen in het vak Regel is:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

`0 15 10 * * ?` plant bijvoorbeeld elke dag een taak om 10:15.00 uur.

De volgende lijsten en de lijst verklaren hoe te om een tijdinterval in de doos van de Regel te beschrijven.

In deze tabel worden de tijdtoename, de toegestane waarden en de jokertekens weergegeven die worden ondersteund:

| Tijdtoenamen | Toegestane waarden | Opmerkingen | Ondersteunde jokertekens |
|--- |--- |--- |--- |
| Seconden | 0-59 |  | `, - * /` |
| Minuten | 0-59 |  | `, - * /` |
| Uren | 0-23 | Let op het gebruik van een 24-uurs klok. | `, - * /` |
| Dag van de maand | 1-31 | U kunt geen numerieke waarde opgeven voor zowel &quot;dag van de maand&quot; als &quot;dag van de week&quot;. Een van deze velden moet een jokerteken `?` gebruiken. | `, - * / ? L C` |
| Maand | 1-12 of jan, feb, mrt, apr, mei, jun, jul, aug, sep, sept, okt, nov, dec | Waarden zijn hoofdlettergevoelig. | `, - * /` |
| Dag van de week | Mon, Tue, Wed, Thu, Fri, Zat, Sun | Waarden zijn hoofdlettergevoelig. U kunt geen numerieke waarde opgeven voor zowel &quot;dag van de maand&quot; als &quot;dag van de week&quot;. Een van deze velden moet een jokerteken `?` gebruiken. | `, - * / ? L C #` |
| Jaar (optioneel) | Leeg of 1970-2099 |  | `, - * /` |


In deze tabel worden de jokertekens beschreven die zijn toegestaan in het vak Regel en hoe u deze kunt gebruiken:

| Jokerteken | Naam | Beschrijving |
|--- |--- |--- |
| `*` | Sterretje | Alle waarden (bijvoorbeeld &quot;elke minuut&quot;). |
| `?` | Vraagteken | Geen specifieke waarde (bijvoorbeeld &quot;een minuut binnen het opgegeven uur&quot;). |
| `,` | Komma | Overige waarden (bijvoorbeeld &quot;maandag en woensdag&quot;). |
| `-` | Afbreekstreepje | Waardenbereik (bijvoorbeeld &quot;Maandag tot vrijdag&quot;). |
| `/` | slash | Toename (bijvoorbeeld &quot;om de 15 minuten&quot;). |
| `L` | Kapitaal L | Laatste &quot;dag van de maand&quot; of &quot;dag van de week&quot; (alleen beschikbaar voor deze velden). Als de maand bijvoorbeeld januari is, plant een L-waarde voor het veld &quot;dag van de maand&quot; de taak voor 31 januari. Voor het veld &quot;Dag van de week&quot; kunt u dit teken alleen invoeren om de taak op zaterdag te plannen. U kunt het met een aantal (bijvoorbeeld, `6L`) gebruiken om de laatste Vrijdag van de maand te specificeren. Geef `L` niet op met de jokertekens voor komma&#39;s of afbreekstreepjes. |
| `#` | Nummerteken | &quot;Nde&quot; weekdag van de maand (alleen beschikbaar voor het veld &quot;Dag van de week&quot;). `6#3` in het veld &quot;dag van de week&quot; geeft bijvoorbeeld de derde vrijdag van de maand aan. De `6` geeft &quot;Vrijdag&quot; aan (de zesde dag van de week) en `3` geeft het derde exemplaar in de maand aan. |
| `C` | # Kapitaal C | Eerste kalender &quot;dag van de maand&quot; of &quot;dag van de week&quot; (alleen beschikbaar voor deze velden). Als u bijvoorbeeld een waarde van `1C` opgeeft voor &quot;dag van de maand&quot;, wordt de eerste dag in de kalender gepland die op of na de vijfde dag plaatsvindt. Voor het veld &quot;dag van de week&quot; typt u `1C` de eerste dag in de kalender die op of na zondag plaatsvindt. |

In deze lijst staan voorbeelden van tijdintervallen in het vak Regel:

* `0 0 12 * * ?` : Elke dag geen
* `0 15 10 ? * *` : 22:15
* `0 0/5 14 * * ?`: Elke 5 minuten tussen 2:00 en 14:55
* `0 0/5 14,18 * * ?` : Elke 5 minuten tussen 2:00 en 2:55 elke dag en elke 5 minuten tussen 6:00 en 6:55 elke dag
* `0 10,44 14 ? 3` : Woensdag om 14:10 en 16:44 uur
* `0 15 10 ? *` : Maandag om 10:15 uur elke weekdag
* `0 15 10 20 * ?` : 10:15 uur op de twintigste dag van elke maand
* `0 15 10 L * ?` : 10:15 uur op de laatste dag van elke maand
* `0 15 10 ? * 6L` : Om 10:15 uur op de laatste vrijdag van elke maand
* `0 15 10 * * 6#3` : Om 10:15 uur op de derde vrijdag van elke maand

## Een upload- of publicatietaak gebruiken als trigger {#using-an-upload-or-publish-job-as-a-trigger}

Wanneer u elementen uploadt via FTP of een publicatietaak uitvoert, kunt u een volgende taak plannen die moet beginnen wanneer het uploaden is voltooid. (Als andere taken volgens de planning moeten beginnen, wordt de taak die u hier instelt, in de wachtrij geplaatst.) De nieuwe baan verzendt een bericht naar het adres u specificeert zodat de code bij die plaats kan worden teweeggebracht. Deze opvolguploadtaak krijgt dezelfde naam als de huidige uploadtaak, maar met het voorvoegsel _Pub.

Als u een upload- of publicatietaak wilt laten activeren door een andere taak, selecteert u **[!UICONTROL Advanced]** op de pagina Uploaden of Publiceren. Voer vervolgens de URL in het tekstveld HTTP-kennisgeving in.
