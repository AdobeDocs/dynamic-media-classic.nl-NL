---
title: Elementen exporteren vanuit Dynamic Media Classic
seo-title: Elementen exporteren vanuit Dynamic Media Classic
description: 'null'
seo-description: Leer hoe u elementen exporteert uit Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Elementen exporteren vanuit Dynamic Media Classic{#exporting-assets-from-dmc}

U kunt elementen die u in Dynamic Media Classic hebt bewerkt, opslaan op een lokaal netwerkstation. Geëxporteerde elementen worden in een ZIP-bestand gebundeld, zodat ze via e-mail kunnen worden gedownload of verzonden.

Het gecomprimeerde ZIP-bestand heeft een maximale bestandsgrootte van 1 GB voor de exporttaak. Houd er ook rekening mee dat u maximaal 500 totale middelen per exporttaak hebt.

Dynamic Media Classic houdt een overzicht van exporttaken bij in het scherm Taken.

**Elementen exporteren uit Dynamic Media Klassiek**

1. Selecteer de elementen die u wilt exporteren en klik op **Bestand** > **Exporteren**.
1. Klik in het venster Geselecteerde elementen exporteren op **Afbeeldingsopties** en geef een of meer van de volgende opties op (beheerders bepalen welke opties beschikbaar zijn voor hun gebruikers):

   * **Voorinstellingen** Optioneel. Kies een voorinstelling voor afbeelding om het element op te maken wanneer u het exporteert. Als u een voorinstelling voor afbeeldingen kiest, zijn de andere opmaakopties niet beschikbaar omdat het element gebruikmaakt van de indelingen die zijn gedefinieerd in de voorinstelling voor afbeeldingen.

   * **Conversie** Zet het elementbestand of de oorspronkelijke afbeelding om.

   * **Grootte** U kunt een standaardgrootte selecteren. U kunt ook op Overige klikken in de vervolgkeuzelijst Grootte, de gewenste maateenheid kiezen en vervolgens de breedte en hoogte opgeven.

      Zie ook Exportopties [opgeven die beschikbaar zijn voor gebruikers](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)van Media Portal.

   * **Indeling** Kies een afbeeldingsindeling.

   * **Kleur** Kies RGB, CMYK of Grijs.

   * **Resolutie**: kies 72, 150 of 300 ppi.

   * **Taaknaam** U kunt een taaknaam aan het exporteren toewijzen.

   * **Voer** eventueel een e-mailadres in om de elementen via e-mail te verzenden. Het e-mailbericht bevat de URL waar de ontvanger de elementen kan downloaden.

1. Klik op **Exporteren**.

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

