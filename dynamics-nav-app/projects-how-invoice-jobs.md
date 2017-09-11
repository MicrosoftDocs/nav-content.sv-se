---
title: "Så här fakturerar du projekt"
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
ms.openlocfilehash: c0dcce83dfba30af38f33a6bf814b15862d5fc19
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-jobs"></a><span data-ttu-id="e3225-102">Så här fakturerar du projekt</span><span class="sxs-lookup"><span data-stu-id="e3225-102">How to: Invoice Jobs</span></span>
<span data-ttu-id="e3225-103">Under projektet kan projektkostnade från resursförbrukning, material och projektrelaterade inköp uppstå.</span><span class="sxs-lookup"><span data-stu-id="e3225-103">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span></span> <span data-ttu-id="e3225-104">Dessa transaktioner bokförs i projektjournalen.</span><span class="sxs-lookup"><span data-stu-id="e3225-104">As the job progresses, these transactions get posted to the job journal.</span></span> <span data-ttu-id="e3225-105">Det är viktigt att alla kostnader registreras i projektjournalen innan kunden faktureras.</span><span class="sxs-lookup"><span data-stu-id="e3225-105">It is important that all costs get recorded in the job journal before you invoice the customer.</span></span>

<span data-ttu-id="e3225-106">Du kan fakturera hela projektet från fönstret **Projektaktivitetsrader** eller fakturera endast valda fakturerbara rader i fönstret **Planeringsrader**.</span><span class="sxs-lookup"><span data-stu-id="e3225-106">You can invoice the whole job from the **Job Task Lines** window or only invoice selected billable lines from the **Planning Lines** window.</span></span> <span data-ttu-id="e3225-107">Faktureringen kan göras när projektet har slutförts eller allt eftersom projektet fortlöper enligt ett faktureringsschema.</span><span class="sxs-lookup"><span data-stu-id="e3225-107">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span></span>

<span data-ttu-id="e3225-108">**OBS**! Om du väljer **Fakturerbart** i fältet **Projektradtyp** på inköpsdokumentet för projektrelaterade inköp, skapas projektplaneringsrader som är klara att faktureras till kunden.</span><span class="sxs-lookup"><span data-stu-id="e3225-108">**Note**: If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="e3225-109">Mer information finns i [Så här hanterar du projektleveranser](projects-how-manage-project-supplies.md).</span><span class="sxs-lookup"><span data-stu-id="e3225-109">For more information, see [How to: Manage Project Supplies](projects-how-manage-project-supplies.md).</span></span>

## <a name="to-create-and-post-a-job-sales-invoice"></a><span data-ttu-id="e3225-110">Så här skapar och bokför du en försäljningsfaktura för ett projekt</span><span class="sxs-lookup"><span data-stu-id="e3225-110">To create and post a job sales invoice</span></span>  
<span data-ttu-id="e3225-111">Du kan skapa en faktura för ett projekt för en eller flera projektaktiviteter för en kund, antingen när det arbete som ska faktureras har slutförts eller när datumet för fakturering, som är baserat på ett faktureringsschema, har infallit.</span><span class="sxs-lookup"><span data-stu-id="e3225-111">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span></span>

<span data-ttu-id="e3225-112">Från fönstret **Projekt** kan du fakturera en kund genom att välja projekt och sedan välja åtgärden **Skapa jobbförsäljningsfaktura**.</span><span class="sxs-lookup"><span data-stu-id="e3225-112">From the **Jobs** window, you can invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span></span> <span data-ttu-id="e3225-113">Efterföljande procedur visar hur du kan använda ett batch-jobb för att fakturera flera projekt.</span><span class="sxs-lookup"><span data-stu-id="e3225-113">The following procedure shows how to use a batch job to invoice multiple jobs.</span></span>  

