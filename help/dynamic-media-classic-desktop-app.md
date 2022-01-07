---
title: Adobe Dynamic Media Classic desktop app - Now available
description: Meer weten over Adobe Dynamic Media Classic-bureaubladtoepassingen?
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 085ff63afc73d120fdc29a93b56e5d926eb93e34
workflow-type: tm+mt
source-wordcount: '1909'
ht-degree: 0%

---

# Nu beschikbaar: Adobe Dynamic Media Classic-bureaubladtoepassing {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic-gebruikers hebben nu toegang tot een nieuwe desktop app-ervaring die niet langer afhankelijk is van de Adobe Flash-technologie in de browser.

Deze nieuwe app is nu beschikbaar voor Windows® en macOS.

>[!IMPORTANT]
>
>Adobe raadt u aan de nieuwe Adobe Dynamic Media Classic-bureaubladtoepassing uiterlijk op 1 oktober 2020 te installeren. Als u dit doet, hebt u een soepele overgang voordat de Adobe Flash Player op 31 december 2020 wordt afgekeurd. Na die datum kunt u zich niet meer aanmelden bij de browserversie van de Adobe Dynamic Media Classic-gebruikersinterface met het label Adobe Dynamic Media Classic in het product.

See the FAQ for the [New Adobe Dynamic Media Classic sign-in experience now available.](/help/new-ui-2020.md)

## Systeemvereisten voor Adobe Dynamic Media Classic-bureaubladtoepassing {#system-requirements-dmc-app}

De Adobe Dynamic Media Classic-bureaubladtoepassing is compatibel met de volgende besturingssystemen:

* macOS 10.10 of hoger.
* Windows® 7 of hoger.

>[!NOTE]
>
>Upgrademelding in de Adobe Dynamic Media Classic-bureaubladtoepassing wordt niet gegenereerd voor *klein* lozingen. Customers who benefit from fixes in a minor release can upgrade.

## Oplossingen in de nieuwste versie (20.22.1) {#release-jan2022}

Beeldbewerking **[!UICONTROL Save]** de knoppen waren niet functioneel.

* Beeldbewerking **[!UICONTROL Save]** de knoppen waren niet functioneel.
* In de Vastgestelde redacteurs, **[!UICONTROL Close]**, **[!UICONTROL Save]**, en **[!UICONTROL Save As]** knoppen worden uitgeschakeld na het schuiven van elementen in het dialoogvenster **[!UICONTROL Add Assets]** deelvenster.
* **[!UICONTROL Play]** button in Video Detail view did not work.
* Kan niet invoeren `d` en `e` in **[!UICONTROL Username]** en **[!UICONTROL Password]** velden wanneer macOS Monterey wordt uitgevoerd.
* De resterende analyse-API&#39;s zijn verplaatst naar versie 2.0.

## Oplossingen in release 20.21.3 {#release-sept2021}

