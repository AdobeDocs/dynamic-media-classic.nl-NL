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

Zie [ een VideoKijker toevoegen of uitgeven vooraf ingesteld ](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Zie ook [ vooraf instelt van de Kijker toevoegen en uitgeven ](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic kan bijschriftbestanden omzetten in de indeling JSON (JavaScript Object Notation). Deze conversie betekent dat u de JSON-tekst kunt insluiten in een webpagina als een verborgen, maar volledige transcriptie van de video. Zoekprogramma&#39;s kunnen dan door de inhoud kruipen en deze indexeren, zodat de video&#39;s gemakkelijker te vinden zijn en klanten meer informatie krijgen over de video-inhoud.

Zie [ statische (niet beeld) inhoud ](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) binnen voor meer informatie over het gebruiken van de functie JSON in een URL.

**om titels aan een video toe te voegen:**

1. Maak uw videobijschriftbestand met een externe toepassing buiten Adobe Dynamic Media Classic op basis van het viewertype dat u gebruikt.

   | Type viewer | Ondertitelingsbestand |
   |--- |--- |
   | HTML5 | Als u een HTML5-videoviewer gebruikt, moet u ervoor zorgen dat het bijschriftbestand dat u maakt, voldoet aan de WebVTT-standaard (Web Video Text Tracks). De bestandsnaamextensie voor ondertiteling is `.VTT` . U kunt meer informatie over de WebVTT ondertitelingsnorm leren.<br><br>[ zie WebVTT ](https://w3c.github.io/webvtt/): Het formaat van de Tracks van de Tekst van het Web Video. <br><br> er zijn vele websites die zowel vrije als op prijs-gebaseerde hulpmiddelen en de diensten aanbieden die u aan auteurWebVTT titeldossiers kunt gebruiken. <br><br> volg de instructies op het scherm van een plaats aan auteur en sla uw WebVTT- dossier op. Wanneer u klaar bent, kopieert u de inhoud van het bijschriftbestand en plakt u deze in een teksteditor zonder opmaak en slaat u het bestand op met de bestandsnaamextensie VTT. <br><br><b> Nota:</b> voor globale steun van videotitels in andere talen dan het Engels, vereist de norm WebVTT dat u afzonderlijke `.VTT` dossiers creeert en roept voor elke taal u wilt steunen. <br><br> over het algemeen, wilt u het dossier van de titelVTT de zelfde naam zoals het videodossier noemen, en het toevoegen met titels. Hierdoor kunt u de generatie van de video-URL&#39;s automatiseren met behulp van uw bestaande systeem voor webcontentbeheer. |

1. Upload in Adobe Dynamic Media Classic uw WebVTT-, DFXP- of SMPTE XML-bijschriftbestand.

   Zie [ dossiers ](uploading-files.md#uploading_files) uploaden.

1. Navigeer in het deelvenster Elementenbibliotheek aan de linkerkant naar de elementenmap die het videobestand bevat dat u wilt koppelen aan het bijschriftbestand dat u hebt geüpload.
1. Selecteer in het deelvenster Asset Browse één video-element en selecteer vervolgens onder de miniatuurafbeelding van het element **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** .
1. In de lijst van de Kijker, vind de HTML5 kijker genoemd **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_donker**, of **Universal_HTML5_MixedMedia_light**, dan één van het volgende doen:

   * Selecteer **[!UICONTROL Copy URL]** helemaal rechts van de naam voor een pop-upviewerbeleving.

     Voeg de gekopieerde URL van de video toe aan de volgende syntaxis, zodat u deze kunt koppelen aan de gekopieerde URL naar het bijschriftbestand:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Noteer de `,1` aan het einde van het pad voor de bijschrift-URL. Onmiddellijk na de VTT-bestandsnaamextensie in het pad kunt u optioneel de knop voor een gesloten bijschrift op de videospelerbalk in- of uitschakelen door in te stellen op respectievelijk `1` of `0` .

   * Voor een ingesloten videoviewerervaring selecteert u **[!UICONTROL Embed Code]** helemaal rechts van de naam.

     Selecteer **[!UICONTROL Copy to Clipboard]** in het dialoogvenster Code insluiten.

     Voor de HTML5 `Universal_HTML5_Video` -, `Universal_HTML5_MixedMedia_dark` - of `Universal_HTML5_MixedMedia_light` -viewers voegt u de gekopieerde Insluitcode als volgt toe:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Noteer de `,1` aan het einde van het URL-pad. Onmiddellijk na de VTT-bestandsnaamextensie in het URL-pad kunt u optioneel de bijschriftknop op de videospelerbalk in- of uitschakelen door in te stellen op respectievelijk `1` of `0` .