1. <span data-ttu-id="e3225-114">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt - Skapa förs.faktura** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="e3225-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Job Create Sales Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e3225-115">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="e3225-115">Fill in the fields as necessary.</span></span> <span data-ttu-id="e3225-116">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="e3225-116">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="e3225-117">Ange filter om du vill begränsa de projekt som ska bearbetas av batch-jobbet.</span><span class="sxs-lookup"><span data-stu-id="e3225-117">Set filters if you want to limit the jobs that the batch job will process.</span></span>
3. <span data-ttu-id="e3225-118">Klicka på **OK** för att skapa fakturorna.</span><span class="sxs-lookup"><span data-stu-id="e3225-118">Choose the **OK** button to create the invoices.</span></span>  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a><span data-ttu-id="e3225-119">Så här skapar du flera projektförsäljningsfakturor från projektplaneringsrader</span><span class="sxs-lookup"><span data-stu-id="e3225-119">To create multiple job sales invoices from job planning lines</span></span>  
<span data-ttu-id="e3225-120">Du kan skapa en faktura från projektplaneringsrader och då ange antal av artikeln, resursen eller redovisningskontot som du vill fakturera.</span><span class="sxs-lookup"><span data-stu-id="e3225-120">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span></span>

1. <span data-ttu-id="e3225-121">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="e3225-121">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="e3225-122">Öppna ett relevant projekt.</span><span class="sxs-lookup"><span data-stu-id="e3225-122">Open a relevant job.</span></span>
3. <span data-ttu-id="e3225-123">Markera ett projekt där fältet **Typ av projektaktivitet** innehåller **Bokföring** och klicka sedan på åtgärden **Projektplaneringsrader**.</span><span class="sxs-lookup"><span data-stu-id="e3225-123">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span></span>  
4. <span data-ttu-id="e3225-124">Gå till fältet **Antal att överföra till faktura** på en projektplaneringsrad och ange antal av artikeln, resursen, typen av redovisningskonto som du vill fakturera.</span><span class="sxs-lookup"><span data-stu-id="e3225-124">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span></span>  
5. <span data-ttu-id="e3225-125">Välj åtgärden **Skapa försäljningsfaktura**.</span><span class="sxs-lookup"><span data-stu-id="e3225-125">Choose the **Create Sales Invoice** action.</span></span>
6. <span data-ttu-id="e3225-126">I fönstret **Projekt - Skapa förs.faktura** anger du bokföringsdatum och om du vill skapa en ny faktura eller koppla denna faktura till en befintlig.</span><span class="sxs-lookup"><span data-stu-id="e3225-126">In the **Job Create Sales Invoice** window, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span></span>
7. <span data-ttu-id="e3225-127">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="e3225-127">Choose the **OK** button.</span></span>

    <span data-ttu-id="e3225-128">På projektplaneringsradens fält **Antal överfört till faktura** kan du se antalet.</span><span class="sxs-lookup"><span data-stu-id="e3225-128">On the job planning line, in the **Qty. Transferred to Invoice** field, you can see the quantity.</span></span>

8. <span data-ttu-id="e3225-129">I fönstret **Projektplaneringsrader** väljer du åtgärden **Försäljningsfakturor/kreditnotor**.</span><span class="sxs-lookup"><span data-stu-id="e3225-129">In the **Job Planning Lines** window, choose the **Sales Invoices/Credit Memos** action.</span></span>

    <span data-ttu-id="e3225-130">Fönstret **Försäljningsfaktura** öppnas och visar antalet som du har överfört till fakturan.</span><span class="sxs-lookup"><span data-stu-id="e3225-130">The **Sales Invoice** window opens, showing the quantity that you have transferred to the invoice.</span></span>  
9. <span data-ttu-id="e3225-131">Gör ytterligare ändringar och välj sedan åtgärden **Bokför**.</span><span class="sxs-lookup"><span data-stu-id="e3225-131">Make any additional changes, and then choose the **Post** action.</span></span>

