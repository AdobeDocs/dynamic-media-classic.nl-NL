---
title: Bijschriften toevoegen aan video
description: Leer hoe u bijschriften aan video kunt toevoegen
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
translation-type: tm+mt
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 1%

---

# Bijschriften toevoegen aan video{#adding-captions-to-video}

U kunt het bereik van uw video&#39;s uitbreiden naar wereldwijde markten door ondertiteling toe te voegen aan enkele video&#39;s of aan Adaptive Video Sets. Door ondertiteling toe te voegen vermijdt u de noodzaak om de audio te dupliceren, of de behoefte om inheemse sprekers te gebruiken om de audio voor elke verschillende taal opnieuw op te nemen. De video wordt afgespeeld in de taal waarin deze is opgenomen. Er verschijnen ondertitels in vreemde talen, zodat mensen in verschillende talen het audiogedeelte nog steeds kunnen begrijpen.

Ondertiteling maakt ook een betere toegankelijkheid mogelijk door ondertiteling te gebruiken voor doven of slechthorenden.

>[!NOTE]
>
>De gebruikte videospeler moet de weergave van bijschriften ondersteunen.

U configureert het effect Bijschrift en bewerkt het menu Bijschrift zelf, inclusief de menutekst voor een van de volgende gebruikers:

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` viewer
* `Universal_HTML5_MixedMedia_light` viewer

zie [Een voorinstelling voor een videoviewer toevoegen of bewerken](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Zie ook [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).

Dynamic Media Classic kan bijschriftbestanden omzetten in de JSON-indeling (JavaScript™ Object Notation). Met deze conversie kunt u de JSON-tekst insluiten in een webpagina als een verborgen, maar volledige transcriptie van de video. Zoekprogramma&#39;s kunnen dan door de inhoud kruipen en deze indexeren, zodat de video&#39;s gemakkelijker te vinden zijn en klanten meer informatie krijgen over de video-inhoud.

Zie [Statische (niet-afbeeldings) inhoud](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) in *Adobe Image Serving API Help* voor meer informatie over het gebruik van de JSON-functie in een URL.

**Bijschriften toevoegen aan video**

1. Maak uw videobijschriftbestand met een externe toepassing buiten Dynamic Media Classic op basis van het viewertype dat u gebruikt.

   | Type viewer | Ondertitelingsbestand |
   |--- |--- |
   | HTML5 | Als u een HTML5-videoviewer gebruikt, moet u ervoor zorgen dat het bijschriftbestand dat u maakt, voldoet aan de WebVTT-standaard (Web Video Text Tracks). De bestandsnaamextensie voor ondertiteling is .vtt. U kunt meer informatie over de WebVTT ondertitelingsnorm leren.<br><br>[Zie WebVTT](https://w3c.github.io/webvtt/): De indeling Webvideoteksttracks. <br><br>Er zijn zowel gratis als tegen betaling voor gereedschappen en services die u kunt gebruiken voor het maken van bijschriftbestanden buiten Dynamic Media Classic. Als u bijvoorbeeld een eenvoudig videobijschriftbestand zonder opmaak wilt maken, kunt u de volgende gratis gereedschappen voor het maken en bewerken van bijschriften gebruiken: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Gebruik voor de beste resultaten het gereedschap in Internet Explorer 9 of hoger, Google Chrome of Safari. <br><br>Plak in het veld URL van het videobestand  <b>invoeren de URL van </b> het videobestand in het gereedschap en klik vervolgens op  <b>Laden</b>. <br><br>Als u bijvoorbeeld een klassieke Dynamic Media-URL voor uw videobestand gebruikt, dubbelklikt u op een afzonderlijk video-element (geen adaptieve videoset of een Master video) om deze te openen in de gedetailleerde weergave. Vouw URL&#39;s uit en sluit code in in het rechterdeelvenster van de detailweergave. Klik vervolgens onder de groep Mobiele apparaten rechts van Mobiel (progressief) op URL kopiëren. Dit proces geeft u URL aan het videodossier zelf dat u in <b>ga URL van videodossier</b> gebied dan kunt kleven. Internet Explorer, Chrome of Safari kunnen de video vervolgens op een native manier afspelen. Volg nu de aanwijzingen op het scherm van de site om het WebVTT-bestand te ontwerpen en op te slaan. Wanneer u klaar bent, kopieert u de inhoud van het bijschriftbestand en plakt u deze in een teksteditor zonder opmaak en slaat u het bestand op met de bestandsnaamextensie .vtt. <br><br><b>Opmerking:</b> voor wereldwijde ondersteuning van videobijschriften in andere talen dan Engels, vereist de WebVTT-standaard dat u afzonderlijke .vtt-bestanden maakt en aanroepen voor elke taal die u wilt ondersteunen. <br><br>Over het algemeen wilt u het VTT-bestand van het bijschrift dezelfde naam geven als het videobestand en dit bestand toevoegen met bijschriften. Hierdoor kunt u het genereren van video-URL&#39;s automatiseren met behulp van uw bestaande systeem voor webcontentbeheer. |

1. Upload in Dynamic Media Classic uw WebVTT-, DFXP- of SMPTE XML-bijschriftbestand.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die het videobestand bevat dat u wilt koppelen aan het bijschriftbestand dat u hebt geüpload.
1. Selecteer in het deelvenster Asset Browse één video-element en klik vervolgens onder de miniatuurafbeelding van het element op **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Zoek in de Viewer List-tabel naar de HTML5-viewer **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_donker** of **Universal_HTML5_MixedMedia_light** en voer een van de volgende handelingen uit:

   * Voor een ervaring van de pop-up videokijker, klik **[!UICONTROL Copy URL]** uiterst rechts van de naam.

      Voeg de gekopieerde URL van de video toe aan de volgende syntaxis om deze te koppelen aan de gekopieerde URL naar het bijschriftbestand:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Noteer `,1` aan het einde van het pad voor de bijschrift-URL. Direct na de bestandsnaamextensie .vtt in het pad kunt u optioneel de knop voor een gesloten bijschrift op de videospelerbalk in- of uitschakelen door respectievelijk `1` of `0` in te stellen.

   * Voor een ingesloten videoviewerervaring klikt u op **[!UICONTROL Embed Code]** helemaal rechts van de naam.

      Klik in het dialoogvenster Code insluiten op **[!UICONTROL Copy to Clipboard]**.

      Voeg voor de HTML5- `Universal_HTML5_Video`-, `Universal_HTML5_MixedMedia_dark`- of `Universal_HTML5_MixedMedia_light`-viewers de gekopieerde insluitcode als volgt toe:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Noteer `,1` aan het einde van het URL-pad. Direct na de bestandsnaamextensie .vtt in het URL-pad kunt u optioneel de bijschriftknop op de videospelerbalk in- of uitschakelen door respectievelijk `1` of `0` in te stellen.
