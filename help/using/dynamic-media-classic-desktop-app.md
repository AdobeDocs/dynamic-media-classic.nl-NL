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

Adobe Dynamic Media Classic-gebruikers hebben nu toegang tot een nieuwe bureaubladervaring die niet langer afhankelijk is van de Adobe Flash-technologie in de browser.

Deze nieuwe app is nu beschikbaar voor Windows® en macOS.

>[!IMPORTANT]
>
>Adobe raadt u aan de nieuwe Adobe Dynamic Media Classic-bureaubladtoepassing uiterlijk op 1 oktober 2020 te installeren. Als u dit doet, hebt u een soepele overgang voordat de Flash Player van de Adobe op 31 december 2020 wordt afgekeurd. Na die datum kunt u zich niet meer aanmelden bij de browserversie van de Adobe Dynamic Media Classic-gebruikersinterface met het label Adobe Dynamic Media Classic in het product.

Zie de veelgestelde vragen voor de [Nieuwe Adobe Dynamic Media Classic-aanmelding is nu beschikbaar.](/help/using/new-ui-2020.md)

## Systeemvereisten voor Adobe Dynamic Media Classic-bureaubladtoepassing {#system-requirements-dmc-app}

De Adobe Dynamic Media Classic-bureaubladtoepassing is compatibel met de volgende besturingssystemen:

* macOS 10.10 of hoger.
* Windows® 7 of hoger.

Zie de volledige systeemvereisten op [Systeemvereisten voor Adobe Dynamic Media Classic-bureaubladtoepassing](/help/using/system-requirements.md).

Upgrademelding in de Adobe Dynamic Media Classic-bureaubladtoepassing wordt niet gegenereerd voor *klein* lozingen. Klanten die van moeilijke situaties in een minder belangrijke versie profiteren kunnen bevorderen.

## Alleen opgelost in de nieuwste release (20.22.2) macOS {#release-feb2022}

