---
title: "Lägga upp och använda standardrader för återkommande försäljning och inköp"
description: "Du kan definiera försäljningsrader och inköpsrader som du gör ofta och infoga dem på försäljnings- och inköpsdokument för att snabbt fylla i raderna med standardinformationen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, replenishment
ms.date: 07/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d3e7b514dfc91346a697b3c85cf36d7d69f56ddc
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-recurring-sales-and-purchase-lines"></a>Så här: Skapa återkommande försäljnings- och inköpsrader
Om du ofta behöver skapa försäljnings- och inköpsrader med liknande information, kan du ställa in standardraderna så att du sedan kan infoga på återkommande försäljning och inköpsdokument, till exempel för återkommande påfyllningsorder.  

I följande procedur beskrivs hur du arbetar med in standardförsäljningsrader. Det fungerar på liknande sätt för standardstandardinköpsrader.  

## <a name="to-set-up-standard-sales-lines"></a>Så här skapar du standardförsäljningsrader  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Standardtextkoder**, och välj sedan relaterad länk.  
2. I fönstret **Standard förs.rader** väljer du åtgärden **Ny**.  
3. I snabbfliken **Allmänt** fyller du i nödvändiga fält. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. I snabbfliken **Rader** ange information i fälten för att förbereda försäljningsrader som återspeglar de standardrader som du förväntar dig att använda som återkommande rader på försäljningsdokument.  

## <a name="to-insert-standard-sales-lines-on-a-sales-invoice"></a>Infoga standardförsäljningsrader i en försäljningsfaktura
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Standardtextkoder**, och välj sedan relaterad länk.
2. Öppna den försäljningsfaktura du vill infoga en eller flera standardförsäljningsrader på.
3. Välj åtgärden **få återkommande förs.rader**.
4. I fönstret **återkommande försäljningsrader** välj sökknappen i fältet **kod** och välj sedan en uppsättning standardförsäljningsrader.
5. Välj **OK** för att infoga standardförsäljningsraderna på fakturan, där du kan använda eller redigera informationen.

## <a name="to-create-multiple-sales-invoices-based-on-standard-sales-lines"></a>Så här: skapa flera försäljningsfakturor utifrån standardförsäljningskoder
Du kan använda batch-jobbet **Skapa återkommande försäljningsfakt.** för att skapa försäljningsfakturor enligt standardförsäljningsrader som tilldelats till kunderna och med bokföringsdatum som infaller inom de giltighetsdatum som du anger på standardförsäljningskoden.

I fönstret **Återkommande försäljningsrader** kan du också ange en metod för autogirobetalning och medgivande för autogiro. De försäljningsfakturor som skapas med batch-jobbet **Skapa återkommande försäljningsfakt.** tar sedan med information som krävs för att kräva betalning för försäljningsfakturorna med SEPA-autogiro. Mer information finns i [Kräva in betalningar med SEPA direktdebitering](finance-collect-payments-with-sepa-direct-debit.md).

1. Välj ikonen ![söka efter sida eller rapport](media/ui-search/search_small.png "ikonen söka efter sida eller rapport"), ange **Skapa återkommande försäljningsfakturor** och välj sedan relaterad länk.
2. I fönstret **Skapa återkommande försäljningsfakt.** fyller du i de fälten efter behov.
3. I fältet **kod** anger du koden för standardförsäljningsrader som tilldelats kunden som du vill skapa fakturor för.
4. Välj **OK**.

Fakturor skapas för kunder med den angivna standardkundförs.koden och angiven information om direktdebitering, för bokföring på det angivna datumet.

## <a name="see-also"></a>Se även  
[Försäljning](sales-manage-sales.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

