---
title: "Så här skapar du specialorder"
description: "Du kan skapa en specialorder för en specifik artikel som inte finns i lagret och som ska levereras till en specifik kund. Leverantören levererar artikeln till distributionslagret så att du sedan kan leverera den till kunden, som en enskild leverans eller tillsammans med andra artiklar på en annan order."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 596b9a5638e551a8165429308a68a4c8dddb6a06
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-create-special-orders"></a><span data-ttu-id="9d202-104">Så här skapar du specialorder</span><span class="sxs-lookup"><span data-stu-id="9d202-104">How to: Create Special Orders</span></span>
<span data-ttu-id="9d202-105">Du kan skapa en specialorder för en specifik artikel som inte finns i lagret och som ska levereras till en specifik kund.</span><span class="sxs-lookup"><span data-stu-id="9d202-105">You can create a special order for a specific nonstock item to be shipped to a specific customer.</span></span> <span data-ttu-id="9d202-106">Leverantören levererar artikeln till distributionslagret så att du sedan kan leverera den till kunden, som en enskild leverans eller tillsammans med andra artiklar på en annan order.</span><span class="sxs-lookup"><span data-stu-id="9d202-106">Your vendor ships the item to your warehouse and you can then ship the item on to your customer either independently or together with other items on another order.</span></span>  

<span data-ttu-id="9d202-107">Specialorder anger att inköps- och försäljningsordern är länkade för att säkerställa att den specifika ej lagerförda artikeln plockas och levereras till kunden.</span><span class="sxs-lookup"><span data-stu-id="9d202-107">Special orders imply that the purchase and sales order are linked to ensure that the specific nonstock item is picked and delivered to the customer.</span></span>  

<span data-ttu-id="9d202-108">Innan den här funktionen kan användas måste de kund-, leverantörs- och artikelkort som behövs för ordern läggas upp.</span><span class="sxs-lookup"><span data-stu-id="9d202-108">Before you can use this feature, you must first set up the customer, vendor, and item cards necessary for the order.</span></span>  

## <a name="to-create-a-special-order"></a><span data-ttu-id="9d202-109">Så här skapar du en specialorder</span><span class="sxs-lookup"><span data-stu-id="9d202-109">To create a special order</span></span>  
1.  <span data-ttu-id="9d202-110">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningsorder** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9d202-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Order**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9d202-111">Välj åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="9d202-111">Choose the **New** action.</span></span> <span data-ttu-id="9d202-112">Skapa och fyll i  försäljningsorder för artikeln.</span><span class="sxs-lookup"><span data-stu-id="9d202-112">Create and fill in a  sales order for the item.</span></span> <span data-ttu-id="9d202-113">Mer information finns i [Så här säljer du produkter](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="9d202-113">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
3.  <span data-ttu-id="9d202-114">Fyll i försäljningsraden på snabbfliken **Rader** .</span><span class="sxs-lookup"><span data-stu-id="9d202-114">On the **Lines** FastTab, fill in the sales line.</span></span> <span data-ttu-id="9d202-115">I fältet **Inköpskod**, välj en inköpskod som har fältet **Specialorder** markerat.</span><span class="sxs-lookup"><span data-stu-id="9d202-115">In the **Purchasing Code** field, select a purchasing code that has the **Special Order** field selected.</span></span>

    <span data-ttu-id="9d202-116">Därefter måste du skapa en inköpsorder från ett inköpsförslag.</span><span class="sxs-lookup"><span data-stu-id="9d202-116">You must now create a purchase order from a requisition worksheet.</span></span>  