* macOS Monterey: pagina voor het uploaden van bestanden bevroren bij volgende uploads. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Oplossingen in de nieuwste versie (20.22.1) {#release-jan2022}

* Wanneer u een afbeelding bewerkt, worden de **[!UICONTROL Save]** de knoppen waren niet functioneel.
* In de Vastgestelde redacteurs, **[!UICONTROL Close]**, **[!UICONTROL Save]**, en **[!UICONTROL Save As]** knoppen worden uitgeschakeld na het schuiven van elementen in het dialoogvenster **[!UICONTROL Add Assets]** deelvenster.
* De **[!UICONTROL Play]** in de weergave Videodetails werkte niet.
* Kan niet invoeren `d` en `e` in **[!UICONTROL Username]** en **[!UICONTROL Password]** velden wanneer macOS Monterey wordt uitgevoerd.
* De resterende analyse-API&#39;s zijn verplaatst naar versie 2.0.

## Oplossingen in release 20.21.3 {#release-sept2021}

* Verbroken miniaturen voor elementen die zijn weergegeven na een periode van inactiviteit in de bureaubladtoepassing.
* De bureaubladtoepassing reageert niet meer, meestal na bewerkingen instellen.
* Modus Verduistering en vergrendeling aanvragen ingeschakeld onder **[!UICONTROL Test Image Serving]**.

  Zie [De service Beveiligde tests](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Bijgewerkt verificatiemechanisme met Adobe Analytics. Relevant voor nieuwe integraties of als sommige analytische variabelen moeten worden bijgewerkt vanuit de Dynamic Media Classic-bureaubladtoepassing.

  Zie [Aanmelden bij Adobe Analytics](/help/using/log-analytics.md) voor bijgewerkte stappen.

## Oplossingen in release 20.21.2 {#minor-release}

* Bekende beperking in 20.21.1: de **[!UICONTROL Server]** de vervolgkeuzelijst op het aanmeldingsscherm was leeg.
* In **[!UICONTROL Upload Job Options]**, de standaardwaarde voor de laagnaam onder **[!UICONTROL Photoshop Options]**, is nu **[!UICONTROL Photoshop and Layer Name]**. Lagen in het PSD-bestand worden geüpload als aparte afbeeldingen.
   * De eerdere standaardinstelling van **[!UICONTROL Layer name]**, de afbeeldingen een naam geven na de naam van de laag of het laagnummer in het PSD-bestand. Het laagnummer is gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen waren.
   * De nieuwe standaard van **[!UICONTROL Photoshop and Layer Name]**, geeft u de afbeeldingen een naam na het PSD-bestand, gevolgd door de laagnaam of het laagnummer. Het laagnummer wordt gebruikt als de laagnamen in het PSD-bestand standaard Photoshop-laagnamen zijn.
   * Aangezien laagafbeeldingen in Adobe Dynamic Media Classic nu unieke namen hebben, worden bestaande PSD of sjablonen niet bijgewerkt (welke gedeelde laagnamen in de originele PSD-bestanden).
* Verbroken miniaturen van elementen.

## Oplossingen in release 20.21.1 {#latest-fixes-desktop-app}

* Aanmeldingsproblemen vanwege time-out resulterend in het volgende bericht: *Deze gebruiker kan zonder toestemming aan de groep of groepen worden toegewezen. Neem contact op met de beheerder.*
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

      * [macOS (.DMG): downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE): downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * De vorige versie is beschikbaar op het volgende:

      * [macOS (.DMG): downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE): downloaden](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Voer een van de volgende handelingen uit op basis van het installatieprogramma dat u hebt gedownload.

   * **macOS** -In de **[!UICONTROL Drag & drop to install]** dialoogvenster, slepen **[!UICONTROL Adobe Dynamic Media Classic]** en zet hem neer **[!UICONTROL Applications]**.

     ![Installeren via slepen en neerzetten op macOS](/help/using/assets/dragondrop-install1.png)

   * In de **[!UICONTROL Applications]** tikt u op het Adobe Dynamic Media Classic-pictogram.
   * Tik in het dialoogvenster **[!UICONTROL Open]** om de Adobe Dynamic Media Classic-bureaubladtoepassing te openen.

     ![Gedownloade app openen](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - Voer het binaire bestand van het installatieprogramma uit en volg de aanwijzingen op het scherm om de bureaubladtoepassing te installeren.

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![Aanmelden bij Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Als u zich wilt aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing, gebruikt u dezelfde gegevens als waarmee u zich in de browser hebt aangemeld bij Adobe Dynamic Media Classic.

   Voor de **[!UICONTROL Server]** voor gebruik, zie de volgende afbeelding voor het productiemilieu:

   | Server | URL browser |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

1. Na aanmelden ziet u de vertrouwde ervaring van de gebruikersinterface van de browser. U kunt uw dagelijkse Adobe Dynamic Media Classic-activiteiten op de desktopapp op de gebruikelijke wijze voortzetten.

## Downloaden en *stilzwijgend* installeer de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing op macOS {#install-silent-mac-dmc-app}

Zie ook:

* [Download en installeer de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing op Mac of Windows](#installation-dmc-app)
* [Download en installeer zonder toezicht de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing in Windows](#install-silent-windows-dmc-app)

Om te downloaden en *stilzwijgend* Installeer de nieuwste versie van de Adobe Dynamic Media Classic-bureaubladtoepassing op macOS:

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing voor macOS.

   * [macOS (.DMG): downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Koppel het gedownloade beeld van de Schijf (.DMG) aan een montageselocatie gebruikend het volgende bevel:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Het APP-bestand kopiëren naar **[!UICONTROL Applications]** met de volgende opdracht:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![Aanmelden bij Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Als u zich wilt aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing, gebruikt u dezelfde gegevens als waarmee u zich in de browser hebt aangemeld bij Adobe Dynamic Media Classic.

   Voor de **[!UICONTROL Server]** voor gebruik, zie de volgende afbeelding voor het productiemilieu:

   | Server | URL browser |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

## Downloaden en *stilzwijgend* de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing installeren op Windows® {#install-silent-windows-dmc-app}

Het bevel dat u gebruikt is voor een basisMSI stille installatie. Het installatieprogramma van de Adobe Dynamic Media Classic-bureaubladtoepassing is echter een installatieprogramma van InstallScript MSI dat is gemaakt met InstallShield. Wanneer u het installatieprogramma uitvoert in de recordmodus, wordt gebruikersinteractie opgenomen in een reactiebestand. Dit reactiebestand wordt vervolgens gebruikt voor een installatie op de achtergrond, zoals beschreven in [Installatie in stille modus uitvoeren](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Zie ook:

* [Download en installeer de nieuwste Adobe Dynamic Media Classic-bureaubladtoepassing op Mac of Windows](#installation-dmc-app)

* [Download en installeer zonder toezicht de nieuwste Adobe Dynamic Media Classic desktop app op macOS](#install-silent-mac-dmc-app)

Om te downloaden en *stilzwijgend* installeer de nieuwste versie van de Adobe Dynamic Media Classic-bureaubladtoepassing op Windows®:

1. Verwijder eventuele oudere versies van Adobe Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing.

   * [Windows® (.EXE): downloaden](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Voer het installatieprogramma in recordmodus uit met de volgende opdracht:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Voer in het venster van het GUI-installatieprogramma de stappen uit om te installeren, zodat interacties/invoer, zoals de installatielocatie, worden opgenomen in `Setup.iss` bestand.

1. Het gemaakte bestand kopiëren `Setup.iss` en `adobe-dynamic-media-classic-20.22.1.exe` naar andere computer.

1. Voer de volgende opdracht voor een installatie op de achtergrond uit:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Details over opdrachtregelparameters zijn beschikbaar op [De bevel-lijn van Setup.exe en Update.exe parameters](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Wanneer u de toepassing opent, wordt de nieuwe Adobe Dynamic Media Classic-aanmeldingspagina weergegeven:

   ![Aanmelden bij Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Als u zich wilt aanmelden bij de Adobe Dynamic Media Classic-bureaubladtoepassing, gebruikt u dezelfde gegevens als waarmee u zich in de browser hebt aangemeld bij Adobe Dynamic Media Classic.

   Voor de **[!UICONTROL Server]** voor gebruik, zie de volgende afbeelding voor het productiemilieu:

   | Server | URL browser |
   | --- | --- |
   | NA Productie (Noord-Amerika) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Middle East, and Africa) | https://s7sps3.scene7.com/ |
   | APAC-productie (Azië-Stille Oceaan) | https://s7sps5.scene7.com/ |

## Video doorlopen bij gebruik van Adobe Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Kijk eens naar [video doorlopen bij gebruik van Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/nl/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (2 minuten 36 seconden).

## De afbeeldingscache en de assetcache op uw computer wissen met de bureaubladtoepassing {#clear-cache}

1. Tik in de Adobe Dynamic Media Classic-bureaubladtoepassing in de rechterbovenhoek op **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Op de **[!UICONTROL Personal Setup]** pagina, onder de **[!UICONTROL Desktop]** Voer een van de volgende handelingen uit:
   * Tik op **[!UICONTROL Clear Image Cache]** tikt u vervolgens op **[!UICONTROL OK]**.
   * Tik op **[!UICONTROL Clear Asset Cache]** tikt u vervolgens op **[!UICONTROL OK]**.
1. Tik rechtsonder op de pagina op **[!UICONTROL Close]**.

### De afbeeldingscache en de elementcache handmatig wissen

U kunt de cache van afbeeldingen en elementen niet alleen wissen met de bureaubladtoepassing, maar u kunt de cache ook handmatig rechtstreeks wissen vanuit het bestandssysteem.

1. Navigeer op basis van uw besturingssysteem naar het volgende:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Bekende beperkingen in Adobe Dynamic Media Classic 20.21.1

* De **[!UICONTROL Server]** De vervolgkeuzelijst is leeg na het bijwerken naar Adobe Dynamic Media Classic-bureaubladtoepassing 20.21.1: scenario: installeer en meld u aan bij Adobe Dynamic Media Classic 20.20.1 of 20.20.2 en sluit vervolgens de toepassing. Vervolgens gaat u naar Adobe Dynamic Media Classic 20.21.1. Wanneer u zich probeert aan te melden, **[!UICONTROL Server]** vervolgkeuzelijst in de **[!UICONTROL Sign-in to your account]** is leeg. Als u dit probleem wilt oplossen, moet u [de cache handmatig wissen](#clear-cache) (zie bovenstaande stappen).

## Bekende beperkingen in Adobe Dynamic Media Classic 20.20.1 (vastgesteld in 20.20.2)

**_Alleen van toepassing op Windows® - Is er een beperking op het aantal bestanden dat kan worden geüpload via de interface van de bureaubladtoepassing?_**<br>Ja, er kunnen maximaal 150 bestanden tegelijk worden geüpload met de interface van de bureaubladtoepassing.

**_Is van toepassing op Windows® en macOS - Hoe schakel ik tussen bedrijven?_**<br>Ga als volgt te werk om tussen bedrijven te schakelen:

* Selecteer in de Adobe Dynamic Media Classic-app het nieuwe bedrijf in de vervolgkeuzelijst met bedrijven.
* Tik op **[!UICONTROL OK]** om u af te melden en de app te sluiten.

  ![Start de app opnieuw om het nieuwe bedrijf te gebruiken](/help/using/assets/dmclassic-new-company1.png)

* Start Adobe Dynamic Media Classic opnieuw en meld u vervolgens op de gebruikelijke wijze aan om met het nieuwe bedrijf te werken.

## Tips en trucs

**_Ik zie het deelvenster Media Cart niet op de landingspagina van Adobe Dynamic Media Classic._**<br>Tik in Adobe Dynamic Media Classic op **[!UICONTROL Setup > Personal Setup]**. Controleer of in de sectie Browser **[!UICONTROL Show MediaPortal Features]**&#x200B;is geselecteerd (ingeschakeld). Tikken **[!UICONTROL Save > Close]**.

**_De publicatiestatus (groene indicator) van een element wordt niet correct weergegeven._**<br>In de gebruikersinterface van de browser was opnieuw aanmelden bij de gebruikersinterface vereist om de juiste publicatiestatus van elementen te zien. In de bureaubladtoepassing heeft Adobe een **[!UICONTROL Refresh]**&#x200B;op de werkbalk, rechts van **[!UICONTROL Select None]**&#x200B;knop. Tik op de knop **[!UICONTROL Refresh]**&#x200B;om de laatste status van alle elementen op de opgegeven pagina te zien. Geen heraanmelding vereist zoals met de gebruikersinterface van de browser.

![Pictogram Vernieuwen](/help/using/assets/refresh-icon1.png)
*Pictogram Vernieuwen*

**_Ik zie geen voorinstellingen voor batchsets werken in de bureaubladtoepassing._**<br>Tikken **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Zorgen voor de relevante **[!UICONTROL Batch Set Preset]**&#x200B;is ingeschakeld. Klikken **[!UICONTROL Save and Submit upload]**.
