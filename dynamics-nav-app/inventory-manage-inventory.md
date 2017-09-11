---
title: Hantera lager
author: SorenGP
ms.custom: na
ms.date: 11/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 7f6ce99476a459e7c7d29a9224b5b992271a8b56
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="manage-inventory"></a><span data-ttu-id="ff966-102">Hantera lager</span><span class="sxs-lookup"><span data-stu-id="ff966-102">Manage Inventory</span></span>
<span data-ttu-id="ff966-103">För varje fysisk produkt som du handlar i måste du skapa ett artikelkort av typen Lagersaldo.</span><span class="sxs-lookup"><span data-stu-id="ff966-103">For each physical product that you trade in you must create an item card of type Inventory.</span></span> <span data-ttu-id="ff966-104">Artiklar som du erbjuder till kunder men inte håller i lager kan du registrera som ej lagerförd artikel, som du kan omvandla till lagerartiklar vid behov.</span><span class="sxs-lookup"><span data-stu-id="ff966-104">Items that you offer to customers but do not keep in inventory you can register as nonstock items, which you can convert to inventory items when necessary.</span></span> <span data-ttu-id="ff966-105">Du kan öka eller minska kvantiteten för en artikel i lager, genom att bokföra direkt till artikeltransaktionerna, till exempel efter en fysisk inventering eller, om du inte vill registrera inköp.</span><span class="sxs-lookup"><span data-stu-id="ff966-105">You can increase or decrease the quantity of an item in inventory by posting directly to the item ledger entries, for example, after a physical count or if you do not record purchases.</span></span>

<span data-ttu-id="ff966-106">Lagerökningar och lagerminskningar registreras även naturligtvis när du bokför inköps- och försäljningsdokument.</span><span class="sxs-lookup"><span data-stu-id="ff966-106">Inventory increases and decreases are naturally also recorded when you post purchase and sales documents respectively.</span></span> <span data-ttu-id="ff966-107">Mer information finns i [Så här bokför du inköp](purchasing-how-record-purchases.md), [Så här säljer du produkter](sales-how-sell-products.md) och [Så här fakturerar du försäljning](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="ff966-107">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md), [How to: Sell Products](sales-how-sell-products.md), and [How to: Invoice Sales](sales-how-invoice-sales.md).</span></span>

<span data-ttu-id="ff966-108">För att öka en översikt av artiklar och för att söka efter dem kan du kategorisera artiklar och ge dem attribut för att söka och sortera förbi.</span><span class="sxs-lookup"><span data-stu-id="ff966-108">To increase your overview of items and to help you find them, you can categorize items and give them attributes to search and sort by.</span></span>   

<span data-ttu-id="ff966-109">**Obs!** I Dynamics NAV refereras en produkt till termen “item”.</span><span class="sxs-lookup"><span data-stu-id="ff966-109">**Note**: In Dynamics NAV, a product is referred to using the term “item”.</span></span>

