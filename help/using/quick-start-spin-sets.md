---
title: "Snel starten: centrifuges"
description: Een inleiding en Snel starten om te draaien zodat u in Adobe Dynamic Media Classic snel aan de slag kunt.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Snel starten: centrifuges{#quick-start-spin-sets}

Een centrifugeerset simuleert de echte handeling waarbij een object wordt omgedraaid om het te onderzoeken. Met centrifuges kunt u items vanuit elke hoek bekijken en de belangrijkste visuele details vanuit elke hoek ophalen. Een centrifugeerset simuleert een kijkervaring van 360 graden. Adobe Dynamic Media Classic biedt eendimensionale centrifuges waarin gebruikers een item kunnen roteren en tweedimensionale centrifuges waarin gebruikers het item kunnen roteren en spiegelen. Bovendien kunnen gebruikers met een paar eenvoudige muisklikken in- en uitzoomen op een vrije vorm en een willekeurige weergave pannen. Op deze manier kunnen gebruikers een item vanuit een bepaald gezichtspunt nader onderzoeken.

![Afbeeldingen voor een Draaiset.](/help/using/assets/spin_set.png)

Draaisets accepteren ook afbeeldingen met hyperlinks. Een afbeelding met hyperlinks is een gebied in een afbeelding in de centrifugeset dat een deelvenster met rollover-tekst weergeeft. Wanneer de gebruiker een Kaart van het Beeld selecteert, wordt een actie van één of andere soort teweeggebracht. Een webpagina wordt bijvoorbeeld gestart zodat de gebruiker meer over een product kan leren. Als u een afbeelding met hyperlinks wilt aanwijzen in een Draaiset, verschijnt er een omtrek rond de Afbeeldingskaart zelf wanneer de gebruiker de muisaanwijzer erboven plaatst.

Zie [Afbeeldingen met hyperlinks maken](creating-image-maps.md).

Zie [Afbeeldings- en centrifuges: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) trainingsvideo.

Wanneer u een reeks van de Rotatie creeert, adviseert de Adobe de volgende beste praktijken en handhaaft de volgende grenzen:

| Limiettype voor centrifugeren instellen | Beste praktijken | Oplegde limiet |
| --- | --- | --- |
| Maximumaantal rijen/kolommen per 2D-set | 12-18 afbeeldingen per set | 1000 |

Zie ook [Dynamic Media-beperkingen](/help/using/limitations.md).

Deze centrifuges zijn ontworpen om snel aan de slag te gaan met centrifuge-technieken in Adobe Dynamic Media Classic. Voer stap 1 tot en met 7 uit. Aan het eind van elke stap, kunt u een onderwerpverbinding selecteren om meer te leren.

## 1. Maak en upload de afbeeldingen

U hebt minstens 8-12 opnamen van een item nodig voor een eendimensionale centrifugeset en 16-24 voor een tweedimensionale centrifugeset. De opnamen moeten regelmatig worden gemaakt om de indruk te wekken dat het item draait en wordt gespiegeld. Als een eendimensionale centrifugeset bijvoorbeeld 12 opnamen bevat, roteert u het item 30° (360/12) voor elke opname.

Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Upload]** om draaiafbeeldingen van uw computer of netwerk te uploaden naar Adobe Dynamic Media Classic.

Zie [Richtlijnen voor het maken van centrifuges](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Een centrifugeset maken

Als u een centrifugeset wilt maken, gaat u op de algemene navigatiebalk naar **[!UICONTROL Build]** > **[!UICONTROL Spin Sets]**. Kies in het dialoogvenster Grootte van paginaset het gewenste aantal rijen en cellen en selecteer **[!UICONTROL OK]**. Vervolgens sleept u de afbeeldingen naar het raster op de pagina Draaien.

Zie [Een centrifugeset maken](creating-spin-set.md#creating-a-spin-set).

## 3. Een centerset bewerken

Als u een centrifugeset wilt bewerken, gaat u naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. Selecteer een centrifugeset en selecteer vervolgens **[!UICONTROL Edit]**. Voeg afbeeldingen toe, verwijder deze en wijzig de positie ervan. U kunt de positie van rijen in tweedimensionale centrifuges wijzigen.

Zie [Een centrifugeset bewerken](creating-spin-set.md#editing-a-spin-set).

## 4. Voorinstellingen voor een draaiende set viewers instellen

Beheerders kunnen voorinstellingen van de voorinstelling Spin Set Viewer maken. Deze voorinstellingen bepalen de vormgeving van de viewer voor de centrifugeset. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

Selecteer op de pagina Voorinstellingen viewer de optie **[!UICONTROL Add]** selecteert u vervolgens **[!UICONTROL Spin Set Viewer]** in de vervolgkeuzelijst en selecteer vervolgens **[!UICONTROL Add]**. Kies opties in het dialoogvenster `Configure Viewer` pagina, selecteert u vervolgens **[!UICONTROL Save]**.

Zie [Voorinstellingen voor een draaiende viewer instellen](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Een voorvertoning van een centerset weergeven

Selecteer de centrifugeset in het deelvenster Bladeren en selecteer **[!UICONTROL Preview]**. Houd op de pagina Voorvertoning de muisknop ingedrukt en sleep de aanwijzer naar links of rechts om het item visueel te &quot;draaien&quot;.

Zie [Een voorvertoning van een centrifugeset weergeven](previewing-spin-set.md#previewing-a-spin-set).

## 6. Een centrifugeerset publiceren

Als u een Spin-set publiceert, wordt deze op Adobe Dynamic Media Classic-servers geplaatst, zodat deze dynamisch aan uw website of toepassing kan worden geleverd. Het activeert ook het koord URL dat de Vastgestelde Rotatie van de Servers van het Beeld van Dynamic Media aan uw Website of toepassing roept.

Als u een centrifugeset wilt publiceren, markeert u deze voor publicatie door de optie **[!UICONTROL Mark for Publish]** naast de naam in het deelvenster Bladeren. Selecteer op de algemene navigatiebalk de optie **[!UICONTROL Publish]** om een publicatie te starten. Selecteer op de pagina Publiceren de optie **[!UICONTROL Submit Publish]**.

Zie [Een centrifugeerset publiceren](publishing-spin-set.md#publishing-a-spin-set).

## 7. Koppel een centrifugeerset aan een webpagina

Adobe Dynamic Media Classic maakt URL-callout-tekenreeksen voor centrifuges en activeert deze na publicatie. U kunt deze URL&#39;s kopiëren vanaf de pagina Voorbeeld.

Selecteer de centrifugeset en selecteer vervolgens **[!UICONTROL Preview]**. Selecteer een voorinstelling voor een centrifugeset viewer. Selecteer vervolgens de optie **[!UICONTROL Copy URL]**.

Zie [Een centrifugeerset koppelen aan een webpagina](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
