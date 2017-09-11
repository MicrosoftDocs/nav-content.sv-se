---
title: "Så här kan du skapa tidrapporter"
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
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a><span data-ttu-id="7e11c-102">Så här kan du skapa tidrapporter</span><span class="sxs-lookup"><span data-stu-id="7e11c-102">How to: Set Up Time Sheets</span></span>
<span data-ttu-id="7e11c-103">Tidrapporter i Dynamics NAV administrerar tidregistrering veckovis (sju dagar i taget).</span><span class="sxs-lookup"><span data-stu-id="7e11c-103">Time sheets in Dynamics NAV handle time registration in weekly increments of seven days.</span></span> <span data-ttu-id="7e11c-104">Du kan använda dem för att spåra den tid som används för projektet och du kan använda dem för att registrera enkel resurstimregistrering.</span><span class="sxs-lookup"><span data-stu-id="7e11c-104">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span></span> <span data-ttu-id="7e11c-105">Innan du kan använda tidrapporter måste du ange hur du vill att de ska registreras och konfigureras.</span><span class="sxs-lookup"><span data-stu-id="7e11c-105">Before you can use time sheets, you must specify how you want them to be set up and configured.</span></span>

<span data-ttu-id="7e11c-106">När du har ställt in hur organisationen ska använda tidrapporter, kan du ange om och hur tidrapporter godkänns.</span><span class="sxs-lookup"><span data-stu-id="7e11c-106">After you have set up how your organization will use time sheets, you can specify if and how time sheets are approved.</span></span> <span data-ttu-id="7e11c-107">Beroende på organisationens behov kan du ange:</span><span class="sxs-lookup"><span data-stu-id="7e11c-107">Depending on the needs of your organization, you can designate:</span></span>

- <span data-ttu-id="7e11c-108">En eller flera användare som tidrapportsadministratör och godkännare för alla tidrapporter.</span><span class="sxs-lookup"><span data-stu-id="7e11c-108">One or more users as the time sheet administrator and approver for all time sheets.</span></span>
- <span data-ttu-id="7e11c-109">En tidrapportsgodkännare för varje resurs.</span><span class="sxs-lookup"><span data-stu-id="7e11c-109">A time sheet approver for each resource.</span></span>

<span data-ttu-id="7e11c-110">När du har konfigurerat tidrapporter, kan du skapa tidrapporter för resurser, tilldela dem till projektplaneringsrader och bokföra tidrapportrader.</span><span class="sxs-lookup"><span data-stu-id="7e11c-110">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span></span> <span data-ttu-id="7e11c-111">Mer information finns i [Så här använder du tidrapporter](projects-how-use-time-sheets.md).</span><span class="sxs-lookup"><span data-stu-id="7e11c-111">For more information, see [How to: Use Time Sheets](projects-how-use-time-sheets.md).</span></span>

## <a name="to-set-up-general-information-for-time-sheets"></a><span data-ttu-id="7e11c-112">Så här anger du allmän information för tidrapporter</span><span class="sxs-lookup"><span data-stu-id="7e11c-112">To set up general information for time sheets</span></span>  

1. <span data-ttu-id="7e11c-113">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resursinställningar** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="7e11c-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7e11c-114">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="7e11c-114">Fill in the fields as necessary.</span></span> <span data-ttu-id="7e11c-115">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="7e11c-115">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="7e11c-116">För fältet **Tidrapport per projektgodkännande** väljer du ett av följande alternativ.</span><span class="sxs-lookup"><span data-stu-id="7e11c-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span></span>

|<span data-ttu-id="7e11c-117">Alternativ</span><span class="sxs-lookup"><span data-stu-id="7e11c-117">Option</span></span> |<span data-ttu-id="7e11c-118">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="7e11c-118">Description</span></span>|
|---|---|
|<span data-ttu-id="7e11c-119">**Aldrig**</span><span class="sxs-lookup"><span data-stu-id="7e11c-119">**Never**</span></span>|<span data-ttu-id="7e11c-120">Användaren i fältet **Användar-ID för tidrapportens godkännare** på resurskortet godkänner tidrapporten.</span><span class="sxs-lookup"><span data-stu-id="7e11c-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span>|
|<span data-ttu-id="7e11c-121">**Alltid**</span><span class="sxs-lookup"><span data-stu-id="7e11c-121">**Always**</span></span>|<span data-ttu-id="7e11c-122">Användaren i fältet **Ansvarig person** på projektkortet godkänner tidrapporten.</span><span class="sxs-lookup"><span data-stu-id="7e11c-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span></span>|
|<span data-ttu-id="7e11c-123">**Enbart maskin**</span><span class="sxs-lookup"><span data-stu-id="7e11c-123">**Machine Only**´</span></span>|<span data-ttu-id="7e11c-124">Om maskinens tidrapport är länkad till ett projekt, godkänner användaren i fältet **Ansvarig person** på projektkortet tidrapporten.</span><span class="sxs-lookup"><span data-stu-id="7e11c-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span></span> <span data-ttu-id="7e11c-125">Om maskinens tidrapport är länkad till en resurs, godkänner användaren i fältet **Användar-ID för tidrapportens godkännare** på resurskortet tidrapporten.</span><span class="sxs-lookup"><span data-stu-id="7e11c-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span>

