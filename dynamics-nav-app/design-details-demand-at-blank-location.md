---
title: "Designdetaljer - Efterfrågan och tillgång"
description: "Detta ämne introducerar begreppet etfterfrågan, som är den gemensamma termen som vanligtvis används för alla typer av bruttobehov, t.ex försäljningsorder och komponentbehov från en produktionsorder."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d744b55835f5553e249a536e0fca0eb0046fda7b
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-demand-and-supply"></a>Designdetaljer: Efterfrågan och tillgång
Efterfrågan är den gemensamma termen som vanligtvis används för alla typer av bruttobehov, t.ex försäljningsorder och komponentbehov från en produktionsorder. Dessutom tillåter programmet mer tekniska typer av efterfrågan, till exempel negativt lagersaldo och inköpsreturer.  
  
Tillgång är den term som vanligtvis används för alla typer av positivt eller ankommande antal, t.ex. inköpsöverföringar, monteringsöverföringar, produktionsöverföringar och ankommande överföringar. Dessutom kan en försäljningsretur också representera tillgång.  
  
För att sortera ut de många källorna till efterfrågan och tillgång ordnar planeringssystemet dem på två tidslinjer som kallas lagerprofiler. En profil innehåller efterfråganshändelser och den andra innehåller motsvarande tillgångshändelser. Varje händelse representerar en ordernätverksenhet, till exempel en försäljningsorderrad, en artikeltransaktion eller en produktionsorderrad.  
  
När lagerprofiler laddas balanseras de olika uppsättningarna med efterfrågan-tillgång för att skapa ut en tillförselplan som uppfyller de angivna målen.  
  
Planeringsparametrar och lagernivåer är andra typer av efterfrågan och tillgång, som genomgår integrerad motkontering för att fylla på lagerartiklar. Mer information finns i [Designdetaljer: Hantera partiformningsmetoder](design-details-handling-reordering-policies.md).  
  
## <a name="see-also"></a>Se även  
[Designdetaljer: Balansera efterfrågan och tillgång](design-details-balancing-demand-and-supply.md)   
[Designdetaljer: Centrala koncept i planeringssystemet](design-details-central-concepts-of-the-planning-system.md)   
[Designdetaljer: Leveransplanering](design-details-supply-planning.md)
