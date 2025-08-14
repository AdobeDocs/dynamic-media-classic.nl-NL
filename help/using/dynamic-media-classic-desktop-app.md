---
title: Adobe Dynamic Media Classic desktop
description: Meer weten over de Adobe Dynamic Media Classic-bureaubladtoepassing die nu beschikbaar is?
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1903'
ht-degree: 0%

---

# Nu beschikbaar: Adobe Dynamic Media Classic-bureaubladtoepassing {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic-gebruikers hebben nu toegang tot een nieuwe bureaubladtoepassing die niet langer afhankelijk is van Adobe Flash-technologie in de browser.

Deze nieuwe app is nu beschikbaar voor Windows® en macOS.

>[!IMPORTANT]
>
>Adobe raadt u aan de nieuwe Adobe Dynamic Media Classic-bureaubladtoepassing uiterlijk op 1 oktober 2020 te installeren. Zo hebt u een vloeiende overgang voordat Adobe Flash Player op 31 december 2020 wordt vervangen. Na die datum kunt u zich niet meer aanmelden bij de browserversie van de Adobe Dynamic Media Classic-gebruikersinterface met het label Adobe Dynamic Media Classic in het product.

Zie FAQ voor het [ Nieuwe teken van Adobe Dynamic Media Classic nu beschikbaar.](/help/using/new-ui-2020.md)

## Systeemvereisten voor Adobe Dynamic Media Classic-bureaubladtoepassing {#system-requirements-dmc-app}

De Adobe Dynamic Media Classic-bureaubladtoepassing is compatibel met de volgende besturingssystemen:

* macOS 10.10 of hoger.
* Windows® 7 of hoger.

Zie de volledige systeemvereisten bij [ vereisten van het Systeem voor de Desktop app van Adobe Dynamic Media Classic ](/help/using/system-requirements.md).

Het bericht van de verbetering binnen de Desktoptoepassing van Adobe Dynamic Media Classic wordt niet geproduceerd voor *minder belangrijke* versies. Klanten die van moeilijke situaties in een minder belangrijke versie profiteren kunnen bevorderen.

## Alleen opgelost in de nieuwste release (20.22.2) macOS {#release-feb2022}

