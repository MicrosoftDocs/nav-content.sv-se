---
title: "Så här skriver du ut en kundremissa"
description: "Du kan hjälpa dina leverantörer göra avstämningar genom att skriva ut en kundremissa innan du bokför en utbetalningsjournal och när du har bokfört en betalning."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: sv-se
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a>Så här skriver du ut en kundremissa
Du skriver ut en kundremissa innan du bokför en utbetalningsjournal och när du har bokfört en betalning. Detta visar leverantörens fakturanummer som hjälper leverantörer att göra avstämningar.

##<a name="to-print-remittance-advice"></a>Så här skriver du ut en kundremissa
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Utbetalningsjournal** och välj sedan relaterad länk.  
2. I fönstret **betalningsjournal** väljer du den betalning för vilken kundremissa måste skrivas ut för.  
3. Välj åtgärden **Skriv ut kundremissa**.  
4. I batchjobbet **Kundremissa - Journal** på snabbfliken **Redovisningsjournalrad** väljer du lämpliga filter.  
  
    >[!Note]
    > Du kan filtrera med hjälp av leverantörens externa dokumentnummer för att matcha betalningar till fakturor.

5. Välj lämpliga filter på snabbfliken **Leverantör**.  
6. Välj **Skriv ut** om du vill skriva ut rapporten eller välj **Förhandsgranska** om du vill visa den nu.  

## <a name="using-remittance-advice-reports"></a>Använda kundremissarapporter
Följande tabell beskriver de rapporter som du kan använda med en kundremissa:

|Rapport|Description|
|----|----|
|Kundremissa – journalrapport|Den här rapporten visar vilka dokument som ska tas med i betalningen. För redovisningsjournalrader kan du ange den journalmall och journal som remissan ska skrivas ut från, datumet för den första aktiviteten som ska skrivas ut och filtrera efter ett dokumentnummer. För leverantörer kan du ange det leverantörsnummer som ska tas med i rapporten. |
|Kundremissa – transaktionsrapport| Den här rapporten visar vilka dokument som ska tas med i betalningen. Du kan definiera rapportens innehåll genom att definiera filter. Du kan ange ytterligare fält på fliken genom att välja fältet **Fält**. För leverantörsreskontratransaktioner kan du ange vilka leverantörer som ska inkluderas i rapporten, datumet för den första aktiviteten som ska skrivas ut, valuta och numret som ska inkluderas. |

> [!Note]
> Kundremissa - journalrapport ger inte stöd för från andra scenarier med tillämpning av olika valutor eller betalningstoleranser. Mer information finns i [Så här aktiverar du koppling av kundreskontratransaktioner till olika valutor](finance-how-enable-application-ledger-entries-different-currencies.md).

> [!Tip]
> Läs mer om hur du arbetar med rapporter i [Visa testrapporter före bokföring](ui-how-view-test-reports-posting.md), [Arbeta med rapporter](ui-work-report.md) och [Söka, filtrera och sortera data ](ui-enter-criteria-filters.md).

##<a name="see-also"></a>Se även  
[Välkommen till Dynamics NAV](across-get-started.md)
