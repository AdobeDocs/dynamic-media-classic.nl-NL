---
title: Dynamic Media-beperkingen
description: Leer over de beste praktijken en de gedwongen grenzen wanneer u een Reeks van het Beeld of een Reeks van de Rotatie creeert, of een PDF uploadt. Meer informatie over niet-ondersteunde combinaties van webbrowsers en besturingssystemen voor Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---

# Dynamic Media-beperkingen

In de volgende secties worden beperkingen in Dynamic Media beschreven.

Dit onderwerp omvat de volgende secties:

* [Aanbevolen werkwijzen en door Dynamic Media opgelegde limieten voor soorten activa](#best-practice-enforced-limits)
* [Niet-ondersteunde combinaties van webbrowsers en besturingssystemen voor Dynamic Media](#unsupported-browser-os)

## Aanbevolen werkwijzen en door Dynamic Media opgelegde limieten voor soorten activa {#best-practice-enforced-limits}

Als u een centrifugeset of een afbeeldingsset maakt of PDF uploadt voor het uitnemen van pagina&#39;s, raadt Adobe u de volgende aanbevolen procedures aan. Adobe handhaaft ook de volgende limieten:

| Element: type Limiet | Beste praktijken | Oplegde limiet |
| --- | --- | --- |
| **Beeld**: Aantal Slimme Uitsnijdingen per beeld | 5 | 100 |
| **Alle reeksen**: Aantal dubbele activa per reeks | Geen duplicaten | 20‡ |
| **Alle reeksen**: Maximum aantal activa per reeks | 5-10 afbeeldingen per set | 1000 |
| **Reeks van de Draai**: Maximum aantal rijen/kolommen per 2D reeks | 12-18 afbeeldingen per set | 1000 |
| **PDF**: Maximum aantal pagina&#39;s voor een PDF die voor extractie moet worden overwogen |  | 100 (voor alle PDF) |

‡ De beste manier is om geen dubbele elementen in een set te hebben. De limiet is 20 duplicaten voor één element. Als u nog een duplicaat voor dat element toevoegt (binnen die set), geeft de aanvraag een fout of wordt het duplicaat genegeerd.

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Niet-ondersteunde combinaties van webbrowsers en besturingssystemen voor Dynamic Media {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Adobe Dynamic Media biedt geen ondersteuning voor de volgende combinaties van webbrowsers en besturingssystemen.

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Internet Explorer 11 + Windows Phone 8.1-update
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Einde van steun voor Veilige Laag 2.0 en 3.0 van de Contactdoos en de Veiligheid van de Laag van het Vervoer 1.0 en 1.1 {#tls}

<!-- CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) -->

Vanaf 30 april 2024 beëindigt Adobe Dynamic Media de steun voor:

* SSL (Secure Socket Layer) 2.0
* SSL 3.0
* TLS (Transport Layer Security) 1.0 en 1.1
* De volgende zwakke ciphers in TLS 1.2:
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384`
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_RSA_WITH_AES_256_GCM_SHA384`
   * `TLS_RSA_WITH_AES_256_CBC_SHA256`
   * `TLS_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_AES_128_GCM_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_256_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_128_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA`
   * `TLS_RSA_WITH_SDES_EDE_CBC_SHA`

