---
title: Bijschriften toevoegen aan video
seo-title: Bijschriften toevoegen aan video
description: 'null'
seo-description: Leer hoe u bijschriften aan video kunt toevoegen
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
translation-type: tm+mt
source-git-commit: 74238f90f45f0fb9a4566915a20a1d41dfb69fe1
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---


# Bijschriften toevoegen aan video{#adding-captions-to-video}

U kunt het bereik van uw video&#39;s uitbreiden naar wereldwijde markten door ondertiteling toe te voegen aan enkele video&#39;s of aan Adaptive Video Sets. Door ondertiteling toe te voegen vermijdt u de noodzaak om de audio te dupliceren, of de behoefte om inheemse sprekers te gebruiken om de audio voor elke verschillende taal opnieuw op te nemen. De video wordt afgespeeld in de taal waarin deze is opgenomen. Er verschijnen ondertitels in vreemde talen, zodat mensen in verschillende talen het audiogedeelte nog steeds kunnen begrijpen.

Ondertiteling maakt ook een betere toegankelijkheid mogelijk door ondertiteling te gebruiken voor doven of slechthorenden.

>[!NOTE]
>
>De gebruikte videospeler moet de weergave van bijschriften ondersteunen.

Zie Een voorinstelling [voor een videoviewer](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) toevoegen of bewerken om het bijschrifteffect te configureren en het menu Bijschrift zelf te bewerken, inclusief de menutekst voor een van de volgende viewers:

* `Universal_HTML5_Video` viewer.
* `Universal_HTML5_MixedMedia_dark` viewer.
* `Universal_HTML5_MixedMedia_light` viewer.

Zie ook Voorinstellingen [voor viewers](application-setup.md#adding_and_editing_viewer_presets)toevoegen en bewerken.

Dynamic Media Classic kan bijschriftbestanden omzetten in de indeling JSON (JavaScript Object Notation). Met deze conversie kunt u de JSON-tekst insluiten in een webpagina als een verborgen, maar volledige transcriptie van de video. Zoekprogramma&#39;s kunnen de inhoud vervolgens verkennen en indexeren, zodat de video&#39;s gemakkelijker te vinden zijn en klanten meer informatie krijgen over de video-inhoud.

Zie [Statische (niet-afbeeldings) inhoud](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html) in de Help *van de* Adobe Image Serving API voor meer informatie over het gebruik van de JSON-functie in een URL.

**Bijschriften toevoegen aan video**

1. Gebruikend een derdetoepassing buiten het Publiceren Scene7 Systeem, creeer uw videobijschriftdossier dat op het viewertype wordt gebaseerd dat u gebruikt.

   | Type viewer | Ondertitelingsbestand |
   |--- |--- |
   | HTML5 | Als u een HTML5-videoviewer gebruikt, moet u ervoor zorgen dat het bijschriftbestand dat u maakt, voldoet aan de WebVTT-standaard (Web Video Text Tracks). De bestandsnaamextensie voor ondertiteling is .vtt. U kunt meer informatie over de WebVTT ondertitelingsnorm leren.<br><br>[Zie WebVTT](https://dev.w3.org/html5/webvtt/): De indeling Webvideoteksttracks. <br><br>Er zijn zowel vrij als betaald voor hulpmiddelen en de diensten die u aan auteursdossiers buiten het Publiceren Scene7 Systeem kunt gebruiken. Als u bijvoorbeeld een eenvoudig videobijschriftbestand zonder opmaak wilt maken, kunt u de volgende gratis gereedschappen voor het maken en bewerken van bijschriften gebruiken: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Voor de beste resultaten gebruikt u het gereedschap in Internet Explorer 9 of hoger, Google Chrome of Safari. <br><br>Plak in het veld URL van het videobestand <b></b> invoeren in het gereedschap de URL van het videobestand en klik vervolgens op <b>Laden</b>. <br><br>Als u bijvoorbeeld een Klassieke URL voor Dynamic Media voor uw videobestand gebruikt, dubbelklikt u in SPS op een afzonderlijk video-element (geen Adaptive Video Set of Master Video) om het te openen in de gedetailleerde weergave. Vouw URL&#39;s uit en sluit code in in het rechterdeelvenster van de detailweergave. Klik vervolgens onder de groep Mobiele apparaten rechts van Mobiel (progressief) op URL kopiëren. Dit proces geeft u URL aan het videodossier zelf dat u in <b>Enter URL van videodossier</b> kunt kleven. Internet Explorer, Chrome of Safari kunnen de video vervolgens op een native manier afspelen. Volg nu de aanwijzingen op het scherm van de site om het WebVTT-bestand te ontwerpen en op te slaan. Wanneer u klaar bent, kopieert u de inhoud van het bijschriftbestand en plakt u deze in een teksteditor zonder opmaak en slaat u het bestand op met de bestandsnaamextensie .vtt. <br><br><b>Opmerking:</b> Voor algemene ondersteuning van videobijschriften in andere talen dan het Engels, dient u er rekening mee te houden dat de WebVTT-standaard vereist dat u afzonderlijke .vtt-bestanden maakt en dat u elke taal die u wilt ondersteunen, aanroept. <br><br>Over het algemeen wilt u het VTT-bestand van het bijschrift dezelfde naam geven als het videobestand en dit bestand toevoegen met bijschriften. Hierdoor kunt u het genereren van video-URL&#39;s automatiseren met behulp van uw bestaande systeem voor webcontentbeheer. |

1. In het Publiceren Scene7 Systeem, upload uw WebVTT, DFXP, of SMPTE dossier van de titel van XML.

   Zie Bestanden [uploaden](uploading-files.md#uploading_files).

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die het videobestand bevat dat u wilt koppelen aan het bijschriftbestand dat u hebt geüpload.
1. Selecteer in het deelvenster Asset Browse één video-element en klik vervolgens onder de miniatuurafbeelding van het element op **Voorvertoning** > **Viewer List**.
1. Zoek in de Viewer List-tabel naar de HTML5-viewer **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_donker** of **Universal_HTML5_MixedMedia_light** en voer een van de volgende handelingen uit:

   * Voor een ervaring van de pop-up videokijker, klik **Exemplaar URL** aan uiterst rechts van de naam.

      Voeg de gekopieerde URL van de video toe aan de volgende syntaxis om deze te koppelen aan de gekopieerde URL naar het bijschriftbestand:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Noteer het `,1` aan het einde van het pad voor de bijschrift-URL. Direct na de bestandsnaamextensie .vtt in het pad kunt u de knop voor een gesloten bijschrift op de videospelerbalk in- of uitschakelen door respectievelijk in te stellen op `1` of `0`.

   * Voor een ingesloten videoviewerervaring klikt u op Code **** insluiten helemaal rechts van de naam.

      Klik in het dialoogvenster Code insluiten op **Kopiëren naar klembord**.

      Voeg voor de HTML5- `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`of `Universal_HTML5_MixedMedia_light` viewers de gekopieerde insluitcode als volgt toe:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Noteer het `,1` aan het einde van het URL-pad. Direct na de bestandsnaamextensie .vtt in het URL-pad kunt u de bijschriftknop op de videospelerbalk in- of uitschakelen door respectievelijk in te stellen op `1` of `0`.

