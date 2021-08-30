---
title: '"Snel starten: Sets draaien"'
description: Een inleiding en Snel starten om te draaien zodat u snel aan de slag kunt in Adobe Dynamic Media Classic.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Snel starten: Sets draaien{#quick-start-spin-sets}

Een centrifugeerset simuleert de echte handeling waarbij een object wordt omgedraaid om het te onderzoeken. Met centrifuges kunt u items vanuit elke hoek bekijken en de belangrijkste visuele details vanuit elke hoek verkrijgen. Een centrifugeerset simuleert een kijkervaring van 360°. Adobe Dynamic Media Classic biedt eendimensionale centrifuges waarin gebruikers een item kunnen roteren en tweedimensionale centrifuges waarin gebruikers het item kunnen roteren en spiegelen. Bovendien kunnen gebruikers met een paar eenvoudige muisklikken in- en uitzoomen op een vrije vorm en een willekeurige weergave pannen. Op deze manier kunnen gebruikers een item vanuit een bepaald gezichtspunt nader onderzoeken.

![Afbeeldingen voor een centrifugeerset.](/help/assets/spin_set.png)

Draaisets accepteren ook afbeeldingen met hyperlinks. Een afbeelding met hyperlinks is een gebied in een afbeelding in de centrifugeset dat een deelvenster met rollover-tekst weergeeft. Wanneer de gebruiker op een afbeelding met hyperlinks klikt, wordt een handeling van een bepaalde aard geactiveerd. Er wordt bijvoorbeeld een webpagina gestart zodat de gebruiker meer over een product kan leren. Als u een afbeelding met hyperlinks wilt aanwijzen in een centrifugeset, verschijnt er een omtrek rond de afbeelding met hyperlinks als de gebruiker de muisaanwijzer erboven plaatst.

Zie [Afbeeldingskaarten maken](creating-image-maps.md).

Deze centrifugeert Snel starten is ontworpen om snel aan de slag te gaan met centrifugetechnieken in Adobe Dynamic Media Classic. Voer stap 1 tot en met 7 uit. Aan het eind van elke stap, kunt u een onderwerpverbinding selecteren om meer te leren.

## 1. De afbeeldingen maken en uploaden

U hebt minstens 8-12 opnamen van een item nodig voor een eendimensionale centrifugeset en 16-24 voor een tweedimensionale centrifugeset. De opnamen moeten regelmatig worden gemaakt om de indruk te wekken dat het item draait en wordt gespiegeld. Als een eendimensionale centrifugeset bijvoorbeeld 12 opnamen bevat, roteert u het item 30° (360°/12) voor elke opname.

Selecteer **[!UICONTROL Upload]** op de algemene navigatiebalk om draaiafbeeldingen van uw computer of netwerk te uploaden naar Adobe Dynamic Media Classic.

Zie [Richtlijnen voor het maken van centrifugeerbare afbeeldingen](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Een centrifugeset maken

Als u een centrifugeset wilt maken, gaat u op de algemene navigatiebalk naar **[!UICONTROL Build]** > **[!UICONTROL Spin Sets]**. Kies in het dialoogvenster Grootte van paginaset het gewenste aantal rijen en cellen en selecteer **[!UICONTROL OK]**. Vervolgens sleept u afbeeldingen naar het raster op de pagina Draaien.

Zie [Een centrifugeerset maken](creating-spin-set.md#creating-a-spin-set).

## 3. Een draaiset bewerken

Als u een centrifugeset wilt bewerken, gaat u op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. Selecteer een centrifugeerset en selecteer **[!UICONTROL Edit]**. Voeg afbeeldingen toe, verwijder deze en wijzig de positie ervan. U kunt de positie van rijen in tweedimensionale centrifuges wijzigen.

Zie [Een centrifugeset bewerken](creating-spin-set.md#editing-a-spin-set).

## 4. Voorinstellingen voor draaiende viewer instellen

Beheerders kunnen voorinstellingen van de voorinstelling Spin Set Viewer maken. Deze voorinstellingen bepalen de vormgeving van de viewer voor de centrifugeset. Als u een nieuwe voorinstelling voor een centrifugeset-viewer wilt instellen, gaat u op de algemene navigatiebalk naar **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

Selecteer **[!UICONTROL Add]** op de pagina Voorinstellingen viewer, selecteer **[!UICONTROL Spin Set Viewer]** in de vervolgkeuzelijst en selecteer **[!UICONTROL Add]**. Kies opties in de Configure pagina van de Kijker, dan selecteer **[!UICONTROL Save]**.

Zie [Voorinstellingen voor centrifugeren instellen voor viewer](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Een voorvertoning van een centrifugeset weergeven

Selecteer de centrifugeset in het deelvenster Bladeren en selecteer **[!UICONTROL Preview]**. Houd op de pagina Voorvertoning de muisknop ingedrukt en sleep de aanwijzer naar links of rechts om het item visueel te &quot;draaien&quot;.

Zie [Een voorvertoning van een centrifugeset weergeven](previewing-spin-set.md#previewing-a-spin-set).

## 6. Een centrifugeerset publiceren

Als u een Spin-set publiceert, wordt deze op Adobe Dynamic Media Classic-servers geplaatst, zodat deze dynamisch aan uw website of toepassing kunnen worden geleverd. Het activeert ook de URL-tekenreeks die de Spin Set van Dynamic Media Image-servers naar uw website of toepassing aanroept.

Als u een centrifugeset wilt publiceren, markeert u deze voor publicatie door het pictogram **[!UICONTROL Mark for Publish]** naast de naam ervan in het deelvenster Bladeren te selecteren. Selecteer **[!UICONTROL Publish]** op de algemene navigatiebalk om een publicatie te starten. Selecteer **[!UICONTROL Submit Publish]** in het scherm Publiceren.

Zie [Een centrifugeerset publiceren](publishing-spin-set.md#publishing-a-spin-set).

## 7. Een centrifugeerset koppelen aan een webpagina

Adobe Dynamic Media Classic maakt URL-bijschrifttekenreeksen voor centrifuges en activeert deze na publicatie. U kunt deze URL&#39;s kopiëren vanaf de voorvertoningspagina.

Selecteer de centrifugeset en selecteer **[!UICONTROL Preview]**. Selecteer een voorinstelling voor een centrifugeset viewer. Selecteer vervolgens **[!UICONTROL Copy URL]**.

Zie [Een centrifugeerset koppelen aan een webpagina](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
