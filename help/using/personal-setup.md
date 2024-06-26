---
title: Persoonlijke instelling
description: Alle gebruikers kunnen montages op het Persoonlijke scherm van de Opstelling van Adobe Dynamic Media Classic veranderen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Persoonlijke instelling {#personal-setup}

Alle gebruikers kunnen montages op het Persoonlijke scherm van de Opstelling veranderen. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.

>[!NOTE]
>
>Het persoonlijke scherm van de Opstelling maakt een lijst van welke gebruikersrol u in Adobe Dynamic Media Classic hebt: De Beheerder van het Bedrijf, Beheerder, of Gebruiker.

De Persoonlijke montages van de Opstelling controleren het standaardgedrag van het Browse paneel, hoe u e-mail, en wachtwoordmontages ontvangt. Vergeet niet te selecteren **[!UICONTROL Save]** nadat u deze instellingen hebt gewijzigd.

## Mijn accountgegevens

Hiermee worden uw accountnaam, naam, gebruikersnaam (e-mailadres) en toegewezen gebruikersrol geïdentificeerd.

## Desktop

* **Afbeeldingscache wissen**: Hiermee verwijdert u alle Adobe Dynamic Media-afbeeldingsbestanden in de cache van de computer.
* **Asset Cache wissen**: Hiermee verwijdert u alle Adobe Dynamic Media-bestanden met middelen uit de cache van uw computer.

U kunt de cache van afbeeldingen en elementen niet alleen wissen met de bureaubladtoepassing, maar u kunt de cache ook handmatig rechtstreeks wissen vanuit het bestandssysteem. Navigeer op basis van uw besturingssysteem naar het volgende:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Extensie Creative Suite

**Adobe Dynamic Media Creative Suite Extension installeren:**

1. Ga in Adobe Dynamic Media Classic op de werkbalk naar **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** Selecteer onder Extensie Creative Suites de optie **[!UICONTROL Download Now]** om de `s7csxs.zxp` bestand.
1. Selecteer de **[!UICONTROL Installation]** en **[!UICONTROL System Requirements]** koppelingen voor aanvullende informatie over de extensie.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **[!UICONTROL Thumbnail Size]**: hiermee bepaalt u de standaardgrootte van miniatuurafbeeldingen in de rasterweergave in het deelvenster Bladeren.
* **[!UICONTROL Default Asset Library View]**: Hiermee bepaalt u of de elementen in de elementenbibliotheek voor samenstellen als miniaturen of op naam worden weergegeven. Als u met grote hoeveelheden elementen werkt in de Asset Library, kunt u de elementen op naam bekijken. Als u bijvoorbeeld een grote eCatalog maakt met veel PDF-bestanden, kunt u de elementen op naam weergeven om de lijst korter te maken.
* **[!UICONTROL Default Browse Sort Order]**: Hiermee bepaalt u de volgorde waarin elementen standaard worden weergegeven in het deelvenster Bladeren. Kies een sorteercriterium in het menu en bepaal of u oplopende of aflopende sortering wilt.
* **[!UICONTROL Default Browse Location]**: Hiermee kunt u de bladerlocatie instellen op de standaardlocatie, de laatste bladermap of een specifieke locatie waarnaar u navigeert en die u herkent. U kunt ook de locatie van de browsers instellen om de bestanden en mappen in oplopende of aflopende volgorde te sorteren.
* **[!UICONTROL Default Browse View]**: Hiermee wordt bepaald of de rasterweergave of lijstweergave de standaardweergave is die u ziet wanneer u het deelvenster Bladeren voor het eerst opent.
* **[!UICONTROL Splash Screen Display]**: Hiermee wordt bepaald of er welkomstschermen worden weergegeven, inclusief het welkomstwelkomstscherm.
* **[!UICONTROL Show ToolTips]**: Hiermee bepaalt u of knopinfo wordt weergegeven wanneer u de aanwijzer over knoppen, menu&#39;s en navigatiekoppelingen beweegt. Knopinfo beschrijft de interface-items op het scherm.
* **[!UICONTROL Checkerboard Background]**: geeft een laag met een schaakbordpatroon achter afbeeldingen weer, zodat u gemakkelijk de transparante gebieden van een afbeelding met een alfakanaal kunt zien.
* **[!UICONTROL Show File Size]**: Hiermee geeft u de bestandsgrootte van een element weer wanneer u bladert.
* **[!UICONTROL Include UDFs in Search]**: Schakel deze optie uit als u de systeemprestaties voor de meeste metagegevenszoekopdrachten die u uitvoert, wilt verbeteren.

  Als de meeste zoekopdrachten in metagegevens van nut zijn wanneer u door de gebruiker gedefinieerde velden opneemt, kunt u deze optie selecteren en inschakelen. Als alternatief kunt u Geavanceerd zoeken gebruiken om u een gerichtere en snellere zoekervaring te bieden dan door door de gebruiker gedefinieerde velden op te nemen.

  Zie [Een geavanceerde zoekopdracht uitvoeren](searching-assets.md#conducting_an_advanced_search).

  Zie ook [Door gebruiker gedefinieerde velden](application-setup.md#user_defined_fields).

* **[!UICONTROL Basic Search Type]**: U kunt uit twee opties kiezen: **[!UICONTROL Contains]** zoekt de volledige tekenreeks naar de opgegeven waarde; **[!UICONTROL StartsWith]** zoekt vanaf het begin van de tekenreeks en retourneert sneller resultaten dan **[!UICONTROL Contains]**. Beide opties overschrijven de standaard die is ingesteld in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]** door de beheerder.
* **[!UICONTROL Show Command Feedback]**: Selecteer deze optie om de weergave van opdrachtaanvragen naar de server in te schakelen. Schakel deze optie uit.
* **[!UICONTROL Show Dialog During Export]**: Selecteer deze optie om tijdens het exporteren een pop-updialoogvenster weer te geven. Als u deze optie uitschakelt (uitschakelt), kunt u nog steeds naar de pagina Taken gaan om de resultaten van de export op te halen.

## E-mail

* **[!UICONTROL Email Options]**: Kies hoe Adobe Dynamic Media Classic u per e-mail op de hoogte moet brengen wanneer het uploaden en publiceren taken zijn voltooid. U kunt berichten voor het voltooien van een taak alleen ontvangen als er waarschuwingen of fouten zijn opgetreden.
* **[!UICONTROL Email Scope]**: Hiermee bepaalt u of u alle e-mailberichten voor uw bedrijf ontvangt of alleen e-mailberichten over uploaden en publiceren die u hebt gestart.
* **[!UICONTROL Email Types]**: Hiermee wordt bepaald of u op de hoogte wordt gesteld wanneer het uploaden van taken en het publiceren van taken zijn voltooid.

## Taal

* **[!UICONTROL Preferred Language]**: Bepaalt de taal die u voor de interface wilt gebruiken.

## Wachtwoord

* **[!UICONTROL Current Password]**: Voer het wachtwoord voor uw huidige wachtwoord in.
* **[!UICONTROL New Password]**: Voer een nieuw, geldig wachtwoord in. Uw wachtwoord moet aan de volgende vereisten voldoen:
   * Het moet 8-25 tekens lang zijn.
   * Bevat ten minste één kleine letter.
   * Bevat ten minste één hoofdletter.
   * Bevat ten minste één getal.
   * Bevat ten minste een van de volgende speciale tekens: `# $ &: _ : { }`
* **[!UICONTROL Re-Type Password]**: Voer het nieuwe wachtwoord opnieuw in om te bevestigen dat u het correct hebt ingevoerd.
* **[!UICONTROL Password Expiration]**: Hiermee wordt bepaald of uw wachtwoord na 72 dagen verloopt als beveiligingsmaatregel. Als u Ja hebt geselecteerd, wordt u gevraagd om na 72 dagen een wachtwoord te maken.
