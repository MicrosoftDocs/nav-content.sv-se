---
title: "Scenarioexempel - Definiera dynamisk distribution beräknad på sålda artiklar"
description: "I det här avsnittet innehåller exempel på hur du definierar fördelningar med dynamisk fördelning. I exemplet ändrar du dynamisk fördelning av kostnaderna för de SALES-kostnadsstället för att det ska fungera med den nya kostnadsbäraren IT EQUIPMENT. IT EQUIPMENT-paketet har artikelnummer i intervallet 8904-W till 8924-W. Du kan använda föregående års försäljningssiffror för att beräkna antalet andelen. Fördelningen bokförs på hjälpkostnadstypen 9903."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 32310933bb8eb483bd30270802c8943c55423a2f
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="scenario-example-defining-dynamic-allocations-based-on-items-sold"></a><span data-ttu-id="536ca-107">Scenarioexempel: Definiera dynamisk distribution beräknad på sålda artiklar</span><span class="sxs-lookup"><span data-stu-id="536ca-107">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>
<span data-ttu-id="536ca-108">I det här avsnittet innehåller exempel på hur du definierar fördelningar med dynamisk fördelning.</span><span class="sxs-lookup"><span data-stu-id="536ca-108">This topic shows an example of how to define allocations by using the dynamic allocation method.</span></span> <span data-ttu-id="536ca-109">I exemplet ändrar du dynamisk fördelning av kostnaderna för de SALES-kostnadsstället för att det ska fungera med den nya kostnadsbäraren IT EQUIPMENT.</span><span class="sxs-lookup"><span data-stu-id="536ca-109">In the example, you change the dynamic allocation of the costs for the SALES cost center to support the new cost object IT EQUIPMENT.</span></span> <span data-ttu-id="536ca-110">IT EQUIPMENT-paketet har artikelnummer i intervallet 8904-W till 8924-W.</span><span class="sxs-lookup"><span data-stu-id="536ca-110">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span></span> <span data-ttu-id="536ca-111">Du kan använda föregående års försäljningssiffror för att beräkna antalet andelen.</span><span class="sxs-lookup"><span data-stu-id="536ca-111">You use the previous year’s sales figures to calculate the share.</span></span> <span data-ttu-id="536ca-112">Fördelningen bokförs på hjälpkostnadstypen 9903.</span><span class="sxs-lookup"><span data-stu-id="536ca-112">The allocation is posted to the helping cost type 9903.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="536ca-113">Exemplet använder demonstrationsdata i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="536ca-113">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-dynamic-allocations-based-on-items-sold-in-the-previous-year"></a><span data-ttu-id="536ca-114">Så här definierar du dynamisk fördelning beräknad på sålda artiklar under föregående år</span><span class="sxs-lookup"><span data-stu-id="536ca-114">To define dynamic allocations based on items sold in the previous year</span></span>  

1.  <span data-ttu-id="536ca-115">Välj ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kostnadsfördelningar** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="536ca-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="536ca-116">I fönstret **Kostnadsfördelning** väljer du åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="536ca-116">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="536ca-117">I fältet **ID**, tryck på Retur eller ange ett id.</span><span class="sxs-lookup"><span data-stu-id="536ca-117">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="536ca-118">Ange **1** i fältet **Nivå**.</span><span class="sxs-lookup"><span data-stu-id="536ca-118">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="536ca-119">I fälten **Giltig från** och **Giltig till** anger du datum.</span><span class="sxs-lookup"><span data-stu-id="536ca-119">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="536ca-120">Ange **FÖRS** i fältet **Kod för kostnadsställe**.</span><span class="sxs-lookup"><span data-stu-id="536ca-120">In the **Cost Center Code** field, enter **SALES**.</span></span>  
7.  <span data-ttu-id="536ca-121">I fältet **Kreditera till kostnadstyp** anger du kostnadstyp **9903**.</span><span class="sxs-lookup"><span data-stu-id="536ca-121">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  
8.  <span data-ttu-id="536ca-122">I fältet **Målkostnadstyp** anger du kostnadstyp **9903**.</span><span class="sxs-lookup"><span data-stu-id="536ca-122">In the **Target Cost Type** field, enter the cost type **9903**.</span></span>  
9. <span data-ttu-id="536ca-123">I fältet **Målkostnadsobjekt** välj **Ny** för att skapa den nya kostnadsbäraren IT EQUIPMENT och fyll i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="536ca-123">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span></span> <span data-ttu-id="536ca-124">Välj **IT EQUIPMENT**.</span><span class="sxs-lookup"><span data-stu-id="536ca-124">Select **IT EQUIPMENT**.</span></span> <span data-ttu-id="536ca-125">Låt fältet **Målkostnadsställe** vara tomt.</span><span class="sxs-lookup"><span data-stu-id="536ca-125">Leave the **Target Cost Center** field blank.</span></span>  
10. <span data-ttu-id="536ca-126">I fältet **Typ av fördelningsmål**, välj **Alla kostnader** för att definiera hur upplupna kostnader ska fördelas.</span><span class="sxs-lookup"><span data-stu-id="536ca-126">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span></span>  
11. <span data-ttu-id="536ca-127">I fältet **Bas** välj fördelningsbasen **Sålda artikler (belopp)**.</span><span class="sxs-lookup"><span data-stu-id="536ca-127">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span></span>  
12. <span data-ttu-id="536ca-128">I fältet **Nummerfilter** anger du **8904-W..8924-W**.</span><span class="sxs-lookup"><span data-stu-id="536ca-128">In the **No. Filter** field, enter **8904-W..8924-W**.</span></span>  
13. <span data-ttu-id="536ca-129">I fältet **Kod för datumfilter** anger du **Föregående år**.</span><span class="sxs-lookup"><span data-stu-id="536ca-129">In the **Date Filter Code** field, enter **Last Year**.</span></span>  
14. <span data-ttu-id="536ca-130">Välj åtgärden **Beräkna fördelningsnyckel** för att beräkna andelen.</span><span class="sxs-lookup"><span data-stu-id="536ca-130">Choose the **Calculate Allocation Key** action to calculate the share.</span></span>  

    > [!IMPORTANT]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="536ca-131"> använder föregående år försäljningssiffror för att beräkna en andel för 1596,50 BVA till 100 procent för IT EQUIPMENT-paketet.</span><span class="sxs-lookup"><span data-stu-id="536ca-131"> uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span></span> <span data-ttu-id="536ca-132">Det innebär att alla sålda artiklar föregående år är fördelade på kostnadsbäraren IT EQUIPMENT.</span><span class="sxs-lookup"><span data-stu-id="536ca-132">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span></span>  

## <a name="see-also"></a><span data-ttu-id="536ca-133">Se även</span><span class="sxs-lookup"><span data-stu-id="536ca-133">See Also</span></span>  
 <span data-ttu-id="536ca-134">[Skapa filter för dynamiska fördelningsbaser](finance-setting-filters-for-dynamic-allocation-bases.md) </span><span class="sxs-lookup"><span data-stu-id="536ca-134">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span></span>  
 <span data-ttu-id="536ca-135">[Så här: ställa in fördelningskälla och mål](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="536ca-135">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 <span data-ttu-id="536ca-136">[Definiera och fördela kostnader](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="536ca-136">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 <span data-ttu-id="536ca-137">[Terminologi i kostnadsredovisning](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="536ca-137">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="536ca-138">Om kostnadsredovisning</span><span class="sxs-lookup"><span data-stu-id="536ca-138">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

