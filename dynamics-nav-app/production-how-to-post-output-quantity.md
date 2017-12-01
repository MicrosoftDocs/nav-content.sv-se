---
title: "Så här: Batch-bokför produktionsutflöde och körtid"
description: "Utflödesantalet representerar det pågående arbetet som det färdiga antalet."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 266c3f52dda22133acebf6052326ab57551b2ec0
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-batch-post-output-and-run-times"></a>Så här: Batch-bokför utflöde och körtid
Utflödesantalet representerar det pågående arbetet som det färdiga antalet.  

> [!NOTE]
> Endast när du bokför utflödesantalet för den sista operationen uppdateras lagret automatiskt.  

## <a name="to-post-output-quantities-for-one-or-more-production-order-lines"></a>Om du vill bokföra utflödeskvantiteter för produktion av en eller flera orderrader
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Utflödesjournal** och välj sedan relaterad länk.  
2. Fyll i fälten med data om produktionsorden och utdata. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Om operationen har slutförts, välj fältet **FÄRDIG**.  

    Om lagerplatser används på det lagerställe där artiklarna ska placeras, men bearbetning av artikelinförsel inte krävs,  ska journalraden tilldelas en lagerplatskod som anger var artiklarna ska placeras på distributionslagret. Mer information finnsi [Så här: för in produktions- eller monteringsutflöde](warehouse-how-to-put-away-production-output.md).  

4. Om du vill bokföra operationerna väljer du åtgärden **Bokför**. Utflödesantalet bokförs. Artikeln är nu tillgänglig för leverans.  

## <a name="to-post-run-times-for-one-or-more-production-order-lines"></a>Om du vill bokföra körtider för produktion av en eller flera rader
Bearbetningstiden representerar det pågående arbetet som nödvändig arbetstid.    

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Utflödesjournal** och välj sedan relaterad länk.  
2. Fyll i fälten med data om produktionsorden och utdata.  
3.  Om operationen har slutförts, välj fältet **FÄRDIG**.  
4. Välj åtgärden **bokför** för att bokföra spenderad tid per operation. Kapacitetstransaktioner uppdateras för använt arbete eller maskingrupper.

## <a name="see-also"></a>Se även  
[Produktion](production-manage-manufacturing.md)    
[Ställa in Produktion](production-configure-production-processes.md)  
[Planerad](production-planning.md)      
[Lagersaldo](inventory-manage-inventory.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

