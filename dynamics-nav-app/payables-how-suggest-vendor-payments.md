---
title: "Så här använder du betalningsförslag för leverantörer"
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
ms.openlocfilehash: 3ede5942798e34fd0e4b3ab8cc48ca94eed3d1a4
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-suggest-vendor-payments"></a><span data-ttu-id="5f152-102">Så här använder du betalningsförslag för leverantörer</span><span class="sxs-lookup"><span data-stu-id="5f152-102">How to: Suggest Vendor Payments</span></span>
<span data-ttu-id="5f152-103">I fönstret **Utbetalningsjournal** kan du använda en funktion för att föreslå betalningsrader enligt dina inställningar, till exempel betalningar som förfaller snart eller betalningar där en kassarabatt är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="5f152-103">In the **Payment Journal** window, you can use a function to suggest payment lines according to your settings, such as payments that are due soon or payments where a payment discount is available.</span></span>

<span data-ttu-id="5f152-104">För att dra helt nytta av funktionen Betalningsförslag för lev. måste du först prioritera leverantörerna.</span><span class="sxs-lookup"><span data-stu-id="5f152-104">To benefit fully from the Suggest Vendor Payments function, you must first prioritize your vendors.</span></span> <span data-ttu-id="5f152-105">Mer information finns i [Så här prioriterar du leverantörer](purchasing-how-prioritize-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="5f152-105">For more information, see [How to: Prioritize Vendors](purchasing-how-prioritize-vendors.md).</span></span>

<span data-ttu-id="5f152-106">Leverantörstransaktioner som inte har en markering **Stoppad** tas inte med i batch-jobbet.</span><span class="sxs-lookup"><span data-stu-id="5f152-106">Vendor entries that are not marked **On Hold** are not included in the batch job.</span></span>  

<span data-ttu-id="5f152-107">**Viktigt!** Om du vill utnyttja kassarabatterna och har angett ett disponibelt belopp, används beloppet först för prioriterade leverantörstransaktioner som förfallit, ordnade efter prioritet, därefter för förfallna leverantörstransaktioner som inte prioriterats, och till sist för öppna leverantörstransaktioner berättigade till kassarabatter, ordnade efter leverantörsnummer.</span><span class="sxs-lookup"><span data-stu-id="5f152-107">**Important**: If you want to take advantage of payment discounts and have entered an available amount, the amount will be used for prioritized overdue vendor entries first in order of priority, and then for overdue vendor entries that are not prioritized, and finally for open vendor entries that qualify for payment discounts in order of vendor number.</span></span>

## <a name="to-use-the-suggest-vendor-payments-function"></a><span data-ttu-id="5f152-108">Om du vill använda funktionen Betalningsförslag för lev.</span><span class="sxs-lookup"><span data-stu-id="5f152-108">To use the Suggest Vendor Payments function</span></span>
1. <span data-ttu-id="5f152-109">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningsjournal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="5f152-109">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="5f152-110">Öppna den relevanta journalen och välj sedan åtgärden **Betalningsförslag för lev.**.</span><span class="sxs-lookup"><span data-stu-id="5f152-110">Open the relevant journal, and then choose the **Suggest Vendor Payments** action.</span></span>
3. <span data-ttu-id="5f152-111">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="5f152-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="5f152-112">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="5f152-112">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="5f152-113">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="5f152-113">Choose the **OK** button.</span></span>

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a><span data-ttu-id="5f152-114">Så här infogar du förfallodatum som bokföringsdatum på betalningsjournalrader</span><span class="sxs-lookup"><span data-stu-id="5f152-114">To insert the due date as posting date on payment journal lines</span></span>
<span data-ttu-id="5f152-115">När du använder **Betalningsförslag för lev.**-batchjobbet för att skapa betalningsrader för leverantörer, kan du fylla två specialfält så att de genererade raderna använder förfallodatumet för att beräkna bokföringsdatumet.</span><span class="sxs-lookup"><span data-stu-id="5f152-115">When you use the **Suggest Vendor Payments** batch job to create payment lines for your vendors, you can fill two special fields to make sure that the generated lines use the due date to calculate the posting date.</span></span> <span data-ttu-id="5f152-116">Dessa fält är **Beräkna bokföringsdatum från dokumentets förfallodatum** och **Dokumentets förfallodatum är förskjutet**.</span><span class="sxs-lookup"><span data-stu-id="5f152-116">These fields are **Calculate Posting Date from Applies-to-Doc Due Date** and **Applies-to-Doc Due Date Offset**.</span></span>

<span data-ttu-id="5f152-117">**Viktigt!** Du kan inte använda fältet **Beräkna bokföringsdatum från dokumentets förfallodatum** tillsammans med fältet **Utnyttja kassarabatter** eller fältet **Summering per leverantör**.</span><span class="sxs-lookup"><span data-stu-id="5f152-117">**Important**: You cannot use the **Calculate Posting Date from Applies-to-Doc Due Date** field together with the **Find Payment Discounts** field or the **Summarize per Vendor** field.</span></span> <span data-ttu-id="5f152-118">Anledningen är att om bokföringsdatumet baseras på förfallodatum, så kan en kassarabatt kanske inte beräknas korrekt eftersom bokföringsdatumet kan inträffa efter kassarabattdatumet.</span><span class="sxs-lookup"><span data-stu-id="5f152-118">The reason is that if the posting date is based on the due date, then some payment discount may not be calculated correctly, because the posting date could occur after the payment discount date.</span></span>
<span data-ttu-id="5f152-119">Om det beräknade bokföringsdatum inträffar tidigare flyttas bokföringsdatumet fram till arbetsdatumet, och en varning visas.</span><span class="sxs-lookup"><span data-stu-id="5f152-119">Also, if the calculated posting date occurs in the past, then the posting date will be moved up to the work date, and a warning is displayed.</span></span>

<span data-ttu-id="5f152-120">Du kan även skapa betalningsrader manuellt genom att använda förfallodatum för att beräkna bokföringsdatum</span><span class="sxs-lookup"><span data-stu-id="5f152-120">Alternatively, you can also manually create payment lines using the due date to calculate the posting date.</span></span> <span data-ttu-id="5f152-121">När du har kopplat leverantörsreskontratransaktioner kan du använda åtgärden **Beräkna bokföringsdatum**.</span><span class="sxs-lookup"><span data-stu-id="5f152-121">After you have applied vendor ledger entries, you can use the **Calculate Posting Date** action.</span></span> <span data-ttu-id="5f152-122">Detta upptaerar bokföringsdatumet på journalraden till förfallodatum på den relaterade inköpsfakturan.</span><span class="sxs-lookup"><span data-stu-id="5f152-122">This will update the posting date on the journal line with the due date of the related purchase invoice.</span></span> <span data-ttu-id="5f152-123">Mer information finns i [Så här kopplar du inköpstransaktioner manuellt](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="5f152-123">For more information, see [How to: Apply Purchase Transactions Manually](payables-how-apply-purchase-transactions-manually.md).</span></span>  

<span data-ttu-id="5f152-124">**Obs!** Om inköpsfakturan har förfallit kommer bokföringsdatum att anges till arbetsdatumet, och teckensnittet på raden ändras till röd färg.</span><span class="sxs-lookup"><span data-stu-id="5f152-124">**Note**: If the purchase invoice is overdue, then the posting date will be set to the work date, and the font on the line will change to red color.</span></span>

## <a name="see-also"></a><span data-ttu-id="5f152-125">Se även</span><span class="sxs-lookup"><span data-stu-id="5f152-125">See Also</span></span>
[<span data-ttu-id="5f152-126">Hantera likviditet</span><span class="sxs-lookup"><span data-stu-id="5f152-126">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="5f152-127">Gör utbetalningar</span><span class="sxs-lookup"><span data-stu-id="5f152-127">Make Payments</span></span>](payables-make-payments.md)  
[<span data-ttu-id="5f152-128">Arbeta med redovisningsjournaler</span><span class="sxs-lookup"><span data-stu-id="5f152-128">Work with General Journals</span></span>](ui-work-general-journals.md)

