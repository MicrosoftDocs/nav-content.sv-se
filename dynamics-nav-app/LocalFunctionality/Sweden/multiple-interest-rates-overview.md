---
title: "Flera räntesatser – översikt"
description: "För varje räntevillkorskod kan du ange flera räntesatser så att du kan beräkna dröjsmålsränta med flera räntesatser för en särskild period."
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
ms.openlocfilehash: 5fb19c692c85949cfcf4efda33ee6e0f8292b25c
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="multiple-interest-rates-overview"></a><span data-ttu-id="e3995-103">Flera räntesatser – översikt</span><span class="sxs-lookup"><span data-stu-id="e3995-103">Multiple Interest Rates Overview</span></span>
<span data-ttu-id="e3995-104">För varje räntevillkorskod kan du ange flera räntesatser så att du kan beräkna dröjsmålsränta med flera räntesatser för en särskild period.</span><span class="sxs-lookup"><span data-stu-id="e3995-104">For each finance charge term code, you can specify multiple interest rates so that you can calculate finance charges with multiple interest rates for a specific period.</span></span> <span data-ttu-id="e3995-105">Detta är praktiskt om du debiterar olika räntor på försenade betalningar.</span><span class="sxs-lookup"><span data-stu-id="e3995-105">This is helpful if you charge different interest on payments that are late.</span></span> <span data-ttu-id="e3995-106">Ränteberäkningen görs på samma sätt för alla dröjsmålsräntor, men räntan kan variera under en viss period.</span><span class="sxs-lookup"><span data-stu-id="e3995-106">The interest calculation is the same for each financial charge, with variation only in the rate of interest for a specific period.</span></span>  

## <a name="creating-finance-charges"></a><span data-ttu-id="e3995-107">Skapa dröjsmålsräntor</span><span class="sxs-lookup"><span data-stu-id="e3995-107">Creating Finance Charges</span></span>  
<span data-ttu-id="e3995-108">När du skapar en räntefaktura innehåller raderna dröjsmålsräntor med olika räntesatser för varje tidsperiod.</span><span class="sxs-lookup"><span data-stu-id="e3995-108">When you create a finance charge memo, the memo lines show the finance charges with different interest rates for each time period.</span></span> <span data-ttu-id="e3995-109">För varje räntevillkor kan du ange en beskrivning och du kan definiera en beskrivning som används när flera räntesatser används.</span><span class="sxs-lookup"><span data-stu-id="e3995-109">For finance charge terms, you can define descriptions for each term, and you can define a description that is used when multiple interest rates are used.</span></span>  

<span data-ttu-id="e3995-110">För att kunna använda flera räntesatser måste du först definiera en räntevillkorskod, och du måste sedan lägga till flera räntesatsrader i villkoren.</span><span class="sxs-lookup"><span data-stu-id="e3995-110">To use multiple interest rates, you must first define a finance charge term, and you must then add multiple interest rate lines to the terms.</span></span> <span data-ttu-id="e3995-111">Mer information finns i [Så här ställer du in flera räntesatser](how-to-set-up-multiple-interest-rates.md).</span><span class="sxs-lookup"><span data-stu-id="e3995-111">For more information, see [How to: Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md).</span></span>  

<span data-ttu-id="e3995-112">Om det inte finns flera räntesatser använder [!INCLUDE[navnow](../../includes/navnow_md.md)] den räntesats och den period som definieras i fönstret **Räntevillkor** för hela beräkningsperioden.</span><span class="sxs-lookup"><span data-stu-id="e3995-112">If no multiple interest rates exist, [!INCLUDE[navnow](../../includes/navnow_md.md)] will use the interest rate and period that is defined in the **Finance Charge Terms** window for the whole period of calculation.</span></span>  

## <a name="delayed-payments"></a><span data-ttu-id="e3995-113">Försenade betalningar</span><span class="sxs-lookup"><span data-stu-id="e3995-113">Delayed Payments</span></span>  
<span data-ttu-id="e3995-114">Flera räntesatser används för olika perioder för försenade betalningar i handelstransaktioner.</span><span class="sxs-lookup"><span data-stu-id="e3995-114">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span></span> <span data-ttu-id="e3995-115">En myndighet anger till exempel den högsta räntan som kan tas ut för en kund.</span><span class="sxs-lookup"><span data-stu-id="e3995-115">For example, a government specifies the maximum interest to be levied for a consumer.</span></span> <span data-ttu-id="e3995-116">Den räntan kan ändras två gånger per år, den 1 januari och den 1 juli.</span><span class="sxs-lookup"><span data-stu-id="e3995-116">This interest rate can be changed twice a year on 01 January and 01 July.</span></span> <span data-ttu-id="e3995-117">Räntesatsen mellan företag avtalas av parterna och det finns ingen gräns för den kundgruppen.</span><span class="sxs-lookup"><span data-stu-id="e3995-117">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span></span> <span data-ttu-id="e3995-118">Den räntesatsen ligger vanligtvis 4 procent över den normala bankräntan.</span><span class="sxs-lookup"><span data-stu-id="e3995-118">The announced rate is usually four percent more than the normal bank interest.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e3995-119">Se även</span><span class="sxs-lookup"><span data-stu-id="e3995-119">See Also</span></span>  
 <span data-ttu-id="e3995-120">[Så här ställer du in flera räntesatser](how-to-set-up-multiple-interest-rates.md) </span><span class="sxs-lookup"><span data-stu-id="e3995-120">[How to: Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md) </span></span>  
 [<span data-ttu-id="e3995-121">Så här kräver du in utestående saldon</span><span class="sxs-lookup"><span data-stu-id="e3995-121">How to: Collect Outstanding Balances</span></span>](../../receivables-collect-outstanding-balances.md)

