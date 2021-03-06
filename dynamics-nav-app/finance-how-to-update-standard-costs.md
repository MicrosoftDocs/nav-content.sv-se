---
title: "Så här kan du uppdatera standardkostnader"
description: "Du måste regelbundet uppdatera standardkostnader för komponenter och överföra de nya kostnaderna till den överordnade artikeln."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: dd2bb16af611be7f7720fdf07eb65fd268aba039
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-update-standard-costs"></a>Så här kan du uppdatera standardkostnader
Du måste regelbundet uppdatera standardkostnader för komponenter och överföra de nya kostnaderna till den överordnade artikeln. Processen består typiskt av följande fyra steg:  

1.  Uppdatera kostnader på komponent- och kapacitetsnivå. Mer information finns i batch-jobbet **Föreslå artikelstandardkostnad**.  
2.  Konsolidera och summera komponent- och kapacitetskostnader för att beräkna den totala produktions- eller monteringskostnaden för artiklarna.  
3.  Använd standardkostnaderna som angavs när du körde de föregående batch-jobben. Standardkostnaderna börjar inte gälla förrän de implementeras. Mer information finns i Implementera standardkostnadsändringar.  
4.  Inför ändringarna för att uppdatera fältet **Styckkostnad** för artikelkortet och utföra lageromvärderingen. Mer information finns i [Så här omvärderar du lager](inventory-how-revalue-inventory.md).  

Mer information finns i [Om att beräkna standardkostnad](finance-about-calculating-standard-cost.md).  
## <a name="to-update-standard-costs"></a>Uppdatera standardkostnader  
1.  Kör batch-jobbet **Justera kost. - artikeltrans.**  
2.  Kör batch-jobbet **Bokför lagerkostnad i redov.**  
3.  Öppna **Standardkostnadsformulär** och använd en eller flera av följande funktioner:  

    1.  Kör batch-jobbet **Föreslå artikelstandardkostnad**.  
    2.  Granska resultaten och gör nödvändiga ändringar.  
    3.  Kör batch-jobbet **Föreslå standardkostnad för kapacitet**.  
    4.  Granska resultaten och gör nödvändiga ändringar.
    5. Kör batch-jobbet **Uppsummerad standardkostnad**.
    6.  Granska resultaten och gör nödvändiga ändringar.
    7.  Kör batch-jobbet **Implementera standardkostnadsändringar**.  
4.  Granska och bokför fönstret  **Omvärderingsjournal** , vilken har fyllts på med transaktioner från föregående steg i den här processen.  

## <a name="see-also"></a>Se även  
 [Om beräkning av standardkostnad](finance-about-calculating-standard-cost.md)   
 [Hantera lagerkostnader](finance-manage-inventory-costs.md)   
 [Designdetaljer: Värderingsprinciper](design-details-costing-methods.md) [[Finans](finance.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

