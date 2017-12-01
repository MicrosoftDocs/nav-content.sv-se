---
title: "Så här bokför du preliminära fakturor med ankomstregistrering"
description: "Med en ankomstregistrering kan du bokföra en preliminär inköpsfaktura, som du senare skriver över när du bokför fakturan som vanligt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 894b1bbd97c5469281a1d5e1173b1870e301c45a
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-post-preliminary-invoices-by-using-inward-registration"></a><span data-ttu-id="0ba01-103">Så här bokför du preliminära fakturor med ankomstregistrering</span><span class="sxs-lookup"><span data-stu-id="0ba01-103">How to: Post Preliminary Invoices by Using Inward Registration</span></span>
<span data-ttu-id="0ba01-104">Med en ankomstregistrering kan du bokföra en preliminär inköpsfaktura, som du senare skriver över när du bokför fakturan som vanligt.</span><span class="sxs-lookup"><span data-stu-id="0ba01-104">Use an inward registration to post a preliminary purchase invoice, which you overwrite later when you post the invoice normally.</span></span> <span data-ttu-id="0ba01-105">Mer information finns i Ankomstregistrering.</span><span class="sxs-lookup"><span data-stu-id="0ba01-105">For more information, see Inward Registration.</span></span>  

## <a name="to-post-a-preliminary-invoice"></a><span data-ttu-id="0ba01-106">Så här bokför du en preliminär faktura</span><span class="sxs-lookup"><span data-stu-id="0ba01-106">To post a preliminary invoice</span></span>  

1.  <span data-ttu-id="0ba01-107">Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inköpsfakturor** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="0ba01-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0ba01-108">Välj en faktura eller skapa en ny faktura.</span><span class="sxs-lookup"><span data-stu-id="0ba01-108">Select an invoice, or create a new invoice.</span></span>  
3.  <span data-ttu-id="0ba01-109">Välj åtgärd **Ankomstregistrering**.</span><span class="sxs-lookup"><span data-stu-id="0ba01-109">Choose the **Inward Registration** action.</span></span>  
4.  <span data-ttu-id="0ba01-110">Välj **Ny**, ange ett leverantörsfakturanummer i huvudet i fönstret **Ankomstregistrering** och fyll sedan i raderna på det sätt som beskrivs i följande tabell.</span><span class="sxs-lookup"><span data-stu-id="0ba01-110">Choose **New**, enter a vendor invoice number on the header of the **Inward Registration** window, and then fill in the lines as described in the following table.</span></span>  

    |<span data-ttu-id="0ba01-111">Fält</span><span class="sxs-lookup"><span data-stu-id="0ba01-111">Field</span></span>|<span data-ttu-id="0ba01-112">Description</span><span class="sxs-lookup"><span data-stu-id="0ba01-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="0ba01-113">**Moms produktbokföringsmall**</span><span class="sxs-lookup"><span data-stu-id="0ba01-113">**VAT Prod. Posting Group**</span></span>|<span data-ttu-id="0ba01-114">Ange en momsbokföringsmall.</span><span class="sxs-lookup"><span data-stu-id="0ba01-114">Enter a VAT posting group.</span></span> <span data-ttu-id="0ba01-115">Den här koden används tillsammans med rörelsebokföringsmallen för moms för att hämta momssatsen och momsberäkningstypen.</span><span class="sxs-lookup"><span data-stu-id="0ba01-115">This code is used in conjunction with the VAT business posting group to retrieve the VAT percentage and the VAT calculation type.</span></span>|  
    |<span data-ttu-id="0ba01-116">**Produktbokföringsmall**</span><span class="sxs-lookup"><span data-stu-id="0ba01-116">**Gen. Prod. Posting Group**</span></span>|<span data-ttu-id="0ba01-117">Ange en generell bokföringsmall.</span><span class="sxs-lookup"><span data-stu-id="0ba01-117">Enter a general posting group.</span></span>|  

5.  <span data-ttu-id="0ba01-118">Om du vill bokföra preliminära fakturan väljer du åtgärden **Bokför**.</span><span class="sxs-lookup"><span data-stu-id="0ba01-118">Choose the **Post** action to post the preliminary invoice.</span></span>  
6.  <span data-ttu-id="0ba01-119">Välj **Ja** för att bekräfta att du vill bokföra ankomstregistreringen.</span><span class="sxs-lookup"><span data-stu-id="0ba01-119">Choose the **Yes** button to confirm that you want to post the inward registration.</span></span>  

<span data-ttu-id="0ba01-120">Nu skapas en ankomstregistrering. Den representerar den preliminära fakturabokföringen tills du senare skriver över den med den slutgiltiga fakturabokföringen.</span><span class="sxs-lookup"><span data-stu-id="0ba01-120">An inward registration is now created to represent the preliminary invoice posting until you overwrite it with the final invoice posting later.</span></span> <span data-ttu-id="0ba01-121">Du kan visa den positiva transaktionen som skapas i fönstret **Ankomstreg.trans.**.</span><span class="sxs-lookup"><span data-stu-id="0ba01-121">You can see the resulting positive entry in the **Inward Reg. Entry** window.</span></span>  

<span data-ttu-id="0ba01-122">Om du vill ångra ankomstregistreringen före den slutgiltiga fakturabokföringen måste du återföra ankomstregistreringen manuellt.</span><span class="sxs-lookup"><span data-stu-id="0ba01-122">If you want to cancel the inward registration before the final invoice posting, then you must reverse the inward registration manually.</span></span> <span data-ttu-id="0ba01-123">Mer information finns i [Så här återför du preliminära fakturor med ankomstregistrering](how-to-reverse-preliminary-invoices-by-using-inward-registration.md)</span><span class="sxs-lookup"><span data-stu-id="0ba01-123">For more information, see [How to: Reverse Preliminary Invoices by Using Inward Registration](how-to-reverse-preliminary-invoices-by-using-inward-registration.md)</span></span>  

## <a name="see-also"></a><span data-ttu-id="0ba01-124">Se även</span><span class="sxs-lookup"><span data-stu-id="0ba01-124">See Also</span></span>  
 <span data-ttu-id="0ba01-125">[Så här registrerar du inköp](../../purchasing-how-record-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="0ba01-125">[How to: Record Purchases](../../purchasing-how-record-purchases.md) </span></span>  
 <span data-ttu-id="0ba01-126">[Så här återför du preliminära fakturor med ankomstregistrering](how-to-reverse-preliminary-invoices-by-using-inward-registration.md) </span><span class="sxs-lookup"><span data-stu-id="0ba01-126">[How to: Reverse Preliminary Invoices by Using Inward Registration](how-to-reverse-preliminary-invoices-by-using-inward-registration.md) </span></span>  
 <span data-ttu-id="0ba01-127">[Så här: rapportera moms till skattemyndigheterna](../../finance-how-report-vat.md) </span><span class="sxs-lookup"><span data-stu-id="0ba01-127">[How to: Report VAT to Tax Authorities](../../finance-how-report-vat.md) </span></span>  
 [<span data-ttu-id="0ba01-128">Lokal funktionalitet för Sverige</span><span class="sxs-lookup"><span data-stu-id="0ba01-128">Sweden Local Functionality</span></span>](sweden-local-functionality.md)

