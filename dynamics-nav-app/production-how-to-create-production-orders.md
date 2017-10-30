---
title: "Så här skapar du ett produktionsorderhuvud"
description: "Du kan skapa en produktionsorder manuellt och första steget är då att skapa ett produktionsorderhuvud."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 653451206fe0baec63e9db4cce7626357bb00942
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-production-order-headers"></a>Så här skapar du ett produktionsorderhuvud
Du kan skapa en produktionsorder manuellt och första steget är då att skapa ett produktionsorderhuvud.

Produktionsorder skapas vanligtvis automatiskt av en planeringsfunktion för att uppfylla ett behov som är känt. Mer information finns i [Planering](production-planning.md).   

I det följande procedur skapas en fast planerad produktionsorder. Du kan också skapa produktionsorder med annan status.  

## <a name="to-create-a-production-order-header"></a>Så här skapar du ett produktionsorderhuvud  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Fasta planerade prod.order** och välj sedan relaterad länk.  
2.  Välj åtgärden **Ny**.  
3.  I fältet **Nr.** skriver du numret på den artikel som har beställts.  
4.  Välj produktionsorderns ursprung i fältet **Ursprungstyp**.

    Här kan du välja att skapa en familj av artiklar. Mer information finns i [Så här arbetar du med produktionsfamiljer](production-how-work-family.md).
5.  Välj artikelnummer, familj eller försäljningshuvud som produktionsordern ska skapas för i fältet **Ursprungsnr** .  
6.  Fyll i fälten **Antal** och **Förfallodatum** enligt aktuella specifikationer.  

När produktionsbehov ändras, till exempel komponenter och operationer, kan du snabbt omplanera produktionsordern. Mer information finns i [så här: Omplanera eller uppdatera produktionsorder direkt](production-how-to-replan-refresh-production-orders.md). 

## <a name="see-also"></a>Se även  
[Produktion](production-manage-manufacturing.md)    
[Ställa in Produktion](production-configure-production-processes.md)  
[Planerad](production-planning.md)      
[Lagersaldo](inventory-manage-inventory.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

