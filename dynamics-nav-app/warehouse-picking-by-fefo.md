---
title: "Så här: Aktivera plockning med FEFO"
description: "FEFO-metoden (First-Expired-First-Out) är en sorteringsmetod som säkerställer att de äldsta artiklar, de med de tidigaste utgångsdatumen, plockas först."
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
ms.openlocfilehash: d3977cd235293d685490464e51aec16a95d01e9d
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-picking-items-by-fefo"></a><span data-ttu-id="94815-103">Så här: Aktivera plockning av artiklar med FEFO</span><span class="sxs-lookup"><span data-stu-id="94815-103">How to: Enable Picking Items by FEFO</span></span>
<span data-ttu-id="94815-104">FEFO-metoden (First-Expired-First-Out) är en sorteringsmetod som säkerställer att de äldsta artiklar, de med de tidigaste utgångsdatumen, plockas först.</span><span class="sxs-lookup"><span data-stu-id="94815-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span></span>  

 <span data-ttu-id="94815-105">Den här funktionen fungerar bara, när dessa villkor är uppfyllt:</span><span class="sxs-lookup"><span data-stu-id="94815-105">This functionality only works when the following criteria are met:</span></span>  

-   <span data-ttu-id="94815-106">Artikel måste ha en serie-/partinummer.</span><span class="sxs-lookup"><span data-stu-id="94815-106">The item must have a serial/lot number.</span></span>  
-   <span data-ttu-id="94815-107">På artikelns artikelspårningskod har angetts, fältet **SN specifik spårning för dist.lager** , eller **Parti specifik spårning distr.lager** måste väljas.</span><span class="sxs-lookup"><span data-stu-id="94815-107">On the item’s item tracking code setup, the **SN-Specific Warehouse Tracking** field or the **Lot-Specific Warehouse Tracking** field must be selected.</span></span>  
-   <span data-ttu-id="94815-108">Artikeln måste bokföras till lagret med ett utgångsdatum.</span><span class="sxs-lookup"><span data-stu-id="94815-108">The item must be posted to inventory with an expiration date.</span></span>  
-   <span data-ttu-id="94815-109">På lagerställekortet måste kryssrutan **Begär plockning** vara markerad.</span><span class="sxs-lookup"><span data-stu-id="94815-109">On the location card, the **Require Pick** check box must be selected.</span></span>  
-   <span data-ttu-id="94815-110">Kryssrutan **Plocka enligt FEFO** på lagerställekortet måste vara markerat.</span><span class="sxs-lookup"><span data-stu-id="94815-110">On the location card, the **Pick According to FEFO** check box must be selected.</span></span>  
-   <span data-ttu-id="94815-111">På lagerställekortet måste kryssrutan **Lagerplats ska finnas** vara markerad.</span><span class="sxs-lookup"><span data-stu-id="94815-111">On the location card, the **Bin Mandatory** check box must be selected.</span></span>  

 <span data-ttu-id="94815-112">När alla kriterier uppfylls, sorteras serie-/partinumrerade artiklar som ska plockas med de äldsta första alla plockningar och transporter, utom artiklar som använder SN-närmare visst eller partispecifik spårning.</span><span class="sxs-lookup"><span data-stu-id="94815-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="94815-113">Om någon serie-/partinumrerade artiklar använder specifik spårning, är de respekterade först och under dem, listas de återstående, icke-specifika serie-/partinummer enligt FEFO.</span><span class="sxs-lookup"><span data-stu-id="94815-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span></span>  

 <span data-ttu-id="94815-114">Om två serie-/partinumrerade artiklar har samma utgångsdatum, väljs artikeln med det lägsta serie - eller partinummer.</span><span class="sxs-lookup"><span data-stu-id="94815-114">If two serial/lot-numbered items have the same expiration date, then the program selects the item with the lowest serial or lot number.</span></span> <span data-ttu-id="94815-115">Om serie - eller partinummer är samma, väljs artikeln som registrerades först.</span><span class="sxs-lookup"><span data-stu-id="94815-115">If the serial or lot numbers are the same, then the program selects the item that was registered first.</span></span>  

> [!NOTE]  
>  -   <span data-ttu-id="94815-116">När du plockar serie-/partinumrerade artiklar på lagerplatser som har ställs in för dirigerad artikelinförsel och plockning, plockas bara kvantiteter på lagerplatser av typen *Plock* enligt FEFO.</span><span class="sxs-lookup"><span data-stu-id="94815-116">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span></span>  
> -   <span data-ttu-id="94815-117">Om du vill aktivera transporter enligt FEFO antingen i **lagerförflyttning** fönster eller **Transportförslag** fönstret, måste du lämna **Från binge** fältet tomt.</span><span class="sxs-lookup"><span data-stu-id="94815-117">To enable movements according to FEFO, either in the **Inventory Movement** window or the **Movement Worksheet** window, you must leave the **From Bin** field empty.</span></span>  
> -   <span data-ttu-id="94815-118">Om fältet **Endast utgångsbokföring** är markerat kommer endast artiklar som inte har förfallit att tas med i plockningen.</span><span class="sxs-lookup"><span data-stu-id="94815-118">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span></span> <span data-ttu-id="94815-119">Detta gäller även om du inte använder plockning enligt FEFO.</span><span class="sxs-lookup"><span data-stu-id="94815-119">This applies even if you are not using Pick according to FEFO.</span></span>  

## <a name="see-also"></a><span data-ttu-id="94815-120">Se även</span><span class="sxs-lookup"><span data-stu-id="94815-120">See Also</span></span>  
<span data-ttu-id="94815-121">[Plocka artiklar](warehouse-pick-items.md) </span><span class="sxs-lookup"><span data-stu-id="94815-121">[Picking Items](warehouse-pick-items.md) </span></span>  
<span data-ttu-id="94815-122">[Så här: plocka artiklar för Dist.lager utleverans](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="94815-122">[How to: Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
<span data-ttu-id="94815-123">[Så här plockar du artiklar med Lagerplockning](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="94815-123">[How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
[<span data-ttu-id="94815-124">Designdetaljer: Lagerstyrning</span><span class="sxs-lookup"><span data-stu-id="94815-124">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
[<span data-ttu-id="94815-125">Lagersaldo</span><span class="sxs-lookup"><span data-stu-id="94815-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="94815-126">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="94815-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

