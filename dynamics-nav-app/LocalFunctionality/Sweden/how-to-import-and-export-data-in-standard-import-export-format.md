---
title: "Så här importerar och exporterar du data i SIE-format (Standard Import Export)"
description: Du kan importera och exportera redovisningsdata i SIE-format (Standard Import Export).
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
ms.openlocfilehash: 21f398ff2a3cd5fc3cd1e854728048d898a5602f
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-import-and-export-data-in-standard-import-export-format"></a><span data-ttu-id="71794-103">Så här importerar och exporterar du data i SIE-format (Standard Import Export)</span><span class="sxs-lookup"><span data-stu-id="71794-103">How to: Import and Export Data in Standard Import Export Format</span></span>
<span data-ttu-id="71794-104">Du kan importera och exportera redovisningsdata i SIE-format (Standard Import Export).</span><span class="sxs-lookup"><span data-stu-id="71794-104">You can import and export general ledger data according to the standard import export (SIE) format.</span></span> <span data-ttu-id="71794-105">Genom att ange SIE-dimensioner och -filtyper kan du ange vilken detaljnivå import- eller exporttransaktionerna ska ha.</span><span class="sxs-lookup"><span data-stu-id="71794-105">By specifying SIE dimensions and file types, you can specify the level of detail covered by import or export transactions.</span></span> <span data-ttu-id="71794-106">Mer information finns i [SIE-grupp](http://go.microsoft.com/fwlink/?LinkID=164870&clcid=0x41d).</span><span class="sxs-lookup"><span data-stu-id="71794-106">For more information, see [Standard Import Export Group](http://go.microsoft.com/fwlink/?LinkID=164870&clcid=0x41d).</span></span>  

## <a name="to-import-data-in-sie-format"></a><span data-ttu-id="71794-107">Så här importerar du data i SIE-format</span><span class="sxs-lookup"><span data-stu-id="71794-107">To import data in SIE format</span></span>  

1.  <span data-ttu-id="71794-108">Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **SIE-import** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="71794-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **SIE Import**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="71794-109">Fyll i fälten enligt beskrivningen i följande tabell.</span><span class="sxs-lookup"><span data-stu-id="71794-109">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="71794-110">Fält</span><span class="sxs-lookup"><span data-stu-id="71794-110">Field</span></span>|<span data-ttu-id="71794-111">Description</span><span class="sxs-lookup"><span data-stu-id="71794-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="71794-112">**Filnamn**</span><span class="sxs-lookup"><span data-stu-id="71794-112">**File Name**</span></span>|<span data-ttu-id="71794-113">Ange namnet på och sökvägen till filen du vill importera.</span><span class="sxs-lookup"><span data-stu-id="71794-113">Enter the name and path of the file that you want to import.</span></span>|  
    |<span data-ttu-id="71794-114">**Redovisningsjournalmall**</span><span class="sxs-lookup"><span data-stu-id="71794-114">**Gen. Journal Template**</span></span>|<span data-ttu-id="71794-115">Välj en redovisningsjournalmall.</span><span class="sxs-lookup"><span data-stu-id="71794-115">Select a general journal template.</span></span>|  
    |<span data-ttu-id="71794-116">**Redovisningsjournal**</span><span class="sxs-lookup"><span data-stu-id="71794-116">**Gen. Journal Batch**</span></span>|<span data-ttu-id="71794-117">Välj en redovisningsjournal.</span><span class="sxs-lookup"><span data-stu-id="71794-117">Select a general journal batch.</span></span>|  
    |<span data-ttu-id="71794-118">**Dimensioner**</span><span class="sxs-lookup"><span data-stu-id="71794-118">**Dimensions**</span></span>|<span data-ttu-id="71794-119">Markera SIE-dimensionerna du vill importera.</span><span class="sxs-lookup"><span data-stu-id="71794-119">Select the SIE dimensions to import.</span></span>|  
    |<span data-ttu-id="71794-120">**Infoga redovisningskonto**</span><span class="sxs-lookup"><span data-stu-id="71794-120">**Insert G/L Account**</span></span>|<span data-ttu-id="71794-121">Välj det här alternativet om redovisningskontot i importfilen saknas i kontoplanen och måste skapas under importprocessen.</span><span class="sxs-lookup"><span data-stu-id="71794-121">Select if the general ledger account in the import file is missing in the chart of accounts and needs to be set up during the import process.</span></span>|  
    |<span data-ttu-id="71794-122">**Använd nummerserie för dok.nr**</span><span class="sxs-lookup"><span data-stu-id="71794-122">**Use Number Series for Doc. No.**</span></span>|<span data-ttu-id="71794-123">Välj det här alternativet om det inte finns något dokumentnummer i importfilen.</span><span class="sxs-lookup"><span data-stu-id="71794-123">Select if a document number is not provided in the import file.</span></span>|  

3.  <span data-ttu-id="71794-124">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="71794-124">Choose the **OK** button.</span></span>  

## <a name="to-export-data-in-sie-format"></a><span data-ttu-id="71794-125">Så här exporterar du data i SIE-format</span><span class="sxs-lookup"><span data-stu-id="71794-125">To export data in SIE format</span></span>  

1.  <span data-ttu-id="71794-126">Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **SIE-import** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="71794-126">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **SIE Export**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="71794-127">Välj lämpliga filter på snabbfliken **Redovisningskonto**.</span><span class="sxs-lookup"><span data-stu-id="71794-127">On the **G/L Account** FastTab, choose the appropriate filters.</span></span>  
3.  <span data-ttu-id="71794-128">Fyll i fälten enligt beskrivningen i följande tabell på snabbfliken **Alternativ**.</span><span class="sxs-lookup"><span data-stu-id="71794-128">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="71794-129">Fält</span><span class="sxs-lookup"><span data-stu-id="71794-129">Field</span></span>|<span data-ttu-id="71794-130">Description</span><span class="sxs-lookup"><span data-stu-id="71794-130">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="71794-131">**Filtyp**</span><span class="sxs-lookup"><span data-stu-id="71794-131">**File Type**</span></span>|<span data-ttu-id="71794-132">Välj typen av fil du vill skapa.</span><span class="sxs-lookup"><span data-stu-id="71794-132">Select the type of file to be created.</span></span> <span data-ttu-id="71794-133">Välj något av följande alternativ:</span><span class="sxs-lookup"><span data-stu-id="71794-133">Select from one of the following options:</span></span><br /><br /> <span data-ttu-id="71794-134">-   **År - Slutsaldon** - Innehåller årligt utgående saldo för alla konton i kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="71794-134">-   **Year - End Balances** - Contains the annual account balance carried forward for all accounts in the chart of accounts.</span></span><br /><span data-ttu-id="71794-135">-   **Periodiska saldon** - Innehåller årligt utgående saldo och månatliga förändringar för alla konton i kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="71794-135">-   **Periodic Balances** - Contains the annual account balance carried forward and monthly changes for all accounts in the chart of accounts.</span></span><br /><span data-ttu-id="71794-136">-   **Objektsaldon** - Innehåller årligt utgående kontosaldo, månatliga förändringar och saldon på objektnivån, till exempel kostnadsenheter och projekt, för alla konton i kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="71794-136">-   **Object Balances** - Contains the annual account balance carried forward, monthly changes, and balances on the object level, such as cost units and projects, for all accounts in the chart of accounts.</span></span><br /><span data-ttu-id="71794-137">-   **Transaktioner** - Innehåller alla redovisningstransaktioner för perioden.</span><span class="sxs-lookup"><span data-stu-id="71794-137">-   **Transactions** - Contains all the general ledger entries for the period.</span></span>|  
    |<span data-ttu-id="71794-138">**Filnamn**</span><span class="sxs-lookup"><span data-stu-id="71794-138">**File Name**</span></span>|<span data-ttu-id="71794-139">Ange namnet på och sökvägen till filen du vill skapa.</span><span class="sxs-lookup"><span data-stu-id="71794-139">Enter the name and path of the file that you want to create.</span></span>|  
    |<span data-ttu-id="71794-140">**Kontakt**</span><span class="sxs-lookup"><span data-stu-id="71794-140">** Contact**</span></span>|<span data-ttu-id="71794-141">Ange kontaktperson.</span><span class="sxs-lookup"><span data-stu-id="71794-141">Enter the contact person.</span></span> <span data-ttu-id="71794-142">Fältet är ett tillval.</span><span class="sxs-lookup"><span data-stu-id="71794-142">This field is optional.</span></span>|  
    |<span data-ttu-id="71794-143">**Kommentarer**</span><span class="sxs-lookup"><span data-stu-id="71794-143">**Comments**</span></span>|<span data-ttu-id="71794-144">Beskriv filens innehåll.</span><span class="sxs-lookup"><span data-stu-id="71794-144">Describe the content of the file.</span></span>|  
    |<span data-ttu-id="71794-145">**Dimensioner**</span><span class="sxs-lookup"><span data-stu-id="71794-145">**Dimensions**</span></span>|<span data-ttu-id="71794-146">Markera dimensionerna du vill exportera.</span><span class="sxs-lookup"><span data-stu-id="71794-146">Select the dimensions to export.</span></span>|  
    |<span data-ttu-id="71794-147">**Räkenskapsår**</span><span class="sxs-lookup"><span data-stu-id="71794-147">**Fiscal Year**</span></span>|<span data-ttu-id="71794-148">Ange räkenskapsåret.</span><span class="sxs-lookup"><span data-stu-id="71794-148">Enter the fiscal tax year.</span></span>|  

4.  <span data-ttu-id="71794-149">Välj knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="71794-149">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="71794-150">Se även</span><span class="sxs-lookup"><span data-stu-id="71794-150">See Also</span></span>  
 <span data-ttu-id="71794-151">[SIE-grupp](http://go.microsoft.com/fwlink/?LinkID=164870&clcid=0x41d) </span><span class="sxs-lookup"><span data-stu-id="71794-151">[Standard Import Export Group](http://go.microsoft.com/fwlink/?LinkID=164870&clcid=0x41d) </span></span>  
 [<span data-ttu-id="71794-152">Lokal funktionalitet för Sverige</span><span class="sxs-lookup"><span data-stu-id="71794-152">Sweden Local Functionality</span></span>](sweden-local-functionality.md)

