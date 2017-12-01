---
title: "Så här ställer du in flera räntesatser"
description: "Du kan beräkna dröjsmålsränta med flera räntesatser för en särskild period. Ränteberäkningen görs på samma sätt för alla dröjsmålsräntor, men räntan kan variera under en viss period."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: af5533bea9dd7d3a289c34eedc3836f789702cb3
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-multiple-interest-rates"></a>Så här ställer du in flera räntesatser
Du kan beräkna dröjsmålsränta med flera räntesatser för en särskild period. Ränteberäkningen görs på samma sätt för alla dröjsmålsräntor, men räntan kan variera under en viss period.  

Du kan till exempel debitera kunder enligt detta om de betalar för sent.  

## <a name="to-set-up-multiple-interest-rates"></a>Så här ställer du in flera räntesatser  

1.  Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Räntevillkor** och välj sedan relaterad länk.    
2.  Gå till fönstret **Räntevillkor** välj räntevillkoret och välj sedan åtgärden **Räntesatser**.  
3.  Fyll i fälten enligt beskrivningen i följande tabell.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Startdatum**|Ange startdatum för varje räntesatskod.|  
    |**Räntesats**|Ange den procentsats som ska användas vid beräkning av räntan.|  
    |**Ränteperiod (dagar)**|Ange perioden för varje räntesats.|  

4.  Välj **OK**.  
5.  Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Betalningspåminnelsevillkor** och välj sedan relaterad länk.  
6.  Gå till fönstret **Betalningspåminnelsevillkor** välj villkoret och välj sedan åtgärden **Nivåer**.  
7.  Markera fältet **Beräkna ränta** i fönstret **Betalningspåminnelsenivåer**.  

När du skickar ut en räntefaktura, visar fakturan dröjsmålsräntan med flera räntesatser för en viss tidsperiod. Räntefakturan innehåller även kontaktinformation för kunden, företaget som skickar räntefakturan, det ytterligare beloppet och totalt belopp. Den ingående transaktionen på räntefakturan visas i fet stil. Dröjsmålsräntan beräknas med flera räntesatser för en viss tidsperiod och skrivs ut efter den ingående transaktionen på räntefakturan.  

## <a name="see-also"></a>Se även  
 [Så här kräver du in utestående saldon](../../receivables-collect-outstanding-balances.md)

