---
title: Bijschriften toevoegen aan video
description: Leer hoe u bijschriften aan video toevoegt in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Bijschriften toevoegen aan video {#add-captions-to-video}

Vergroot het bereik van uw video&#39;s tot wereldwijde markten. U kunt dit doen door ondertiteling toe te voegen aan enkele video&#39;s of Adaptieve videosets. Door ondertiteling toe te voegen vermijdt u de noodzaak om de audio te dupliceren, of de behoefte om inheemse sprekers te gebruiken om de audio voor elke verschillende taal opnieuw op te nemen. De video wordt afgespeeld in de taal waarin deze is opgenomen. Er verschijnen ondertitels in vreemde talen, zodat mensen in verschillende talen het audiogedeelte nog steeds kunnen begrijpen.

Ondertiteling maakt ook een betere toegankelijkheid mogelijk door ondertiteling te gebruiken voor doven of slechthorenden.

>[!NOTE]
>
>De gebruikte videospeler moet de weergave van bijschriften ondersteunen.

U configureert het effect Bijschrift en bewerkt het menu Bijschrift zelf, inclusief de menutekst voor een van de volgende gebruikers:

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` viewer
* `Universal_HTML5_MixedMedia_light` viewer

Zie [Een voorinstelling voor een video-viewer toevoegen of bewerken](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Zie ook [Viewer-voorinstellingen toevoegen en bewerken](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic kan bijschriftbestanden omzetten in de indeling JSON (JavaScript Object Notation). Deze conversie betekent dat u de JSON-tekst kunt insluiten in een webpagina als een verborgen, maar volledige transcriptie van de video. Zoekprogramma&#39;s kunnen dan door de inhoud kruipen en deze indexeren, zodat de video&#39;s gemakkelijker te vinden zijn en klanten meer informatie krijgen over de video-inhoud.

Zie [Statische (niet-grafische) inhoud serveren](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) voor meer informatie over het gebruik van de JSON-functie in een URL.

**Bijschriften toevoegen aan een video:**

1. Maak uw videobijschriftbestand met een externe toepassing buiten Adobe Dynamic Media Classic op basis van het viewertype dat u gebruikt.

   | Type viewer | Ondertitelingsbestand |
   |--- |--- |
   | HTML 5 | Als u een HTML5-videoviewer gebruikt, moet u ervoor zorgen dat het bijschriftbestand dat u maakt, voldoet aan de WebVTT-standaard (Web Video Text Tracks). De bestandsnaamextensie van de ondertiteling is `.VTT`. U kunt meer informatie over de WebVTT ondertitelingsnorm leren.<br><br>[Zie WebVTT](https://w3c.github.io/webvtt/): De indeling Webvideoteksttracks. <br><br>Er zijn vele websites die zowel gratis als op vergoeding gebaseerde hulpmiddelen en de diensten aanbieden die u aan auteurWebVTT titeldossiers kunt gebruiken. <br><br>Volg de aanwijzingen op het scherm van een site om het WebVTT-bestand te ontwerpen en op te slaan. Wanneer u klaar bent, kopieert u de inhoud van het bijschriftbestand en plakt u deze in een teksteditor zonder opmaak en slaat u het bestand op met de bestandsnaamextensie VTT. <br><br><b>Opmerking:</b> Voor algemene ondersteuning van videobijschriften in andere talen dan Engels, is het vereist dat u voor de WebVTT-standaard een aparte `.VTT` bestanden en oproepen voor elke taal die u wilt ondersteunen. <br><br>Over het algemeen wilt u het VTT-bestand van het bijschrift dezelfde naam geven als het videobestand en dit bestand toevoegen met bijschriften. Hierdoor kunt u de generatie van de video-URL&#39;s automatiseren met behulp van uw bestaande systeem voor webcontentbeheer. |

1. Upload in Adobe Dynamic Media Classic uw WebVTT-, DFXP- of SMPTE XML-bijschriftbestand.

   Zie [Bestanden uploaden](uploading-files.md#uploading_files).

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die het videobestand bevat dat u wilt koppelen aan het bijschriftbestand dat u hebt geüpload.
1. Selecteer in het deelvenster Asset Browse één video-element en selecteer vervolgens onder de miniatuurafbeelding van het element **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Zoek in de tabel Viewer List naar de HTML5-viewer met de naam **Univeral_HTML5_Video**, **Universal_HTML5_GemengdMedia_donker**, of **Universal_HTML5_MixedMedia_light** Voer vervolgens een van de volgende handelingen uit:

   * Voor een pop-upviewerervaring voor video selecteert u **[!UICONTROL Copy URL]** helemaal rechts van de naam.

     Voeg de gekopieerde URL van de video toe aan de volgende syntaxis, zodat u deze kunt koppelen aan de gekopieerde URL naar het bijschriftbestand:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Noteer de `,1` aan het einde van het pad voor de bijschrift-URL. Onmiddellijk na de VTT-bestandsnaamextensie in het pad kunt u de knop voor een gesloten bijschrift op de videospelerbalk desgewenst in- of uitschakelen door in te stellen op `1` of `0`, respectievelijk.

   * Voor een ingesloten videoviewerervaring selecteert u **[!UICONTROL Embed Code]** helemaal rechts van de naam.

     Selecteer in het dialoogvenster Code insluiten **[!UICONTROL Copy to Clipboard]**.

     Voor de HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, of `Universal_HTML5_MixedMedia_light` Viewers, voeg de gekopieerde Insluitcode als volgt toe:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Noteer de `,1` aan het einde van het URL-pad. Onmiddellijk na de VTT-bestandsnaamextensie in het URL-pad kunt u de bijschriftknop op de videospelerbalk desgewenst in- of uitschakelen door in te stellen op `1` of `0`, respectievelijk.
