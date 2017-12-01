---
title: Designdetaljer - Lagerstyrning
description: "Det här avsnittet innehåller en översikt över design, begrepp och metoder sombakom lagerhanteringsfunktionerna i [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: c2af8902f40b01307557cef0c284308f226c183d
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-warehouse-management"></a><span data-ttu-id="65c5c-103">Designdetaljer: Lagerstyrning</span><span class="sxs-lookup"><span data-stu-id="65c5c-103">Design Details: Warehouse Management</span></span>
<span data-ttu-id="65c5c-104">Denna dokumentation visar en översikt över begrepp och principer som används i lagerstyrningsfunktioner i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="65c5c-104">This documentation gives an overview of the concepts and principles that are used in the Warehouse Management features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="65c5c-105">Den förklarar designen bakom centrala lagerfunktioner och hur lagerstyrning integreras med andra funktioner i försörjningskedjan.</span><span class="sxs-lookup"><span data-stu-id="65c5c-105">It explains the design behind central warehouse features and how warehousing integrates with other supply chain features.</span></span>  

<span data-ttu-id="65c5c-106">För att skilja mellan de olika komplexitetsnivåerna i lagerstyrningen är dokumentationen uppdelad i två allmänna grupper, grundläggande och avancerad lagerkonfigurationer, som anges med avsnittsrubriker.</span><span class="sxs-lookup"><span data-stu-id="65c5c-106">To differentiate the different complexity levels of the warehousing, this documentation is divided into two general groups, Basic and Advanced warehouse configurations, indicated by section titles.</span></span> <span data-ttu-id="65c5c-107">Den här enkla differentieringen täcker olika komplexitetsnivåer som definieras av produktpartiklar och lagerplatsinställningar.</span><span class="sxs-lookup"><span data-stu-id="65c5c-107">This simple differentiation covers different complexity levels as defined by product granules and location setup.</span></span> <span data-ttu-id="65c5c-108">Mer information finns i [Designdetaljer: Lagerstyrningsinställningar](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="65c5c-108">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="65c5c-109">I det här avsnittet</span><span class="sxs-lookup"><span data-stu-id="65c5c-109">In This Section</span></span>  
[<span data-ttu-id="65c5c-110">Designdetaljer: Översikt över distributionslager</span><span class="sxs-lookup"><span data-stu-id="65c5c-110">Design Details: Warehouse Overview</span></span>](design-details-warehouse-overview.md)  
[<span data-ttu-id="65c5c-111">Designdetaljer: Lagerstyrningsinställningar</span><span class="sxs-lookup"><span data-stu-id="65c5c-111">Design Details: Warehouse Setup</span></span>](design-details-warehouse-setup.md)  
[<span data-ttu-id="65c5c-112">Designdetaljer: Ankommande distributionslagerflöde</span><span class="sxs-lookup"><span data-stu-id="65c5c-112">Design Details: Inbound Warehouse Flow</span></span>](design-details-inbound-warehouse-flow.md)  
[<span data-ttu-id="65c5c-113">Designdetaljer: Interna distributionslagerflöden</span><span class="sxs-lookup"><span data-stu-id="65c5c-113">Design Details: Internal Warehouse Flows</span></span>](design-details-internal-warehouse-flows.md)  
[<span data-ttu-id="65c5c-114">Designdetaljer: Disposition i distributionslagret</span><span class="sxs-lookup"><span data-stu-id="65c5c-114">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="65c5c-115">Designdetaljer: Avgående distributionslagerflöde</span><span class="sxs-lookup"><span data-stu-id="65c5c-115">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="65c5c-116">Designdetaljer: Integrering med lager</span><span class="sxs-lookup"><span data-stu-id="65c5c-116">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)

