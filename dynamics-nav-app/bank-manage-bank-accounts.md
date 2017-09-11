---
title: Hantera bankkonton
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d97c3afba0e899768bda1b637c4f288db210d38c
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="manage-bank-accounts"></a><span data-ttu-id="003aa-102">Hantera bankkonton</span><span class="sxs-lookup"><span data-stu-id="003aa-102">Manage Bank Accounts</span></span>
<span data-ttu-id="003aa-103">Du måste regelbundet stämma av dina banktransaktionerna i Dynamics NAV med de relaterade transaktionerna på dina bankkonton i din bank och sedan bokföra saldot till ditt bankkonto.</span><span class="sxs-lookup"><span data-stu-id="003aa-103">At regular intervals, you must reconcile your bank ledger entries in Dynamics NAV with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="003aa-104">Du kan utföra denna aktivitet antingen som en del av bearbetning av betalningarna som representeras på kontoutdraget i **Betalningsavstämningsjournal**.</span><span class="sxs-lookup"><span data-stu-id="003aa-104">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="003aa-105">Eller så kan du utföra aktiviteten separat från betalningsbehandling i fönstret **Bankkontoavstämning** som stöder checktransaktioner</span><span class="sxs-lookup"><span data-stu-id="003aa-105">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports check ledger entries.</span></span> <span data-ttu-id="003aa-106">I båda fallen fyller du i fönstren genom att importera kontoutdraget till Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="003aa-106">In both cases, you fill the windows by importing the bank statement into Dynamics NAV.</span></span>

<span data-ttu-id="003aa-107">Ibland kan du överföra belopp mellan bankkontot i Dynamics NAV för att visa överföringar på din bank.</span><span class="sxs-lookup"><span data-stu-id="003aa-107">Sometimes, you need to transfer amounts between bank account in Dynamics NAV to reflect transfers at your bank.</span></span> <span data-ttu-id="003aa-108">Du utför denna aktivitet i fönstret **redovisningsjournal** på olika sätt beroende på pengarnas valuta.</span><span class="sxs-lookup"><span data-stu-id="003aa-108">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="003aa-109">Innan du kan hantera bankkonton, måste du registrera varje bankkonto som bankkontokort.</span><span class="sxs-lookup"><span data-stu-id="003aa-109">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="003aa-110">Dessutom måste du skapa elektroniska tjänster som du kan använda för kontoutdragsimport-och betalningsfilexport.</span><span class="sxs-lookup"><span data-stu-id="003aa-110">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="003aa-111">Mer information finns i [Skapa bankkonton](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="003aa-111">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="003aa-112">I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.</span><span class="sxs-lookup"><span data-stu-id="003aa-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="003aa-113">Om du vill</span><span class="sxs-lookup"><span data-stu-id="003aa-113">To</span></span> |<span data-ttu-id="003aa-114">Gå till</span><span class="sxs-lookup"><span data-stu-id="003aa-114">See</span></span> |
|---|----|
|<span data-ttu-id="003aa-115">Stämma av bankkonton i samband med betalningsbehandling i fönstret **Betalningsavstämningsjournal**.</span><span class="sxs-lookup"><span data-stu-id="003aa-115">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span>|[<span data-ttu-id="003aa-116">Koppla utbetalningar automatiskt och stämma av bankkonton</span><span class="sxs-lookup"><span data-stu-id="003aa-116">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|<span data-ttu-id="003aa-117">Du kan stämma av bankkonton inklusive checktransaktioner som en separat aktivitet i fönstret **Bankkontoavstämning**.</span><span class="sxs-lookup"><span data-stu-id="003aa-117">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span>|[<span data-ttu-id="003aa-118">Så här stämmer du av bankkonton separat</span><span class="sxs-lookup"><span data-stu-id="003aa-118">How to: Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md)|
|<span data-ttu-id="003aa-119">bokföra överföringar mellan bankkonton i samma valuta eller olika valutor.</span><span class="sxs-lookup"><span data-stu-id="003aa-119">Post transfers between bank accounts in the same currency or in different currencies.</span></span>|[<span data-ttu-id="003aa-120">Så här överför du banktillgångar</span><span class="sxs-lookup"><span data-stu-id="003aa-120">How to: Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)
## <a name="see-also"></a><span data-ttu-id="003aa-121">Se även</span><span class="sxs-lookup"><span data-stu-id="003aa-121">See Also</span></span>  
[<span data-ttu-id="003aa-122">Konfigurera bank</span><span class="sxs-lookup"><span data-stu-id="003aa-122">Set Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="003aa-123">Hantera kundreskontra</span><span class="sxs-lookup"><span data-stu-id="003aa-123">Manage Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="003aa-124">[Hantera likviditet](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="003aa-124">[Manage Payables](payables-manage-payables.md)  </span></span>  
[<span data-ttu-id="003aa-125">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="003aa-125">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="003aa-126">Över affärsområden</span><span class="sxs-lookup"><span data-stu-id="003aa-126">Across Business Areas</span></span>](ui-across-business-areas.md)

