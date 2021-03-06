---
title: "Så här kan du planera projektorder"
description: "Den här planeringsåtgärden påbörjas från en försäljningsorder, och inställningarna i fönstret **Förs.orderplanering** används. När du har skapat en projektproduktionsorder kan du planera den ytterligare med hjälp av fönstret **Orderplanering**."
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
ms.openlocfilehash: a03cdaf16b25cbcf030e9a33c538ea3df96a1fe9
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-project-orders"></a>Så här kan du planera projektorder
Den här planeringsåtgärden påbörjas från en försäljningsorder, och inställningarna i fönstret **Förs.orderplanering** används. När du har skapat en projektproduktionsorder kan du planera den ytterligare med hjälp av fönstret **Orderplanering**.  

## <a name="to-create-a-project-production-order"></a>Så här skapar du en projektproduktionsorder  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningsorder** och välj sedan relaterad länk.  
2.  Markera den försäljningsorder som motsvarar produktionsprojektet och välj sedan åtgärden **planering**.  
4.  I fönstret **Förs.orderplanering** väljer du åtgärden **Skapa prod.order**.  
5.  I fönstret **Skapa order från försäljning**, i fältet **Ordertyp** markerar du **Prod.order per order**.  
6.  Välj **Ja**.  
7.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Produktionsorder** och välj sedan relaterad länk.
8. Öppna den produktionsorder som du skapade nyss.  

    Observera att fältet **Ursprungstyp** för produktionsordern visas **Försäljningshuvud**, och ordern innehåller flera rader (en för varje försäljningsradartikel som måste skapas).  
9. Välj åtgärden **Planerad**.
10. I fönstret **Orderplanering** väljer du åtgärden **uppdatera** för att beräkna det nya behovet.  

Orderhuvudraden för projektordern visas, och alla rader med ouppfyllda behov expanderas under den. Även om produktionsordern innehåller rader för flera producerade artiklar så visas det totala behovet för alla produktionsorderrader under en orderhuvudrad i fönstret **Orderplanering**, och det ursprungliga kundnamnet visas. Du kan nu fortsätta med att planera för behovet enligt beskrivningen i [Så här: Planera för nya behov per order](production-how-to-plan-for-new-demand.md).  

> [!NOTE]  
>  Behovsrader i projektproduktionsordern, som har **Prod. Order** i sitt **Återanskaffningssystem** -fält, motsvarar underliggande produktionsorder. När du har genererats dessa produktionsorder, måste du återigen beräkna en plan i fönstret **Orderplanering** för att identifiera några ouppfyllda komponentbehov för dem. I så fall visas de som behovsrader under en typisk rad i ett produktionsorderhuvud, dvs. att projektrelationen inte längre visas i fönstret. Men om du använder orderspårningsfunktionen kan du se bakåt och framåt i alla leveransorder som skapas under den ursprungliga försäljningsordern.  

## <a name="see-also"></a>Se även
[Planerad](production-planning.md)   
[Ställa in Produktion](production-configure-production-processes.md)  
[Produktion](production-manage-manufacturing.md)    
[Lagersaldo](inventory-manage-inventory.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Designdetaljer: Leveransplanering](design-details-supply-planning.md)   
[Skapa metodtips: leveransplanering](setup-best-practices-supply-planning.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