<span data-ttu-id="e3225-132">**OBS**! Ovanstående förfarande är liknande för att skapa, granska och publicera en projektrelaterad försäljningskreditnota.</span><span class="sxs-lookup"><span data-stu-id="e3225-132">**Note**: The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span></span>

## <a name="to-calculate-and-post-job-completion-entries"></a><span data-ttu-id="e3225-133">Så här kan du beräkna och bokföra slutförda projekt</span><span class="sxs-lookup"><span data-stu-id="e3225-133">To calculate and post job completion entries</span></span>  
<span data-ttu-id="e3225-134">När du har slutfört alla aktiviteter i ett projekt, bland annat bokföringen och faktureringen av förbrukning, måste du uppdatera projektet så att projektet får **Statusen** **Slutförd**.</span><span class="sxs-lookup"><span data-stu-id="e3225-134">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span></span> <span data-ttu-id="e3225-135">Sedan måste du återföra alla PIA som har bokförs i redovisningen.</span><span class="sxs-lookup"><span data-stu-id="e3225-135">Then, you must reverse any WIP that has been posted to the general ledger.</span></span>

1. <span data-ttu-id="e3225-136">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="e3225-136">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e3225-137">Välj ett öppet projekt och välj sedan åtgärden **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="e3225-137">Select an open job, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="e3225-138">Markera **Slutförd** i fältet **Status** .</span><span class="sxs-lookup"><span data-stu-id="e3225-138">In the **Status** field, select **Completed**.</span></span>
4. <span data-ttu-id="e3225-139">Följ hjälpstegen steg för att beräkna och bokföra PIA.</span><span class="sxs-lookup"><span data-stu-id="e3225-139">Follow the assistance steps to calculate and post WIP.</span></span> <span data-ttu-id="e3225-140">Följ alternativt steg 5 och 6 för att göra det manuellt.</span><span class="sxs-lookup"><span data-stu-id="e3225-140">Alternatively, follows steps 5 and 6 to do so manually.</span></span>  
5. <span data-ttu-id="e3225-141">Välj åtgärden **Beräkna PIA**.</span><span class="sxs-lookup"><span data-stu-id="e3225-141">Choose the **Calculate WIP** action.</span></span>
6. <span data-ttu-id="e3225-142">I fönstret **Projekt - Beräkna PIA** fyller du i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="e3225-142">In the **Job Calculate WIP** window, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="e3225-143">De PIA-transaktioner för jobbet som skapas när du kör batch-jobbet kommer nu att ha fältet **Slutfört projekt** markerat för att visa att de är slutförda.</span><span class="sxs-lookup"><span data-stu-id="e3225-143">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span></span>  

7. <span data-ttu-id="e3225-144">Välj åtgärden **Projekt - Bokför PIA i redovisning**.</span><span class="sxs-lookup"><span data-stu-id="e3225-144">Choose the **Job Post WIP to G/L** action.</span></span>
8. <span data-ttu-id="e3225-145">I fönstret **Projekt - Bokför PIA i redovisning** fyller du i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="e3225-145">In the **Job Post WIP to G/L** window, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="e3225-146">De PIA-transaktioner för jobbet som skapas när du kör batch-jobbet kommer nu att ha fältet **Slutfört projekt** markerat för att visa att de är slutförda.</span><span class="sxs-lookup"><span data-stu-id="e3225-146">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="e3225-147">Se även</span><span class="sxs-lookup"><span data-stu-id="e3225-147">See Also</span></span>
[<span data-ttu-id="e3225-148">Hantera projekt</span><span class="sxs-lookup"><span data-stu-id="e3225-148">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="e3225-149">Finans</span><span class="sxs-lookup"><span data-stu-id="e3225-149">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="e3225-150">[Hantera inköp](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="e3225-150">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="e3225-151">[Hantera försäljning](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="e3225-151">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="e3225-152">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="e3225-152">Work With Dynamics NAV</span></span>](ui-work-product.md)  

