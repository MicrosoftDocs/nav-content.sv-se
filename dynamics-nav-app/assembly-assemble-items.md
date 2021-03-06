---
title: Monteringshantering
description: "För att hantera företag som levererar till produkter till kunder genom att slå ihop komponenter i enkla processer utan behov av produktionsfunktionen, innehåller  funktionen för att sammanställa artiklar som integreras med befintliga funktioner, till exempel försäljning, planering, reservationer och lagerhantering."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4e0490e63268edd68a22e61b25311aa133c507c1
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="assembly-management"></a>Monteringshantering
För att hantera företag som levererar till produkter till kunder genom att slå ihop komponenter i enkla processer utan behov av produktionsfunktionen, innehåller [!INCLUDE[d365fin](includes/d365fin_md.md)] funktionen för att sammanställa artiklar som integreras med befintliga funktioner, till exempel försäljning, planering, reservationer och lagerhantering.  

 En monteringsartikel definieras som en säljbar artiklar som innehåller en monteringsstruktur. Mer information finns i [Så här arbetar du med strukturer](inventory-how-work-BOMs.md).

 Monteringsorder är den interna order, som en produktionsorder, som används för att hantera monteringsprocessen och för att koppla försäljningskraven med relevanta lageraktiviteter. Monteringsorder skiljer sig från andra ordertyper, eftersom de avser både förbrukning och utflöde, när de bokförs. Monteringsorderhuvudet reagerar på samma sätt som en orderrad, och monteringsorderrader reagerar på samma sätt som förbrukningsjournalrader.  

 För att stödja en just-i-tid-lagerstrategi och kapaciteten för att anpassa produkter till kundförfrågan, kan monteringsorder automatiskt skapas och kopplas så snart försäljningsorderraden skapas. Kopplingen mellan försäljningsbehov och monteringsleveransen gör att försäljningsorderhandläggare kan anpassa monteringsartikeln löpande, ge löfte om leveransdatum enligt komponentdisposition och att bokföra utflödet och utleveransen av monterade artiklar direkt monterad utifrån försäljningsorder gränssnitt. Mer information finns i [så här: sälja artiklar monterde mot order](assembly-how-to-sell-items-assembled-to-order.md).  

 På en orderrad kan du sälja en kvantitet som är tillgänglig, och måste plockas från lagret tillsammans med ett antal som måste monteras till i ordern. Det finns vissa regler för att styra distributionen på sådana antal för att se till att antalet för montering mot kundorder åsidosätter lagersaldot i en delbetalning leverans. Mer information finns i avsnittet Kombinationsscenarion i [Förstå montering mot order och montering mot lager](assembly-assemble-to-order-or-assemble-to-stock.md).  

 Särskild funktioner finns för att styra fältet av montering mot kundorder. När antalet för montering mot kundorder är klar för utleverans, lagerarbetaren i kostnad bokför en lagerplockning för försäljningsorderraden i fråga. Detta skapar en lagerförflyttning för komponenterna, bokför monteringsutflöde och försäljningsorderleveransen. Mer information finns i avsnittet ”hantera artiklar för montering mot kundorder i lagerplockningar” i [Så här plockar du artiklar med Lagerplockning](warehouse-how-to-pick-items-with-inventory-picks.md).

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.   

|**Om du vill**|**Gå till**|  
|------------|-------------|  
|Lära dig mer om skillnaden mellan monterings artiklar direkt före leverans försäljningsorder och monterings artiklar som används för lagret.|[Förstå montering mot kundorder och montering mot lager](assembly-assemble-to-order-or-assemble-to-stock.md)|
|Fyll i fälten på lagerställekort och i lagerinställningar för att definiera hur artiklar överförs till och från monteringsavdelningen.|[Så här: Ställa in grundläggande dist.lager med operationsområden](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)|
|Anpassa en monteringsartikel till ett kundkrav under försäljningsprocessen och konvertera till en försäljning när den godkänns.|[Så här skapar du en offert för montering mot kundorder-försäljning](assembly-how-to-quote-an-assemble-to-order-sale.md)|
|Kombinera komponenter för att skapa en artikel i ett enkelt behandling till order eller lager.|[Så här: Artiklar monteras](assembly-how-to-assemble-items.md)|  
|Sälj monteringsartiklar som inte är tillgängliga genom att skapa en länkad monteringsorder för att tillhandahålla hela eller delvisa försäljningsorderantal.|[Så här säljer du en artikel som monterats mot kundorder](assembly-how-to-sell-items-assembled-to-order.md)|
|Om några artiklar för montering mot kundorder redan finns i lager kan du dra av antalet från monteringsordern och reservera det från lagret.|[Så här säljer du lagerartiklar i flöde för montering mot kundorder](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md)|  
|Du kan få en monteringsorder att automatiskt tillhandahålla en del av, eller hela, försäljningsorderns antal när du säljer monteringsartiklar från lagret när inte alla artiklar är tillgängliga.|[Så här säljer du artiklar för montering mot kundorder och lagerartiklar ihop](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md)|
|Ångra en bokförd monteringsorder, till exempel för att ordern har bokförts med misstag som måste rättas.|[Så här: Ångra monteringbokning](assembly-how-to-undo-assembly-posting.md)|
|Lära dig mer om skillnaden mellan monteringsstrukturer och produktionsstrukturer och de berörda bearbeta skillnaderna.|[Så här arbetar du med strukturer](inventory-how-work-BOMs.md)|
|Lära dig hur tillverkningsförbrukning och utflöde hanteras, när du bokför monteringsorder och utifrån hur artikel och resurskostnaderna är behandlats och biztalk-dokumenten distribueras till redovisningen.|[Designdetaljer: Bokföring av monteringsorder](design-details-assembly-order-posting.md)|  

## <a name="see-also"></a>Se även  
[Så här arbetar du med strukturer](inventory-how-work-BOMs.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

