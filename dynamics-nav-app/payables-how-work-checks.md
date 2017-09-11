---
title: "Så här arbetar du med checkar"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a><span data-ttu-id="5f6d5-102">Så här arbetar du med checkar</span><span class="sxs-lookup"><span data-stu-id="5f6d5-102">How to: Work With Checks</span></span>
<span data-ttu-id="5f6d5-103">Dynamics NAV stödjer elektroniskt och manuellt utfärdande av checkar.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-103">Dynamics NAV supports electronic and manual check issuance.</span></span> <span data-ttu-id="5f6d5-104">För båda metoder används utbetalningsjournalen för att utfärda checkar till leverantörer.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-104">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="5f6d5-105">Du kan även makulera checkar och granska checktransaktioner.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-105">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="5f6d5-106">I processen för att utfärda checkar får du förslag på betalningar, transaktioner skapas och datorcheckar skrivs ut.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-106">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

<span data-ttu-id="5f6d5-107">Skrivaren måste vara korrekt inställd med checkformulären, och du måste definiera vilken checklayout som ska användas.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-107">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="5f6d5-108">Mer information finns i [Så här definierar du checklayouter](finance-setup-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="5f6d5-108">For more information, see [How to: Define Check Layouts](finance-setup-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="5f6d5-109">Så här kan du utfärda checkar</span><span class="sxs-lookup"><span data-stu-id="5f6d5-109">To issue checks</span></span>
1. <span data-ttu-id="5f6d5-110">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningsjournal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="5f6d5-111">Fyll i journalen med relevanta utbetalningar, till exempel genom att använda funktionen Betalningsförslag för lev.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-111">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="5f6d5-112">Mer information finns i [Så här föreslår du leverantörsbetalningar](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="5f6d5-112">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="5f6d5-113">I fältet **bankbetalningstyp** på journalrader för betalning, som du vill att göra med checkar väljer du ett av följande alternativ:</span><span class="sxs-lookup"><span data-stu-id="5f6d5-113">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

 - <span data-ttu-id="5f6d5-114">**Datorcheck** Välj alternativet om du vill att programmet ska upprätta, och senare skriva ut, en check på beloppet på utbetalningsjournalens rad.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-114">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="5f6d5-115">Du måste skriva ut checkarna, innan du kan bokföra journalraderna.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-115">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="5f6d5-116">Du kan bara välja **Datorcheck** eller **Handskriven check** om **Motkontotyp** eller **Kontotyp** är Bankkonto.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-116">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

 - <span data-ttu-id="5f6d5-117">**Manuell check** Välj alternativet om du vill skriva en check för hand och vill att programmet ska upprätta en motsvarande checktransaktion för beloppet.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-117">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="5f6d5-118">Med det här alternativen kan du inte skriva ut checkar från Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-118">By using this option, you cannot print checks from Dynamics NAV.</span></span> <span data-ttu-id="5f6d5-119">Du kan bara välja **Manuell check** eller **Handskriven check** om **Motkontotyp** eller **Kontotyp** är Bankkonto.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-119">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

    <span data-ttu-id="5f6d5-120">**Obs!** Du måste skriva ut datorcheckarna, innan du kan bokföra de relaterade journalraderna.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-120">**Note**: You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="5f6d5-121">Vid datorcheckar väljer du **Skriv ut check**.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-121">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="5f6d5-122">I fönstret **Check** fyller du i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-122">In the **Check** window, fill in the fields as necessary.</span></span> <span data-ttu-id="5f6d5-123">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-123">Choose a field to read a short description of the field or link to more information.</span></span>
6. <span data-ttu-id="5f6d5-124">Välj knappen **Skriv ut**.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-124">Choose the **Print** button.</span></span>

<span data-ttu-id="5f6d5-125">**Obs!** Om du vill skriva ut checkar i flera olika valutor från olika bankkonton måste du köra batch-jobbet **Skriv ut check** separat för varje valuta och ange bankkontot.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-125">**Note**: If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="5f6d5-126">Att skriva ut checkar som inte har bokförts</span><span class="sxs-lookup"><span data-stu-id="5f6d5-126">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="5f6d5-127">Du kan makulera checkar som inte har bokförts när de har skrivits ut, genom att använda åtgärden **Makulera check** i fönstret **Betalningsjournal**.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-127">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>
1. <span data-ttu-id="5f6d5-128">I fönstret **Betalningsjournal** väljer du **Makulera check** och sedan väljer du checken som ska annulleras.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-128">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="5f6d5-129">Så här makulerar du checkar:</span><span class="sxs-lookup"><span data-stu-id="5f6d5-129">To void checks</span></span>
<span data-ttu-id="5f6d5-130">När checkbetalning har bokförts, kan du bara ångra (makulera) checkar från de resulterande banktransaktionerna.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-130">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="5f6d5-131">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-131">In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="5f6d5-132">Välj det relevanta bankkontot och välj åtgärden **Redigerat** och välj sedan åtgärden **checktransaktioner**.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-132">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="5f6d5-133">I fönstret **checktransaktioner** väljer du åtgärden **Makuler check**.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-133">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="5f6d5-134">Markera kryssrutan **Makulera endast check**.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-134">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="5f6d5-135">Välj knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="5f6d5-135">Choose the **OK**button.</span></span>

## <a name="see-also"></a><span data-ttu-id="5f6d5-136">Se även</span><span class="sxs-lookup"><span data-stu-id="5f6d5-136">See Also</span></span>
[<span data-ttu-id="5f6d5-137">Hantera likviditet</span><span class="sxs-lookup"><span data-stu-id="5f6d5-137">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="5f6d5-138">Konfigurera bank</span><span class="sxs-lookup"><span data-stu-id="5f6d5-138">Set Up Banking</span></span>](bank-setup-banking.md)  

