---
title: "Så här skapar du cykler för affärsmöjligheter och cykeletapper"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 756e9b2f33fe66cd4c2b4e26ca4390683bd087af
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-set-up-opportunity-sales-cycles-and-cycle-stages"></a><span data-ttu-id="83b54-102">Så här skapar du cykler för affärsmöjligheter och cykeletapper</span><span class="sxs-lookup"><span data-stu-id="83b54-102">How to: Set Up Opportunity Sales Cycles and Cycle Stages</span></span>
<span data-ttu-id="83b54-103">Innan du börjar använda affärsmöjligheter måste du skapa försäljningscykler och försäljningscykeletapper.</span><span class="sxs-lookup"><span data-stu-id="83b54-103">Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages.</span></span> <span data-ttu-id="83b54-104">En försäljningscykel består av en serie etapper från den första kontakten till en genomförd försäljning.</span><span class="sxs-lookup"><span data-stu-id="83b54-104">A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale.</span></span> <span data-ttu-id="83b54-105">Varje etapp kan ha vissa krav som måste uppfyllas, till exempel att kräva en förs.offert innan en affärsmöjlighet kan gå till nästa etapp.</span><span class="sxs-lookup"><span data-stu-id="83b54-105">Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage.</span></span> <span data-ttu-id="83b54-106">Du kan också ange om en etapp kan hoppas över.</span><span class="sxs-lookup"><span data-stu-id="83b54-106">You can also specify whether a stage can be skipped.</span></span> <span data-ttu-id="83b54-107">Du kan skapa ett valfritt antal försäljningscykler och så många etapper som behövs inom en försäljningscykel.</span><span class="sxs-lookup"><span data-stu-id="83b54-107">You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.</span></span>

<span data-ttu-id="83b54-108">Att använda affärsmöjlighetscykeler omfattar att skapa försäljningscykelkoden och definiera de olika etapperna i cykeln och sedan tilldela cykeln till affärsmöjligheter.</span><span class="sxs-lookup"><span data-stu-id="83b54-108">Implementing opportunity sales cycles involves setting up the sales cycle code, defining the different stages of the cycle, and then assigning the cycle to opportunities.</span></span>

## <a name="to-set-up-an-opportunity-sales-cycle-code"></a><span data-ttu-id="83b54-109">Så här skapar du cykler för affärsmöjlighetskod</span><span class="sxs-lookup"><span data-stu-id="83b54-109">To set up an opportunity sales cycle code</span></span>
1. <span data-ttu-id="83b54-110">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Försäljningscykler** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="83b54-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales Cycles**, and then choose the related link.</span></span> <span data-ttu-id="83b54-111">Fönstret **Försäljningscykler** öppnas och visar alla befintliga försäljningscyklar.</span><span class="sxs-lookup"><span data-stu-id="83b54-111">The **Sales Cycles** window opens, and lists all the existing sales cycles.</span></span>
2. <span data-ttu-id="83b54-112">Välj åtgärden **Ny** och fyll i fälten.</span><span class="sxs-lookup"><span data-stu-id="83b54-112">Choose the **New** action, and fill in the fields.</span></span>

<span data-ttu-id="83b54-113">Upprepa stegen för varje säljcykel du vill skapa.</span><span class="sxs-lookup"><span data-stu-id="83b54-113">Repeat these steps to set up as many sales cycles as you want.</span></span> <span data-ttu-id="83b54-114">När du har skapat cykler för affärsmöjligheter vill du kanske skapa de olika etapperna i varje cykel.</span><span class="sxs-lookup"><span data-stu-id="83b54-114">After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.</span></span>

## <a name="to-define-opportunity-sales-cycle-stages"></a><span data-ttu-id="83b54-115">Om du vill definiera etapper för försäljningscykel för affärsmöjligheter</span><span class="sxs-lookup"><span data-stu-id="83b54-115">To define opportunity sales cycle stages</span></span>
1. <span data-ttu-id="83b54-116">I fönstret **Försäljningscykler** markerar du den försäljningscykel för affärsmöjligheter som du vill ställa in etapper för och väljer sedan åtgärden **Etapper**.</span><span class="sxs-lookup"><span data-stu-id="83b54-116">In the **Sales Cycles** window, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action.</span></span> <span data-ttu-id="83b54-117">Fönstret **Försäljningscykeletapper** öppnas.</span><span class="sxs-lookup"><span data-stu-id="83b54-117">The **Sales Cycle Stages** window opens.</span></span>
2. <span data-ttu-id="83b54-118">Välj åtgärden **Ny** för att skapa en ny etapp i försäljningscykeln.</span><span class="sxs-lookup"><span data-stu-id="83b54-118">Choose the **New** action to enter a new stage in the sales cycle.</span></span>

<span data-ttu-id="83b54-119">Upprepa stegen för varje etapp du vill skapa i försäljningscykeln.</span><span class="sxs-lookup"><span data-stu-id="83b54-119">Repeat these steps to set up as many stages as you want within the sales cycle.</span></span>

## <a name="to-assign-stage-cycle-to-an-opportunity"></a><span data-ttu-id="83b54-120">Så här tilldelar du försäljningscykeln till affärsmöjligheten.</span><span class="sxs-lookup"><span data-stu-id="83b54-120">To assign stage cycle to an opportunity</span></span>
<span data-ttu-id="83b54-121">När du har lagt till försäljningscykeln till affärsmöjligheten, kan du börja lägga till affärsmöjligheter och sedan tilldela etappen för försäljningscykeln till affärsmöjligheten genom att ange fältet **försäljningscykelkod**.</span><span class="sxs-lookup"><span data-stu-id="83b54-121">After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field.</span></span> <span data-ttu-id="83b54-122">Mer information finnsi [Så här skapar du Försäljningsmöjligheter](marketing-how-create-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="83b54-122">For more information, see [How to: Create Sales Opportunities](marketing-how-create-opportunities.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="83b54-123">Se även</span><span class="sxs-lookup"><span data-stu-id="83b54-123">See Also</span></span>  
[<span data-ttu-id="83b54-124">Behandlar försäljningsmöjligheter</span><span class="sxs-lookup"><span data-stu-id="83b54-124">Processing Sales Opportunities</span></span>](marketing-processing-sales-opportunities.md)  
[<span data-ttu-id="83b54-125">Hantera försäljning</span><span class="sxs-lookup"><span data-stu-id="83b54-125">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="83b54-126">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="83b54-126">Working with Dynamics NAV</span></span>](ui-work-product.md)

