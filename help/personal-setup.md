---
title: Persoonlijke instelling
description: Alle gebruikers kunnen montages op het Persoonlijke scherm van de Opstelling van Adobe Dynamic Media Klassiek veranderen.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Persoonlijke instelling {#personal-setup}

Alle gebruikers kunnen montages op het Persoonlijke scherm van de Opstelling veranderen. Om het Persoonlijke scherm van de Opstelling te openen, klik Opstelling > Persoonlijke Opstelling.

>[!NOTE]
>
>Het Persoonlijke scherm van de Opstelling maakt een lijst van welke gebruikersrol u in de Klassiek van Adobe Dynamic Media hebt: Bedrijfsbeheerder, beheerder of gebruiker.

De Persoonlijke montages van de Opstelling controleren het standaardgedrag van het Browse Comité, hoe u e-mail, en wachtwoordmontages ontvangt. Vergeet niet op Opslaan te klikken nadat u deze instellingen hebt gewijzigd.

## Mijn accountgegevens

Hiermee worden uw accountnaam, naam, gebruikersnaam (e-mailadres) en toegewezen gebruikersrol geïdentificeerd.

## Desktop

* **Cache**  van afbeelding wissen - Hiermee worden alle in de Adobe Dynamic Media-cache opgeslagen afbeeldingsbestanden van de computer verwijderd.
* **Asset Cache**  wissen - Hiermee worden alle elementbestanden uit de Adobe Dynamic Media-cache van de computer verwijderd.

U kunt de cache van afbeeldingen en elementen niet alleen wissen met de bureaubladtoepassing, maar u kunt de cache ook handmatig rechtstreeks wissen vanuit het bestandssysteem. Navigeer op basis van uw besturingssysteem naar het volgende:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Extensie Creative Suite

**Adobe Dynamic Media Creative Suite Extension installeren:**

1. Klik in Adobe Dynamic Media Classic op de werkbalk op **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** onder Extensie Creative Suites op **[!UICONTROL Download Now]** om het `s7csxs.zxp`-bestand te downloaden.
1. Klik op de koppelingen **[!UICONTROL Installation]** en **[!UICONTROL System Requirements]** voor meer informatie over de extensie.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **Miniatuurgrootte**  - Hiermee bepaalt u de standaardgrootte van miniatuurafbeeldingen in de rasterweergave in het deelvenster Bladeren.
* **Standaardweergave**  van elementenbibliotheek - Hiermee bepaalt u of de elementen in de elementenbibliotheek voor buildsets als miniaturen of op naam worden weergegeven. Als u met grote hoeveelheden elementen werkt in de Asset Library, kunt u de elementen op naam bekijken. Als u bijvoorbeeld een grote eCatalog maakt met veel PDF-bestanden, kunt u de elementen op naam weergeven om de lijst korter te maken.
* **Standaard Bladeren in sorteervolgorde**  - Hiermee bepaalt u de volgorde waarin elementen standaard in het deelvenster Bladeren worden weergegeven. Kies een sorteercriterium in het menu en bepaal of u oplopende of aflopende sortering wilt.
* **Standaard door:bladeren Plaats**  - laat u de doorbladerplaats aan het gebrek, de laatste doorbladerde omslag, of aan een specifieke plaats plaatsen die u aan navigeert en identificeert. U kunt ook de locatie van de browsers instellen om de bestanden en mappen in oplopende of aflopende volgorde te sorteren.
* **Standaardweergave**  Bladeren - Hiermee bepaalt u of Rasterweergave of Lijstweergave de standaardweergave is die u ziet wanneer u het deelvenster Bladeren eerst opent.
* **Welkomstscherm**  - Hiermee wordt bepaald of er welkomstschermen, inclusief het welkomstwelkomstscherm, worden weergegeven.
* **Knopinfo**  tonen - Hiermee bepaalt u of knopinfo wordt weergegeven wanneer u de aanwijzer over knoppen, menu&#39;s en navigatiekoppelingen beweegt. Knopinfo beschrijft de interface-items op het scherm.
* **Achtergrond**  van klembord - Hiermee geeft u een schaakbordlaag achter afbeeldingen weer, zodat u gemakkelijk de transparante gebieden van een afbeelding met een alfakanaal kunt zien.
* **Bestandsgrootte**  tonen - De bestandsgrootte van een element wordt weergegeven wanneer u bladert.
* **UDF&#39;s opnemen in zoekopdracht**  - Schakel deze optie uit als u de systeemprestaties voor de meeste metagegevenszoekopdrachten wilt verbeteren (standaard).

   Als de meeste zoekopdrachten in metagegevens van nut zijn wanneer u door de gebruiker gedefinieerde velden opneemt, kunt u deze optie selecteren en inschakelen. U kunt ook Geavanceerd zoeken gebruiken om u een gerichtere en snellere zoekervaring te bieden dan het opnemen van door de gebruiker gedefinieerde velden.

   Zie [Een geavanceerde zoekopdracht uitvoeren](searching-assets.md#conducting_an_advanced_search).

   Zie ook [Door gebruiker gedefinieerde velden](application-setup.md#user_defined_fields).

* **Standaardzoektype**  - U kunt uit twee opties kiezen:  **[!UICONTROL Contains]** zoekt de volledige tekenreeks naar de opgegeven waarde;  **[!UICONTROL StartsWith]** zoekt vanaf het begin van de tekenreeks en retourneert sneller dan  **[!UICONTROL Contains]**. Bij beide opties wordt de standaardinstelling genegeerd die door de beheerder in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]** is ingesteld.
* **Feedback**  van opdracht tonen - Selecteer deze optie om de weergave van opdrachtaanvragen op de server in te schakelen. Schakel deze optie uit om de selectie uit te schakelen.
* **Dialoogvenster tonen tijdens exporteren**  - Selecteren om tijdens het exporteren een pop-upvenster weer te geven. Als u deze optie uitschakelt (uitschakelt), kunt u nog steeds naar de pagina Taken gaan om de resultaten van de export op te halen.

## E-mail

* **E-mailopties**  - Kies hoe u Adobe Dynamic Media Classic u per e-mail op de hoogte wilt brengen wanneer het uploaden en publiceren taken zijn voltooid. U kunt berichten voor het voltooien van een taak alleen ontvangen als er waarschuwingen of fouten zijn opgetreden.
* **E-mailbereik**  - Hiermee bepaalt u of u alle taken per e-mail voor uw bedrijf ontvangt of alleen e-mail over uploaden en publiceren van taken die u hebt gestart.
* **E-mailtypen**  - Hiermee bepaalt u of u op de hoogte wordt gesteld wanneer het uploaden van taken en het publiceren van taken zijn voltooid.

## Taal

* **Gewenste Taal**  - bepaalt de taal u voor de interface wilt gebruiken.

## Wachtwoord

* **Huidig wachtwoord**  - Voer het wachtwoord voor uw huidige wachtwoord in.
* **Nieuw wachtwoord**  - Voer een nieuw, geldig wachtwoord in. Uw wachtwoord moet aan de volgende vereisten voldoen:
   * Tussen 8 en 25 tekens lang zijn.
   * Bevat ten minste één kleine letter.
   * Bevat ten minste één hoofdletter.
   * Bevat minstens één getal.
   * Bevat ten minste een van de volgende speciale tekens: `# $ & - _ : { }`
* **Voer het nieuwe wachtwoord**  opnieuw in om te bevestigen dat u het correct invoert.
* **Wachtwoordvervaldatum**  - Hiermee wordt bepaald of uw wachtwoord na 72 dagen verloopt als beveiligingsmaatregel. Als u Ja selecteert, wordt u gevraagd om na 72 dagen een wachtwoord te maken.
