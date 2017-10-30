---
title: "Ställ in status för serviceorder och reparationer"
description: "Du måste ställa in nio olika alternativ för reparationsstatus som anger hur reparationen och underhållet av serviceartiklarna på serviceorder framskrider."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d7dbc4cfc06d4c74476a04512bd368a0ab26f837
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-statuses-for-service-orders-and-repairs"></a>Så här: ställa in status för serviceorder och reparationer
Du måste ställa in olika alternativ för reparationsstatus som anger hur reparationen och underhållet av serviceartiklarna på serviceorder framskrider. Du måste skapa åtminstone nio reparationsstatusalternativ som identifierar situationer eller åtgärder som vidtagits då serviceartiklar servas.  

Du kan ange prioriteringsnivåer för alternativen för serviceorderstatus. Det finns fyra prioriteter: Hög, medelhög, medellåg och låg.  
  
När du ändrar en serviceartikels reparationsstatus på serviceordern uppdateras serviceorderns status. Varje serviceartikels reparationsstatus är kopplad till serviceorderstatusen. Om serviceartiklarna är kopplade till två eller fler serviceorderstatusalternativ väljs den serviceorderstatus som har högst prioritet.  

## <a name="to-set-up-a-repair-status"></a>Så här skapar du en reparationsstatus  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Reparationsstatus** och välj sedan relaterad länk. 2. Skapa en ny reparationsstatus.  
3. Fyll i fälten **Kod** och **Beskrivning**.  
4. I fältet **serviceorderstatus** väljer du orderstatus att länka reparationsstatusen till. Fältet **Prioritet** visar prioriteten för den serviceorderstatus som du har valt.  
5. Välj en reparationsstatus Du kan bara välja en.  
6. Välj fältet **Bokföring tillåten** om du vill kunna bokföra serviceorder som innefattar serviceartiklar med aktuell reparationsstatus.  
7. Markera kryssrutan **Förestående status tillåten** om du vill kunna ändra serviceorderns status manuellt till alternativet **Förestående** på serviceorder som innefattar serviceartiklar med aktuell reparationsstatus.  
8. Markera kryssrutorna **Pågående status tillåten**, **Färdig status tillåten** och **Stoppad status tillåten** på samma sätt.
  
## <a name="to-set-up-service-status-priorities"></a>Så här skapar du servicestatusprioriteter  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceorderstatus** och välj sedan relaterad länk.  
2. Välj den serviceorderstatus som du vill ange prioritet för.  
3. I fältet **Prioritet** väljer du önskad prioritet för aktuell serviceorderstatus. Upprepa det här steget för varje status.  
  
## <a name="see-also"></a>Se även  
[Förstå serviceorderstatus och reparationsstatus]()  
[Ställa in servicehantering](service-setup-service.md)  

