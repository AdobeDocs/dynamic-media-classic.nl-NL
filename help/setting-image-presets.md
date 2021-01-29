---
title: Voorinstellingen afbeelding instellen
description: Leer hoe u voorinstellingen voor afbeeldingen instelt.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 10%

---


# Voorinstellingen afbeelding instellen{#setting-up-image-presets}

Net als bij een macro is een voorinstelling voor afbeeldingen een vooraf gedefinieerde verzameling opdrachten voor het vergroten of verkleinen en opmaken van de grootte die onder een naam zijn opgeslagen. Als u wilt weten hoe Voorinstellingen afbeelding werken, kunt u ervan uitgaan dat elke productafbeelding op uw website moet worden weergegeven met twee verschillende grootten: 500 x 500 pixels en 150 x 150 pixels. U maakt twee voorinstellingen voor afbeeldingen, een voorinstelling genaamd &quot;Vergroten&quot;, waarmee u afbeeldingen met 500 x 500 pixels kunt weergeven en een voorinstelling genaamd &quot;Miniatuur&quot; om afbeeldingen met 150 x 150 pixels weer te geven. Als u afbeeldingen wilt leveren met de grootte &quot;Vergroten&quot; en &quot;Miniatuur&quot;, zoekt een Dynamic Media Image Server naar de definitie van de voorinstelling Afbeelding vergroten en Afbeelding miniatuur. Vervolgens genereert de server dynamisch een afbeelding met de grootte en opmaakspecificaties van elke voorinstelling voor afbeeldingen.

Dynamic Media Classic wordt geleverd met verschillende &quot;best practices&quot; voor voorinstellingen voor afbeeldingen die al zijn ingesteld voor gebruik. Beheerders kunnen ook nieuwe voorinstellingen voor afbeeldingen maken. Als u een voorinstelling voor afbeeldingen wilt maken, begint u helemaal opnieuw of u kunt een bestaande voorinstelling opnieuw gebruiken en opslaan onder een andere naam.

Afbeeldingen die kleiner worden wanneer ze dynamisch van een server worden geleverd, kunnen scherper en gedetailleerder worden. Daarom bevat elke voorinstelling voor afbeeldingen opmaakbesturingselementen waarmee u een afbeelding kunt optimaliseren wanneer deze met een bepaalde grootte wordt geleverd. Met deze besturingselementen zorgt u ervoor dat uw afbeeldingen scherp en duidelijk zijn wanneer ze aan uw website of toepassing worden geleverd.

## Een voorinstelling {#creating-an-image-preset} voor afbeeldingen maken

U kunt uw eigen Voorinstellingen voor afbeeldingen maken als u een bedrijfsbeheerder bent. U kunt nieuwe voorinstellingen voor afbeeldingen maken of beginnen met een standaardvoorinstelling voor afbeeldingen die beschikbaar is in Dynamic Media Classic, deze bewerken en opslaan onder een andere naam.

**Een voorinstelling voor afbeeldingen maken**

1. Klik **Setup** > **Voorinstellingen afbeelding**.

   U kunt naar de naam van een voorinstelling voor afbeeldingen op dit scherm bladeren om een voorvertoning van een bestaande voorinstelling voor afbeeldingen weer te geven. Als u een naam selecteert voor de voorinstelling Afbeelding, wijzigt de grootte en de weergave van de voorbeeldafbeelding in het voorvertoningsvenster.

1. Voer een van de volgende handelingen uit:

   * **Een**
voorinstelling voor afbeelding makenKlik op Toevoegen.

   * **Een**
voorinstelling voor afbeelding bewerkenBlader naar de voorinstelling voor afbeeldingen die het meest lijkt op de voorinstelling die u wilt maken en klik op Bewerken.

1. Voer een naam in voor de voorinstelling voor afbeelding.
1. Voer afmetingen voor de breedte en hoogte in pixels in. Deze metingen bepalen de grootte waarmee afbeeldingen worden geleverd.
1. Vul het scherm Voorinstelling toevoegen of Voorinstelling bewerken in. Zie [Opties voor voorinstellingen afbeelding](application-setup.md#image_preset_options) voor meer informatie.

   Dynamic Media Classic raadt de volgende opties voor &#39;best practices&#39; aan om te beginnen:

   * ****
IndelingKies een indeling die aan uw vereisten voldoet. Alle webbrowsers ondersteunen de JPEG-afbeeldingsindeling. Deze biedt een goede balans tussen kleine bestandsgrootten en afbeeldingskwaliteit. JPEG-afbeeldingen gebruiken echter een compressieschema met dataverlies dat ongewenste afbeeldingsartefacten kan veroorzaken als de compressie-instelling te laag is. Daarom wordt in Dynamic Media Classic aangeraden de compressiekwaliteit (op de schuifregelaar) in te stellen op 75. Deze instelling biedt een goede balans tussen afbeeldingskwaliteit en kleine bestandsgrootte.

   * ****
VerscherpenSelecteer Verscherpen niet (dit verscherpingsfilter biedt minder controle dan de instellingen voor Onscherp masker).

   * **Nieuwe pixels berekenen in**
modusKies Bi-Cubic.

   * **Onscherp maskeren (USM)-**
optiesVoer de hier weergegeven instellingen in:
   | Type voorinstelling | Grootte | USM: Hoeveelheid | USM: Straal | USM: Drempel |
   |--- |--- |--- |--- |--- |
   | Cross-Sell (miniatuur) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatuur | 150 x 150 | 1,1 | 1 | 5 |
   | Hoofd | 350 x 350 | 3 | 3 | 6 |
   | Vergroten | 500 x 500 | 1,2 | 1,2 | 5 |

1. Klik **Opslaan**.

De Klassieke de &quot;beste praktijken&quot;opties van Dynamic Media voor het creëren van Beeld hier worden vermeld die vooraf instelt zijn algemene aanbevelingen; verscherpen is zeer subjectief . Deze &quot;beste praktijken&quot;montages waren gebaseerd op een 2000x 2000 master beeld; de instellingen voor grotere of kleinere stramienen kunnen verschillend zijn. Als u de instellingen voor Onscherp masker wilt aanpassen, raadt Dynamic Media Classic de volgende bereiken aan:

* ****
HoeveelheidTussen 0,8 en 1,5.

* ****
StraalTussen 0,6 en 2.

* ****
DrempelVan 1-6.

Als u een voorinstelling voor afbeeldingen wilt verwijderen, selecteert u deze in het scherm Voorinstellingen afbeelding en selecteert u de knop Verwijderen.

>[!MORELIKETHIS]
>
>* [Voorinstellingen voor afbeeldingen maken en bewerken](application-setup.md#creating_and_editing_image_presets)
>* [Voorinstellingsopties voor afbeelding](application-setup.md#image_preset_options)
>* [Een voorvertoning weergeven van een afbeeldingselement op basis van de voorinstelling voor afbeelding](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

