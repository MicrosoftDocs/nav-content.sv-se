---
title: "Så här använder du resurser för projekt"
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: cced4bca42b74c2664fd18770f1616c57286e1c3
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-resources-for-jobs"></a><span data-ttu-id="f5ab9-102">Så här använder du resurser för projekt</span><span class="sxs-lookup"><span data-stu-id="f5ab9-102">How to: Use Resources for Jobs</span></span>
<span data-ttu-id="f5ab9-103">Du registrerar förbrukning av resurser i projektjournalen för att hålla reda på kostnader, priser och de specifika projekttyper som är kopplade till projekt.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-103">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="f5ab9-104">Mer information finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="f5ab9-104">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="f5ab9-105">Du kan även bokföra förbrukningen av en resurs i en resursjournal eller projektjournal.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-105">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="f5ab9-106">Transaktioner bokförda i resursjournaler påverkar inte redovisningen.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-106">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="f5ab9-107">Så här tilldelar du resurser till projekt</span><span class="sxs-lookup"><span data-stu-id="f5ab9-107">To assign resources to jobs</span></span>
<span data-ttu-id="f5ab9-108">Du tilldelar resurser till projekt genom att skapa planeringsrader för projektet.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-108">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="f5ab9-109">Mer information finns i [Så här skapar du Projekt](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="f5ab9-109">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="f5ab9-110">Registrera resursförbrukning för ett projekt</span><span class="sxs-lookup"><span data-stu-id="f5ab9-110">To record resource usage for a job</span></span>

1. <span data-ttu-id="f5ab9-111">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projektjournaler** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="f5ab9-112">Öppna den relevanta projektjournalen och fyll sedan i fälten som behövs.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-112">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> <span data-ttu-id="f5ab9-113">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-113">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="f5ab9-114">När journalen är slutförd väljer du åtgärden **Bokföra**.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-114">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="f5ab9-115">Justera resurspriser</span><span class="sxs-lookup"><span data-stu-id="f5ab9-115">To adjust resource prices</span></span>  
<span data-ttu-id="f5ab9-116">Om du vill ändra kostnader eller priser för många resurser på en gång kan du använda ett batch-jobb .</span><span class="sxs-lookup"><span data-stu-id="f5ab9-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="f5ab9-117">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Justera resurskost./-priser** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-117">In the top right corner, choose the **Search for Page or Report** icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="f5ab9-118">Fyll i fälten på en rad efter behov och välj sedan knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

<span data-ttu-id="f5ab9-119">**Obs**! Batch-jobbet varken skapar eller justerar alternativa kostnader eller priser för resurser.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-119">**Note**: This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="f5ab9-120">Detta ändrar bara innehållet i fältet på resurskortet för fältet **Justeringsfält** som du har valt i batch-jobbet.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="f5ab9-121">Justeringarna börjar gälla direkt för resurser så kontrollera justeringsfaktorerna innan du kör batch-jobbet.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="f5ab9-122">Så här får du förslag till resursprisändringar enligt befintliga alternativa priser:</span><span class="sxs-lookup"><span data-stu-id="f5ab9-122">To get resource price change suggestions based on existing alternate prices</span></span>  
<span data-ttu-id="f5ab9-123">Om du redan har skapat alternativa priser för några resurser kan du använda batch-jobbet för att skapa flera alternativa resurspriser.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="f5ab9-124">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resursprisändringar** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-124">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="f5ab9-125">Välj åtgärden **Föreslå res.prisändring (pris)** och fyll sedan i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="f5ab9-126">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-126">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="f5ab9-127">När batch-jobbet har avslutats visar fönstret **Resursprisändringar** resultatet av batch-jobbet.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-127">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="f5ab9-128">Så här får du förslag till resursprisändringar enligt standardpriser</span><span class="sxs-lookup"><span data-stu-id="f5ab9-128">To get resource price change suggestions based on standard prices</span></span>  
<span data-ttu-id="f5ab9-129">Om du vill skapa flera alternativa resurspriser baserat på standardpriserna på resurskorten kan du använda ett batch-jobb .</span><span class="sxs-lookup"><span data-stu-id="f5ab9-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="f5ab9-130">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resursprisändringar** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="f5ab9-131">Välj åtgärden **Föreslå res.prisändring (res)** och fyll sedan i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="f5ab9-132">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-132">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="f5ab9-133">När batch-jobbet har avslutats öppnar du fönstret **Resursprisändringar** för att visa resultatet av batch-jobbet.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-133">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="f5ab9-134">Så här får du förslag till resursprisändringar baserat på alternativa priser</span><span class="sxs-lookup"><span data-stu-id="f5ab9-134">To get resource price change suggestions based on alternate prices</span></span>  
<span data-ttu-id="f5ab9-135">Om du redan har skapat alternativa priser för några resurser kan du använda batch-jobbet för att skapa flera alternativa resurspriser.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="f5ab9-136">I rutan **Sök** anger du **Föreslå res.prisändring (pris)** och väljer sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-136">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f5ab9-137">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-137">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="f5ab9-138">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-138">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="f5ab9-139">När batch-jobbet har avslutats öppnar du fönstret **Resursprisändringar** för att visa resultatet av batch-jobbet.</span><span class="sxs-lookup"><span data-stu-id="f5ab9-139">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="f5ab9-140">Se även</span><span class="sxs-lookup"><span data-stu-id="f5ab9-140">See Also</span></span>
[<span data-ttu-id="f5ab9-141">Hantera projekt</span><span class="sxs-lookup"><span data-stu-id="f5ab9-141">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="f5ab9-142">Finans</span><span class="sxs-lookup"><span data-stu-id="f5ab9-142">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="f5ab9-143">[Hantera inköp](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="f5ab9-143">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="f5ab9-144">[Hantera försäljning](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="f5ab9-144">[Manage Sales](sales-manage-sales.md)   </span></span>  
[<span data-ttu-id="f5ab9-145">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="f5ab9-145">Work With Dynamics NAV</span></span>](ui-work-product.md)  

