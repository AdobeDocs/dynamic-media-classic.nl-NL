---
title: Sjabloonparameters maken
description: Leer hoe u sjabloonparameters maakt.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Sjabloonparameters maken{#creating-template-parameters}

De parameters laten u toe om malplaatjes met maximumflexibiliteit te gebruiken; hiermee kunt u een sjabloonafbeelding dynamisch aanpassen. U kunt bepalen welke tekst- en afbeeldingslagen u wilt opnemen in de sjabloon en in elke laag, welke parameters u wilt weergeven. Als u bijvoorbeeld de aandacht wilt vestigen op een product dat te koop is, kunt u een tekstlaag Op verkoop maken. Later kunt u deze laag verwijderen, maar toch de rest van de sjabloonafbeelding behouden door de parameter Aan verkoop te verwijderen.

Wanneer u malplaatjeparameters creeert, verklaart u in feite welke delen van het malplaatje in een koord URL te roepen. Een URL die met parameters is samengesteld, maakt die items in de URL-tekenreeks beschikbaar. Met blootgestelde parameters, kunt u douaneresultaten van de manier tot stand brengen het malplaatjebeeld dynamisch van de Server van het Beeld wordt geconstrueerd. Op deze manier kunt u een sjabloon dynamisch wijzigen omdat u enkele of alle parameters ervan in een URL kunt aanroepen.

In tekstlaagparameters kunt u de tekstreeks ook een dynamisch veld maken dat is gekoppeld aan waarden in een database. Het is bijvoorbeeld handig om tekst aan een database te koppelen in promoties. U kunt sjabloonafbeeldingen aanpassen zodat ze de naam van de klant of de klant weergeven. U kunt een parameter van de tekstlaag aan een prijsgegevensbestand ook verbinden om de prijs van een punt in een malplaatjebeeld te tonen.

U kunt meerdere keren naar een parameter verwijzen. Gebruik de keuzelijst met invoervak voor elke opdracht in het parameterdialoogvenster om een parameter te selecteren die overeenkomt met die opdracht. (Alle grootteparameters zijn bijvoorbeeld beschikbaar voor de opdracht `size=`, enzovoort). U kunt de parameterverwijzing aan om het even welke parameter opnieuw toewijzen reeds in de combodoos, en aan iets anders noemen niet in de combodoos. In het laatste geval moet de naam uniek zijn. Anders geeft een fout aan dat de parameter bestaat. Wanneer u een parameterverwijzing verwijdert, wordt de parameter verwijderd uit de URL als nergens anders naar wordt verwezen. Wanneer u de standaardwaarde voor een tekstparameter wijzigt, worden alle verwijzingen naar die parameter bijgewerkt. U kunt de update in de laaglijst, in het teruggeven van het malplaatje, en in URL zien. Wanneer u een laagkenmerk wijzigt door grepen vergroten/verkleinen of waarden in het deelvenster Eigenschappen te typen, wordt de parameterwaarde bijgewerkt en worden alle verwijzingen naar de parameter bijgewerkt. Als u bijvoorbeeld de grootte van twee lagen hebt bepaald met behulp van één parameter, worden beide laaggrootten bijgewerkt wanneer een van de laaggrootten wordt gewijzigd. Wanneer u een voorbeeld van een sjabloon bekijkt en een parameter wijzigt, worden alle verwijzingen naar die parameter bijgewerkt.

## Een laag parameters geven {#parameterizing-a-layer}

Voer voor elke laag in de sjabloon de volgende stappen uit om sjabloonparameters te maken:

1. Selecteer in de lijst Lagen de knop Parameters naast de naam van de laag waarvoor u parameters wilt maken. Het scherm Parameters wordt geopend. De naam van elke parameter in de laag, de waarde en het type worden weergegeven.
1. Selecteer de optie Aan naast de naam van elke parameter die u in de sjabloonafbeelding wilt opnemen.
1. Selecteer **[!UICONTROL Close]** om het scherm van Parameters weg te gaan.

>[!NOTE]
>
>U kunt parameters in het scherm van Parameters anders noemen. Als u de naam van een parameter wijzigt, wordt de parameter gemakkelijker herkend in URL-tekenreeksen en gemakkelijker te gebruiken als databasewaarde. Als u de naam van een parameter wilt wijzigen, selecteert u de optie Aan, klikt u op de naam van de parameter en voert u in het veld Naam een nieuwe naam in.

Om een lijst van de parameters te zien u voor uw malplaatje hebt gecreeerd, selecteer de Samenvatting van de Parameter knoop op het scherm van het Malplaatje. Het scherm Parameter Summary wordt geopend. De naam van elke laag wordt weergegeven en als u parameters voor een laag hebt gemaakt, worden de namen en waarden van de parameters weergegeven.

## Dynamische-tekstparameters maken {#creating-dynamic-text-parameters}

Voor tekstlagen kunt u ook van de tekstreeks een dynamisch veld maken dat is gekoppeld aan een databasewaarde. Voer de volgende stappen uit:

1. Selecteer in het scherm Sjabloon de knop Parameters naast de naam van de tekstlaag waarvoor u dynamische tekstparameters wilt maken. De pagina Parameters wordt geopend.
1. Klik op de optie **[!UICONTROL On]** naast de naam van het tekstkenmerk (textAttr).
1. Klik op het tabblad **[!UICONTROL Text]** in het scherm Parameters.
1. Klik op **[!UICONTROL Add Parameter]**. Er wordt een standaardparameternaam weergegeven. U kunt deze naam vervangen door deze te selecteren en er overheen te typen. De huidige tekstreeks wordt de nieuwe naam van de parameter.
1. Klik **[!UICONTROL Close]** om de pagina van Parameters te sluiten.

Als u wilt dat de parameternaam een databasewaarde gebruikt, voegt u de volgende tekenreeks toe aan de URL van de sjabloon:

```as3
?$_2(parameter name)=(database value)
```

De parameternaam wordt vervangen door namen in een databaseveld of Java™-code die bijvoorbeeld de huidige prijs van een item of de naam van een klant aangeven.
