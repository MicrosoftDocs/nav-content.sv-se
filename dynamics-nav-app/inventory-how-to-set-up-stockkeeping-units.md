---
title: "Så här skapar du lagerställeenheter"
description: "Du kan använda lagerställeenheter för att registrera artikelinformation som rör ett visst lagerställe eller en viss variantkod."
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
ms.openlocfilehash: 7ea31e21df842e63dc9d75998d2a0c3dfe65f1d3
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-stockkeeping-units"></a><span data-ttu-id="96a66-103">Så här skapar du lagerställeenheter</span><span class="sxs-lookup"><span data-stu-id="96a66-103">How to: Set Up Stockkeeping Units</span></span>
<span data-ttu-id="96a66-104">Du kan använda lagerställeenheter för att registrera artikelinformation som rör ett visst lagerställe eller en viss variantkod.</span><span class="sxs-lookup"><span data-stu-id="96a66-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span></span>  

 <span data-ttu-id="96a66-105">Lagerplatsenheter fungerar som komplement till artikelkort.</span><span class="sxs-lookup"><span data-stu-id="96a66-105">Stockkeeping units are a supplement to item cards.</span></span> <span data-ttu-id="96a66-106">De ersätter dem inte även om de är relaterade till dem.</span><span class="sxs-lookup"><span data-stu-id="96a66-106">They do not replace them, although they are related to them.</span></span> <span data-ttu-id="96a66-107">Med lagerställeenheter kan du ha olika information om en artikel på ett visst lagerställe (t.ex. ett distributionslager eller ett distributionscenter) eller om en särskild variant, (t.ex. olika hyllnummer och olika återanskaffningsinformation) av samma artikel.</span><span class="sxs-lookup"><span data-stu-id="96a66-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution center, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span></span>  

## <a name="to-set-up-a-stockkeeping-unit"></a><span data-ttu-id="96a66-108">Så här skapar du lagerställeenheter</span><span class="sxs-lookup"><span data-stu-id="96a66-108">To set up a stockkeeping unit</span></span>  

1.  <span data-ttu-id="96a66-109">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställeenheter**, och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="96a66-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Stockkeeping Units**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="96a66-110">Välj åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="96a66-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="96a66-111">Fyll i fälten på kortet.</span><span class="sxs-lookup"><span data-stu-id="96a66-111">Fill in the fields on the card.</span></span> <span data-ttu-id="96a66-112">Följande fält är obligatoriska: **Artikelnr**, **Lagerställekod**och/eller **Variantkod**.</span><span class="sxs-lookup"><span data-stu-id="96a66-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="96a66-113">När du har skapat den första lagerställeenheten för en artikel, markeras kryssrutan **Lagerställeenhet finns** på **artikelkortet**.</span><span class="sxs-lookup"><span data-stu-id="96a66-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span></span>  

<span data-ttu-id="96a66-114">Om du vill skapa flera lagerställeenheter för en artikel, kan du använda batch-jobbet **Skapa lagerställeenhet**.</span><span class="sxs-lookup"><span data-stu-id="96a66-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="96a66-115">Informationen på **lagerställeenhetskortet** har högre prioritet än informationen på **artikelkortet**.</span><span class="sxs-lookup"><span data-stu-id="96a66-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span></span>  

## <a name="see-also"></a><span data-ttu-id="96a66-116">Se även</span><span class="sxs-lookup"><span data-stu-id="96a66-116">See Also</span></span>  
[<span data-ttu-id="96a66-117">Så här registrerar du nya objekt</span><span class="sxs-lookup"><span data-stu-id="96a66-117">How to: Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="96a66-118">Ställa in lagerstyrning</span><span class="sxs-lookup"><span data-stu-id="96a66-118">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="96a66-119">Lagerstyrning</span><span class="sxs-lookup"><span data-stu-id="96a66-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="96a66-120">Lagersaldo</span><span class="sxs-lookup"><span data-stu-id="96a66-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="96a66-121">[Monteringshantering](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="96a66-121">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="96a66-122">Designdetaljer: Lagerstyrning</span><span class="sxs-lookup"><span data-stu-id="96a66-122">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="96a66-123">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="96a66-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

