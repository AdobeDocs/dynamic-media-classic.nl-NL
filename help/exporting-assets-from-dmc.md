---
title: Elementen exporteren uit Adobe Dynamic Media Classic
description: Leer hoe u elementen exporteert van Adobe Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Elementen exporteren uit Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

U kunt elementen die u hebt bewerkt in Adobe Dynamic Media Classic opslaan op een lokale netwerkschijf. Geëxporteerde elementen worden in een ZIP-bestand gebundeld, zodat ze via e-mail kunnen worden gedownload of verzonden.

Het gecomprimeerde ZIP-bestand heeft een maximale bestandsgrootte van 1 GB voor de exporttaak. Bovendien kunt u maximaal 500 elementen per exporttaak gebruiken.

Adobe Dynamic Media Classic houdt een overzicht bij van exporttaken in het scherm Taken.

**Elementen exporteren uit Adobe Dynamic Media Classic:**

1. Selecteer de elementen die u wilt exporteren en ga naar **[!UICONTROL File]** > **[!UICONTROL Export]**.
1. Klik in het venster Geselecteerde elementen exporteren op **[!UICONTROL Image Options]** en geef vervolgens een van de volgende opties op (beheerders bepalen welke opties beschikbaar zijn voor hun gebruikers):

   * **[!UICONTROL Presets]** - Kies desgewenst een voorinstelling voor afbeelding om het element op te maken wanneer u het exporteert. Als u een voorinstelling voor afbeeldingen kiest, zijn de andere opmaakopties niet beschikbaar omdat het element gebruikmaakt van de indelingen die zijn gedefinieerd in de voorinstelling voor afbeeldingen.

   * **[!UICONTROL Conversion]** - Zet het elementbestand of de oorspronkelijke afbeelding om.

   * **[!UICONTROL Size]** - U kunt een standaardgrootte selecteren. U kunt ook **[!UICONTROL Other]** selecteren in de vervolgkeuzelijst **[!UICONTROL Size]**, de gewenste maateenheid kiezen en vervolgens de breedte en hoogte opgeven.

      Zie ook [Exportopties opgeven die beschikbaar zijn voor gebruikers van Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Format]** - Kies een afbeeldingsindeling.

   * **[!UICONTROL Color]** - Kies RGB, CMYK of Grijs.

   * **[!UICONTROL Resolution]** - Kies 72 ppi, 150 ppi of 300 ppi.

   * **[!UICONTROL Job Name]** - U kunt een taaknaam aan het exporteren toewijzen.

   * **[!UICONTROL Send Email To]** - U kunt desgewenst een e-mailadres invoeren als u de middelen per e-mail wilt verzenden. Het e-mailbericht bevat de URL waar de ontvanger de elementen kan downloaden.

1. Selecteer **[!UICONTROL Export]**.

Er worden drie basisuitvoeracties ondersteund:

* Origineel bestand (het oorspronkelijke bestand voor het element exporteren)
* Omzetten met voorinstelling (gebruik een voorinstelling voor afbeeldingen om het element op te maken)
* Omzetten zonder voorinstelling (gebruik het dialoogvenster Exporteren om afbeeldingsopties op te geven)

De volgende elementtypen kunnen niet worden geëxporteerd. Alle andere genereren een exportbewerking.

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
* PDF (geconverteerde pagina&#39;s worden gegenereerd)
* PostScript®

Het volgende gedrag treedt op wanneer een groot aantal verschillende soorten activa in de exporter worden ingevoerd:

* Alle elementtypen die niet kunnen worden geëxporteerd, worden uit de lijst verwijderd voordat de taak wordt verzonden
* Als een conversie wordt aangevraagd, worden alle typen die kunnen worden omgezet, geëxporteerd als origineel
