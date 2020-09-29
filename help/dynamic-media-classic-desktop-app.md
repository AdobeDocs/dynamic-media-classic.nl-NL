---
title: Adobe Dynamic Media Classic-bureaubladtoepassing - Nu beschikbaar
seo-title: Adobe Dynamic Media Classic-bureaubladtoepassing - Nu beschikbaar
description: 'null'
seo-description: Meer informatie over Dynamic Media Classic-bureaubladtoepassing.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 477a8fd6ffee00cd586d91f6eeda8e676753a90f
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---


# Nu beschikbaar: Adobe Dynamic Media Classic-bureaubladtoepassing {#dynamic-media-classic-desktop-app}

Gebruikers van Dynamic Media Classic hebben nu toegang tot een nieuwe bureaubladtoepassing die niet langer afhankelijk is van Adobe Flash in de browser.

Deze nieuwe app is nu beschikbaar voor Windows en macOS.

>[!IMPORTANT]
>
>We raden u aan de nieuwe Adobe Dynamic Media Classic-bureaubladtoepassing tegen 1 oktober 2020 te installeren. Als u dit doet, hebt u een soepele overgang voordat de Adobe Flash Player op 31 december 2020 wordt afgekeurd. Op die datum kunt u zich niet meer aanmelden bij de browserversie van de gebruikersinterface van Adobe Dynamic Media Classic, die in het product als Dynamic Media Classic wordt aangeduid.

Raadpleeg de veelgestelde vragen voor het [nieuwe digitale inloggen voor dynamische media.](/help/new-ui-2020.md)

## Systeemvereisten voor Adobe Dynamic Media Classic-bureaubladtoepassing {#system-requirements-dmc-app}

Adobe Dynamic Media Classic-bureaubladtoepassing is compatibel met de volgende besturingssystemen:
* macOS X 10.10 of hoger.
* Windows 7 of hoger.

## Download en installeer Adobe Dynamic Media Classic-bureaubladtoepassing op MacOS of Windows {#installation-dmc-app}

Zie ook:

