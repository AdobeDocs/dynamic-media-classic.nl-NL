---
title: Elementen exporteren uit Adobe Dynamic Media Classic
description: Leer hoe u middelen uit Adobe Dynamic Media Classic exporteert.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Elementen exporteren uit Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

U kunt elementen die u in Adobe Dynamic Media Classic hebt bewerkt, opslaan op een lokaal netwerkstation. Geëxporteerde elementen worden in een ZIP-bestand gebundeld, zodat ze via e-mail kunnen worden gedownload of verzonden.

Het gecomprimeerde ZIP-bestand heeft een maximale bestandsgrootte van 1 GB voor de exporttaak. Bovendien kunt u maximaal 500 elementen per exporttaak gebruiken.

Adobe Dynamic Media Classic houdt een overzicht bij van het exporteren van taken in het scherm Taken.

**Elementen exporteren uit Adobe Dynamic Media Classic:**

1. Selecteer de elementen die u wilt exporteren en ga naar **[!UICONTROL File]** > **[!UICONTROL Export]**.
1. Klik in het venster Geselecteerde elementen exporteren op **[!UICONTROL Image Options]** en geef vervolgens een of meer van de volgende opties op (beheerders bepalen welke opties beschikbaar zijn voor hun gebruikers):

   * **[!UICONTROL Presets]**: Kies desgewenst een voorinstelling voor afbeelding om het element op te maken wanneer u het exporteert. Als u een voorinstelling voor afbeeldingen kiest, zijn de andere opmaakopties niet beschikbaar omdat het element gebruikmaakt van de indelingen die zijn gedefinieerd in de voorinstelling voor afbeeldingen.

   * **[!UICONTROL Conversion]**: Zet het elementbestand of de oorspronkelijke afbeelding om.

   * **[!UICONTROL Size]**: U kunt een standaardgrootte selecteren. U kunt ook **[!UICONTROL Other]** van de **[!UICONTROL Size]** kiest u de gewenste maateenheid en geeft u vervolgens de breedte en de hoogte op.

     Zie ook [Beschikbare exportopties voor gebruikers van Media Portal opgeven](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Format]**: Kies een afbeeldingsindeling.

   * **[!UICONTROL Color]**: Kies RGB, CMYK of Grijs.

   * **[!UICONTROL Resolution]**: Kies 72 ppi, 150 ppi of 300 ppi.

   * **[!UICONTROL Job Name]**: U kunt een taaknaam aan het exporteren toewijzen.

   * **[!UICONTROL Send Email To]**: Optioneel. Voer een e-mailadres in als u de middelen per e-mail wilt verzenden. In het e-mailbericht wordt de URL weergegeven waar de ontvanger de elementen kan downloaden.

1. Selecteren **[!UICONTROL Export]**.

Er worden drie basisuitvoeracties ondersteund:

* Origineel bestand (het oorspronkelijke bestand voor het element exporteren)
* Omzetten met voorinstelling (gebruik een voorinstelling voor afbeelding om het element op te maken)
* Omzetten zonder voorinstelling (gebruik het dialoogvenster Exporteren om afbeeldingsopties op te geven)

De volgende elementtypen kunnen niet worden geëxporteerd. Alle andere genereren een exportbewerking.

* Afbeeldingssets
* Rendersets
* Sets draaien
* Mediasets
* Multibitsnelheidsets
* eCatalogs

Bovendien kunnen sjablonen niet worden geëxporteerd als een &quot;oorspronkelijk bestand&quot;.

Met conversie kunt u de volgende elementtypen exporteren:

* Afbeeldingen
* Sjablonen
* Aangepaste afbeeldingen
* PDF (geconverteerde pagina&#39;s worden gegenereerd)
* PostScript®

Het volgende gedrag treedt op wanneer een grote selectie van verschillende soorten activa in de exporter wordt ingevoerd:

* Alle elementtypen die niet kunnen worden geëxporteerd, worden uit de lijst verwijderd voordat de taak wordt verzonden
* Als een conversie wordt aangevraagd, worden alle typen die kunnen worden omgezet, geëxporteerd als origineel
