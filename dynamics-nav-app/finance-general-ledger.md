---
title: Redovisningen och kontoplanen
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Redovisningen och kontoplanen
Redovisningen lagrar dina ekonomiska data, och kontoplanen visar de konton som alla redovisningstransaktioner bokförs på. Dynamics NAV inkluderar en standardkontoplan som är klar att stödja din verksamhet.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Redovisningsinställning och bokföringingsinställning
Den centrala delen av dina affärsprocesser är redovisningen och konfigurationen av hur data bokförs i redovisningen.
I fönstret **Redovisningsinställningar** anger du hur du vill hantera vissa bokföringsfrågor i företaget. Det innehåller fakturaavrundningdetaljer, adressformat och om du vill använda en ytterligare rapporteringvaluta, till exempel.
På liknande sätt i fönstret **Bokföringsinställningar** anger du hur du vill ange kombinationer av allmän bokföringsmallar och allmäna produktbokföringsmallar. Du fyller i en rad för varje kombination av rörelse- och produktbokföringsmall.  

## <a name="the-chart-of-accounts"></a>Kontoplanen
Kontoplanen visar alla konton. Härifrån kan du öppna olika rapporter, som visar redovisningstransaktioner och saldon, och du kan avsluta resultaträkningen. Från Kontoplan kan du öppna varje Redovisningskonto och lägga till eller ändra inställningar. Du kan också visa en lista med bokföringsmallar som bokför på det konto.  

Dynamics NAV kommer att förhindra att du tar bort ett redovisningskonto som lagrar data som behövs i kontoplanen.  

## <a name="account-categories"></a>Kontokategorier
Med kontokategorier kan du mappa redovisningskonton till kategorier som en anpassning av strukturen på din redovisning.  

Fönstret **Redovisningskontokategorier** visar de befintliga huvudkategorierna och delkategorierna och redovisningskontona som du har tilldelat varje kategori. Du kan skapa nya delkategorier och tilldela de kategorierna till befintliga konton.  

Du kan gruppera kontokategorierna, genom att dra in individuella delkategorier. Detta gör det lätt för dig att få en översikt, eftersom varje journal visar ett totalt saldo. Du kan till exempel skapa delkategorier för andra typer av anläggningstillgångar och sedan skapa kategorigrupper för t.ex. anläggningstillgångar jämfört med omsättningstillgångar. Du skapar en kategorigrupp, genom att dra in andra delkategorier under en rad i fönstret **redovisningskontokategorier**.  

För varje delkategori kan du ange om konton för den kategorin måste tas med i vissa typer av ekonomiska rapporter. Du kan använda kontokategorier för att ändra layout på din redovisning. Till exempel har det standardinställda saldo vid kontoavstämning en enkelt transaktion för kontanter under tillgångar. Om du vill att saldo vid kontoavstämning ska ha underposter för handkassa och checkräkningskonto, kan du lägga till två nya delkategorier, ange de extra rapportdefinitionen Kassakonton för var och en av dem och dra in dem under den delkategorin Kontanter. När du har genererat kontouppställningar baserat på ändringarna, kommer lagerkontosaldot nästa saldo vid kontoavstämning visa ett totalt saldo för kontanter och två rader med saldon för handkassa och checkräkningskontot.     

##<a name="see-also"></a>Se även
[Finans](finance-setup.md)  
[Ställa in eller ändra kontoplanen](finance-setup-setup-chart-accounts.md)  
[Kontouppställningar](finance-setup-account-schedule.md)  

