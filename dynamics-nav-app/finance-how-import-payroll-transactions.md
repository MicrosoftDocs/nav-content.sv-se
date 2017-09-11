---
title: "Så här Importera du lönetransaktioner "
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d5e70a0a1659c7facdeec3f0971eda43ff8a03cc
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-import-payroll-transactions"></a><span data-ttu-id="7a55e-102">Så här Importera du lönetransaktioner </span><span class="sxs-lookup"><span data-stu-id="7a55e-102">How to: Import Payroll Transactions</span></span>
<span data-ttu-id="7a55e-103">För att ta hänsyn till lönutbetalningar och relaterade transaktioner måste du importera och bokföra finansiella transaktioner som gjorts av ditt lönesystem i redovisningen.</span><span class="sxs-lookup"><span data-stu-id="7a55e-103">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="7a55e-104">För att göra detta måste du först importera en csv.</span><span class="sxs-lookup"><span data-stu-id="7a55e-104">To do this, you first import a csv.</span></span> <span data-ttu-id="7a55e-105">-fil som du får från löneleverantören till fönstret **Redovisningsjournal**.</span><span class="sxs-lookup"><span data-stu-id="7a55e-105">file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="7a55e-106">Sedan mappar du de externa kontona i lönefilen till det relevanta redovisningskontot.</span><span class="sxs-lookup"><span data-stu-id="7a55e-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="7a55e-107">Slutligen bokför du lönetransaktioner enligt kontomappningen.</span><span class="sxs-lookup"><span data-stu-id="7a55e-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="7a55e-108">Att importera en lönefil</span><span class="sxs-lookup"><span data-stu-id="7a55e-108">To import a payroll file</span></span>
1. <span data-ttu-id="7a55e-109">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournaler** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="7a55e-109">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="7a55e-110">I relevant redovisningsjournal väljer du åtgärden **Importera lönetransaktioner**.</span><span class="sxs-lookup"><span data-stu-id="7a55e-110">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span>
3. <span data-ttu-id="7a55e-111">I fönstret **Importera** markerar du relevant lönefil och väljer sedan knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="7a55e-111">In the **Import** window, select the relevant payroll file, and then choose the **OK** button.</span></span> <span data-ttu-id="7a55e-112">Filen måste vara i CSV-format.</span><span class="sxs-lookup"><span data-stu-id="7a55e-112">The file must be in CSV format.</span></span> 
4. <span data-ttu-id="7a55e-113">Följ stegen i fönstret **Importera lönetransaktioner** för att importera transaktioner och mappa konton och välj sedan knappen **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="7a55e-113">Follow the steps in the **Import Payroll Transactions** window to import transactions and map accounts, and then choose the **Finish** button.</span></span>

    <span data-ttu-id="7a55e-114">Redovisningsjournalen fylls med rader som representerar de transaktioner som lönefilen innehåller och med de relevanta kontona i kolumnen **Redovisningskonto**.</span><span class="sxs-lookup"><span data-stu-id="7a55e-114">The general journal is filled with lines representing the transactions that the payroll file contains and with the relevant accounts in the **G/L Account** column.</span></span>
4. <span data-ttu-id="7a55e-115">Ändra eller bokför journalrader som för alla andra redovisningtransaktioner.</span><span class="sxs-lookup"><span data-stu-id="7a55e-115">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="7a55e-116">Mer information finns i [Så här arbetar du med redovisningsjournaler](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="7a55e-116">For more information, see [How to: Work With General Journals](ui-work-general-journals.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="7a55e-117">Se även</span><span class="sxs-lookup"><span data-stu-id="7a55e-117">See Also</span></span>
[<span data-ttu-id="7a55e-118">Finans</span><span class="sxs-lookup"><span data-stu-id="7a55e-118">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="7a55e-119">Så här arbetar du med redovisningsjournaler</span><span class="sxs-lookup"><span data-stu-id="7a55e-119">How to: Work With General Journals</span></span>](ui-work-general-journals.md)  

