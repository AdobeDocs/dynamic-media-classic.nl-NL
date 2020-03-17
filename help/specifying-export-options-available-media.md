---
title: Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal
seo-title: Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal
description: 'null'
seo-description: Leer hoe u exportopties opgeeft die beschikbaar zijn voor gebruikers van Media Portal.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal {#specifying-export-options-available-to-media-portal-users}

Als de beheerder hun toestemming geeft, kunnen de gebruikers van het Portaal van Media beelden opnieuw formatteren aangezien zij hen uitvoeren. Ze kunnen bijvoorbeeld de grootte, de bestandsindeling en de afbeeldingskwaliteit wijzigen. Als u afbeeldingen automatisch opnieuw opmaakt terwijl ze worden geëxporteerd, bespaart u tijd omdat u de afbeeldingen niet afzonderlijk opnieuw hoeft op te maken. Bovendien kunnen beheerders een voorinstelling maken. Dit is een vooraf ingestelde selectie van instellingen voor de afbeeldingsindeling. U kunt een voorinstelling gebruiken wanneer u afbeeldingen exporteert om deze opnieuw op te maken volgens de specificaties van uw bedrijf.

De volgende twee beperkingen zijn van toepassing als u afbeeldingselementen exporteert via een door de gebruiker gedefinieerde conversie of als u originele hoofdafbeeldingen exporteert:

* Het gecomprimeerde Zip-exportbestand heeft een maximale bestandsgrootte van 1 GB voor de exporttaak.
* Per exporttaak kunt u maximaal 500 elementen in totaal gebruiken.

Zie ook het [Uitvoeren van activa van het Publiceren Scene7 Systeem](exporting-assets-scene7-publishing-system.md#exporting_assets_from_scene7_publishing_system).

**Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal**

1. Klik op **Instellen** > **Voorinstellingen** afbeelding.
1. Selecteer een of meer van de volgende opties in het venster Voorinstellingen afbeelding:

   * **Schakel Door gebruiker gedefinieerde omzetting** inschakelen Als deze optie is geselecteerd, kunnen gebruikers een andere optie kiezen in de vervolgkeuzelijst Grootte in het venster Geselecteerde elementen exporteren. Vervolgens kunnen gebruikers een maateenheid kiezen, zoals pixels of centimeters, en vervolgens de gewenste breedte en hoogte opgeven. Wanneer deze bestanden worden geëxporteerd of gedownload, worden de afbeeldingsbestanden opnieuw opgemaakt.

      Wanneer u **pixels** kiest in de vervolgkeuzelijst **Grootte**, mag de resulterende breedte x hoogte van de afbeelding niet groter zijn dan 100 miljoen pixels. Deze grootte is 10.000 x 10.000 pixels voor een vierkante afbeelding of ongeveer 8.000 x 12.000 pixels voor een afbeelding met de hoogte-breedteverhouding 2x3. Deze formaatbeperking geldt niet als u originele hoofdafbeeldingen exporteert.

      Schakel deze optie uit als u wilt dat gebruikers bestanden downloaden zonder ze opnieuw op te maken terwijl ze worden gedownload.

   * **Met Origineel** exporteren kunt u originele hoofdafbeeldingen exporteren. In het deelvenster Geselecteerde elementen exporteren kunnen gebruikers het vervolgkeuzemenu Conversie openen en Origineel exporteren kiezen om de oorspronkelijke bestanden te exporteren. Schakel deze optie uit als u gebruikers wilt dwingen een voorinstelling voor afbeeldingen te kiezen of conversieopties wilt kiezen wanneer zij afbeeldingen exporteren.

>[!MORELIKETHIS]
>
>* [Voorinstellingen afbeelding](application-setup.md#image_presets)
>* [Toegangsrechten voor een groep kiezen voor Voorinstelling afbeelding](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

