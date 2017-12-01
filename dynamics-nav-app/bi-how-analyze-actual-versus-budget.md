---
title: Analysera faktiska kontra budget
description: Beskriver hur du analyserar faktiska belopp kontra budgeterade belopp
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: da2cdce3ada29fff98ceb875414f750a8af51855
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-analyze-actual-amounts-versus-budgeted-amounts"></a><span data-ttu-id="39e18-103">Så här: Analysera faktiska belopp kontra budgeterade belopp</span><span class="sxs-lookup"><span data-stu-id="39e18-103">How to: Analyze Actual Amounts Versus Budgeted Amounts</span></span>
<span data-ttu-id="39e18-104">Som en del av att samla in, analysera och dela dina företagsdata, kan du visa faktiska belopp och budgeterade belopp för alla konton och för flera perioder.</span><span class="sxs-lookup"><span data-stu-id="39e18-104">As a part of gathering, analyzing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span></span>

<span data-ttu-id="39e18-105">Om du vill analysera budgeterade belopp, måste du först skapa budgetar.</span><span class="sxs-lookup"><span data-stu-id="39e18-105">To analyze budgeted amounts, you must first create budgets.</span></span> <span data-ttu-id="39e18-106">(Mer information finns i [Så här skapar du budgetar](finance-how-create-budgets.md).)</span><span class="sxs-lookup"><span data-stu-id="39e18-106">For more information, see [How to: Create Budgets](finance-how-create-budgets.md).</span></span>

## <a name="to-view-a-budget"></a><span data-ttu-id="39e18-107">Så här visar du en budget</span><span class="sxs-lookup"><span data-stu-id="39e18-107">To view a budget</span></span>
<span data-ttu-id="39e18-108">Om du vill kan du filtrera transaktionerna i en budget med dimensioner och på så sätt visa vissa bestämda budgetar.</span><span class="sxs-lookup"><span data-stu-id="39e18-108">In a budget with dimensions, you can filter the entries and see specific budgets.</span></span>

1. <span data-ttu-id="39e18-109">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Val av rapportlayout** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="39e18-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>
2. <span data-ttu-id="39e18-110">I fönstret **Redovisningsbudgetar** öppnar du budgeten du vill visa.</span><span class="sxs-lookup"><span data-stu-id="39e18-110">In the **G/L Budgets** window, open the budget that you want to view.</span></span>  
3. <span data-ttu-id="39e18-111">Högst upp i fönstret fyller du i fälten för att definiera vad som ska visas.</span><span class="sxs-lookup"><span data-stu-id="39e18-111">At the top of the window, fill in the fields as necessary to define what is shown.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="39e18-112">Om du har valt **Period** i antingen **Visa som rader** eller **Visa som kolumner**  måste du fylla i fältet **Visa efter**.</span><span class="sxs-lookup"><span data-stu-id="39e18-112">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span></span> <span data-ttu-id="39e18-113">Om du inte har valt **Period** i antingen **Visa som rader** eller i **Visa som kolumner** anger du önskad period i fältet **Datumfilter**.</span><span class="sxs-lookup"><span data-stu-id="39e18-113">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="39e18-114">Endast transaktioner från redovisningsbudgeten med de filterkoder som du anger på snabbfliken **Filter** tas med i beräkningen.</span><span class="sxs-lookup"><span data-stu-id="39e18-114">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span></span> <span data-ttu-id="39e18-115">Budgettransaktioner med andra filterkoder eller utan filterkoder inkluderas inte.</span><span class="sxs-lookup"><span data-stu-id="39e18-115">Budget entries with other filter codes or without any filter codes are not included.</span></span> <span data-ttu-id="39e18-116">Så länge filtret finns kvar i fönstret visas endast budgettransaktionerna med dessa filterkoder i budgeten.</span><span class="sxs-lookup"><span data-stu-id="39e18-116">As long as the filter remains on the window, the budget only displays the budget entries with these filter codes.</span></span>  

> [!TIP]  
>   <span data-ttu-id="39e18-117">Om du vill ändra budgeten kan du redigera budgettransaktionerna.</span><span class="sxs-lookup"><span data-stu-id="39e18-117">If you want to modify the budget, you can modify the budget entries.</span></span> <span data-ttu-id="39e18-118">Välj beloppet för att visa de underliggande redovisningsbudgettransaktioner.</span><span class="sxs-lookup"><span data-stu-id="39e18-118">Choose an amount to view the underlying general ledger budget entries.</span></span>

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a><span data-ttu-id="39e18-119">Så här visar du faktiska och budgeterade belopp för alla konton</span><span class="sxs-lookup"><span data-stu-id="39e18-119">To view actual and budgeted amounts for all accounts</span></span>  
<span data-ttu-id="39e18-120">Du kan visa redovisningsbudgetar och jämföra dem med faktiska belopp i flera olika moduler i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="39e18-120">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

