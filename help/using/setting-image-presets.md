---
title: Voorinstellingen afbeelding instellen
description: Leer hoe u voorinstellingen voor afbeeldingen instelt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 1%

---

# Voorinstellingen afbeelding instellen{#setting-up-image-presets}

Net als bij een macro is een voorinstelling voor afbeeldingen een vooraf gedefinieerde verzameling opdrachten voor het vergroten of verkleinen en opmaken van de grootte die onder een naam zijn opgeslagen. Als u wilt weten hoe Voorinstellingen afbeelding werken, veronderstelt u dat elke productafbeelding op uw website moet worden weergegeven met twee verschillende grootten: 500 × 500 pixels en 150 × 150 pixels. U maakt twee voorinstellingen voor afbeeldingen, een voorinstelling genaamd &quot;Vergroten&quot;, waarmee u afbeeldingen met 500 x 500 pixels kunt weergeven en een voorinstelling genaamd &quot;Miniatuur&quot; om afbeeldingen met 150 x 150 pixels weer te geven. Als u afbeeldingen wilt leveren met de grootte &quot;Vergroten&quot; en &quot;Miniatuur&quot;, wordt in een Dynamic Media Image Server de definitie van de voorinstelling &quot;Afbeelding vergroten&quot; en &quot;Voorinstelling miniatuurafbeelding&quot; opgezocht. Vervolgens genereert de server dynamisch een afbeelding met de grootte en opmaakspecificaties van elke voorinstelling voor afbeeldingen.

Adobe Dynamic Media Classic wordt geleverd met verschillende &quot;best practice&quot;-voorinstellingen voor afbeeldingen die al zijn ingesteld voor gebruik. Beheerders kunnen ook voorinstellingen voor afbeeldingen maken. Als u een voorinstelling voor afbeeldingen wilt maken, begint u helemaal opnieuw of u kunt een bestaande voorinstelling opnieuw gebruiken en opslaan onder een andere naam.

Afbeeldingen die kleiner worden wanneer ze dynamisch van een server worden geleverd, kunnen scherper en gedetailleerder worden. Daarom bevat elke voorinstelling voor afbeeldingen opmaakbesturingselementen waarmee u een afbeelding kunt optimaliseren wanneer deze met een bepaalde grootte wordt geleverd. Deze controles zorgen ervoor dat uw beelden scherp en duidelijk zijn wanneer zij aan uw Website of toepassing worden geleverd.

## Een voorinstelling voor afbeeldingen maken {#creating-an-image-preset}

U kunt uw eigen Voorinstellingen van het Beeld creëren als u een Beheerder van het Bedrijf bent. U kunt voorinstellingen voor afbeeldingen maken of beginnen met een standaardvoorinstelling voor afbeeldingen die door Adobe Dynamic Media Classic wordt verschaft, deze bewerken en opslaan onder een andere naam.

**om een Vooraf ingesteld Beeld tot stand te brengen:**

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** .

   U kunt naar de naam van een voorinstelling voor afbeeldingen op dit scherm bladeren om een voorvertoning van een bestaande voorinstelling voor afbeeldingen weer te geven. Als u een naam selecteert voor een voorinstelling voor afbeelding, wijzigt de grootte en de weergave van de voorbeeldafbeelding in het voorvertoningsvenster.

1. Voer een van de volgende handelingen uit:

   * **creeer een Vooraf ingesteld Beeld**: Selecteer **[!UICONTROL Add]**.
   * **geef een Beeld uit vooraf ingesteld**: doorblader aan het Beeld vooraf ingesteld dat het meest als is u wilt creëren en dan selecteren **[!UICONTROL Edit]**.

1. Voer een naam in voor de voorinstelling voor afbeelding.
1. Voer afmetingen voor de breedte en hoogte in pixels in. Deze metingen bepalen de grootte waarop de beelden worden geleverd.
1. Vul het scherm Voorinstelling toevoegen of Voorinstelling bewerken in. Voor details, zie [ Vooraf ingestelde het Beeld opties ](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic raadt de volgende opties voor &#39;best practices&#39; aan om te beginnen:

   * **[!UICONTROL Format]**: kies JPEG of een andere indeling die aan uw vereisten voldoet. Alle webbrowsers ondersteunen de JPEG-afbeeldingsindeling. Deze indeling biedt een goede balans tussen kleine bestandsgrootten en afbeeldingskwaliteit. JPEG-afbeeldingen gebruiken echter een compressieschema met gegevensverlies dat ongewenste afbeeldingsartefacten kan veroorzaken als de compressie-instelling te laag is. Daarom raadt Adobe Dynamic Media Classic aan de compressiekwaliteit (op de schuifregelaar) in te stellen op 75. Deze instelling biedt een goede balans tussen afbeeldingskwaliteit en kleine bestandsgrootte.

   * **[!UICONTROL Sharpening]**: selecteer Verscherpen niet (dit verscherpingsfilter biedt minder controle dan **[!UICONTROL Unsharp Masking]** -instellingen).

   * **[!UICONTROL Resample Mode]**: kies **[!UICONTROL Bi-Cubic]** .

   * **[!UICONTROL Unsharp Masking]** (USM): voer de volgende instellingen in:

   | Type voorinstelling | Grootte | USM: hoeveelheid | USM: Straal | USM: Drempel |
   | --- | --- | --- | --- | --- |
   | Cross-Sell (miniatuur) | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniatuur | 150 × 150 | 1,1 | 1 | 5 |
   | Hoofd | 350 × 350 | 1 | 1 | 6 |
   | Vergroten | 500 × 500 | 1,2 | 1,2 | 5 |

1. Selecteer **[!UICONTROL Save]** .

De Adobe Dynamic Media Classic-opties voor &#39;aanbevolen procedures&#39; voor het maken van voorinstellingen voor afbeeldingen in deze lijst zijn algemene aanbevelingen. Verscherpen is zeer subjectief. Deze &quot;beste praktijken&quot;montages waren gebaseerd op een 2000 × 2000 primaire beeld; de montages voor grotere of kleinere primaire dossiers kunnen verschillend zijn. Adobe Dynamic Media Classic raadt het volgende bereik aan als u de instellingen voor Onscherp masker wilt aanpassen:

* **[!UICONTROL Amount]** : tussen `.8` en `1.5` .

* **[!UICONTROL Radius]** : tussen `.6` en `2` .

* **[!UICONTROL Threshold]**: van `1` tot en met `6` .

Als u een voorinstelling voor een afbeelding wilt verwijderen, selecteert u deze in het scherm Voorinstellingen afbeelding en selecteert u vervolgens **[!UICONTROL Delete]** .

>[!MORELIKETHIS]
>
>* [ creeer en geef Beeld uit vooraf instelt ](application-setup.md#creating_and_editing_image_presets)
>* [ Vooraf ingestelde Beeld opties ](application-setup.md#image_preset_options)
>* [ Voorproef een beeldactiva die op zijn Vooraf ingesteld Beeld wordt gebaseerd ](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
