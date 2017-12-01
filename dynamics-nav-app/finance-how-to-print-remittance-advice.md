---
title: "Så här skriver du ut en kundremissa"
description: "Du kan hjälpa dina leverantörer göra avstämningar genom att skriva ut en kundremissa innan du bokför en utbetalningsjournal och när du har bokfört en betalning."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 7c7004ac5ded9436861bf5034f59a9c2bcd99dd0
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---

#<a name="how-to-print-remittance-advice"></a><span data-ttu-id="0c02d-103">Så här skriver du ut en kundremissa</span><span class="sxs-lookup"><span data-stu-id="0c02d-103">How to: Print Remittance Advice</span></span>
<span data-ttu-id="0c02d-104">Du skriver ut en kundremissa innan du bokför en utbetalningsjournal och när du har bokfört en betalning.</span><span class="sxs-lookup"><span data-stu-id="0c02d-104">You can print remittance advice before posting a payment journal and after posting a payment.</span></span> <span data-ttu-id="0c02d-105">Detta visar leverantörens fakturanummer som hjälper leverantörer att göra avstämningar.</span><span class="sxs-lookup"><span data-stu-id="0c02d-105">This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.</span></span>

##<a name="to-print-remittance-advice"></a><span data-ttu-id="0c02d-106">Så här skriver du ut en kundremissa</span><span class="sxs-lookup"><span data-stu-id="0c02d-106">To print remittance advice</span></span>
1. <span data-ttu-id="0c02d-107">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Utbetalningsjournal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="0c02d-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0c02d-108">I fönstret **betalningsjournal** väljer du den betalning för vilken kundremissa måste skrivas ut för.</span><span class="sxs-lookup"><span data-stu-id="0c02d-108">In the **Payment Journal** window, select the payment for which remittance advice must be printed.</span></span>  
3. <span data-ttu-id="0c02d-109">Välj åtgärden **Skriv ut kundremissa**.</span><span class="sxs-lookup"><span data-stu-id="0c02d-109">Choose the **Print Remittance Advice** action.</span></span>  
4. <span data-ttu-id="0c02d-110">I batchjobbet **Kundremissa - Journal** på snabbfliken **Redovisningsjournalrad** väljer du lämpliga filter.</span><span class="sxs-lookup"><span data-stu-id="0c02d-110">In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.</span></span>  
  
    >[!Note]
    > <span data-ttu-id="0c02d-111">Du kan filtrera med hjälp av leverantörens externa dokumentnummer för att matcha betalningar till fakturor.</span><span class="sxs-lookup"><span data-stu-id="0c02d-111">You can filter using the vendor's external document number to match payments with invoices.</span></span>

5. <span data-ttu-id="0c02d-112">Välj lämpliga filter på snabbfliken **Leverantör**.</span><span class="sxs-lookup"><span data-stu-id="0c02d-112">On the **Vendor** FastTab, choose the appropriate filters.</span></span>  
6. <span data-ttu-id="0c02d-113">Välj **Skriv ut** om du vill skriva ut rapporten eller välj **Förhandsgranska** om du vill visa den nu.</span><span class="sxs-lookup"><span data-stu-id="0c02d-113">Choose **Print** to print the report, or choose **Preview** to view it now.</span></span>  

## <a name="using-remittance-advice-reports"></a><span data-ttu-id="0c02d-114">Använda kundremissarapporter</span><span class="sxs-lookup"><span data-stu-id="0c02d-114">Using Remittance Advice Reports</span></span>
<span data-ttu-id="0c02d-115">Följande tabell beskriver de rapporter som du kan använda med en kundremissa:</span><span class="sxs-lookup"><span data-stu-id="0c02d-115">The following table describes the reports that you can use with remittance advice:</span></span>

|<span data-ttu-id="0c02d-116">Rapport</span><span class="sxs-lookup"><span data-stu-id="0c02d-116">Report</span></span>|<span data-ttu-id="0c02d-117">Description</span><span class="sxs-lookup"><span data-stu-id="0c02d-117">Description</span></span>|
|----|----|
|<span data-ttu-id="0c02d-118">Kundremissa – journalrapport</span><span class="sxs-lookup"><span data-stu-id="0c02d-118">Remittance Advice - Journal Report</span></span>|<span data-ttu-id="0c02d-119">Den här rapporten visar vilka dokument som ska tas med i betalningen.</span><span class="sxs-lookup"><span data-stu-id="0c02d-119">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="0c02d-120">För redovisningsjournalrader kan du ange den journalmall och journal som remissan ska skrivas ut från, datumet för den första aktiviteten som ska skrivas ut och filtrera efter ett dokumentnummer.</span><span class="sxs-lookup"><span data-stu-id="0c02d-120">For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number.</span></span> <span data-ttu-id="0c02d-121">För leverantörer kan du ange det leverantörsnummer som ska tas med i rapporten.</span><span class="sxs-lookup"><span data-stu-id="0c02d-121">For vendors, you can enter the vendor numbers to include in the report.</span></span> |
|<span data-ttu-id="0c02d-122">Kundremissa – transaktionsrapport</span><span class="sxs-lookup"><span data-stu-id="0c02d-122">Remittance Advice - Entries Report</span></span>| <span data-ttu-id="0c02d-123">Den här rapporten visar vilka dokument som ska tas med i betalningen.</span><span class="sxs-lookup"><span data-stu-id="0c02d-123">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="0c02d-124">Du kan definiera rapportens innehåll genom att definiera filter.</span><span class="sxs-lookup"><span data-stu-id="0c02d-124">You define the report contents by setting filters.</span></span> <span data-ttu-id="0c02d-125">Du kan ange ytterligare fält på fliken genom att välja fältet **Fält**.</span><span class="sxs-lookup"><span data-stu-id="0c02d-125">You can set additional fields on the tab by choosing the **Field** field.</span></span> <span data-ttu-id="0c02d-126">För leverantörsreskontratransaktioner kan du ange vilka leverantörer som ska inkluderas i rapporten, datumet för den första aktiviteten som ska skrivas ut, valuta och numret som ska inkluderas.</span><span class="sxs-lookup"><span data-stu-id="0c02d-126">For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include.</span></span> |

> [!Note]
> <span data-ttu-id="0c02d-127">Kundremissa - journalrapport ger inte stöd för från andra scenarier med tillämpning av olika valutor eller betalningstoleranser.</span><span class="sxs-lookup"><span data-stu-id="0c02d-127">The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances.</span></span> <span data-ttu-id="0c02d-128">Mer information finns i [Så här aktiverar du koppling av kundreskontratransaktioner till olika valutor](finance-how-enable-application-ledger-entries-different-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="0c02d-128">For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).</span></span>

> [!Tip]
> <span data-ttu-id="0c02d-129">Läs mer om hur du arbetar med rapporter i [Visa testrapporter före bokföring](ui-how-view-test-reports-posting.md), [Arbeta med rapporter](ui-work-report.md) och [Söka, filtrera och sortera data ](ui-enter-criteria-filters.md).</span><span class="sxs-lookup"><span data-stu-id="0c02d-129">For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="0c02d-130">Se även</span><span class="sxs-lookup"><span data-stu-id="0c02d-130">See Also</span></span>  
[<span data-ttu-id="0c02d-131">Välkommen till Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0c02d-131">Welcome to Dynamics NAV</span></span>](across-get-started.md)
