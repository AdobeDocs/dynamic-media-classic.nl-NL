---
title: Bijschriften toevoegen aan video
description: Leer hoe u bijschriften aan video toevoegt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 1%

---

# Bijschriften toevoegen aan video {#adding-captions-to-video}

U kunt het bereik van uw video&#39;s uitbreiden naar wereldwijde markten door ondertiteling toe te voegen aan enkele video&#39;s of aan Adaptive Video Sets. Door ondertiteling toe te voegen vermijdt u de noodzaak om de audio te dupliceren, of de behoefte om inheemse sprekers te gebruiken om de audio voor elke verschillende taal opnieuw op te nemen. De video wordt afgespeeld in de taal waarin deze is opgenomen. Er verschijnen ondertitels in vreemde talen, zodat mensen in verschillende talen het audiogedeelte nog steeds kunnen begrijpen.

Ondertiteling maakt ook een betere toegankelijkheid mogelijk door ondertiteling te gebruiken voor doven of slechthorenden.

>[!NOTE]
>
>De gebruikte videospeler moet de weergave van bijschriften ondersteunen.

U configureert het effect Bijschrift en bewerkt het menu Bijschrift zelf, inclusief de menutekst voor een van de volgende gebruikers:

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` viewer
* `Universal_HTML5_MixedMedia_light` viewer

Zie [Een voorinstelling voor een videoviewer toevoegen of bewerken](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Zie ook [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic kan bijschriftbestanden omzetten in de indeling JSON (JavaScript Object Notation). Met deze conversie kunt u de JSON-tekst insluiten in een webpagina als een verborgen, maar volledige transcriptie van de video. Zoekprogramma&#39;s kunnen dan door de inhoud kruipen en deze indexeren, zodat de video&#39;s gemakkelijker te vinden zijn en klanten meer informatie krijgen over de video-inhoud.

Zie [Statische (niet-grafische) inhoud serveren](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) in de *Adobe Image Serving API Help* voor meer informatie over het gebruik van de functie JSON in een URL.

**Bijschriften toevoegen aan video:**

1. Maak uw videobijschriftbestand met een externe toepassing buiten Adobe Dynamic Media Classic op basis van het viewertype dat u gebruikt.

   | Type viewer | Ondertitelingsbestand |
   |--- |--- |
   | HTML5 | Als u een HTML5-videoviewer gebruikt, moet u ervoor zorgen dat het bijschriftbestand dat u maakt, voldoet aan de WebVTT-standaard (Web Video Text Tracks). De bestandsnaamextensie voor ondertiteling is .vtt. U kunt meer informatie over de WebVTT ondertitelingsnorm leren.<br><br>[Zie WebVTT](https://w3c.github.io/webvtt/): De indeling Webvideoteksttracks. <br><br>Er zijn zowel gratis als tegen betaling voor gereedschappen en services die u kunt gebruiken voor het maken van bijschriftbestanden buiten Adobe Dynamic Media Classic. Als u bijvoorbeeld een eenvoudig videobijschriftbestand zonder opmaak wilt maken, kunt u de volgende gratis gereedschappen voor het maken en bewerken van bijschriften gebruiken: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>U bereikt het beste resultaat met het gereedschap in Internet Explorer 9 of hoger, Google Chrome of Safari. <br><br>In het hulpmiddel, in <b>URL van videobestand invoeren</b> veld, plakt u de URL van het videobestand en selecteert u <b>Laden</b>. <br><br>Als u bijvoorbeeld een Adobe Dynamic Media Classic-URL voor uw videobestand gebruikt, dubbelklikt u op een afzonderlijk video-element (geen adaptieve videoset of primaire video) om deze te openen in de gedetailleerde weergave. Vouw URL&#39;s uit en sluit code in in het rechterdeelvenster van de detailweergave. Selecteer vervolgens onder de groep Mobiele apparaten, rechts van Mobiel (progressief) <b>URL kopiëren</b>. Dit proces geeft u URL aan het videodossier zelf dat u dan in het <b>URL van videobestand invoeren</b> veld. Internet Explorer, Chrome of Safari kunnen de video vervolgens op een native manier afspelen. Volg nu de aanwijzingen op het scherm van de site om het WebVTT-bestand te ontwerpen en op te slaan. Wanneer u klaar bent, kopieert u de inhoud van het bijschriftbestand en plakt u deze in een teksteditor zonder opmaak en slaat u het bestand op met de bestandsnaamextensie VTT. <br><br><b>Opmerking:</b> Voor algemene ondersteuning van videobijschriften in andere talen dan het Engels, vereist de WebVTT-standaard dat u afzonderlijke .vtt-bestanden maakt en dat u elke taal die u wilt ondersteunen, aanroept. <br><br>Over het algemeen wilt u het VTT-bestand van het bijschrift dezelfde naam geven als het videobestand en dit bestand toevoegen met bijschriften. Hierdoor kunt u het genereren van video-URL&#39;s automatiseren met behulp van uw bestaande systeem voor webcontentbeheer. |

1. Upload in Adobe Dynamic Media Classic uw WebVTT-, DFXP- of SMPTE XML-bijschriftbestand.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die het videobestand bevat dat u wilt koppelen aan het bijschriftbestand dat u hebt geüpload.
1. Selecteer in het deelvenster Asset Browse één video-element en selecteer vervolgens onder de miniatuurafbeelding van het element de optie **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Zoek in de tabel Viewer List naar de HTML5-viewer met de naam **Univeral_HTML5_Video**, **Universal_HTML5_GemengdMedia_donker**, of **Universal_HTML5_MixedMedia_light** Voer vervolgens een van de volgende handelingen uit:

   * Voor een pop-upviewerervaring voor video selecteert u **[!UICONTROL Copy URL]** helemaal rechts van de naam.

      Voeg de gekopieerde URL van de video toe aan de volgende syntaxis, zodat u deze kunt koppelen aan de gekopieerde URL naar het bijschriftbestand:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Noteer de `,1` aan het einde van het pad voor de bijschrift-URL. Onmiddellijk na de VTT-bestandsnaamextensie in het pad kunt u de knop voor een gesloten bijschrift op de videospelerbalk desgewenst in- of uitschakelen door in te stellen op `1` of `0`, respectievelijk.

   * Voor een ingesloten videoviewerervaring selecteert u **[!UICONTROL Embed Code]** helemaal rechts van de naam.

      Selecteer in het dialoogvenster Code insluiten de optie **[!UICONTROL Copy to Clipboard]**.

      Voor de HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, of `Universal_HTML5_MixedMedia_light` viewers, voegt u de gekopieerde insluitcode als volgt toe:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Noteer de `,1` aan het einde van het URL-pad. Onmiddellijk na de VTT-bestandsnaamextensie in het URL-pad kunt u de bijschriftknop op de videospelerbalk desgewenst in- of uitschakelen door in te stellen op `1` of `0`, respectievelijk.
