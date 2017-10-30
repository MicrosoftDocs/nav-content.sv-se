---
title: "Så här återför du en utflödesbokföring"
description: "Det finns tillfällen när bokföring av utflöde måste återföras. Ett exempel på detta är om det inträffar ett informationsregistreringsfel och ett felaktigt utflödesbelopp bokförs i en produktionsorder."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 21eda3d822ca162b2d97f34eddc21f745e34f561
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-reverse-output-posting"></a><span data-ttu-id="a35b4-104">Så här återför du en utflödesbokföring</span><span class="sxs-lookup"><span data-stu-id="a35b4-104">How to: Reverse Output Posting</span></span>
<span data-ttu-id="a35b4-105">Det finns tillfällen när bokföring av utflöde måste återföras.</span><span class="sxs-lookup"><span data-stu-id="a35b4-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="a35b4-106">Ett exempel på detta är om det inträffar ett informationsregistreringsfel och ett felaktigt utflödesbelopp bokförs i en produktionsorder.</span><span class="sxs-lookup"><span data-stu-id="a35b4-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="a35b4-107">Så här återför du en utflödesbokföring</span><span class="sxs-lookup"><span data-stu-id="a35b4-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="a35b4-108">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Utflödesjournal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="a35b4-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="a35b4-109">Välj din batch.</span><span class="sxs-lookup"><span data-stu-id="a35b4-109">Select your batch.</span></span>  
2. <span data-ttu-id="a35b4-110">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="a35b4-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="a35b4-111">Mer information finns i [Så här: batch-bokför utflöde och körtider](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="a35b4-111">For more information, see [How to: Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="a35b4-112">I fältet **Kopplas till löpnr** väljer du den tillhörande artikeltransaktionen.</span><span class="sxs-lookup"><span data-stu-id="a35b4-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="a35b4-113">Kapaciteten och artikeltransaktionerna återförs.</span><span class="sxs-lookup"><span data-stu-id="a35b4-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="a35b4-114">Bokför återföringen genom att bokföra journalen.</span><span class="sxs-lookup"><span data-stu-id="a35b4-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="a35b4-115">Transaktionerna i utflödesjournalen bokförs som en positiv justering i artikeltransaktionen.</span><span class="sxs-lookup"><span data-stu-id="a35b4-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a35b4-116">Se även</span><span class="sxs-lookup"><span data-stu-id="a35b4-116">See Also</span></span>  
 <span data-ttu-id="a35b4-117">[Produktion](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="a35b4-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="a35b4-118">Ställa in Produktion</span><span class="sxs-lookup"><span data-stu-id="a35b4-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="a35b4-119">[Planerad](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="a35b4-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="a35b4-120">Lagersaldo</span><span class="sxs-lookup"><span data-stu-id="a35b4-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="a35b4-121">Inköp</span><span class="sxs-lookup"><span data-stu-id="a35b4-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="a35b4-122">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a35b4-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

