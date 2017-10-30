---
title: "Så här skapar du en offert för montering mot kundorder-försäljning"
description: "Du kan använda monteringshantering för att anpassa en monteringsartikel till ett kundkrav under försäljningsprocessen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ee62ddff43778bd81d4ed65c2dcdd466b79e422
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a>Så här skapar du en offert för montering mot kundorder-försäljning
Du kan använda monteringshantering för att anpassa en monteringsartikel till ett kundkrav under försäljningsprocessen. Mer information finns i [så här: sälja artiklar monterde mot order](assembly-how-to-sell-items-assembled-to-order.md).  

När du säljer någon annan typ av artikel kan du också skapa en försäljningsoffert för en anpassad monteringsartikel innan du omvandlar den till en försäljningsorder. Den här processen involverar flera extra steg i jämförelse med att skapa en vanlig försäljningsoffert. Den använder en variation av en kopplad monteringsorder, dvs. en monteringsoffert.

> [!NOTE]  
>  Precis som på alla typer av offerter används inte antalet på monteringsoffertar för tillgänglighet, planering eller reservationer.  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a>Så här skapar du en försäljningsoffert för en artikel för montering mot kundorder  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningsoffert** och välj sedan relaterad länk.  
2.  Skapa en försäljningsoffertrad med en rad för en monteringsartikel. För mer information finns i [Så här gör du erbjudanden](sales-how-make-offers.md).  
3.  I fältet **Antal att montera mot kundorder** anger du hela antalet.

    > [!NOTE]  
    >  Du bör inte erbjuda ett delantal i offerten. Därför måste du ange samma antal som du angett i fältet **Antal** på försäljningsoffertraden.  

4.  På snabbfliken **Rader** väljer du **Rad**, **Montering mot kundorder** och sedan **Montering mot kundorderrader**. Alternativt kan du välja fältet **Antal att montera mot kundorder** på raden.  
5.  I fönstret **Montering mot kundorderrader** granskar eller ändrar du monteringsorderrader enligt den offert som kunden begär. Om du vill ha mer information kan du välja åtgärden **Visa dokument** för att öppna hela avropsordern för offerten. Du kan inte ändra innehållet i de flesta fält, och du kan inte bokföra.  
6.  När du har justerat monteringsorderraderna enligt offerten stänger du fönstret **Montering mot kundorderrader** så att du kommer tillbaka till fönstret **Försäljningsoffert**.  
7.  Om kunden accepterar offerten skapar du en försäljningsorder för den offererade monteringsartikeln. För mer information finns i [Så här gör du erbjudanden](sales-how-make-offers.md). Den länkade monteringsofferten och eventuella anpassningar är kopplad till den nya försäljningsordern så att artikelmontering eller -försäljning kan förberedas.  

## <a name="see-also"></a>Se även  
[Monteringshantering](assembly-assemble-items.md)  
[Så här arbetar du med strukturer](inventory-how-work-BOMs.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