* Verbroken miniaturen voor elementen die zijn weergegeven na een periode van inactiviteit in de bureaubladtoepassing.
* Desktop-app reageert niet meer, meestal na bewerkingen instellen.
* Modus Verduistering en vergrendeling aanvragen ingeschakeld onder **[!UICONTROL Test Image Serving]**.

   Zie [De service Beveiligde tests testen](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Bijgewerkt verificatiemechanisme met Adobe Analytics. Relevant voor nieuwe integraties of als sommige analytische variabelen moeten worden bijgewerkt vanuit de Dynamic Media Classic-bureaubladtoepassing.

   Zie [Aanmelden bij Adobe Analytics](/help/log-analytics.md) voor bijgewerkte stappen.

## Oplossingen in release 20.21.2 {#minor-release}

* Bekende beperking in 20.21.1: de **[!UICONTROL Server]** de vervolgkeuzelijst op het aanmeldingsscherm was leeg.
* In **[!UICONTROL Upload Job Options]**, Standaardwaarde voor laagnaamgeving onder **[!UICONTROL Photoshop Options]**, is nu **[!UICONTROL Photoshop and Layer Name]**. Lagen in het PSD-bestand worden geüpload als aparte afbeeldingen.
   * De eerdere standaardinstelling van **[!UICONTROL Layer name]**, de afbeeldingen een naam geven na de naam van de laag of het laagnummer in het PSD-bestand. The layer number was used if the layer names in the PSD file were default Photoshop layer names.
   * De nieuwe standaardinstelling van **[!UICONTROL Photoshop and Layer Name]**, geeft u de afbeeldingen een naam na het PSD-bestand, gevolgd door de laagnaam of het laagnummer. Het laagnummer wordt gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen zijn.
   * Aangezien laagafbeeldingen in Adobe Dynamic Media Classic nu unieke namen hebben, worden bestaande PSD of sjablonen niet bijgewerkt (welke gedeelde laagnamen in de originele PSD-bestanden).
* Broken thumbnails of assets.

## Fixes in release 20.21.1 {#latest-fixes-desktop-app}

* Aanmeldingsproblemen vanwege time-out resulterend in het volgende bericht: *Deze gebruiker kan zonder toestemming aan de groep of groepen worden toegewezen. Neem contact op met de beheerder.*
* Viewer presets get duplicated with each incorrect password attempt.
* Bureaubladtoepassing reageert niet meer vanwege de vele middelen in de hoofdmap. (Vast in Windows®) naar wens werken op macOS.)

## Oplossingen in release 20.20.2 {#previous-version-fixes-desktop-app}

* Geen beperking op het aantal bestanden dat u kunt uploaden via de gebruikersinterface van de bureaubladtoepassing voor zowel macOS als Windows®.
* U hoeft zich niet af te melden bij de bureaubladtoepassing om te schakelen tussen bedrijven.
* Ctrl+V for paste operation now works on Windows®.
* Wanneer in de toekomst een nieuwe versie van de bureaubladtoepassing wordt uitgebracht, zullen gebruikers op de hoogte worden gesteld in de bureaubladtoepassing zelf.

## Download en installeer de nieuwste Adobe Dynamic Media Classic desktop app op macOS of Windows® {#installation-dmc-app}

Zie ook:

