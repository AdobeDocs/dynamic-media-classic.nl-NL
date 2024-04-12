---
title: Beschikbare exportopties voor gebruikers van Media Portal opgeven
description: Leer hoe u exportopties opgeeft die beschikbaar zijn voor gebruikers van Media Portal in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Beschikbare exportopties voor gebruikers van Media Portal opgeven {#specifying-export-options-available-to-media-portal-users}

Als de beheerder hun toestemming geeft, kunnen de gebruikers van het Portaal van Media beelden opnieuw formatteren aangezien zij hen uitvoeren. Ze kunnen bijvoorbeeld de grootte, de bestandsindeling en de afbeeldingskwaliteit wijzigen. Als u afbeeldingen automatisch opnieuw opmaakt terwijl ze worden geëxporteerd, bespaart u tijd omdat u de afbeeldingen niet afzonderlijk opnieuw hoeft op te maken. Bovendien kunnen beheerders een voorinstelling maken. Dit is een vooraf ingestelde selectie van instellingen voor de afbeeldingsindeling. U kunt een voorinstelling gebruiken wanneer u afbeeldingen exporteert om deze opnieuw op te maken volgens de specificaties van uw bedrijf.

De volgende twee beperkingen zijn van toepassing als u afbeeldingselementen exporteert via een door de gebruiker gedefinieerde conversie of als u oorspronkelijke primaire afbeeldingen exporteert:

* Het gecomprimeerde Zip-exportbestand heeft een maximale bestandsgrootte van 1 GB voor de exporttaak.
* Per exporttaak kunt u maximaal 500 elementen in totaal gebruiken.

Zie ook [Elementen exporteren uit Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**U kunt als volgt exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal:**

1. Ga op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Selecteer een of meer van de volgende opties in het venster Voorinstellingen afbeelding:

   * **Door gebruiker gedefinieerde conversie inschakelen** - Als deze optie is geselecteerd, kunnen gebruikers andere opties kiezen in het menu **[!UICONTROL Size]** vervolgkeuzelijst in het venster Geselecteerde elementen exporteren. Vervolgens kunnen gebruikers een maateenheid kiezen, zoals pixels of centimeters, en vervolgens de gewenste breedte en hoogte opgeven. Wanneer ze deze bestanden exporteren of downloaden, worden de afbeeldingsbestanden opnieuw opgemaakt.

     Wanneer **[!UICONTROL pixels]** worden gekozen uit de **[!UICONTROL Size]** In de vervolgkeuzelijst kan de resulterende breedte en hoogte van de afbeelding niet groter zijn dan 100 miljoen pixels. Deze grootte is gelijk aan 10,000 × 10,000 pixels voor een vierkante afbeelding of ongeveer 8,000 × 12,000 pixels voor een afbeelding met een hoogte-breedteverhouding van 2x3. Deze formaatbeperking geldt niet als u originele primaire afbeeldingen exporteert.

     Schakel deze optie uit als u wilt dat gebruikers bestanden downloaden zonder ze opnieuw op te maken terwijl ze worden gedownload.

   * **Origineel exporteren inschakelen** - Hiermee kunt u oorspronkelijke primaire afbeeldingen exporteren. In de **[!UICONTROL Export Selected Assets]** kunnen gebruikers het deelvenster **[!UICONTROL Conversion]** en kiest u **[!UICONTROL Export Original]** om oorspronkelijke bestanden te exporteren. Schakel deze optie uit als u gebruikers wilt dwingen een voorinstelling voor afbeeldingen te kiezen of conversieopties wilt kiezen wanneer ze afbeeldingen exporteren.

>[!MORELIKETHIS]
>
>* [Voorinstellingen afbeelding](application-setup.md#image_presets)
>* [Toegangsrechten voor een groep kiezen voor Voorinstelling afbeelding](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