1. <span data-ttu-id="39e18-121">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kontoplan** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="39e18-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="39e18-122">I fönstret **kontoplan** kan du välja åtgärden **Redovisningssaldo/Budget**.</span><span class="sxs-lookup"><span data-stu-id="39e18-122">In the **Chart of Accounts** window, choose the **G/L Balance/Budget** action.</span></span>
3. <span data-ttu-id="39e18-123">Högst upp i fönstret fyller du i fälten för att definiera vad som ska visas.</span><span class="sxs-lookup"><span data-stu-id="39e18-123">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>  
4. <span data-ttu-id="39e18-124">Välj fältet om du vill visa en specifikation av ett visat belopp.</span><span class="sxs-lookup"><span data-stu-id="39e18-124">To see a specification that makes up the amount shown, choose the field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="39e18-125">De filter som definieras i fönsterhuvudet används både på redovisningstransaktioner och budgettransaktioner.</span><span class="sxs-lookup"><span data-stu-id="39e18-125">The filters you set in the window header will be applied to general ledger entries and also budget entries.</span></span>

<span data-ttu-id="39e18-126">Kolumnerna till vänster innehåller kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="39e18-126">The leftmost columns contain the chart of accounts.</span></span> <span data-ttu-id="39e18-127">Av de fem kolumnerna till höger innehåller de fyra första kolumnerna faktiska och budgeterade debet- och kreditbelopp för alla konton.</span><span class="sxs-lookup"><span data-stu-id="39e18-127">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span></span> <span data-ttu-id="39e18-128">I den femte kolumnen visas det proportionella sambandet mellan de faktiska och de budgeterade beloppen på redovisningskontot.</span><span class="sxs-lookup"><span data-stu-id="39e18-128">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span></span>  

> [!TIP]  
>   <span data-ttu-id="39e18-129">Använd fältet **Visa efter** i fönstret **Redov.saldo/budget** om du vill välja ett tidsintervall.</span><span class="sxs-lookup"><span data-stu-id="39e18-129">Use the **View by** field in the **G/L Balance/Budget** window to select the period length.</span></span> <span data-ttu-id="39e18-130">Använd fältet **Visa som** om du vill bestämma hur beloppen ska beräknas, **Nettoförändring** eller **Saldo t.o.m. datum**.</span><span class="sxs-lookup"><span data-stu-id="39e18-130">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span></span> <span data-ttu-id="39e18-131">Välj åtgärden **Föregående period** eller **Nästa period** för att ändra perioden.</span><span class="sxs-lookup"><span data-stu-id="39e18-131">Choose the **Previous Period** or **Next Period** action to change the period.</span></span>  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a><span data-ttu-id="39e18-132">Så här visar du faktiska och budgeterade belopp för flera perioder</span><span class="sxs-lookup"><span data-stu-id="39e18-132">To view actual and budgeted amounts for several periods</span></span>  
<span data-ttu-id="39e18-133">I stället för att visa de faktiska och budgeterade beloppen för alla konton under en enstaka period kan du visa ett antal perioder för ett enskilt konto.</span><span class="sxs-lookup"><span data-stu-id="39e18-133">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span></span>  

1. <span data-ttu-id="39e18-134">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kontoplan** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="39e18-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="39e18-135">I fönstretden **kontoplan** markerar du relevant redovisningskonto, och välj sedan åtgärden **konto saldo/budget**.</span><span class="sxs-lookup"><span data-stu-id="39e18-135">In the **Chart of Accounts** window, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span></span>  
3. <span data-ttu-id="39e18-136">Högst upp i fönstret fyller du i fälten för att definiera vad som ska visas.</span><span class="sxs-lookup"><span data-stu-id="39e18-136">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>   
4. <span data-ttu-id="39e18-137">Välj fältet om du vill visa en specifikation av ett visat belopp.</span><span class="sxs-lookup"><span data-stu-id="39e18-137">To see a specification of an amount shown, choose the field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="39e18-138">Se även</span><span class="sxs-lookup"><span data-stu-id="39e18-138">See Also</span></span>
<span data-ttu-id="39e18-139">[Affärsstöd](bi.md)
[Så här: arbeta med kontouppställningar](bi-how-work-account-schedule.md)</span><span class="sxs-lookup"><span data-stu-id="39e18-139">[Business Intelligence](bi.md)
[How to: Work with Account Schedules](bi-how-work-account-schedule.md)</span></span>  
[<span data-ttu-id="39e18-140">Ekonomi</span><span class="sxs-lookup"><span data-stu-id="39e18-140">Finance</span></span>](finance.md)  
[<span data-ttu-id="39e18-141">Ställa in Finance</span><span class="sxs-lookup"><span data-stu-id="39e18-141">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="39e18-142">Redovisningen och kontoplanen</span><span class="sxs-lookup"><span data-stu-id="39e18-142">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="39e18-143">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="39e18-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

