---
title: Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal
seo-title: Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal
description: 'null'
seo-description: Leer hoe u exportopties opgeeft die beschikbaar zijn voor gebruikers van Media Portal.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---


# Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal {#specifying-export-options-available-to-media-portal-users}

Als de beheerder hun toestemming geeft, kunnen de gebruikers van het Portaal van Media beelden opnieuw formatteren aangezien zij hen uitvoeren. Ze kunnen bijvoorbeeld de grootte, de bestandsindeling en de afbeeldingskwaliteit wijzigen. Als u afbeeldingen automatisch opnieuw opmaakt terwijl ze worden geëxporteerd, bespaart u tijd omdat u de afbeeldingen niet afzonderlijk opnieuw hoeft op te maken. Bovendien kunnen beheerders een voorinstelling maken. Dit is een vooraf ingestelde selectie van instellingen voor de afbeeldingsindeling. U kunt een voorinstelling gebruiken wanneer u afbeeldingen exporteert om deze opnieuw op te maken volgens de specificaties van uw bedrijf.

De volgende twee beperkingen gelden als u afbeeldingselementen exporteert via een door de gebruiker gedefinieerde conversie of als u originele master afbeeldingen exporteert:

* Het gecomprimeerde Zip-exportbestand heeft een maximale bestandsgrootte van 1 GB voor de exporttaak.
* Per exporttaak kunt u maximaal 500 elementen in totaal gebruiken.

Zie ook [Elementen exporteren uit Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal**

1. Klik **Setup** > **Voorinstellingen afbeelding**.
1. Selecteer een of meer van de volgende opties in het venster Voorinstellingen afbeelding:

   * **Schakel Door gebruiker gedefinieerde**
conversieAls deze optie is geselecteerd, kunnen gebruikers een andere optie kiezen in de vervolgkeuzelijst Grootte in het venster Geselecteerde elementen exporteren. Vervolgens kunnen gebruikers een maateenheid kiezen, zoals pixels of centimeters, en vervolgens de gewenste breedte en hoogte opgeven. Wanneer deze bestanden worden geëxporteerd of gedownload, worden de afbeeldingsbestanden opnieuw opgemaakt.

      Wanneer **pixels** worden gekozen uit **Grootte**
in de vervolgkeuzelijst kan de resulterende breedte x hoogte van de afbeelding niet groter zijn dan 100 miljoen pixels. Deze grootte is 10.000 x 10.000 pixels voor een vierkante afbeelding of ongeveer 8.000 x 12.000 pixels voor een afbeelding met de hoogte-breedteverhouding 2x3. Deze formaatbeperking geldt niet als u originele master afbeeldingen exporteert.

      Schakel deze optie uit als u wilt dat gebruikers bestanden downloaden zonder ze opnieuw op te maken terwijl ze worden gedownload.

   * **Schakel**
Origineel exporteren in. Hiermee kunt u originele master afbeeldingen exporteren. In het deelvenster Geselecteerde elementen exporteren kunnen gebruikers het vervolgkeuzemenu Conversie openen en Origineel exporteren kiezen om de oorspronkelijke bestanden te exporteren. Schakel deze optie uit als u gebruikers wilt dwingen een voorinstelling voor afbeeldingen te kiezen of conversieopties wilt kiezen wanneer zij afbeeldingen exporteren.

>[!MORELIKETHIS]
>
>* [Voorinstellingen afbeelding](application-setup.md#image_presets)
>* [Toegangsrechten voor een groep kiezen voor Voorinstelling afbeelding](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

