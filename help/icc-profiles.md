---
title: ICC-profielen
seo-title: ICC-profielen
description: 'null'
seo-description: Meer informatie over ICC-profielen.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC-profielen{#icc-profiles}

Een ICC-profiel (International Color Consortium) is een bestand waarin wordt beschreven hoe afbeeldingsbestanden correct moeten worden omgezet van de ene kleurruimte naar de andere. Met ICC-profielen kunt u de juiste kleuren voor uw afbeeldingen verkrijgen. Als u bijvoorbeeld afbeeldingen die zijn ontworpen om op een computerscherm te worden afgedrukt, correct wilt weergeven, kunt u een ICC-profiel kiezen. Dit profiel zet de afbeelding om in een andere kleurruimte en zorgt ervoor dat de kleuren online correct worden weergegeven.

In het het Publiceren Scene7 Systeem, kunt u een ICC profiel kiezen om beelden in een verschillende kleurenruimte om te zetten wanneer u de beelden uploadt. Alle standaard Photoshop ICC-profielen zijn standaard beschikbaar in SPS. Selecteer het menu Kleurprofiel om de namen van kleurprofielen weer te geven in het scherm Uploaden. Kies vervolgens Aangepast van > Naar en kies een ICC-profielnaam in de menu&#39;s Omgezet van en Omgezet naar. Zie Opties voor het bewerken van [afbeeldingen tijdens het uploaden](image-editing-options-upload.md#image-editing-options-at-upload).

U kunt niet alleen de standaard-ICC-profielen gebruiken, maar u kunt ook andere ICC-profielen uploaden naar SPS en deze beschikbaar maken voor kleurruimteconversie. Schakel over naar de gedetailleerde weergave in het deelvenster Bladeren om de profielklasse, het type kleurruimte en het PCS-type van een ICC-profiel te onderzoeken.

## ICC-profielen uploaden {#uploading-icc-profiles}

U kunt ICC-profielen uploaden met dezelfde technieken als waarmee u bestanden uploadt. U kunt ICC-profielen opslaan in elke map SPS. Zie [Uw bestanden](uploading-files.md#uploading_your_files)uploaden.

## Een ICC-profiel controleren {#examining-an-icc-profile}

Als u een ICC-profiel wilt onderzoeken, selecteert u het in het deelvenster Bladeren en geeft u het weer in de gedetailleerde weergave. In de gedetailleerde weergave wordt deze informatie over ICC-profielen weergegeven:

**Profielklasse** Het ICC (International Color Consortium) definieert elke klasse voor een type toepassing. Invoerprofielen zijn bijvoorbeeld van toepassing op apparaten zoals digitale camera&#39;s en scanners en op printers.

**Type** kleurruimte Dit getal is de &#39;invoer&#39;-kleurruimte van het profiel, zoals gedefinieerd door de ICC. Het type kleurruimte definieert het aantal componenten van de kleurruimte en de interpretatie van deze componenten. RGB is bijvoorbeeld een kleurruimte met drie componenten: rood, groen en blauw. Het type kleurruimte definieert de specifieke kleurkenmerken van de ruimte niet (bijvoorbeeld de kleurafbeeldingen van de primaire kleuren).

**PCS-type** Dit PCS-type is de &#39;uitvoer&#39;-kleurruimte van het profiel, de profielverbindingsruimte. Een kleurprofiel kan bijvoorbeeld RGB omzetten in een PCS, dat het vervolgens omzet in CMYK.

Voor invoer-, weergave- of uitvoerprofielen die nuttig zijn voor het labelen van kleuren of afbeeldingen, is het PCS-type XYZ of Lab. Interpreteer dit profiel als de overeenkomstige specifieke kleurruimte die is gedefinieerd in de ICC-specificatie.