|<span data-ttu-id="ff966-110">Om du vill</span><span class="sxs-lookup"><span data-stu-id="ff966-110">To</span></span> |<span data-ttu-id="ff966-111">Gå till</span><span class="sxs-lookup"><span data-stu-id="ff966-111">See</span></span> |
|---|----|
|<span data-ttu-id="ff966-112">Skapa artikelkort för varje lagerartikel som du handlar med.</span><span class="sxs-lookup"><span data-stu-id="ff966-112">Create item cards for inventory item that you trade in.</span></span>|[<span data-ttu-id="ff966-113">Så här registrerar du nya produkter</span><span class="sxs-lookup"><span data-stu-id="ff966-113">How to: Register New Products</span></span>](inventory-how-register-new-products.md)|
|<span data-ttu-id="ff966-114">Att hålla en översikt över artiklar och hjälpa dig att hitta och sortera artiklar genom att ordna dem i kategorier.</span><span class="sxs-lookup"><span data-stu-id="ff966-114">Maintain an overview of items and help you find and sort items by organizing them in categories.</span></span>|[<span data-ttu-id="ff966-115">Så här kategoriserar du artiklar</span><span class="sxs-lookup"><span data-stu-id="ff966-115">How to: Categorize Items</span></span>](inventory-how-categorize-items.md)|  
|<span data-ttu-id="ff966-116">Tilldela artikelattribut med olika värdetyper till artiklarna för att hjälpa dig att sortera och hitta artiklar.</span><span class="sxs-lookup"><span data-stu-id="ff966-116">Assign item attributes of different value types to your items to help you sort and find items.</span></span>|[<span data-ttu-id="ff966-117">Så här arbetar du med Artikelattribut</span><span class="sxs-lookup"><span data-stu-id="ff966-117">How to: Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)|
|<span data-ttu-id="ff966-118">Skapa artikelkort för vissa artiklar som du erbjuder till kunder, men inte håller i lager.</span><span class="sxs-lookup"><span data-stu-id="ff966-118">Create special item cards for items that you offer to customers but do not maintain inventory for.</span></span>|[<span data-ttu-id="ff966-119">Så här arbetar du med Ej lagerförda artiklar</span><span class="sxs-lookup"><span data-stu-id="ff966-119">How to: Work with Nonstock Items</span></span>](inventory-how-work-nonstock-items.md)|
|<span data-ttu-id="ff966-120">Uppskatta eller skriv av värdet av en eller flera artiklar i lager genom att bokföra deras faktiska, beräknade värde.</span><span class="sxs-lookup"><span data-stu-id="ff966-120">Appreciate or depreciate the value of one or more items in inventory by posting their current, calculated value.</span></span>|[<span data-ttu-id="ff966-121">Så här omvärderar du lager</span><span class="sxs-lookup"><span data-stu-id="ff966-121">How to: Revalue Inventory</span></span>](inventory-how-revalue-inventory.md)|
|<span data-ttu-id="ff966-122">Justera artikelkostnader, antingen automatiskt eller manuellt, för att vidarebefordra kostnadsförändringar från ingående transaktioner till deras relaterade utgående transaktioner.</span><span class="sxs-lookup"><span data-stu-id="ff966-122">Adjust item costs, either automatically or manually, to forward cost changes from inbound entries to their related outbound entries.</span></span>|[<span data-ttu-id="ff966-123">Så här justerar du artikelkostnader</span><span class="sxs-lookup"><span data-stu-id="ff966-123">How to: Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|
|<span data-ttu-id="ff966-124">Återspegla lagervärdeändringar i företagets redovisning genom att bokföra lagerkostnader, antingen automatiskt eller manuellt, till de relaterade lagerkontona i redovisningen.</span><span class="sxs-lookup"><span data-stu-id="ff966-124">Reflect inventory value changes in your company books by posting inventory costs, either automatically or manually, to the related inventory accounts in the general ledger.</span></span>|[<span data-ttu-id="ff966-125">Så här kan du bokföra lagerkostnader i redovisningen</span><span class="sxs-lookup"><span data-stu-id="ff966-125">How to: Post Inventory Costs to the General Ledger</span></span>](inventory-how-post-inventory-cost-gl.md)|

## <a name="see-also"></a><span data-ttu-id="ff966-126">Se även</span><span class="sxs-lookup"><span data-stu-id="ff966-126">See Also</span></span>  
[<span data-ttu-id="ff966-127">Hantera inköp</span><span class="sxs-lookup"><span data-stu-id="ff966-127">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="ff966-128">Hantera försäljning</span><span class="sxs-lookup"><span data-stu-id="ff966-128">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="ff966-129">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="ff966-129">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="ff966-130">Över affärsområden</span><span class="sxs-lookup"><span data-stu-id="ff966-130">Across Business Areas</span></span>](ui-across-business-areas.md)

