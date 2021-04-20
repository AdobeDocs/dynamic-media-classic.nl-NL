---
title: Elementen exporteren vanuit Dynamic Media Classic
description: Leer hoe u elementen exporteert van Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Elementen exporteren uit Dynamic Media Classic{#exporting-assets-from-dmc}

U kunt elementen die u in Dynamic Media Classic hebt bewerkt, opslaan op een lokaal netwerkstation. Geëxporteerde elementen worden in een ZIP-bestand gebundeld, zodat ze via e-mail kunnen worden gedownload of verzonden.

Het gecomprimeerde ZIP-bestand heeft een maximale bestandsgrootte van 1 GB voor de exporttaak. Houd er ook rekening mee dat u maximaal 500 totale middelen per exporttaak hebt.

Dynamic Media Classic houdt een overzicht van exporttaken bij in het scherm Taken.

**Elementen exporteren uit Dynamic Media Classic**

1. Selecteer de elementen die u wilt exporteren en klik op **Bestand** > **Exporteren**.
1. Klik in het venster Geselecteerde elementen exporteren op **Afbeeldingsopties** en geef vervolgens een van de volgende opties op (beheerders bepalen welke opties beschikbaar zijn voor hun gebruikers):

   * ****
VoorinstellingenOptioneel kiest u een voorinstelling voor afbeelding om het element op te maken wanneer u het exporteert. Als u een voorinstelling voor afbeeldingen kiest, zijn de andere opmaakopties niet beschikbaar omdat het element gebruikmaakt van de indelingen die zijn gedefinieerd in de voorinstelling voor afbeeldingen.

   * ****
ConversionConverteer het elementbestand of de oorspronkelijke afbeelding.

   * ****
GrootteU kunt een standaardgrootte selecteren. U kunt ook op Overige klikken in de vervolgkeuzelijst Grootte, de gewenste maateenheid kiezen en vervolgens de breedte en hoogte opgeven.

      Zie ook [Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * ****
IndelingKies een afbeeldingsindeling.

   * ****
KleurKies RGB, CMYK of Grijs.

   * ****
ResolutieKies 72, 150 of 300 ppi.

   * **Taaknaam**
U kunt een taaknaam aan het exporteren toewijzen.

   * **U kunt**
desgewenst een e-mailadres verzenden om de elementen per e-mail te verzenden. Het e-mailbericht bevat de URL waar de ontvanger de elementen kan downloaden.

1. Klik **Exporteren**.

Er worden drie basisuitvoeracties ondersteund:

* Origineel bestand (het oorspronkelijke bestand voor het element exporteren)
* Omzetten met voorinstelling (gebruik een voorinstelling voor afbeeldingen om het element op te maken)
* Omzetten zonder voorinstelling (gebruik het dialoogvenster Exporteren om afbeeldingsopties op te geven)

De volgende elementtypen kunnen niet worden geëxporteerd. Alle anderen moeten een exportbewerking genereren.

* Afbeeldingsets
* Rendersets
* Sets draaien
* Mediasets
* Sets met meerdere bitsnelheden
* eCatalogs

Bovendien kunnen sjablonen niet worden geëxporteerd als een &quot;oorspronkelijk bestand&quot;.

Met conversie kunt u de volgende elementtypen exporteren:

* Afbeeldingen
* Sjablonen
* Aangepaste afbeeldingen
* PDF (converteerde pagina&#39;s worden gegenereerd)
* PostScript

Het volgende gedrag treedt op wanneer een groot aantal verschillende soorten activa in de exporter worden ingevoerd:

* Alle elementtypen die niet kunnen worden geëxporteerd, worden uit de lijst verwijderd voordat de taak wordt verzonden
* Als een conversie wordt aangevraagd, worden alle typen die kunnen worden omgezet, geëxporteerd als origineel

