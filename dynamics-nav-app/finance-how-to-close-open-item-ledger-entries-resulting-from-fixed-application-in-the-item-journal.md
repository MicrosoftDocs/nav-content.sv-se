---
title: "Så här kan du avsluta öppna artikeltransaktioner som skapas från en fast koppling i artikeljournalen"
description: "Du kan använda fältet **Kopplas från löpnr** i fönstret **Artikeljournal** för att skapa en fast koppling mellan en inkommande transaktion och den ursprungliga utgående transaktionen. Till exempel, för att korrigera utgående transaktion eller bearbeta dess retur."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b0b0daad01f8108d035739e387b38af4f0311ff9
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a>Så här kan du avsluta öppna artikeltransaktioner som skapas från en fast koppling i artikeljournalen
Du kan använda fältet **Kopplas från löpnr** i fönstret **Artikeljournal** för att skapa en fast koppling mellan en inkommande transaktion och den ursprungliga utgående transaktionen. Till exempel, för att korrigera utgående transaktion eller bearbeta dess retur. Mer information finns i Kopplas från löpnr.  

> [!IMPORTANT]  
>  Fast koppling som gjorts på det här sättet gäller endast kostnaden, inte antal. På så sätt kommer den bokförda positiv artikeltransaktion inte avsluta det kopplade avgående transaktion, och att stå öppen. Detta gäller också när du bokför en fast koppling för en positiv transaktion på en negativ transaktion som inte har avslutats av en vanlig positiva transaktion, kommer både negativ och de positiva transaktionerna finns kvar öppna.  
>   
>  Det innebär att du inte kan avsluta en lagerperiod, om sådan transaktion finns.  

I följande procedur beskrivs hur du avslutar sådana transaktioner genom att utföra två korrigerande bokföringar i artikeljournalen.  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a>Om du vill avsluta öppna artikeltransaktioner som skapas från ett fast koppling i artikeljournalen  

1.  Använd fältet **Kopplas från löpnr** om du vill bokföra en positiv justering med motsvarande antal. Denna åtgärd stänger den ursprungliga negativ transaktion med en fast koppling.  
2.  Använd fältet **Kopplas till löpnr** om du vill bokföra en negativ justering. Denna åtgärd stänger den korrigerande positiva transaktionen med en fast koppling.  

## <a name="see-also"></a>Se även  
[ Så här kan du ta bort och koppla om artikeltransaktioner](finance-how-to-remove-and-reapply-item-entries.md)  
 [Så här behandlar du försäljningreturer och annulleringar](sales-how-process-sales-returns-cancellations.md)   
 [Ställa in lagervärdering och lagerkostnad](finance-set-up-inventory-valuation-and-costing.md)   
 [Hantera lagerkostnader](finance-manage-inventory-costs.md)   
 [Designdetaljer: Värderingsprinciper](design-details-costing-methods.md)

