---
title: "Så här: Tilldela standardlagerplatser till artiklar"
description: "Om du använder lagerplatser för ett lagerställe blir det mycket enklare för dig att leverera, inleverera och flytta artiklar om du tilldelar dem standardlagerplatser. När en artikel tilldelas en standardlagerplats kommer denna lagerplats att föreslås varje gång du påbörjar en transaktion för artikeln."
documentationcenter: 
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
ms.openlocfilehash: 7cec85ca0e564f7591534c4f18a1b5e0a1fe62a5
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-assign-default-bins-to-items"></a><span data-ttu-id="9c7c4-104">Så här: Tilldela standardlagerplatser till artiklar</span><span class="sxs-lookup"><span data-stu-id="9c7c4-104">How to: Assign Default Bins to Items</span></span>
<span data-ttu-id="9c7c4-105">Om du använder lagerplatser för ett lagerställe blir det mycket enklare för dig att leverera, inleverera och flytta artiklar om du tilldelar dem standardlagerplatser.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="9c7c4-106">När en artikel tilldelas en standardlagerplats kommer denna lagerplats att föreslås varje gång du påbörjar en transaktion för artikeln.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="9c7c4-107">Standardlagerplatser definieras i fönstret **Lagerplatsinnehåll**.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-107">Default bins are defined in the **Bin Content** window.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="9c7c4-108">Så här tilldelar du en standardlagerplats till en artikel</span><span class="sxs-lookup"><span data-stu-id="9c7c4-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="9c7c4-109">Välj ikonen ![Sök efter sidan eller rapporten](media/ui-search/search_small.png "ikonen Sök efter sidan eller rapporten"), ange **Lagerplatsinnehålluppl förslag** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span></span>  
2.  <span data-ttu-id="9c7c4-110">Fyll i lagerplatskoden och information om artiklar för respektive lagerplats som du vill ange som standard för en artikel.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="9c7c4-111">Se till att välja **Standard** här fältet.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="9c7c4-112">Välj åtgärden **Skapa lagerplatsinnehåll**.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="9c7c4-113">Din artikel tilldelas nu standardlagerplatser.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9c7c4-114">Vid införsel av artiklar som inte har tilldelats någon standardlagerplats, kommer den lagerplats där artikeln införs att anges som standardlagerplats.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="9c7c4-115">Så här ändrar du standardlagerplatser en artikel</span><span class="sxs-lookup"><span data-stu-id="9c7c4-115">To change the default bin for an item</span></span>  
<span data-ttu-id="9c7c4-116">Ibland kan det bli nödvändigt att ändra tilldelningen av standardlagerplats för en viss artikel, eller tilldela en ny artikel en standardlagerplats.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="9c7c4-117">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerplatsinnehåll** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Contents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9c7c4-118">Välj tillämplig lagerställekod i fältet **Lagerställefilter**.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="9c7c4-119">Sök efter aktuell post för standardlagerplatsinnehåll för artikeln och avmarkera kryssrutan **Standardlagerplats**.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="9c7c4-120">Sök efter raden för lagerplatsinnehåll för den lagerplats som du vill använda som ny standardlagerplats.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="9c7c4-121">Markera kryssrutan **Standardlagerplats**.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9c7c4-122">När en artikel införs för första gången och den inte har tilldelats någon standardlagerplats, kommer den lagerplats där artikeln införs att anges som standardlagerplats.</span><span class="sxs-lookup"><span data-stu-id="9c7c4-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9c7c4-123">Se även</span><span class="sxs-lookup"><span data-stu-id="9c7c4-123">See Also</span></span>  
[<span data-ttu-id="9c7c4-124">Lagerstyrning</span><span class="sxs-lookup"><span data-stu-id="9c7c4-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="9c7c4-125">Lagersaldo</span><span class="sxs-lookup"><span data-stu-id="9c7c4-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="9c7c4-126">[Ställa in lagerstyrning](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="9c7c4-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="9c7c4-127">[Monteringshantering](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="9c7c4-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="9c7c4-128">Designdetaljer: Lagerstyrning</span><span class="sxs-lookup"><span data-stu-id="9c7c4-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="9c7c4-129">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9c7c4-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

