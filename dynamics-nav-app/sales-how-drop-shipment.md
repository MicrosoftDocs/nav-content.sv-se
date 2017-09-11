---
title: "Så här utför du direktleveranser"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: a726c8c24d8f843b33b4df4d85ad2b5eab3790e7
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="b66e5-102">Så här utför du direktleveranser</span><span class="sxs-lookup"><span data-stu-id="b66e5-102">How to: Make Drop Shipments</span></span>
<span data-ttu-id="b66e5-103">Direktleverans innebär leverans av artiklar från någon av företagets leverantörer direkt till någon av företagets kunder.</span><span class="sxs-lookup"><span data-stu-id="b66e5-103">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="b66e5-104">När en försäljningsorder är markerad för direktleverans, och du skapar en inköpsorder där du anger kunden i fältet **Förs.kundnr.**</span><span class="sxs-lookup"><span data-stu-id="b66e5-104">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="b66e5-105">kan du länka de två dokumenten och därmed instruera leverantören att leverera direkt till kunden.</span><span class="sxs-lookup"><span data-stu-id="b66e5-105">field, then you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="b66e5-106">Så här skapar du försäljningsorder för direktleveranser</span><span class="sxs-lookup"><span data-stu-id="b66e5-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="b66e5-107">För att förbereda en direktleverans skapar du en försäljningsorder för en artikel som vanligt, förutom att du måste ange på försäljningsraden att försäljningen kräver direktleverans.</span><span class="sxs-lookup"><span data-stu-id="b66e5-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="b66e5-108">Skapa en försäljningsorder för en artikel.</span><span class="sxs-lookup"><span data-stu-id="b66e5-108">Create a sales order for an item.</span></span> <span data-ttu-id="b66e5-109">Mer information finns i [Så här säljer du produkter](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="b66e5-109">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="b66e5-110">På försäljningsorderraden för direktleveransartikeln markerar du kryssrutan **Direktleverans**.</span><span class="sxs-lookup"><span data-stu-id="b66e5-110">On the sales order line for the drop-shipment item, select the **Drop Shipment** check box.</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="b66e5-111">Så här skapar du inköpsorder för direktleverans</span><span class="sxs-lookup"><span data-stu-id="b66e5-111">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="b66e5-112">Om du vill förbereda en direktleverans för den artikel som ska säljas kan du skapa en inköpsorder som vanligt förutom att du måste ange på inköpsordern att den ska levereras till din kund och inte till dig själv.</span><span class="sxs-lookup"><span data-stu-id="b66e5-112">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="b66e5-113">Skapa en inköpsorder.</span><span class="sxs-lookup"><span data-stu-id="b66e5-113">Create a purchase order.</span></span> <span data-ttu-id="b66e5-114">Fyll inte i några fält på raderna.</span><span class="sxs-lookup"><span data-stu-id="b66e5-114">Do not fill any fields on the lines.</span></span> <span data-ttu-id="b66e5-115">Mer information finns i [Så här registrerar du inköp](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="b66e5-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="b66e5-116">I fältet **Förs.kundnr.**</span><span class="sxs-lookup"><span data-stu-id="b66e5-116">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="b66e5-117">markerar du kunden som du säljer till.</span><span class="sxs-lookup"><span data-stu-id="b66e5-117">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="b66e5-118">Välj åtgärden **Direktleverans** och välj sedan åtgärden **Hämta förs.order**.</span><span class="sxs-lookup"><span data-stu-id="b66e5-118">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="b66e5-119">I fönstret **Försäljningslista** väljer du den försäljningsorder som du förberedde i avsnittet "Så här skapar du försäljningsorder för direktleveranser".</span><span class="sxs-lookup"><span data-stu-id="b66e5-119">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="b66e5-120">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="b66e5-120">Choose the **OK** button.</span></span>

<span data-ttu-id="b66e5-121">Radinformationen från försäljningsordern infogas på inköpsorderraden.</span><span class="sxs-lookup"><span data-stu-id="b66e5-121">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="b66e5-122">Du kan nu instruera leverantören att leverera artiklarna till kunden, till exempel genom att e-posta inköpsordern som en PDF.</span><span class="sxs-lookup"><span data-stu-id="b66e5-122">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="b66e5-123">Om du vill se den länkade inköpsordern från försäljningsordern</span><span class="sxs-lookup"><span data-stu-id="b66e5-123">To view the linked purchase order from the sales order</span></span>
1. <span data-ttu-id="b66e5-124">Markera försäljningsordern direktleverans, välj åtgärden **Order**, välj åtgärden **Direktleverans** och välj sedan åtgärden **Inköpsorder**.</span><span class="sxs-lookup"><span data-stu-id="b66e5-124">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

<span data-ttu-id="b66e5-125">Den länkade inköpsordern öppnas.</span><span class="sxs-lookup"><span data-stu-id="b66e5-125">The linked purchase order opens.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="b66e5-126">Så här bokför du en direktutleverans</span><span class="sxs-lookup"><span data-stu-id="b66e5-126">To post a drop shipment</span></span>
<span data-ttu-id="b66e5-127">När leverantören har levererat artiklarna kan du bokföra försäljningsordern som levererad.</span><span class="sxs-lookup"><span data-stu-id="b66e5-127">When the vendor has shipped the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="b66e5-128">Du kan också bokföra inköpsordern, men endast med alternativet **Ta emot** tills försäljningsordern har fakturerats.</span><span class="sxs-lookup"><span data-stu-id="b66e5-128">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>
1. <span data-ttu-id="b66e5-129">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Försäljningsorder** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="b66e5-129">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="b66e5-130">Öppna den försäljningsorder som du skapade i avsnittet "Att skapa en försäljningsorder för en direktleverans" .</span><span class="sxs-lookup"><span data-stu-id="b66e5-130">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="b66e5-131">I fältet **Levereras antal** anger du hur många av orderkvantiteten som ska levereras, hela eller delvis orderkvantitet.</span><span class="sxs-lookup"><span data-stu-id="b66e5-131">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
3. <span data-ttu-id="b66e5-132">Välj åtgärden **Bokför** eller **Bokför och skicka**.</span><span class="sxs-lookup"><span data-stu-id="b66e5-132">Choose the **Post** or **Post and Send** action.</span></span>
4. <span data-ttu-id="b66e5-133">Markera antingen alternativet **Leverera** för att fakturera senare eller alternativet **Leverera och fakturera** för att fakturera omedelbart.</span><span class="sxs-lookup"><span data-stu-id="b66e5-133">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="b66e5-134">Se även</span><span class="sxs-lookup"><span data-stu-id="b66e5-134">See Also</span></span>
<span data-ttu-id="b66e5-135">[Så här säljer du produkter](sales-how-sell-products.md)  </span><span class="sxs-lookup"><span data-stu-id="b66e5-135">[How to: Sell Products](sales-how-sell-products.md)  </span></span>  
[<span data-ttu-id="b66e5-136">Så här registrerar du inköp</span><span class="sxs-lookup"><span data-stu-id="b66e5-136">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="b66e5-137">Hantera försäljning</span><span class="sxs-lookup"><span data-stu-id="b66e5-137">Manage Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="b66e5-138">[Hantera lager](inventory-manage-inventory.md)    </span><span class="sxs-lookup"><span data-stu-id="b66e5-138">[Manage Inventory](inventory-manage-inventory.md)    </span></span>  
[<span data-ttu-id="b66e5-139">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="b66e5-139">Work with Dynamics NAV</span></span>](ui-work-product.md)

