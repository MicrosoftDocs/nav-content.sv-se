---
title: Ange villkor i filter
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: df386e1195db385ee053b69fec0f5082d8df4116
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="entering-criteria-in-filters"></a><span data-ttu-id="95a50-102">Ange villkor i filter</span><span class="sxs-lookup"><span data-stu-id="95a50-102">Entering Criteria in Filters</span></span>
<span data-ttu-id="95a50-103">När du vill söka efter data, till exempel kundnamn, adresser eller produktgrupper, anger du kriterier.</span><span class="sxs-lookup"><span data-stu-id="95a50-103">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="95a50-104">I sökkriterier kan du använda alla siffror och bokstäver som du normalt kan använda i det specifika fältet.</span><span class="sxs-lookup"><span data-stu-id="95a50-104">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="95a50-105">Dessutom kan du använda specialtecken som du vill filtrera resultatet ytterligare.</span><span class="sxs-lookup"><span data-stu-id="95a50-105">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="95a50-106">Sök genom att använda snabbfiltret</span><span class="sxs-lookup"><span data-stu-id="95a50-106">Searching using the Quick Filter</span></span>
<span data-ttu-id="95a50-107">Du kan lägga till filter för alla sidor genom att använda snabbfiltret.</span><span class="sxs-lookup"><span data-stu-id="95a50-107">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="95a50-108">Snabbfiltret aktiveras genom att välja ikonen med förstoringsglas i det övre högra hörnet av en sida.</span><span class="sxs-lookup"><span data-stu-id="95a50-108">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="95a50-109">Filtrering av den här typen används för att snabbt ange kriterier.</span><span class="sxs-lookup"><span data-stu-id="95a50-109">This filtering type is used for a fast entry of criteria.</span></span>

<span data-ttu-id="95a50-110">**Viktigt!** Snabbfiltret ger enkelt tillgång till filterdata genom att ange vanlig text, men ger även många alternativet för sökningkriterier.</span><span class="sxs-lookup"><span data-stu-id="95a50-110">**Important**: The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="95a50-111">Beroende på om du anger vanlig text, eller text inklusive symboler, uppför sig snabbfiltret på olika sätt.</span><span class="sxs-lookup"><span data-stu-id="95a50-111">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  
- <span data-ttu-id="95a50-112">Om du anger vanlig text i sökkriterierna tolkas sökkriterierna som en skiftlägesokänslig sökning som innehåller viss text.</span><span class="sxs-lookup"><span data-stu-id="95a50-112">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
- <span data-ttu-id="95a50-113">Om du anger en text inklusive symboler i sökkriterierna tolkas sökkriterierna exakt som du har angett den, och sökningen är skiftlägeskänslig.</span><span class="sxs-lookup"><span data-stu-id="95a50-113">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="95a50-114">Snabbfilterkriterium</span><span class="sxs-lookup"><span data-stu-id="95a50-114">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="95a50-115">Sökkriterier</span><span class="sxs-lookup"><span data-stu-id="95a50-115">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="95a50-116">Tolkat som…</span><span class="sxs-lookup"><span data-stu-id="95a50-116">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="95a50-117">Returer...</span><span class="sxs-lookup"><span data-stu-id="95a50-117">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="95a50-118">>tillverk</span><span class="sxs-lookup"><span data-stu-id="95a50-118">>man</span></span></TD>
    <TD><span data-ttu-id="95a50-119">@*tillverk*</span><span class="sxs-lookup"><span data-stu-id="95a50-119">@*man*</span></span></TD>
    <TD><span data-ttu-id="95a50-120">Alla transaktioner som innehåller texten man och är skiftlägesokänsliga.</span><span class="sxs-lookup"><span data-stu-id="95a50-120">All records that contain the text man and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="95a50-121">>sö</span><span class="sxs-lookup"><span data-stu-id="95a50-121">>se</span></span></TD>
    <TD><span data-ttu-id="95a50-122">@*se*</span><span class="sxs-lookup"><span data-stu-id="95a50-122">@*se*</span></span></TD>
    <TD><span data-ttu-id="95a50-123">Alla transaktioner som innehåller texten se och är skiftlägesokänsliga.</span><span class="sxs-lookup"><span data-stu-id="95a50-123">All records that contain the text se and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="95a50-124">>Tillverk*</span><span class="sxs-lookup"><span data-stu-id="95a50-124">>Man*</span></span></TD>
    <TD><span data-ttu-id="95a50-125">Börjar med Man och är skiftlägeskänsligt.</span><span class="sxs-lookup"><span data-stu-id="95a50-125">Starts with Man and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="95a50-126">Alla poster som börjar med texten Man.</span><span class="sxs-lookup"><span data-stu-id="95a50-126">All records that start with the text Man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="95a50-127">'tillverk'</span><span class="sxs-lookup"><span data-stu-id="95a50-127">'man'</span></span></TD>
    <TD><span data-ttu-id="95a50-128">En exakt text och är skiftlägeskänsligt.</span><span class="sxs-lookup"><span data-stu-id="95a50-128">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="95a50-129">Alla poster som matchar man exakt.</span><span class="sxs-lookup"><span data-stu-id="95a50-129">All records that match man exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="95a50-130">@*tillverk</span><span class="sxs-lookup"><span data-stu-id="95a50-130">@*man</span></span></TD>
    <TD><span data-ttu-id="95a50-131">Slutar på och är skiftlägesokänsligt.</span><span class="sxs-lookup"><span data-stu-id="95a50-131">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="95a50-132">Alla poster som slutar på man.</span><span class="sxs-lookup"><span data-stu-id="95a50-132">All records that end with man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="95a50-133">@man*</span><span class="sxs-lookup"><span data-stu-id="95a50-133">@man*</span></span></TD>
    <TD><span data-ttu-id="95a50-134">Börjar med och skiftlägesokänsligt.</span><span class="sxs-lookup"><span data-stu-id="95a50-134">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="95a50-135">Alla poster som börjar med man.</span><span class="sxs-lookup"><span data-stu-id="95a50-135">All records that start with man.</span></span></TD>
  </TR>
</TABLE>

<span data-ttu-id="95a50-136">**Obs!** Du kan inte använda ett jokertecken när du filtrerar på uppräkningsfält, t.ex fältet **Status** på försäljningsorder.</span><span class="sxs-lookup"><span data-stu-id="95a50-136">**Note**: You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="95a50-137">För att ange ett filter för den här typen av fält kan du ange det numeriska värdet som en filtreringsparameter.</span><span class="sxs-lookup"><span data-stu-id="95a50-137">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="95a50-138">Använd till exempel värdena **0**, **1**, **2** och **3** för att filtrera för dessa alternativ i fältet **Status** på en försäljningsorder, som har värdena **Öppna**, **Släppt**, **Väntar på godkännande** och **Väntar på förskottsbetalning**.</span><span class="sxs-lookup"><span data-stu-id="95a50-138">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="95a50-139">Se även</span><span class="sxs-lookup"><span data-stu-id="95a50-139">See Also</span></span>
[<span data-ttu-id="95a50-140">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="95a50-140">Work with Dynamics NAV</span></span>](ui-work-product.md)

