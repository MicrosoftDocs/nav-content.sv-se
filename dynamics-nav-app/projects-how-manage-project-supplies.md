---
title: "Så här hanterar du projektleveranser"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="55211-102">Så här hanterar du projektleveranser</span><span class="sxs-lookup"><span data-stu-id="55211-102">How to: Manage Job Supplies</span></span>
<span data-ttu-id="55211-103">Att hantera projektleveranser av artiklar, tjänster och utgifter är en viktig del och aspekt av allt projektgenomförande.</span><span class="sxs-lookup"><span data-stu-id="55211-103">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="55211-104">Du kan använda lagerantal eller göra projektspecifika inköp med hjälp av inköpsorder eller inköpsfakturor.</span><span class="sxs-lookup"><span data-stu-id="55211-104">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="55211-105">Ett servicejobb för en dator kan till exempel kräva en ny hårddisk.</span><span class="sxs-lookup"><span data-stu-id="55211-105">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="55211-106">Du skapar då en inköpsfaktura för att köpa en ny hårddisk och registrerar det i projektet.</span><span class="sxs-lookup"><span data-stu-id="55211-106">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="55211-107">Om inköpsprocessen inte kräver att den fysiska transaktionen registreras separat kan ett inköp registreras endast i en inköpsfaktura eller i fönstret **Projektredovisningsjournal**.</span><span class="sxs-lookup"><span data-stu-id="55211-107">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="55211-108">Mer information finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="55211-108">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="55211-109">Köpa artiklar eller tjänster till ett projekt</span><span class="sxs-lookup"><span data-stu-id="55211-109">To purchase items or services for a job</span></span>
<span data-ttu-id="55211-110">Efterföljande procedur visar hur du använder en inköpsfaktura för att köpa produkter till ett projekt.</span><span class="sxs-lookup"><span data-stu-id="55211-110">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="55211-111">Samma steg gäller när du använder en inköpsorder.</span><span class="sxs-lookup"><span data-stu-id="55211-111">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="55211-112">Välj ikonen **söka efter sida eller rapport** i det övre högra hörnet, gå till **Inköpsfakturor** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="55211-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="55211-113">Välj åtgärden **Ny** och fyll i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="55211-113">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="55211-114">Mer information finns i [Så här registrerar du inköp](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="55211-114">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="55211-115">I fälten **Projektnr**.</span><span class="sxs-lookup"><span data-stu-id="55211-115">In the **Job No.**</span></span> <span data-ttu-id="55211-116">och **Projektaktivitetsnr**</span><span class="sxs-lookup"><span data-stu-id="55211-116">and **Job Task No.**</span></span> <span data-ttu-id="55211-117">väljer du informationen för det projekt som du vill köpa artiklar eller tjänster för.</span><span class="sxs-lookup"><span data-stu-id="55211-117">fields, select the information of the job that you want to purchase items or services for.</span></span>  

    <span data-ttu-id="55211-118">Värdet som du väljer i fältet **Projektradtyp** definierar om en planeringsrad skapas när du bokför artikelförbrukningen.</span><span class="sxs-lookup"><span data-stu-id="55211-118">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="55211-119">Om fältet innehåller **Fakturerbart** skapas projektplaneringsrader som är klara att faktureras till kunden.</span><span class="sxs-lookup"><span data-stu-id="55211-119">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="55211-120">Mer information finns i [Så här skapar du fakturaprojekt](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="55211-120">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>

4. <span data-ttu-id="55211-121">Välj åtgärden **Bokföra**.</span><span class="sxs-lookup"><span data-stu-id="55211-121">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="55211-122">Visa värdet på inköp till ett projekt</span><span class="sxs-lookup"><span data-stu-id="55211-122">To view the value of purchases for a job</span></span>  

1. <span data-ttu-id="55211-123">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="55211-123">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="55211-124">Öppna ett relevant projektkort.</span><span class="sxs-lookup"><span data-stu-id="55211-124">Open a relevant job card.</span></span>

    <span data-ttu-id="55211-125">På snabbfliken **Uppgifter** visar fältet **Utestående order** det totala utestående beloppet, i lokal valuta, för lagerartiklar och tjänster för inköpsdokument för projektaktivitetsraden.</span><span class="sxs-lookup"><span data-stu-id="55211-125">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="55211-126">Fältet **Inlevererat bel. ej faktrd** visar värdet för artiklarna som har levererats på inköpsdokument, men ännu inte har fakturerats.</span><span class="sxs-lookup"><span data-stu-id="55211-126">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  

3. <span data-ttu-id="55211-127">Välj något av fälten för att öppna fönstret **Inköpsrader** där du kan granska information om relaterade inköpsdokumentrader, bland annat vilka artiklar eller tjänster som har inlevererats.</span><span class="sxs-lookup"><span data-stu-id="55211-127">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="55211-128">Så här bokför du en projektrelaterad utgift</span><span class="sxs-lookup"><span data-stu-id="55211-128">To post a job-related expense</span></span>  
<span data-ttu-id="55211-129">Om du ådrar dig extraordinära eller engångsutgifter för projekt kan du använda fönstret **Projektredovisningsjournal** för att bokföra dem direkt till det relevanta projektkontot.</span><span class="sxs-lookup"><span data-stu-id="55211-129">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="55211-130">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projektredovisningsjournaler** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="55211-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="55211-131">Skapa en ny rad och registrera information om utgiften, bland annat information i fälten **Projektnr**.</span><span class="sxs-lookup"><span data-stu-id="55211-131">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="55211-132">och **Projektaktivitetsnr**.</span><span class="sxs-lookup"><span data-stu-id="55211-132">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="55211-133">När journalen är slutförd väljer du åtgärden **Bokföra**.</span><span class="sxs-lookup"><span data-stu-id="55211-133">When the journal is complete, choose the **Post** action.</span></span>


## <a name="see-also"></a><span data-ttu-id="55211-134">Se även</span><span class="sxs-lookup"><span data-stu-id="55211-134">See Also</span></span>
[<span data-ttu-id="55211-135">Hantera projekt</span><span class="sxs-lookup"><span data-stu-id="55211-135">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="55211-136">Finans</span><span class="sxs-lookup"><span data-stu-id="55211-136">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="55211-137">[Hantera inköp](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="55211-137">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="55211-138">[Hantera försäljning](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="55211-138">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="55211-139">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="55211-139">Work With Dynamics NAV</span></span>](ui-work-product.md)  

