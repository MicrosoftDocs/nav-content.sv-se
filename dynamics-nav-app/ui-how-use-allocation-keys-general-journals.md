---
title: "Så här använder du fördelningsnycklar i redovisningsjournaler"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d239ab62c4be88ccc4a2ce2669dcc2c20a3c0126
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="8e301-102">Så här använder du fördelningsnycklar i redovisningsjournaler</span><span class="sxs-lookup"><span data-stu-id="8e301-102">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="8e301-103">Du kan fördela en transaktion i en redovisningsjournal på flera olika konton när du bokför journalen.</span><span class="sxs-lookup"><span data-stu-id="8e301-103">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="8e301-104">Fördelningen kan göras efter kvantitet, procentuellt eller med ett belopp.</span><span class="sxs-lookup"><span data-stu-id="8e301-104">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="8e301-105">Så här skapar du fördelningsnycklar</span><span class="sxs-lookup"><span data-stu-id="8e301-105">To set up allocation keys</span></span> 
1. <span data-ttu-id="8e301-106">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Återkommande redov.journal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="8e301-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="8e301-107">Välj fältet **Journalnamn** för att öppna fönstret **redovisningsjournaler**.</span><span class="sxs-lookup"><span data-stu-id="8e301-107">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="8e301-108">Du kan antingen ändra fördelningar på en befintlig journal i listan eller skapa en ny journal med fördelningar.</span><span class="sxs-lookup"><span data-stu-id="8e301-108">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
  * <span data-ttu-id="8e301-109">För att skapa en y journal väljer du åtgärden **Ny** och går vidare till nästa steg för att skapa en ny journal.</span><span class="sxs-lookup"><span data-stu-id="8e301-109">To create a new batch, choose the **New** action, and go to the next step.</span></span>
  * <span data-ttu-id="8e301-110">Välj journalen och gå till steg 7 för att ändra fördelningar av en befintlig journal.</span><span class="sxs-lookup"><span data-stu-id="8e301-110">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="8e301-111">I fältet **Namn** anger du ett namn för journalens som t.ex. RENSNING.</span><span class="sxs-lookup"><span data-stu-id="8e301-111">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="8e301-112">I fältet **beskrivning** anger du en beskrivning som t.ex. Rensning av utläggsjournal.</span><span class="sxs-lookup"><span data-stu-id="8e301-112">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="8e301-113">Stäng fönstret när du är klar.</span><span class="sxs-lookup"><span data-stu-id="8e301-113">When you are done, close the window.</span></span> <span data-ttu-id="8e301-114">En ny, tom återkommande journal öppnas.</span><span class="sxs-lookup"><span data-stu-id="8e301-114">A new, empty recurring journal opens.</span></span> 
6. <span data-ttu-id="8e301-115">Fyll i fälten på raden.</span><span class="sxs-lookup"><span data-stu-id="8e301-115">Fill in the fields in the line.</span></span>
7. <span data-ttu-id="8e301-116">Välj åtgärden **Fördelningar**.</span><span class="sxs-lookup"><span data-stu-id="8e301-116">Choose the **Allocations** action.</span></span> 
8. <span data-ttu-id="8e301-117">Lägg till en rad för varje fördelning.</span><span class="sxs-lookup"><span data-stu-id="8e301-117">Add a line for each allocation.</span></span> <span data-ttu-id="8e301-118">Du måste fylla i fältet **Fördelning %**, **Fördelningskvantitet** eller **Belopp**.</span><span class="sxs-lookup"><span data-stu-id="8e301-118">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="8e301-119">Du måste fylla i **Kontonr.**</span><span class="sxs-lookup"><span data-stu-id="8e301-119">You must also fill in the **Account No.**</span></span> <span data-ttu-id="8e301-120">och om du fördelar transaktionen bland globala dimensioner, fälten för globala dimensioner.</span><span class="sxs-lookup"><span data-stu-id="8e301-120">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="8e301-121">Om du anger ett värde i procent på en rad beräknas beloppet i fältet **Belopp** automatiskt.</span><span class="sxs-lookup"><span data-stu-id="8e301-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="8e301-122">Dessa belopp har motsatt tecken mot det totala beloppet i fältet **Belopp** i den återkommande journalen.</span><span class="sxs-lookup"><span data-stu-id="8e301-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="8e301-123">Välj **OK** för att återgå till fönstret **Återkommande redov.journal** fönstret, när du har angett fördelningsraderna.</span><span class="sxs-lookup"><span data-stu-id="8e301-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="8e301-124">Fältet **Fördelat belopp (USD)** är ifyllt och matchar fältet **Belopp**.</span><span class="sxs-lookup"><span data-stu-id="8e301-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="8e301-125">Bokför journalen.</span><span class="sxs-lookup"><span data-stu-id="8e301-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="8e301-126">För att ändra en fördelningsnyckel som redan har angetts.</span><span class="sxs-lookup"><span data-stu-id="8e301-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="8e301-127">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Återkommande redov.journal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="8e301-127">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="8e301-128">Välj journalen med fördelningen i fältet **Återkommande redov.journal**.</span><span class="sxs-lookup"><span data-stu-id="8e301-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="8e301-129">Välj raden med fördelningen och välj sedan åtgärden **fördelningar**.</span><span class="sxs-lookup"><span data-stu-id="8e301-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="8e301-130">Ändra de relevanta fälten, och stäng fönstret.</span><span class="sxs-lookup"><span data-stu-id="8e301-130">Change the relevant fields, and close the window.</span></span>

## <a name="see-also"></a><span data-ttu-id="8e301-131">Se även</span><span class="sxs-lookup"><span data-stu-id="8e301-131">See Also</span></span>
[<span data-ttu-id="8e301-132">Arbeta med redovisningsjournaler</span><span class="sxs-lookup"><span data-stu-id="8e301-132">Work With General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="8e301-133">Bokför dokument och journaler</span><span class="sxs-lookup"><span data-stu-id="8e301-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)




