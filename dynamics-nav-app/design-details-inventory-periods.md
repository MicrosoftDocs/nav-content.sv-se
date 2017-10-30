---
title: Designdetaljer - Lagerperioder
description: "Bakåtdaterade transaktioner eller kostnadsjusteringar påverkar ofta saldon och lagervärderingar för bokföringsperioder som kanske anses vara stängda. Det kan ha negativ effekt på exakt rapportering, särskilt i globala företag. Funktionen Lagerperioder kan användas för att undvika sådana problem genom att öppna eller att stänga lagerperioder för att begränsa bokföring i en fastställd tidsperiod."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1dd508ee887b28b1696746444145eff6f2bd7ebe
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-inventory-periods"></a><span data-ttu-id="ec25c-105">Designdetaljer: Lagerperioder</span><span class="sxs-lookup"><span data-stu-id="ec25c-105">Design Details: Inventory Periods</span></span>
<span data-ttu-id="ec25c-106">Bakåtdaterade transaktioner eller kostnadsjusteringar påverkar ofta saldon och lagervärderingar för bokföringsperioder som kanske anses vara stängda.</span><span class="sxs-lookup"><span data-stu-id="ec25c-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span></span> <span data-ttu-id="ec25c-107">Det kan ha negativ effekt på exakt rapportering, särskilt i globala företag.</span><span class="sxs-lookup"><span data-stu-id="ec25c-107">This can have adverse effects on accurate reporting, especially within global corporations.</span></span> <span data-ttu-id="ec25c-108">Funktionen Lagerperioder kan användas för att undvika sådana problem genom att öppna eller att stänga lagerperioder för att begränsa bokföring i en fastställd tidsperiod.</span><span class="sxs-lookup"><span data-stu-id="ec25c-108">The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.</span></span>  

 <span data-ttu-id="ec25c-109">En lagerperiod är en period som definieras av ett slutdatum, där du bokför lagringstransaktioner.</span><span class="sxs-lookup"><span data-stu-id="ec25c-109">An inventory period is a period of time, defined by an ending date, in which you post inventory transactions.</span></span> <span data-ttu-id="ec25c-110">När du stänger en lagerperiod kan inga värdeändringar bokföras i den stängda perioden.</span><span class="sxs-lookup"><span data-stu-id="ec25c-110">When you close an inventory period, no value changes can be posted in the closed period.</span></span> <span data-ttu-id="ec25c-111">Det innefattar nya värdebokföringar, förväntade eller fakturerade bokföringar, ändringar i befintliga värden och kostnadsjusteringar.</span><span class="sxs-lookup"><span data-stu-id="ec25c-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span></span> <span data-ttu-id="ec25c-112">Du kan dock fortfarande koppla till en öppen artikeltransaktion som återfinns inom den stängda perioden.</span><span class="sxs-lookup"><span data-stu-id="ec25c-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span></span> <span data-ttu-id="ec25c-113">Mer information finns i [Designdetaljer: Artikelspårning](design-details-item-application.md).</span><span class="sxs-lookup"><span data-stu-id="ec25c-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span></span>  

 <span data-ttu-id="ec25c-114">För att se till att alla transaktionsartiklar i en stängd period är slutliga, måste följande villkor uppfyllas innan en lagerperiod kan stängas:</span><span class="sxs-lookup"><span data-stu-id="ec25c-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before an inventory period can close:</span></span>  

-   <span data-ttu-id="ec25c-115">Alla avgående artikeltransaktioner under perioden måste avslutas (inget negativt lager).</span><span class="sxs-lookup"><span data-stu-id="ec25c-115">All outbound item ledger entries in the period must be closed (no negative inventory).</span></span>  
-   <span data-ttu-id="ec25c-116">Alla objektkostnader i perioden måste justeras.</span><span class="sxs-lookup"><span data-stu-id="ec25c-116">All item costs in the period must be adjusted.</span></span>  
-   <span data-ttu-id="ec25c-117">Alla utsläppta och färdiga produktionsorder i perioden måste kostnadsjusteras.</span><span class="sxs-lookup"><span data-stu-id="ec25c-117">All released and finished production orders in the period must be cost adjusted.</span></span>  

 <span data-ttu-id="ec25c-118">När du stänger en lagerperiod skapas en lagerperiodtransaktion genom att använda numret på den sista artikeljournalen i lagerperioden.</span><span class="sxs-lookup"><span data-stu-id="ec25c-118">When you close an inventory period, an inventory period entry is created by using the number of the last item register that falls in the inventory period.</span></span> <span data-ttu-id="ec25c-119">Dessutom registreras tiden, datumet och användarkoden för den användare som avslutar perioden i lagerperiodtransaktionen.</span><span class="sxs-lookup"><span data-stu-id="ec25c-119">In addition, the time, date, and user code of the user closing the period are recorded in the inventory period entry.</span></span> <span data-ttu-id="ec25c-120">Genom att använda information tillsammans med den sista artikeljournalen för föregående period kan du se vilka lagertransaktioner som bokfördes under lagerperioden.</span><span class="sxs-lookup"><span data-stu-id="ec25c-120">By using this information with the last item register for the previous period, you can see which inventory transactions were posted in the inventory period.</span></span> <span data-ttu-id="ec25c-121">Det är också möjligt att öppna lagerperioder igen om du behöver bokföra i en stängd period.</span><span class="sxs-lookup"><span data-stu-id="ec25c-121">It is also possible to reopen inventory periods if you need to post in a closed period.</span></span> <span data-ttu-id="ec25c-122">När du öppnar en lagerperiod igen skapas en lagerperiodtransaktion.</span><span class="sxs-lookup"><span data-stu-id="ec25c-122">When you reopen an inventory period, an inventory period entry is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ec25c-123">Se även</span><span class="sxs-lookup"><span data-stu-id="ec25c-123">See Also</span></span>  
 <span data-ttu-id="ec25c-124">[Designdetaljer: Lager och kostnadskalkylering](design-details-inventory-costing.md) [Hantera lagerkostnader](finance-manage-inventory-costs.md) [Ekonomi](finance.md)</span><span class="sxs-lookup"><span data-stu-id="ec25c-124">[Design Details: Inventory Costing](design-details-inventory-costing.md) [Managing Inventory Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span></span>  
 [<span data-ttu-id="ec25c-125">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="ec25c-125">Working with Dynamics NAV</span></span>](ui-work-product.md)

