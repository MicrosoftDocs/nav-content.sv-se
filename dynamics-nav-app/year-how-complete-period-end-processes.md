---
title: Avsluta perioder
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a><span data-ttu-id="f92c8-102">Avsluta perioder</span><span class="sxs-lookup"><span data-stu-id="f92c8-102">Close Periods</span></span>
<span data-ttu-id="f92c8-103">Programmet tvingar dig inte att avsluta perioder, men det finns många periodslutsaktiviteter (månadsslut) som du kan utföra om du vill.</span><span class="sxs-lookup"><span data-stu-id="f92c8-103">The application does not force you to close periods, however, there are many period-end (month-end) activities that can be performed in the application if you want.</span></span> <span data-ttu-id="f92c8-104">Det här avsnittet innehåller en översikt över dessa processer och aktiviteter, som kan vara obligatoriska eller inte i ditt företag.</span><span class="sxs-lookup"><span data-stu-id="f92c8-104">This topic provides an overview of these processes and activities, which may or may not be necessary for your company.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="f92c8-105">Redovisning</span><span class="sxs-lookup"><span data-stu-id="f92c8-105">General Ledger</span></span>
* <span data-ttu-id="f92c8-106">Specificera intervall för bokföringsdatum som gäller hela systemet och är användarspecifik.</span><span class="sxs-lookup"><span data-stu-id="f92c8-106">Specify system-wide and user-specific posting period.</span></span>

    <span data-ttu-id="f92c8-107">Detta anger datumen som bokföring kan göras i.</span><span class="sxs-lookup"><span data-stu-id="f92c8-107">This specifies the dates between which postings are allowed.</span></span> <span data-ttu-id="f92c8-108">Beroende på vilka behov som finns i ditt företag kanske du vill begränsa användares intervall för bokföringsdatum i början av periodslutsprocessen eller vid senare tillfälle mot slutet av perioden.</span><span class="sxs-lookup"><span data-stu-id="f92c8-108">Depending on your business needs, you may want to restrict user posting date ranges at the start of the period-end process or at later time towards the end of the period.</span></span> <span data-ttu-id="f92c8-109">Mer information finns [Så här anger du bokföringsperioder](finance-setup-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="f92c8-109">For more information, see [How to: Specify Posting Periods](finance-setup-how-specify-posting-periods.md).</span></span>
* <span data-ttu-id="f92c8-110">Gör alla nödvändiga redovisningsjusteringar.</span><span class="sxs-lookup"><span data-stu-id="f92c8-110">Make all necessary G/L adjustments.</span></span>
* <span data-ttu-id="f92c8-111">Uppdatera och bokför återkommande journaler.</span><span class="sxs-lookup"><span data-stu-id="f92c8-111">Update and post Recurring Journals.</span></span>
<!--* Process Consolidations-->
* <span data-ttu-id="f92c8-112">Kör kontouppställningar enligt följande:</span><span class="sxs-lookup"><span data-stu-id="f92c8-112">Run account schedules as follows:</span></span>
  1. <span data-ttu-id="f92c8-113">Öppna fönstret **Kontouppställning** och klicka på **Skriv ut**.</span><span class="sxs-lookup"><span data-stu-id="f92c8-113">Open the **Account Schedule** window, and choose the **Print** action.</span></span>
  2. <span data-ttu-id="f92c8-114">Fyll i förfrågan om **Kontouppställning** och klicka på **Skriv ut**.</span><span class="sxs-lookup"><span data-stu-id="f92c8-114">Fill the **Account Schedule** request window and choose the **Print** action.</span></span>

## <a name="sales--receivables"></a><span data-ttu-id="f92c8-115">Försäljning & kundreskontra</span><span class="sxs-lookup"><span data-stu-id="f92c8-115">Sales & Receivables</span></span>
* <span data-ttu-id="f92c8-116">Bokför alla försäljningsorder, fakturor, kreditnotor och returorder</span><span class="sxs-lookup"><span data-stu-id="f92c8-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="f92c8-117">Bokför alla inbetalningsjournaler.</span><span class="sxs-lookup"><span data-stu-id="f92c8-117">Post all cash receipt journals.</span></span>
* <span data-ttu-id="f92c8-118">Uppdatera och bokför återkommande journaler som hör till försäljning- och kundreskontra</span><span class="sxs-lookup"><span data-stu-id="f92c8-118">Update and post recurring journals that are related to Sales & Receivables.</span></span>
* <span data-ttu-id="f92c8-119">Stäm av kundreskontra i redovisningen</span><span class="sxs-lookup"><span data-stu-id="f92c8-119">Reconcile accounts receivable to the general ledger.</span></span>
* <span data-ttu-id="f92c8-120">Kör batch-jobbet **Ta bort fakturerade förs.order**</span><span class="sxs-lookup"><span data-stu-id="f92c8-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>

## <a name="purchases--payables"></a><span data-ttu-id="f92c8-121">Inköp & Leverantörsreskontra</span><span class="sxs-lookup"><span data-stu-id="f92c8-121">Purchases & Payables</span></span>
* <span data-ttu-id="f92c8-122">Bokför alla inköps order, fakturor, kreditnotor och returorder</span><span class="sxs-lookup"><span data-stu-id="f92c8-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="f92c8-123">Bokför alla betalningsjournaler.</span><span class="sxs-lookup"><span data-stu-id="f92c8-123">Post all payment journals.</span></span>
* <span data-ttu-id="f92c8-124">Uppdatera och bokför återkommande journaler som relaterar till inköps- och leverantörsreskontra.</span><span class="sxs-lookup"><span data-stu-id="f92c8-124">Update and post recurring journals that are related to purchases & payables.</span></span>
* <span data-ttu-id="f92c8-125">Kör rapporten **Lev.skulder - ålder** och stäm av leverantörsskulder i redovisningen.</span><span class="sxs-lookup"><span data-stu-id="f92c8-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>
* <span data-ttu-id="f92c8-126">Kör batch-jobbet **Ta bort fakturerade inköpsorder**</span><span class="sxs-lookup"><span data-stu-id="f92c8-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="f92c8-127">Beräkna och bearbeta Omsättningsskatt</span><span class="sxs-lookup"><span data-stu-id="f92c8-127">Calculate and Process Sales Tax</span></span>
*  <span data-ttu-id="f92c8-128">Fyll i skattmeddelanden.</span><span class="sxs-lookup"><span data-stu-id="f92c8-128">Complete Tax Statements.</span></span>

## <a name="see-also"></a><span data-ttu-id="f92c8-129">Se även</span><span class="sxs-lookup"><span data-stu-id="f92c8-129">See Also</span></span>
[<span data-ttu-id="f92c8-130">Avsluta år och perioder</span><span class="sxs-lookup"><span data-stu-id="f92c8-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="f92c8-131">Avsluta böcker</span><span class="sxs-lookup"><span data-stu-id="f92c8-131">Close Books</span></span>](year-close-books.md)

