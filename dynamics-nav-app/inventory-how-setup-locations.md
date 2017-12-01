---
title: "Skapa ett lagerställekort och definiera överföringsflöden"
description: "Du kan skapa ett lagerställekort för varje plats som du vill lagra lagerartiklar, till exempel lager eller distributionscenter, och ange flöden för överföring av artiklar mellan olika lagerställen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 2a0d35e11b6a0ee480cf0034c885157fe1de3916
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-locations"></a><span data-ttu-id="db1b5-103">Så här skapar du lagerställen</span><span class="sxs-lookup"><span data-stu-id="db1b5-103">How to: Set Up Locations</span></span>
<span data-ttu-id="db1b5-104">Om du köper, lagrar eller säljer artiklar på mer än en plats eller ett lager, måste du ställa in varje plats med ett lagerställeskort och definiera överföringsflöden.</span><span class="sxs-lookup"><span data-stu-id="db1b5-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="db1b5-105">Du kan sedan skapa dokumentrader för ett visst lagerställe, visa disposition per lagerställe och överföra lager mellan olika lagerställen.</span><span class="sxs-lookup"><span data-stu-id="db1b5-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="db1b5-106">Mer information finns i [Administrera projekt](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="db1b5-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="db1b5-107">Skapa ett nytt lagerställeskort</span><span class="sxs-lookup"><span data-stu-id="db1b5-107">To create a location card</span></span>
1. <span data-ttu-id="db1b5-108">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="db1b5-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="db1b5-109">Välj åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="db1b5-109">Choose the **New** action.</span></span>
3. <span data-ttu-id="db1b5-110">I fönstret **Lagerställeskort** fyller du i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="db1b5-110">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="db1b5-111">Upprepa steg 2 och 3 för varje lagerställe där du vill bedriva lagerhållning.</span><span class="sxs-lookup"><span data-stu-id="db1b5-111">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="db1b5-112">Många fält på lagerställekortet hänvisar till hanteringen av artiklar i ingående och utgående lagerprocesser.</span><span class="sxs-lookup"><span data-stu-id="db1b5-112">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="db1b5-113">Mer information finns i [Ställa in Lagerstyrning](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="db1b5-113">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="db1b5-114">Så här skapar du ett överföringsflöde</span><span class="sxs-lookup"><span data-stu-id="db1b5-114">To create a transfer route</span></span>
1. <span data-ttu-id="db1b5-115">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Överföringsflöden** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="db1b5-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="db1b5-116">Alternativt kan du i fönstret **Lagerställekort** välja åtgärden **Överföringsflöden**.</span><span class="sxs-lookup"><span data-stu-id="db1b5-116">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="db1b5-117">Välj åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="db1b5-117">Choose the **New** action.</span></span>
4. <span data-ttu-id="db1b5-118">I fönstret **Lagerställeskort** fyller du i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="db1b5-118">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="db1b5-119">Du kan nu överföra lagerartiklar mellan två lagerställen.</span><span class="sxs-lookup"><span data-stu-id="db1b5-119">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="db1b5-120">Mer information finns i [Så här överför du lager mellan olika lagerställen](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="db1b5-120">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="db1b5-121">Se även</span><span class="sxs-lookup"><span data-stu-id="db1b5-121">See Also</span></span>
[<span data-ttu-id="db1b5-122">Hantera lager</span><span class="sxs-lookup"><span data-stu-id="db1b5-122">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="db1b5-123">[Så här överför du lager mellan olika lagerställen](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="db1b5-123">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="db1b5-124">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="db1b5-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="db1b5-125">[Anpassa [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span><span class="sxs-lookup"><span data-stu-id="db1b5-125">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span></span>  
[<span data-ttu-id="db1b5-126">Allmänna affärsfunktioner</span><span class="sxs-lookup"><span data-stu-id="db1b5-126">General Business Functionality</span></span>](ui-across-business-areas.md)

