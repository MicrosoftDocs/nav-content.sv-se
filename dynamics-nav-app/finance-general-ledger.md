---
title: Mer information om redovisning och kontoplanen
description: Beskriver redovisningen, kontoplanen och kontokategorierna.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 348a1bcbe6908c7bfd84e99245363e733414aeae
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="understanding-the-general-ledger-and-the-coa"></a>Så här fungerar i redovisningen och kontoplanen
Redovisningen lagrar dina ekonomiska data, och kontoplanen visar de konton som alla redovisningstransaktioner bokförs på. [!INCLUDE[d365fin](includes/d365fin_md.md)] inkluderar en standardkontoplan som är klar att stödja din verksamhet.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Redovisningsinställning och bokföringingsinställning
Inställningarna för redovisningen är kärnan i ekonomiska processer eftersom den definierar hur du bokför data.  

I fönstret **Redovisningsinställningar** anger du hur du vill hantera vissa bokföringsfrågor i företaget som t.ex.:  

* Öresutjämning  
* Adresslayout  
* Ekonomisk rapportering  

På liknande sätt i fönstret **Bokföringsinställningar** anger du hur du vill ange kombinationer av allmän bokföringsmallar och allmäna produktbokföringsmallar. Bokföringsmallar mappar enheter som t.ex. kunder, leverantörer, artiklar, resurser och försäljning och inköpsdokument till redovisningskonton. Du fyller i en rad för varje kombination av rörelse- och produktbokföringsmall. Mer information finns i [Inställning av bokföringsmall](finance-posting-groups.md).  

## <a name="the-chart-of-accounts"></a>Kontoplanen
Kontoplanen visar alla redovisningskonton. Från kontoplanen, kan du göra sådant som:  

* Visa rapporter som visar transaktioner och saldon.  
* Avslut av resultatkonton.  
* Öppna redovisningkontokortet om du vill lägga till eller ändra inställningar.  
* Visa en lista med bokföringsmallar som bokför på det konto.
* Visa separatea debet- och kreditsaldon för ett enskilt konto  

Du kan lägga till, ändra eller ta bort konton i redovisningen. Men för att undvika avvikelser bör du inte ta bort ett redovisningskonto om dess data används i kontoplanen.  

## <a name="account-categories"></a>Kontokategorier
Med kontokategorier kan du mappa redovisningskonton till kategorier som en anpassning av strukturen på din redovisning.  

Fönstret **Redovisningskontokategorier** visar de kategorierna och delkategorierna och redovisningskontona som har tilldelats dem. Du kan skapa nya delkategorier och tilldela de kategorierna till befintliga konton.  

Du skapar en kategorigrupp, genom att dra in andra delkategorier under en rad i fönstret **redovisningskontokategorier**. Detta gör det lätt för dig att få en översikt, eftersom varje journal visar ett totalt saldo. Du kan till exempel skapa delkategorier för andra typer av anläggningstillgångar och sedan skapa kategorigrupper för t.ex. anläggningstillgångar jämfört med omsättningstillgångar.  

För varje delkategori kan du ange om konton för den kategorin måste tas med i vissa typer av ekonomiska rapporter. Du kan använda kontokategorier för att ändra layout på din redovisning.  

Till exempel har det standardinställda saldo vid kontoavstämning en enkelt transaktion för kontanter under tillgångar. Om du vill att saldot överväger handkassa och check, kan du:  

1. Lägga till två nya underkategorierna. En för handkassa och ett för ditt checkkonto.  
2. Ange ytterligare rapportdefinitionen **kassakonton** för dessa underkategorier.  
3. Dra in dem under underkategorin **kontant**.  

Nästa gång du har genererat kontouppställningar kommer saldot visa ett totalt saldo för kontanter och två rader med saldon för handkassa och checkräkningskontot.  

## <a name="see-also"></a>Se även
[Ekonomi](finance.md)  
[Ställa in eller ändra kontoplanen](finance-setup-chart-accounts.md)  
[Affärsstöd](bi.md)  