4. <span data-ttu-id="9d202-117">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inköpsförslag** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9d202-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Requisition Worksheet**, and then choose the related link.</span></span>  
5. <span data-ttu-id="9d202-118">Välj åtgärden **Specialorder** och väljer sedan åtgärden **Hämta förs.order**.</span><span class="sxs-lookup"><span data-stu-id="9d202-118">Choose the **Special Order** action, and then choose the **Get Sales Orders** action.</span></span>  
6.  <span data-ttu-id="9d202-119">I fönstret **Hämta förs.order** visar resultat där **Verifikationsnr** är numret på försäljningsordern.</span><span class="sxs-lookup"><span data-stu-id="9d202-119">In the **Get Sales Orders** window, show results where the **Document No.** is the sales order number.</span></span> <span data-ttu-id="9d202-120">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d202-120">Choose the **OK** button.</span></span> <span data-ttu-id="9d202-121">En inköpsförslagsrad skapas för artikeln.</span><span class="sxs-lookup"><span data-stu-id="9d202-121">A requisition worksheet line is created for the item.</span></span>  
7.  <span data-ttu-id="9d202-122">På inköpsförslagsraden, i fältet **Åtgärdsmeddelande**, väljer du **Ny**.</span><span class="sxs-lookup"><span data-stu-id="9d202-122">On the requisition worksheet line, in the **Action Message** field, select **New**.</span></span>  
8.  <span data-ttu-id="9d202-123">I fönstret **Inköpsförslag** väljer du åtgärden **Verkställ åtgärdsmeddelande**.</span><span class="sxs-lookup"><span data-stu-id="9d202-123">In the **Req. Worksheet** window, choose the **Carry Out Action Message** action.</span></span> <span data-ttu-id="9d202-124">Fönstret **Skapa inköpsorder** visas.</span><span class="sxs-lookup"><span data-stu-id="9d202-124">The **Carry Out Action Msg. - Req.** window opens.</span></span> <span data-ttu-id="9d202-125">Välj knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d202-125">Choose the **OK** button.</span></span>  

    <span data-ttu-id="9d202-126">Du får meddelande om att inköpsorderna har skapats.</span><span class="sxs-lookup"><span data-stu-id="9d202-126">A message appears telling you that the purchase orders have been created.</span></span> <span data-ttu-id="9d202-127">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d202-127">Choost the **OK** button.</span></span>  

<span data-ttu-id="9d202-128">En inköpsorder som skapas som en specialorder för en försäljningsorder respekteras av planeringssystemet när behov och tillgång balanseras.</span><span class="sxs-lookup"><span data-stu-id="9d202-128">A purchase order created as a special order for a sales order is respected by the planning system as it balances demand and supply.</span></span> <span data-ttu-id="9d202-129">Det innebär att inköpsordern (tillgång) förblir länkad till försäljningsordern (behov) även om inköpsorden kan tillgodose ett annat, tidigare behov.</span><span class="sxs-lookup"><span data-stu-id="9d202-129">That is, the purchase order (supply) remains linked to the sales order (demand), even if that purchase order could supply another earlier demand.</span></span> <span data-ttu-id="9d202-130">Mer information finns i [Designdetaljer: Partiformningsmetoder](design-details-reservation-order-tracking-and-action-messaging.md).</span><span class="sxs-lookup"><span data-stu-id="9d202-130">For more information, see [Design Details: Reordering Policies](design-details-reservation-order-tracking-and-action-messaging.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9d202-131">Du kan använda funktionen Specialorder om artikeln redan har reserverats.</span><span class="sxs-lookup"><span data-stu-id="9d202-131">You cannot use the special order functionality if the item is already reserved.</span></span> <span data-ttu-id="9d202-132">Därför, för artiklar som säljs på särskilda order, kontrollera att fältet **Reservera** på artikelkortet har angetts till **alltid**.</span><span class="sxs-lookup"><span data-stu-id="9d202-132">Therefore, for items that are sold on special orders, make sure the **Reserve** field on the item card is not set to **Always**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9d202-133">Se även</span><span class="sxs-lookup"><span data-stu-id="9d202-133">See Also</span></span>  
[<span data-ttu-id="9d202-134">Så här arbetar du med Ej lagerförda artiklar</span><span class="sxs-lookup"><span data-stu-id="9d202-134">How to: Work with Nonstock Items</span></span>](inventory-how-work-nonstock-items.md)  
[<span data-ttu-id="9d202-135">Försäljning</span><span class="sxs-lookup"><span data-stu-id="9d202-135">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="9d202-136">[Så här utför du direktleveranser](sales-how-drop-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="9d202-136">[How to: Make Drop Shipments](sales-how-drop-shipment.md) </span></span>  
[<span data-ttu-id="9d202-137">Designdetaljer: Partiformningsmetoder</span><span class="sxs-lookup"><span data-stu-id="9d202-137">Design Details: Reordering Policies</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="9d202-138">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9d202-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

