---
title: "SÅ här: Dela Dist.lageraktivitetsrader"
description: "I distributionslagerartikelinförslar, -transporter och -plockningar, samt i lagerartikelinförslar och lagerplockningar, föreslås lagerplatser för plockning och införsel av artiklar. det faktiska antalet på den lagerplats som föreslås kanske inte räcker, eller också finns det inte tillräckligt mycket plats på den föreslagna lagerplatsen för införsel av det aktuella antalet. I så fall måste du dela upp raden, så att artiklarna på en rad tas från, eller placeras på, fler än en lagerplats."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d113b83d2c4d21463e1a015e7015bc1f566652f9
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-split-warehouse-activity-lines"></a>SÅ här: Dela Dist.lageraktivitetsrader
I distributionslagerartikelinförslar, -transporter och -plockningar, samt i lagerartikelinförslar och lagerplockningar, föreslås lagerplatser för plockning och införsel av artiklar. det faktiska antalet på den lagerplats som föreslås kanske inte räcker, eller också finns det inte tillräckligt mycket plats på den föreslagna lagerplatsen för införsel av det aktuella antalet. I så fall måste du dela upp raden, så att artiklarna på en rad tas från, eller placeras på, fler än en lagerplats.  

Följande procedur gäller alla distributionslagerdokument, till exempel Dist.lager artikelinförsel, transport och plockningsrader, eller lager, artikelinförsel, transport och plockningsrader.  

## <a name="to-split-warehouse-activity-lines"></a>Att dela Dist.lageraktivitet rader  
1.  Öppna en lageraktivitetsrad där du försöker manipulera ett otillräckligt antal.  
2.  I **Ant. att hantera** fältet, ange det antal som kan hantera.  
3.  På snabbfliken **Rader** väljer du åtgärden **Åtgärder** och väljer sedan åtgärden **Funktioner** och sedan åtgärden **Dela rad**. Det visas en ny rad, som är en kopia av den ursprungliga raden, med den skillnaden att fältet **Ant. att hantera** innehåller det antal som du tog bort från den ursprungliga raden.  
4.  Tilldela den nya raden en lämplig lagerplats och zon, om du använder dirigerad artikelinförsel och plockning, eller fortsätt att dela upp raden efter behov tills du har önskat antal lagerplatser för hela kvantiteten.  

> [!NOTE]  
>  Om lagerstället är inställt på dirigerad artikelinförsel och plockning, och du delar raderna, måste du vara förtrogen med distributionslagret och kunna välja en lagerplats som passar artikelns lagringskrav och uppfyller de allmänna kraven i distributionslagerdokumentet. Du skulle till exempel inte dela en rad i ett plockningsdokument och placera några artiklar i volymlagret.  

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

