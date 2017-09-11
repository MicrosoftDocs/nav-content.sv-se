---
title: "Så här bokför du årsslutstransaktionen"
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
ms.openlocfilehash: fe32ee973c90ba857852ae092acf03db09e648ee
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-post-year-end-closing-entry"></a><span data-ttu-id="2d137-102">Så här bokför du årsslutstransaktionen</span><span class="sxs-lookup"><span data-stu-id="2d137-102">How to: Post Year-End Closing Entry</span></span>
<span data-ttu-id="2d137-103">Som en del av att avsluta böckerna för ett räkenskapsår kommer du att köra batch-jobbet och flyttaöver årets resultat flyttas till ett konto i balansräkningen och avsluta resultaträkningskontona.</span><span class="sxs-lookup"><span data-stu-id="2d137-103">As part of closing the books for a fiscal year, you will run the Close Income Statement batch job to transfer the year's result to an account in the balance sheet and close the income statement accounts.</span></span> <span data-ttu-id="2d137-104">När du har kört batch-jobbet Avslut av resultatkonton måste du öppna den journal du har angett i batch-jobbet och sedan granska och bokföra transaktionerna.</span><span class="sxs-lookup"><span data-stu-id="2d137-104">After you run the Close Income Statement batch job, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="2d137-105">Så här bokför du årsslutstransaktionen</span><span class="sxs-lookup"><span data-stu-id="2d137-105">To post the year end closing entry</span></span>
1. <span data-ttu-id="2d137-106">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="2d137-106">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="2d137-107">I fönstret **Redovisningsjournal** i fältet **Batch-namn** väljer du den batch som innehåller årsavslutstransaktionerna.</span><span class="sxs-lookup"><span data-stu-id="2d137-107">In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="2d137-108">Granska transaktionerna.</span><span class="sxs-lookup"><span data-stu-id="2d137-108">Review the entries.</span></span>
4. <span data-ttu-id="2d137-109">Om du vill bokföra journalen väljer du åtgärden **Bokför**.</span><span class="sxs-lookup"><span data-stu-id="2d137-109">To post the journal, choose the **Post** action.</span></span>

<span data-ttu-id="2d137-110">**Obs!** Om ett fel påträffas visas ett felmeddelande.</span><span class="sxs-lookup"><span data-stu-id="2d137-110">**Note**: If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="2d137-111">Om bokföringen utförs tas de bokförda transaktionerna bort från journalen.</span><span class="sxs-lookup"><span data-stu-id="2d137-111">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="2d137-112">Efter bokföringen bokförs en transaktion på varje resultatkonto så att saldot blir noll och årets resultat överförs till balansräkningen.</span><span class="sxs-lookup"><span data-stu-id="2d137-112">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="2d137-113">Se även</span><span class="sxs-lookup"><span data-stu-id="2d137-113">See Also</span></span>
[<span data-ttu-id="2d137-114">Avsluta böcker</span><span class="sxs-lookup"><span data-stu-id="2d137-114">Close Books</span></span>](year-close-books.md)  
[<span data-ttu-id="2d137-115">Avslut av resultatkonton</span><span class="sxs-lookup"><span data-stu-id="2d137-115">Close Income Statement</span></span>](year-close-income-statement.md)  
[<span data-ttu-id="2d137-116">Så här avslutar du bokföringsperioder</span><span class="sxs-lookup"><span data-stu-id="2d137-116">How to: Close Accounting Periods</span></span>](year-close-account-periods.md)  