* [Download en *stil* installeer Adobe Dynamic Media Classic-bureaubladtoepassing op MacOS](#install-silent-mac-dmc-app)
* [Download en *stil* installeer Adobe Dynamic Media Classic-bureaubladtoepassing in Windows](#install-silent-windows-dmc-app)

1. Verwijder eventuele oudere versies van Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing.

   * [macOS (.DMG) - Download.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.EXE) - Downloaden.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Voer een van de volgende handelingen uit op basis van het installatieprogramma dat u hebt gedownload.

   * **Voor MacOS** - Sleep het bestand naar het **[!UICONTROL Drag & drop to install]** dialoogvenster **[!UICONTROL Adobe Dynamic Media Classic]** en zet het neer op **[!UICONTROL Applications]**.

      ![Installatie van slepen en neerzetten op MacOS](/help/assets/dragondrop-install1.png)

   * Tik in de **[!UICONTROL Applications]** map op het pictogram Adobe Dynamic Media Classic.
   * Tik in het dialoogvenster **[!UICONTROL Open]** om de Klassieke bureaublad-app Adobe Dynamic Media Classic te openen.

      ![Gedownloade app openen](/help/assets/open-dmclassicapp1.png)

   * **Voor Windows** - Voer het binaire bestand van het installatieprogramma uit en volg de aanwijzingen op het scherm om de bureaubladtoepassing te installeren.

1. Wanneer u de toepassing opent, wordt de nieuwe pagina Dynamische Adobe Dynamic Media Classic Sign In weergegeven:

   ![Dynamic Media Classic aanmelden](/help/assets/dmclassic-login1.png)

1. Gebruik dezelfde referenties als uw browserreferenties om u aan te melden bij Adobe Dynamic Media Classic.

   Zie de volgende afbeelding voor de productieomgeving **[!UICONTROL Server]** voor informatie over het gebruik:

   | URL browser | Servernaam bureaubladtoepassing |
   |---|---|
   | https://s7sps1.scene7.com/ | NA (Noord-Amerika) productie |
   | https://s7sps3.scene7.com/ | Productie EMEA (Europa, Midden-Oosten en Afrika) |
   | https://s7sps5.scene7.com/ | APAC-productie (Azië-Stille Oceaan) |

1. Post login UI, zult u het vertrouwde browser ervaring UI opmerken. U kunt uw dagelijkse activiteiten op de gebruikelijke wijze nu uitvoeren op de interface van de bureaubladtoepassing.

## Download en *stil* installeer Adobe Dynamic Media Classic-bureaubladtoepassing op MacOS {#install-silent-mac-dmc-app}

Zie ook:

* [Download en installeer Adobe Dynamic Media Classic-bureaubladtoepassing op Mac of Windows](#installation-dmc-app)
* [Download en *stil* installeer Adobe Dynamic Media Classic-bureaubladtoepassing in Windows](#install-silent-windows-dmc-app)

U kunt als volgt de Adobe Dynamic Media Classic-bureaubladtoepassing voor  media downloaden en *stil* installeren op MacOS:

1. Verwijder eventuele oudere versies van Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing voor macOS.

   * [macOS (.DMG) - Download.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)

1. Koppel het gedownloade beeld van de Schijf (.DMG) aan een montageselocatie gebruikend het volgende bevel:

   `hdiutil attach adobe-dynamic-media-classic-20.20.1.dmg -mountpoint <mount_point_path>`

1. Kopieer het APP-bestand naar de volgende opdracht **[!UICONTROL Applications]** :

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. Wanneer u de toepassing opent, wordt de nieuwe pagina Dynamische Adobe Dynamic Media Classic Sign In weergegeven:

   ![Dynamic Media Classic aanmelden](/help/assets/dmclassic-login1.png)

1. Gebruik dezelfde referenties als uw browserreferenties om u aan te melden bij Adobe Dynamic Media Classic.

   Zie de volgende afbeelding voor de productieomgeving **[!UICONTROL Server]** voor informatie over het gebruik:

   | URL browser | Servernaam bureaubladtoepassing |
   |---|---|
   | https://s7sps1.scene7.com/ | NA (Noord-Amerika) productie |
   | https://s7sps3.scene7.com/ | Productie EMEA (Europa, Midden-Oosten en Afrika) |
   | https://s7sps5.scene7.com/ | APAC-productie (Azië-Stille Oceaan) |

## Download en *stil* installeer Adobe Dynamic Media Classic-bureaubladtoepassing in Windows {#install-silent-windows-dmc-app}

Het bevel dat u gebruikt is voor een basisMSI stille installatie. Het Dynamic Media Classic-bureaubladinstallatieprogramma is echter een installatieprogramma van InstallScript MSI dat is gemaakt met InstallShield. Wanneer u het installatieprogramma uitvoert in de recordmodus, wordt gebruikersinteractie opgenomen in een reactiebestand. Dit reactiebestand wordt vervolgens gebruikt voor een installatie op de achtergrond, zoals wordt beschreven in Installaties [uitvoeren in de modus Stil.](https://docs.flexera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Zie ook:

* [Download en installeer Adobe Dynamic Media Classic-bureaubladtoepassing op Mac of Windows](#installation-dmc-app)
* [Download en *stil* installeer Adobe Dynamic Media Classic-bureaubladtoepassing in Windows](#install-silent-windows-dmc-app)

U kunt als volgt de app Adobe Dynamic Media Classic desktop in Windows downloaden en *stil* installeren:

1. Verwijder eventuele oudere versies van Dynamic Media Classic-bureaubladtoepassingen op uw systeem.

1. Download het nieuwste installatieprogramma voor de Adobe Dynamic Media Classic-bureaubladtoepassing.

   * [Windows (.EXE) - Downloaden.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Voer het installatieprogramma in recordmodus uit met de volgende opdracht:

   `adobe-dynamic-media-classic-20.20.1.exe /r /f1"C:\Setup.iss"`

1. Voer in het venster van het GUI-installatieprogramma de stappen uit om te installeren, zodat interacties/invoer, zoals de installatielocatie, worden opgenomen in het `Setup.iss` bestand.

1. Kopieer het gemaakte `Setup.iss` bestand en `adobe-dynamic-media-classic-20.20.1.exe` naar een andere computer.

1. Voer de volgende opdracht voor een installatie op de achtergrond uit:

   `adobe-dynamic-media-classic-20.20.1.exe /s /f1"C:\Setup.iss"`

   De details over de parameters van de bevellijn zijn beschikbaar bij [Setup.exe en Update.exe bevel-Lijn Parameters.](https://docs.flexera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Wanneer u de toepassing opent, wordt de nieuwe pagina Dynamische Adobe Dynamic Media Classic Sign In weergegeven:

   ![Dynamic Media Classic aanmelden](/help/assets/dmclassic-login1.png)

1. Gebruik dezelfde referenties als uw browserreferenties om u aan te melden bij Adobe Dynamic Media Classic.

   Zie de volgende afbeelding voor de productieomgeving **[!UICONTROL Server]** voor informatie over het gebruik:

   | URL browser | Servernaam bureaubladtoepassing |
   |---|---|
   | https://s7sps1.scene7.com/ | NA (Noord-Amerika) productie |
   | https://s7sps3.scene7.com/ | Productie EMEA (Europa, Midden-Oosten en Afrika) |
   | https://s7sps5.scene7.com/ | APAC-productie (Azië-Stille Oceaan) |


## Video doorlopen bij gebruik van Dynamic Media Classic Desktop App

Bekijk een [videodemo over het gebruik van Dynamic Media Classic Desktop App](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) (Lengte: 2 minuten 36 seconden).

## Bekende beperkingen in Dynamic Media Classic

**_Alleen van toepassing op Windows: is er een beperking op het aantal bestanden dat kan worden geüpload via de interface van de bureaubladtoepassing?_**<br>Ja, er kunnen maximaal 150 bestanden tegelijk worden geüpload via de interface van de bureaubladtoepassing.

**_Is op Vensters en macOS van toepassing - hoe schakel ik tussen bedrijven?_**<br>Ga als volgt te werk om tussen bedrijven te schakelen:
* Selecteer het nieuwe bedrijf in de vervolgkeuzelijst met bedrijven in de Klassieke app Dynamic Media.
* Tik op het moment dat het pop-upvenster verschijnt **[!UICONTROL OK]** om u af te melden en de app te sluiten.

   ![Start de app opnieuw om het nieuwe bedrijf te gebruiken](/help/assets/dmclassic-new-company1.png)
* Start Dynamic Media Classic opnieuw en meld u vervolgens op de gebruikelijke wijze aan om met het nieuwe bedrijf te werken.

## Tips en trucs

**_Ik kan het deelvenster Media Cart niet zien op de landingspagina van Dynamic Media Classic._**<br>Tik op Dynamic Media Classic **[!UICONTROL Setup > Personal Setup]**. Controleer of in de sectie Browser de optie **[!UICONTROL Show MediaPortal Features]**is geselecteerd (ingeschakeld). Tik op **[!UICONTROL Save > Close]**.

**_De publicatiestatus (groene indicator) van een element wordt niet correct weergegeven._**<br>In browser UI, was re-login aan UI vereist om de correcte publicatiestaat van activa te zien. In de bureaubladtoepassing is een pictogram op de werkbalk toegevoegd, rechts van de **[!UICONTROL Refresh]****[!UICONTROL Select None]**knop. Tik op het **[!UICONTROL Refresh]**pictogram om de laatste status van alle elementen op de opgegeven pagina weer te geven. U hoeft zich niet opnieuw aan te melden, zoals in de gebruikersinterface van de browser.

![Pictogram](/help/assets/refresh-icon1.png)*Vernieuwen vernieuwen*

**_Ik zie geen voorinstellingen voor batchsets werken in de bureaubladtoepassing._**<br>Tik op **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Zorg ervoor dat de betreffende functie **[!UICONTROL Batch Set Preset]**is ingeschakeld. Klik op **[!UICONTROL Save and Submit upload]**.