* macOS Monterey: pagina voor het uploaden van bestanden bevroren bij volgende uploads. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Oplossingen in de nieuwste versie (20.22.1) {#release-jan2022}

* Bij het bewerken van een afbeelding waren de knoppen van **[!UICONTROL Save]** niet functioneel.
* In de editors instellen worden de knoppen **[!UICONTROL Close]** , **[!UICONTROL Save]** en **[!UICONTROL Save As]** uitgeschakeld nadat u elementen in het deelvenster **[!UICONTROL Add Assets]** hebt geschoven.
* De knop **[!UICONTROL Play]** in de weergave Videodetails werkte niet.
* Kan `d` en `e` in **[!UICONTROL Username]** - en **[!UICONTROL Password]** -velden niet invoeren wanneer macOS Monterey wordt uitgevoerd.
* De resterende analyse-API&#39;s zijn verplaatst naar versie 2.0.

## Oplossingen in release 20.21.3 {#release-sept2021}

* Verbroken miniaturen voor elementen die zijn weergegeven na een periode van inactiviteit in de bureaubladtoepassing.
* De bureaubladtoepassing reageert niet meer, meestal na bewerkingen instellen.
* Schakel de optie Obfuscation en Locking Mode automatisch in onder **[!UICONTROL Test Image Serving]** .

  Zie [ de Veilige het Testen dienst ](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Bijgewerkt verificatiemechanisme met Adobe Analytics. Relevant voor nieuwe integraties of als sommige analytische variabelen moeten worden bijgewerkt vanuit de Dynamic Media Classic-bureaubladtoepassing.

  Zie [ Logon aan Adobe Analytics ](/help/using/log-analytics.md) voor bijgewerkte stappen.

## Oplossingen in release 20.21.2 {#minor-release}

* Bekende beperking in 20.21.1: de vervolgkeuzelijst **[!UICONTROL Server]** op het aanmeldingsscherm was leeg.
* In **[!UICONTROL Upload Job Options]** is de standaardwaarde voor de laagnaam onder **[!UICONTROL Photoshop Options]** nu **[!UICONTROL Photoshop and Layer Name]** . Lagen in het PSD-bestand worden geüpload als aparte afbeeldingen.
   * De eerdere standaardinstelling van **[!UICONTROL Layer name]** . De afbeeldingen krijgen een naam achter hun laagnaam of laagnummer in het PSD-bestand. Het laagnummer is gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen waren.
   * De nieuwe standaardinstelling **[!UICONTROL Photoshop and Layer Name]** geeft de afbeeldingen een naam na het PSD-bestand, gevolgd door de laagnaam of het laagnummer. Het laagnummer wordt gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen zijn.
   * Aangezien laagafbeeldingen in Adobe Dynamic Media Classic nu unieke namen hebben, worden bestaande PSD of sjablonen niet bijgewerkt (welke gedeelde laagnamen in de originele PSD-bestanden worden weergegeven).
* Verbroken miniaturen van elementen.

## Oplossingen in release 20.21.1 {#latest-fixes-desktop-app}

* Sign in kwesties toe te schrijven aan onderbreking resulterend in het volgende bericht: *Deze gebruiker kan aan de groep of de groepen zonder toestemming worden toegewezen. Neem contact op met de beheerder.*
* Viewer-voorinstellingen worden gedupliceerd bij elke onjuiste wachtwoordpoging.
* Bureaubladtoepassing reageert niet meer vanwege de vele middelen in de hoofdmap. (Vast op Windows®; naar wens werken op macOS.)

## Oplossingen in release 20.20.2 {#previous-version-fixes-desktop-app}

* Geen beperking op het aantal bestanden dat u kunt uploaden via de gebruikersinterface van de bureaubladtoepassing voor zowel macOS als Windows®.
* U hoeft zich niet af te melden bij de bureaubladtoepassing om te schakelen tussen bedrijven.
* Ctrl+V voor plakbewerking werkt nu op Windows®.
* Wanneer in de toekomst een nieuwe versie van de bureaubladtoepassing wordt uitgebracht, zullen gebruikers op de hoogte worden gesteld in de bureaubladtoepassing zelf.

## Download en installeer de nieuwste Adobe Dynamic Media Classic desktop app op macOS of Windows® {#installation-dmc-app}

Zie ook:

* [Download en installeer zonder toezicht de nieuwste Adobe Dynamic Media Classic desktop app op Mac](#install-silent-mac-dmc-app)
* [Download en installeer zonder toezicht de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing in Windows](#install-silent-windows-dmc-app)

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing.

   * De meest recente versie is beschikbaar op het volgende adres:

      * [ macOS (.DMG): Download ](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [ Vensters (.EXE): Download ](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * De vorige versie is beschikbaar op het volgende:

      * [ macOS (.DMG): Download ](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [ Windows® (.EXE): Download ](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Voer een van de volgende handelingen uit op basis van het installatieprogramma dat u hebt gedownload.

   * **macOS** - in de **[!UICONTROL Drag & drop to install]** dialoogdoos, sleep **[!UICONTROL Adobe Dynamic Media Classic]** en laat vallen het op **[!UICONTROL Applications]**.

     ![ belemmering en daling installeert op macOS ](/help/using/assets/dragondrop-install1.png)

   * Tik in de map **[!UICONTROL Applications]** op het Adobe Dynamic Media Classic-pictogram.
   * Tik in het dialoogvenster op **[!UICONTROL Open]** om de Adobe Dynamic Media Classic-bureaubladtoepassing te openen.

     ![ Open gedownloade app ](/help/using/assets/open-dmclassicapp1.png)

   * **Vensters** - stel het installatieprogramma binair in werking en volg de instructies op scherm om Desktop app te installeren.

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![ Adobe Dynamic Media Classic teken binnen ](/help/using/assets/dmclassic-login1.png)

1. Als u zich wilt aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing, gebruikt u dezelfde gegevens als waarmee u zich in de browser hebt aangemeld bij Adobe Dynamic Media Classic.

   Zie de volgende afbeelding voor de productieomgeving voor informatie over het gebruik van **[!UICONTROL Server]** :

   | Server | URL browser |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

1. Na aanmelden ziet u de vertrouwde ervaring van de gebruikersinterface van de browser. U kunt uw dagelijkse Adobe Dynamic Media Classic-activiteiten op de desktopapp op de gebruikelijke wijze voortzetten.

## Download en *stil* installeer de recentste Desktop app van Adobe Dynamic Media Classic op macOS {#install-silent-mac-dmc-app}

Zie ook:

* [Download en installeer de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing op Mac of Windows](#installation-dmc-app)
* [Download en installeer zonder toezicht de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing in Windows](#install-silent-windows-dmc-app)

Om *stil* te downloaden en te installeren de recentste versie van Adobe Dynamic Media Classic Desktop app op macOS:

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing voor macOS.

   * [ macOS (.DMG): Download ](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Koppel het gedownloade beeld van de Schijf (.DMG) aan een montageselocatie gebruikend het volgende bevel:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Kopieer het APP-bestand naar **[!UICONTROL Applications]** met de volgende opdracht:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![ Adobe Dynamic Media Classic teken binnen ](/help/using/assets/dmclassic-login1.png)

1. Als u zich wilt aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing, gebruikt u dezelfde gegevens als waarmee u zich in de browser hebt aangemeld bij Adobe Dynamic Media Classic.

   Zie de volgende afbeelding voor de productieomgeving voor informatie over het gebruik van **[!UICONTROL Server]** :

   | Server | URL browser |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

## Download en *stil* installeer recentste Adobe Dynamic Media Classic Desktopapp op Windows® {#install-silent-windows-dmc-app}

Het bevel dat u gebruikt is voor een basisMSI stille installatie. Het installatieprogramma van de Adobe Dynamic Media Classic-bureaubladtoepassing is echter een installatieprogramma van InstallScript MSI dat is gemaakt met InstallShield. Wanneer u het installatieprogramma uitvoert in de recordmodus, wordt gebruikersinteractie opgenomen in een reactiebestand. Dit reactiedossier wordt dan gebruikt voor een stille installatie zoals die in [ wordt beschreven Lopende installaties op stille wijze ](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Zie ook:

* [Download en installeer de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing op Mac of Windows](#installation-dmc-app)

* [Download en installeer zonder toezicht de nieuwste Adobe Dynamic Media Classic desktop app op macOS](#install-silent-mac-dmc-app)

Om *stil* te downloaden en te installeren de recentste versie van Adobe Dynamic Media Classic Desktop app op Windows®:

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing.

   * [ Windows® (.EXE): Download ](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Voer het installatieprogramma in recordmodus uit met de volgende opdracht:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Voer in het venster van het GUI-installatieprogramma de stappen uit om te installeren, zodat interacties/invoer, zoals de installatielocatie, worden opgenomen in het `Setup.iss` -bestand.

1. Kopieer het gemaakte `Setup.iss` -bestand en `adobe-dynamic-media-classic-20.22.1.exe` naar een andere computer.

1. Voer de volgende opdracht voor een installatie op de achtergrond uit:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   De details over bevel-lijn parameters zijn beschikbaar bij [ Setup.exe en Update.exe bevel-lijn parameters ](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![ Adobe Dynamic Media Classic teken binnen ](/help/using/assets/dmclassic-login1.png)

1. Als u zich wilt aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing, gebruikt u dezelfde gegevens als waarmee u zich in de browser hebt aangemeld bij Adobe Dynamic Media Classic.

   Zie de volgende afbeelding voor de productieomgeving voor informatie over het gebruik van **[!UICONTROL Server]** :

   | Server | URL browser |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

## Video doorlopen bij gebruik van Adobe Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Bekijk a [ videolooppas-door op het gebruiken van de App van de Desktop van Adobe Dynamic Media Classic ](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (Lengte: 2 minuten 36 seconden).

## De afbeeldingscache en de assetcache op uw computer wissen met de bureaubladtoepassing {#clear-cache}

1. Tik in de Adobe Dynamic Media Classic-bureaubladtoepassing rechtsboven op **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** .
1. Voer onder de kop **[!UICONTROL Personal Setup]** op de pagina **[!UICONTROL Desktop]** een van de volgende handelingen uit:
   * Tik op **[!UICONTROL Clear Image Cache]** en tik vervolgens op **[!UICONTROL OK]** om alle afbeeldingsbestanden uit de Adobe Dynamic Media-cache van uw computer te verwijderen.
   * Tik op **[!UICONTROL Clear Asset Cache]** en tik vervolgens op **[!UICONTROL OK]** om alle in de cache opgeslagen Adobe Dynamic Media-bestanden van uw computer te verwijderen.
1. Tik in de rechterbenedenhoek van de pagina op **[!UICONTROL Close]** .

### De afbeeldingscache en de elementcache handmatig wissen

U kunt de cache van afbeeldingen en elementen niet alleen wissen met de bureaubladtoepassing, maar u kunt de cache ook handmatig rechtstreeks wissen vanuit het bestandssysteem.

1. Navigeer op basis van uw besturingssysteem naar het volgende:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Bekende beperkingen in Adobe Dynamic Media Classic 20.21.1

* De vervolgkeuzelijst **[!UICONTROL Server]** is leeg na het bijwerken naar Adobe Dynamic Media Classic-bureaubladtoepassing 20.21.1: Scenario: u installeert en meldt u aan bij Adobe Dynamic Media Classic 20.20.1 of 20.20.2 en sluit vervolgens de toepassing. Vervolgens gaat u naar Adobe Dynamic Media Classic 20.21.1. Wanneer u zich aanmeldt, is de vervolgkeuzelijst **[!UICONTROL Server]** in het dialoogvenster **[!UICONTROL Sign-in to your account]** leeg. Om rond deze kwestie te werken, moet u [ manueel het geheime voorgeheugen ](#clear-cache) ontruimen (zie stappen hierboven).

## Bekende beperkingen in Adobe Dynamic Media Classic 20.20.1 (vastgesteld in 20.20.2)

**_is op slechts Windows® van toepassing - is er een beperking op het aantal dossiers die door Desktop app UI kunnen worden geupload?_**<br>ja, kan een maximum van 150 dossiers tegelijkertijd worden geupload gebruikend Desktop app UI.

**_is op Windows® en macOS van toepassing - hoe ik tussen bedrijven schakelaar?_**<br>om tussen bedrijven te schakelen, doe het volgende:

* Selecteer in de Adobe Dynamic Media Classic-app het nieuwe bedrijf in de vervolgkeuzelijst met bedrijven.
* Tik op **[!UICONTROL OK]** wanneer het pop-upvenster verschijnt om u af te melden en de app te sluiten.

  ![ om het nieuwe bedrijf te gebruiken, begin app ](/help/using/assets/dmclassic-new-company1.png) opnieuw

* Start Adobe Dynamic Media Classic opnieuw en meld u vervolgens op de gebruikelijke wijze aan om met het nieuwe bedrijf te werken.

## Tips en trucs

**_ik kan niet het paneel van de Kar van Media op de het landen pagina van Adobe Dynamic Media Classic zien._**<br>Tik in Adobe Dynamic Media Classic op **[!UICONTROL Setup > Personal Setup]**. Controleer of in de sectie Browser **[!UICONTROL Show MediaPortal Features]**is geselecteerd (ingeschakeld). Tik op **[!UICONTROL Save > Close]**.

**_publiceer staat (groene indicator) van een activa wordt niet correct weerspiegeld._**<br>in het browser gebruikersinterface, werd opnieuw login aan UI vereist om correcte te zien publiceren staat van activa. Adobe heeft in de bureaubladtoepassing het pictogram **[!UICONTROL Refresh]**toegevoegd op de werkbalk, rechts van de knop **[!UICONTROL Select None]**. Tik op het pictogram **[!UICONTROL Refresh]**om de laatste status van alle elementen op de opgegeven pagina weer te geven. Geen heraanmelding vereist zoals met de gebruikersinterface van de browser.

![ verfrist pictogram ](/help/using/assets/refresh-icon1.png)
*verfrissen pictogram*

**_ik zie partijreeks vooraf instelt werkend in Desktop app niet._**<br>Tikken **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Controleer of de betreffende **[!UICONTROL Batch Set Preset]**is ingeschakeld. Klik op **[!UICONTROL Save and Submit upload]**.