* [Download en stil de nieuwste Adobe Dynamic Media Classic desktop app op Mac](#install-silent-mac-dmc-app)
* [Download en stil de nieuwste Adobe Dynamic Media Classic desktop app op Windows®](#install-silent-windows-dmc-app)

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download the latest installer for Adobe Dynamic Media Classic desktop app.

   * The latest version (20.22.1) is available at the following:

      * [macOS (.DMG) - Downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * De vorige versie (20.21.3) is beschikbaar op:

      * [macOS (.DMG) - Downloaden](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)
      * [Windows® (.EXE) - Downloaden](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Voer een van de volgende handelingen uit op basis van het installatieprogramma dat u hebt gedownload.

   * **macOS** -In de **[!UICONTROL Drag & drop to install]** dialoogvenster, slepen **[!UICONTROL Adobe Dynamic Media Classic]** en zet hem neer **[!UICONTROL Applications]**.

      ![Drag and drop install on macOS](/help/assets/dragondrop-install1.png)

   * In de **[!UICONTROL Applications]** tikt u op het Adobe Dynamic Media Classic-pictogram.
   * Tik in het dialoogvenster op **[!UICONTROL Open]** om de Adobe Dynamic Media Classic-bureaubladtoepassing te openen.

      ![Gedownloade app openen](/help/assets/open-dmclassicapp1.png)

   * **Windows** - Voer het binaire bestand van het installatieprogramma uit en volg de aanwijzingen op het scherm om de bureaubladtoepassing te installeren.

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![Aanmelden bij Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. To sign in to the Adobe Dynamic Media Classic desktop app, use the same credentials that you used to log on to Adobe Dynamic Media Classic in the browser.

   Voor de **[!UICONTROL Server]** voor gebruik, zie de volgende afbeelding voor het productiemilieu:

   | Server | URL browser |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

1. Following sign in, notice the familiar browser user interface experience. U kunt uw dagelijkse Adobe Dynamic Media Classic-activiteiten op de desktopapp op de gebruikelijke wijze voortzetten.

## Download and *silent* install the latest Adobe Dynamic Media Classic desktop app on macOS {#install-silent-mac-dmc-app}

Zie ook:

* [Download en installeer de nieuwste Adobe Dynamic Media Classic desktop app op Mac of Windows®](#installation-dmc-app)
* [Download en stil de nieuwste Adobe Dynamic Media Classic desktop app op Windows®](#install-silent-windows-dmc-app)

Om te downloaden en *stil* Installeer de nieuwste versie van de Adobe Dynamic Media Classic-bureaubladtoepassing op macOS:

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing voor macOS.

   * [macOS (.DMG) - Downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)

1. Mount the downloaded Disk Image (.DMG) to a mountpoint location using the following command:

   `hdiutil attach adobe-dynamic-media-classic-20.22.1.dmg -mountpoint <mount_point_path>`

1. Het APP-bestand kopiëren naar **[!UICONTROL Applications]** met de volgende opdracht:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![Adobe Dynamic Media Classic sign in](/help/assets/dmclassic-login1.png)

1. To sign in to the Adobe Dynamic Media Classic desktop app, use the same credentials that you used to log on to Adobe Dynamic Media Classic in the browser.

   For the **[!UICONTROL Server]** to use, see the following mapping for the production environment:

   | Server | URL browser |
   | --- | --- |
   | NA Production (North America) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

## Downloaden en *stil* de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing installeren op Windows® {#install-silent-windows-dmc-app}

The command that you use is for a basic MSI silent installation. However, the Adobe Dynamic Media Classic desktop app installer is an InstallScript MSI installer created using InstallShield. Wanneer u het installatieprogramma uitvoert in de recordmodus, wordt gebruikersinteractie opgenomen in een reactiebestand. Dit reactiebestand wordt vervolgens gebruikt voor een installatie op de achtergrond, zoals beschreven in [Installaties uitvoeren in de modus Stil.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

See also:

* [Download en installeer de nieuwste Adobe Dynamic Media Classic desktop app op Mac of Windows®](#installation-dmc-app)
* [Download en stil de nieuwste Adobe Dynamic Media Classic desktop app op macOS](#install-silent-mac-dmc-app)

Om te downloaden en *stil* Installeer de nieuwste versie van de Adobe Dynamic Media Classic-bureaubladtoepassing op Windows®:

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download the latest installer for Adobe Dynamic Media Classic desktop app.

   * [Windows® (.EXE) - Downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Voer het installatieprogramma in recordmodus uit met de volgende opdracht:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. In the GUI installer window, follow the steps to install so that interactions/inputs, like install location, get recorded in `Setup.iss` file.

1. Het gemaakte bestand kopiëren `Setup.iss` en `adobe-dynamic-media-classic-20.22.1.exe` naar andere computer.

1. Voer de volgende opdracht voor een installatie op de achtergrond uit:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Details about command-line parameters are available at [Setup.exe and Update.exe Command-Line Parameters.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![Aanmelden bij Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Als u zich wilt aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing, gebruikt u dezelfde gegevens als waarmee u zich in de browser hebt aangemeld bij Adobe Dynamic Media Classic.

   Voor de **[!UICONTROL Server]** voor gebruik, zie de volgende afbeelding voor het productiemilieu:

   | Server | Browser URL |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

## Video doorlopen bij gebruik van Adobe Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Kijk eens naar [video doorlopen bij gebruik van Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Lengte: 2 minuten 36 seconden).

## De afbeeldingscache en de assetcache op uw computer wissen met de bureaubladtoepassing {#clear-cache}

1. Tik in de Adobe Dynamic Media Classic-bureaubladtoepassing in de rechterbovenhoek op **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Op de **[!UICONTROL Personal Setup]** pagina, onder de **[!UICONTROL Desktop]** Voer een van de volgende handelingen uit:
   * Tik op **[!UICONTROL Clear Image Cache]** tikt u vervolgens op **[!UICONTROL OK]**.
   * Tik op **[!UICONTROL Clear Asset Cache]** tikt u vervolgens op **[!UICONTROL OK]**.
1. Tik in de rechterbenedenhoek van de pagina op **[!UICONTROL Close]**.

### De afbeeldingscache en de elementcache handmatig wissen

U kunt de cache van afbeeldingen en elementen niet alleen wissen met de bureaubladtoepassing, maar u kunt de cache ook handmatig rechtstreeks wissen vanuit het bestandssysteem.

1. Navigeer op basis van uw besturingssysteem naar het volgende:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Bekende beperking in Adobe Dynamic Media Classic 20.21.1

* De **[!UICONTROL Server]** De vervolgkeuzelijst is leeg na het bijwerken naar Adobe Dynamic Media Classic-bureaubladtoepassing 20.21.1 - Scenario: U installeert en zich binnen aan Adobe Dynamic Media Classic 20.20.1 of 20.20.2, dan sluit de toepassing. Vervolgens gaat u naar Adobe Dynamic Media Classic 20.21.1. Wanneer u zich probeert aan te melden, **[!UICONTROL Server]** vervolgkeuzelijst in het dialoogvenster **[!UICONTROL Sign in to your account]** is leeg. Als u dit probleem wilt oplossen, moet u [de cache handmatig wissen](#clear-cache) (zie bovenstaande stappen).

## Bekende beperkingen in Adobe Dynamic Media Classic 20.20.1 (vastgesteld in 20.20.2)

**_Alleen van toepassing op Windows® - Is er een beperking op het aantal bestanden dat kan worden geüpload via de interface van de bureaubladtoepassing?_**<br>Ja, er kunnen maximaal 150 bestanden tegelijk worden geüpload via de interface van de bureaubladtoepassing.

**_Is van toepassing op Windows® en macOS - hoe schakel ik tussen bedrijven?_**<br>Ga als volgt te werk om tussen bedrijven te schakelen:

* Selecteer in de Adobe Dynamic Media Classic-app het nieuwe bedrijf in de vervolgkeuzelijst met bedrijven.
* Tik op **[!UICONTROL OK]** om u af te melden en de app te sluiten.

   ![Start de app opnieuw om het nieuwe bedrijf te gebruiken](/help/assets/dmclassic-new-company1.png)

* Start Adobe Dynamic Media Classic opnieuw en meld u vervolgens op de gebruikelijke wijze aan om met het nieuwe bedrijf te werken.

## Tips en trucs

**_Ik kan het deelvenster Media Cart niet zien op de landingspagina van Adobe Dynamic Media Classic._**<br>Tik in Adobe Dynamic Media Classic op **[!UICONTROL Setup > Personal Setup]**. Controleer of in de sectie Browser **[!UICONTROL Show MediaPortal Features]**is geselecteerd (ingeschakeld). Tik op **[!UICONTROL Save > Close]**.

**_Publish state (green indicator) of an asset is not reflected correctly._**<br>In the browser user interface, a relogin to the UI was required to see the correct publish state of assets. In the desktop app, Adobe has introduced a **[!UICONTROL Refresh]**icon in the toolbar, to the right of the **[!UICONTROL Select None]**button. Tap the **[!UICONTROL Refresh]**icon to see the latest status of all the assets on the given page. Geen nieuwe aanmelding vereist zoals met de gebruikersinterface van de browser.

![Pictogram Vernieuwen](/help/assets/refresh-icon1.png)
*Pictogram Vernieuwen*

**_Ik zie geen batch-voorinstellingen werken in de bureaubladtoepassing._**<br>Tik op **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Ensure the relevant **[!UICONTROL Batch Set Preset]**is enabled. Klik op **[!UICONTROL Save and Submit upload]**.