## <a name="to-assign-a-time-sheet-administrator"></a><span data-ttu-id="7e11c-126">Så här tilldelar du en tidrapportsadministratör</span><span class="sxs-lookup"><span data-stu-id="7e11c-126">To assign a time sheet administrator</span></span>  

1. <span data-ttu-id="7e11c-127">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Användarinställningar** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="7e11c-127">In the top right corner, choose the **Search for Page or Report** icon, enter **User Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7e11c-128">Lägg till en ny användare om användarlistan inte innehåller den person som du vill ska vara tidrapportsadministratören.</span><span class="sxs-lookup"><span data-stu-id="7e11c-128">Add a new user, if the user list does not include the person who you want to be the time sheet administrator.</span></span> <span data-ttu-id="7e11c-129">För mer information, kontakta administratören.</span><span class="sxs-lookup"><span data-stu-id="7e11c-129">For more information, please contact your administrator.</span></span>  
3. <span data-ttu-id="7e11c-130">Välj en användare som ska vara en tidrapportadministratör och välj sedan kryssrutan **Tidrapportadmin.**</span><span class="sxs-lookup"><span data-stu-id="7e11c-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.**</span></span> <span data-ttu-id="7e11c-131">.</span><span class="sxs-lookup"><span data-stu-id="7e11c-131">check box.</span></span>  

<span data-ttu-id="7e11c-132">**Tips**: Vi rekommenderar att du endast anger en användare som tidrapportsadministratör för ett företag.</span><span class="sxs-lookup"><span data-stu-id="7e11c-132">**Tip**: It is recommended that you designate only one user to be the time sheet administrator for a company.</span></span> <span data-ttu-id="7e11c-133">I följande procedur skapar du en tidrapportägare och godkännare där tidrapportgodkännaren tilldelas för varje resurs.</span><span class="sxs-lookup"><span data-stu-id="7e11c-133">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span></span>  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a><span data-ttu-id="7e11c-134">Så här tilldelar du en tidrapportsägare och en godkännare</span><span class="sxs-lookup"><span data-stu-id="7e11c-134">To assign a time sheets owner and approver</span></span>  

1. <span data-ttu-id="7e11c-135">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resurser** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="7e11c-135">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources**, and then choose the related link.</span></span>
2. <span data-ttu-id="7e11c-136">Välj den resurs som du vill ställa in möjlighet att använda tidrapporter för och markera sedan kryssrutan **Använd tidrapport**.</span><span class="sxs-lookup"><span data-stu-id="7e11c-136">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span></span>  
3. <span data-ttu-id="7e11c-137">I fältet **Användar-ID för tidrapportens ägare** anger du ID för ägaren av tidrapporten.</span><span class="sxs-lookup"><span data-stu-id="7e11c-137">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span></span> <span data-ttu-id="7e11c-138">Ägaren kan ange tidförbrukning på en tidrapport och skicka den för godkännande.</span><span class="sxs-lookup"><span data-stu-id="7e11c-138">The owner can enter time usage on a time sheet and submit it for approval.</span></span> <span data-ttu-id="7e11c-139">Vanligtvis, när resursen är en person, är den person också ägare.</span><span class="sxs-lookup"><span data-stu-id="7e11c-139">In general, when the resource is a person, that person is also the owner.</span></span>  
4. <span data-ttu-id="7e11c-140">I fältet **Användar-ID för tidrapportens godkännare** anger du ID för godkännaren av tidrapporten.</span><span class="sxs-lookup"><span data-stu-id="7e11c-140">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span></span> <span data-ttu-id="7e11c-141">Godkännaren kan godkänna, avvisa eller öppna en tidrapport igen.</span><span class="sxs-lookup"><span data-stu-id="7e11c-141">The approver can approve, reject, or reopen a time sheet.</span></span>  

<span data-ttu-id="7e11c-142">**Obs**! Du kan inte ändra ID på tidrapportsgodkännaren om det finns tidrapporter som inte ännu har behandlats och har statusen **Skickad** eller **Öppen**.</span><span class="sxs-lookup"><span data-stu-id="7e11c-142">**Note**: You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span></span>

## <a name="see-also"></a><span data-ttu-id="7e11c-143">Se även</span><span class="sxs-lookup"><span data-stu-id="7e11c-143">See Also</span></span>
[<span data-ttu-id="7e11c-144">Ange projekthantering</span><span class="sxs-lookup"><span data-stu-id="7e11c-144">Set Up Project Management</span></span>](projects-setup-projects.md)  
[<span data-ttu-id="7e11c-145">Hantera projekt</span><span class="sxs-lookup"><span data-stu-id="7e11c-145">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="7e11c-146">Finans</span><span class="sxs-lookup"><span data-stu-id="7e11c-146">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="7e11c-147">[Hantera inköp](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="7e11c-147">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="7e11c-148">[Hantera försäljning](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="7e11c-148">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="7e11c-149">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="7e11c-149">Work With Dynamics NAV</span></span>](ui-work-product.md)  

