---
title: "Så här ställer du in automatiska kontobokföringsmallar"
description: "Om du vill använda automatiska kontokoder måste du skapa en automatisk kontobokföringsmall."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: dc3819a5fd0ee3c3dee9b7f3ac444f5076da4af7
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-automatic-account-posting-groups"></a><span data-ttu-id="5dd0e-103">Så här ställer du in automatiska kontobokföringsmallar</span><span class="sxs-lookup"><span data-stu-id="5dd0e-103">How to: Set Up Automatic Account Posting Groups</span></span>
<span data-ttu-id="5dd0e-104">Om du vill använda automatiska kontokoder måste du skapa en automatisk kontobokföringsmall.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-104">To use automatic account codes, you must create an automatic account posting group.</span></span>  

## <a name="to-set-up-automatic-account-posting-groups"></a><span data-ttu-id="5dd0e-105">Så här ställer du in automatiska kontobokföringsmallar</span><span class="sxs-lookup"><span data-stu-id="5dd0e-105">To set up automatic account posting groups</span></span>  

1.  <span data-ttu-id="5dd0e-106">Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "Ikonen Söka efter sida eller rapport"), ange **Automatkontering** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Auto. Acc. Groups**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5dd0e-107">Välj åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-107">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="5dd0e-108">Fyll i fälten enligt beskrivningen i följande tabell på snabbfliken **Allmänt**.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-108">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5dd0e-109">Fält</span><span class="sxs-lookup"><span data-stu-id="5dd0e-109">Field</span></span>|<span data-ttu-id="5dd0e-110">Description</span><span class="sxs-lookup"><span data-stu-id="5dd0e-110">Description</span></span>|  
    |-----------|-----------------|  
    |<span data-ttu-id="5dd0e-111">**Nr**</span><span class="sxs-lookup"><span data-stu-id="5dd0e-111">**No.**</span></span>|<span data-ttu-id="5dd0e-112">Ange ett unikt alfanumeriskt nummer för den automatiska kontobokföringsmallen.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-112">Enter a unique alphanumeric number for the automatic account posting group.</span></span>|  
    |<span data-ttu-id="5dd0e-113">**Beskrivning**</span><span class="sxs-lookup"><span data-stu-id="5dd0e-113">**Description**</span></span>|<span data-ttu-id="5dd0e-114">Ange en beskrivning av den automatiska kontobokföringsmallen.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-114">Enter a description for the automatic account posting group.</span></span>|  

4.  <span data-ttu-id="5dd0e-115">Fyll i fälten enligt beskrivningen i följande tabell på snabbfliken **Automatkonteringsrad**.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-115">On the **Automatic Acc. Line** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5dd0e-116">Fält</span><span class="sxs-lookup"><span data-stu-id="5dd0e-116">Field</span></span>|<span data-ttu-id="5dd0e-117">Description</span><span class="sxs-lookup"><span data-stu-id="5dd0e-117">Description</span></span>|  
    |-----------|-----------------|  
    |<span data-ttu-id="5dd0e-118">**Allokeringsprocent**</span><span class="sxs-lookup"><span data-stu-id="5dd0e-118">**Allocation Percentage**</span></span>|<span data-ttu-id="5dd0e-119">Ange procentandelen av ursprungsradbeloppet som ska fördelas.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-119">Enter the percentage of the source line amount that is to be allocated.</span></span>|  
    |<span data-ttu-id="5dd0e-120">**Redovisningskontonr**</span><span class="sxs-lookup"><span data-stu-id="5dd0e-120">**G/L Account No.**</span></span>|<span data-ttu-id="5dd0e-121">Ange numret på redovisningskontot som fördelningen ska bokföras på.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-121">Enter the general ledger account number to which the allocation should be posted.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="5dd0e-122">I fältet **Totalt saldo** summeras fältet **Allokeringsprocent** för de automatiska kontoraderna i en bokföringsmall.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-122">The **Total Balance** field totals the **Allocation Percentage** field for automatic account lines in a posting group.</span></span> <span data-ttu-id="5dd0e-123">Om den totala fördelningsprocenten för en bokföringsmall inte blir noll visas ett felmeddelande när posten bokförs.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-123">If the total allocation percent for a posting group does not balance to zero, an error message will be displayed when the item is posted.</span></span>  

5.  <span data-ttu-id="5dd0e-124">Välj knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="5dd0e-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5dd0e-125">Se även</span><span class="sxs-lookup"><span data-stu-id="5dd0e-125">See Also</span></span>  
 <span data-ttu-id="5dd0e-126">[Automatiska kontokoder](automatic-account-codes.md) </span><span class="sxs-lookup"><span data-stu-id="5dd0e-126">[Automatic Account Codes](automatic-account-codes.md) </span></span>  
 [<span data-ttu-id="5dd0e-127">Ställa in bokföringsmallar</span><span class="sxs-lookup"><span data-stu-id="5dd0e-127">Setting Up Posting Groups</span></span>](../../finance-posting-groups.md)  
 [<span data-ttu-id="5dd0e-128">Arbeta med redovisningsjournaler</span><span class="sxs-lookup"><span data-stu-id="5dd0e-128">Working with General Journals</span></span>](../../ui-work-general-journals.md)

