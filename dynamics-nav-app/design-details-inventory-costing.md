---
title: Designdetaljer - Lagerkalkylering
description: "Dokumentationen ger en detaljerad teknisk inblick i begreppen och principerna som används i lagringsvärderingsfunktionerna i [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8403486a897a3031ad0f488b4eb7e415daa1b8a0
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="a63ae-103">Designdetaljer: Lagerkalkylering</span><span class="sxs-lookup"><span data-stu-id="a63ae-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="a63ae-104">Dokumentationen ger en detaljerad teknisk inblick i begreppen och principerna som används i lagringsvärderingsfunktionerna i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a63ae-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="a63ae-105">Lagervärdering, kallas även kostnadshantering, används vid registrering och rapportering av rörelsens driftskostnader.</span><span class="sxs-lookup"><span data-stu-id="a63ae-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="a63ae-106">I det här avsnittet</span><span class="sxs-lookup"><span data-stu-id="a63ae-106">In This Section</span></span>  
[<span data-ttu-id="a63ae-107">Designdetaljer: Värderingsprinciper</span><span class="sxs-lookup"><span data-stu-id="a63ae-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="a63ae-108">Designdetaljer: Objektkoppling</span><span class="sxs-lookup"><span data-stu-id="a63ae-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="a63ae-109">Designdetaljer: Kostnadsjustering</span><span class="sxs-lookup"><span data-stu-id="a63ae-109">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="a63ae-110">Designdetaljer: Bokföring av förväntad kostnad</span><span class="sxs-lookup"><span data-stu-id="a63ae-110">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="a63ae-111">Designdetaljer: Genomsnittskostnad</span><span class="sxs-lookup"><span data-stu-id="a63ae-111">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="a63ae-112">Designdetaljer: Varians</span><span class="sxs-lookup"><span data-stu-id="a63ae-112">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="a63ae-113">Designdetaljer: Avrundning</span><span class="sxs-lookup"><span data-stu-id="a63ae-113">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="a63ae-114">Designdetaljer: Kostnadskomponenter</span><span class="sxs-lookup"><span data-stu-id="a63ae-114">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="a63ae-115">Designdetaljer: Lagerperioder</span><span class="sxs-lookup"><span data-stu-id="a63ae-115">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="a63ae-116">Designdetaljer: Lagerbokföring</span><span class="sxs-lookup"><span data-stu-id="a63ae-116">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="a63ae-117">Designdetaljer: Bokföring av produktionsorder</span><span class="sxs-lookup"><span data-stu-id="a63ae-117">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="a63ae-118">Designdetaljer: Bokföring av monteringsorder</span><span class="sxs-lookup"><span data-stu-id="a63ae-118">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="a63ae-119">Designdetaljer: Avstämning med redovisningen</span><span class="sxs-lookup"><span data-stu-id="a63ae-119">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="a63ae-120">Designdetaljer: Konton i redovisningen</span><span class="sxs-lookup"><span data-stu-id="a63ae-120">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="a63ae-121">Designdetaljer: Omvärdering</span><span class="sxs-lookup"><span data-stu-id="a63ae-121">Design Details: Revaluation</span></span>](design-details-revaluation.md)

