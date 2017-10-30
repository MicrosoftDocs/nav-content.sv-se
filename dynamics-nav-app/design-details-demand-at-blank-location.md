---
title: "Designdetaljer - Efterfrågan och tillgång"
description: "Detta ämne introducerar begreppet etfterfrågan, som är den gemensamma termen som vanligtvis används för alla typer av bruttobehov, t.ex försäljningsorder och komponentbehov från en produktionsorder."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
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
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="f8b62-103">Designdetaljer: Efterfrågan och tillgång</span><span class="sxs-lookup"><span data-stu-id="f8b62-103">Design Details: Demand and Supply</span></span>
<span data-ttu-id="f8b62-104">Efterfrågan är den gemensamma termen som vanligtvis används för alla typer av bruttobehov, t.ex försäljningsorder och komponentbehov från en produktionsorder.</span><span class="sxs-lookup"><span data-stu-id="f8b62-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="f8b62-105">Dessutom tillåter programmet mer tekniska typer av efterfrågan, till exempel negativt lagersaldo och inköpsreturer.</span><span class="sxs-lookup"><span data-stu-id="f8b62-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  
  
<span data-ttu-id="f8b62-106">Tillgång är den term som vanligtvis används för alla typer av positivt eller ankommande antal, t.ex. inköpsöverföringar, monteringsöverföringar, produktionsöverföringar och ankommande överföringar.</span><span class="sxs-lookup"><span data-stu-id="f8b62-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="f8b62-107">Dessutom kan en försäljningsretur också representera tillgång.</span><span class="sxs-lookup"><span data-stu-id="f8b62-107">In addition, a sales return may also represent supply.</span></span>  
  
<span data-ttu-id="f8b62-108">För att sortera ut de många källorna till efterfrågan och tillgång ordnar planeringssystemet dem på två tidslinjer som kallas lagerprofiler.</span><span class="sxs-lookup"><span data-stu-id="f8b62-108">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="f8b62-109">En profil innehåller efterfråganshändelser och den andra innehåller motsvarande tillgångshändelser.</span><span class="sxs-lookup"><span data-stu-id="f8b62-109">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="f8b62-110">Varje händelse representerar en ordernätverksenhet, till exempel en försäljningsorderrad, en artikeltransaktion eller en produktionsorderrad.</span><span class="sxs-lookup"><span data-stu-id="f8b62-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  
  
<span data-ttu-id="f8b62-111">När lagerprofiler laddas balanseras de olika uppsättningarna med efterfrågan-tillgång för att skapa ut en tillförselplan som uppfyller de angivna målen.</span><span class="sxs-lookup"><span data-stu-id="f8b62-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  
  
<span data-ttu-id="f8b62-112">Planeringsparametrar och lagernivåer är andra typer av efterfrågan och tillgång, som genomgår integrerad motkontering för att fylla på lagerartiklar.</span><span class="sxs-lookup"><span data-stu-id="f8b62-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="f8b62-113">Mer information finns i [Designdetaljer: Hantera partiformningsmetoder](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="f8b62-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f8b62-114">Se även</span><span class="sxs-lookup"><span data-stu-id="f8b62-114">See Also</span></span>  
<span data-ttu-id="f8b62-115">[Designdetaljer: Balansera efterfrågan och tillgång](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="f8b62-115">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="f8b62-116">[Designdetaljer: Centrala koncept i planeringssystemet](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="f8b62-116">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="f8b62-117">Designdetaljer: Leveransplanering</span><span class="sxs-lookup"><span data-stu-id="f8b62-117">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
