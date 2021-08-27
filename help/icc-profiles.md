---
title: ICC-profielen (International Color Consortium)
description: Meer informatie over ICC-profielen vindt u in Adobe Dynamic Media Classic.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# ICC-profielen{#icc-profiles}

Een ICC-profiel (International Color Consortium) is een bestand waarin wordt beschreven hoe afbeeldingsbestanden correct moeten worden omgezet van de ene kleurruimte naar de andere. Met ICC-profielen kunt u de juiste kleuren voor uw afbeeldingen verkrijgen. Als u bijvoorbeeld afbeeldingen die zijn ontworpen om op een computerscherm te worden afgedrukt, correct wilt weergeven, kunt u een ICC-profiel kiezen. Dit profiel zet de afbeelding om in een andere kleurruimte en zorgt ervoor dat de kleuren online correct worden weergegeven.

In Adobe Dynamic Media Classic kunt u een ICC-profiel kiezen om afbeeldingen om te zetten in een andere kleurruimte wanneer u de afbeeldingen uploadt. Alle standaard Photoshop ICC-profielen zijn standaard beschikbaar op Adobe Dynamic Media Classic. Selecteer het menu Kleurprofiel om de namen van kleurprofielen weer te geven in het scherm Uploaden. Kies vervolgens Aangepast van > Naar en kies een ICC-profielnaam in de menu&#39;s Omgezet van en Omgezet naar.

Zie [Opties voor het bewerken van afbeeldingen tijdens het uploaden](image-editing-options-upload.md#image-editing-options-at-upload).

Naast het gebruik van de standaard-ICC-profielen kunt u andere ICC-profielen uploaden naar Adobe Dynamic Media Classic en deze beschikbaar maken voor kleurruimteconversie. Schakel over naar de detailweergave in het deelvenster Bladeren om de profielklasse, het type kleurruimte en het PCS-type van een ICC-profiel te onderzoeken.

## ICC-profielen uploaden {#uploading-icc-profiles}

U kunt ICC-profielen uploaden met dezelfde technieken als waarmee u bestanden uploadt. ICC-profielen kunt u opslaan in elke Adobe Dynamic Media Classic-map.

Zie [Uw bestanden uploaden](uploading-files.md#uploading_your_files).

## Een ICC-profiel controleren {#examining-an-icc-profile}

Als u een ICC-profiel wilt onderzoeken, selecteert u het in het deelvenster Bladeren en geeft u het weer in de gedetailleerde weergave. In de gedetailleerde weergave wordt deze informatie over ICC-profielen weergegeven:

* **[!UICONTROL Profile Class]** - Het ICC (International Color Consortium) definieert elke klasse voor een type toepassing. Invoerprofielen zijn bijvoorbeeld van toepassing op apparaten zoals digitale camera&#39;s en scanners en op printers.

* **[!UICONTROL Color Space Type]** - Dit getal is de &#39;invoer&#39;-kleurruimte van het profiel, zoals gedefinieerd door de ICC. Het type kleurruimte definieert het aantal componenten van de kleurruimte en de interpretatie van deze componenten. RGB is bijvoorbeeld een kleurruimte met drie componenten: rood, groen en blauw. Het type kleurruimte definieert de specifieke kleurkenmerken van de ruimte niet (bijvoorbeeld de kleurafbeeldingen van de primaire kleuren).

* **[!UICONTROL PCS Type]** - Dit PCS-type is de &#39;uitvoer&#39;-kleurruimte van het profiel, de profielverbindingsruimte. Een kleurprofiel kan bijvoorbeeld RGB omzetten in een PCS, dat het vervolgens omzet in CMYK.

Voor invoer-, weergave- of uitvoerprofielen die nuttig zijn voor het labelen van kleuren of afbeeldingen, is het PCS-type XYZ of Lab. Interpreteer dit profiel als de overeenkomstige specifieke kleurruimte die is gedefinieerd in de ICC-specificatie.
