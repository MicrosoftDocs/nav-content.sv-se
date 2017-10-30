---
title: "Söka efter data och ange filterkriterier"
description: "Beskriver hur du arbetar med filter, till exempel snabbfiltret för att förfina resultaten när du söker efter data."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f981d303f75bba627e224e49b9e2f2818246fe39
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="searching-filtering-and-sorting-data"></a><span data-ttu-id="46127-103">Söka, filtrera och sortera data</span><span class="sxs-lookup"><span data-stu-id="46127-103">Searching, Filtering, and Sorting Data</span></span>
<span data-ttu-id="46127-104">Det finns några saker som du kan göra som hjälper dig att hitta, precisera och skanna poster i en lista.</span><span class="sxs-lookup"><span data-stu-id="46127-104">There are a few things that you can do that will help you find, pinpoint, and scan records in a list.</span></span> <span data-ttu-id="46127-105">Dessa inkluderar sortering, sökning och filtrering.</span><span class="sxs-lookup"><span data-stu-id="46127-105">These include sorting, searching and filtering.</span></span>

<span data-ttu-id="46127-106">När du vill söka efter data, till exempel kundnamn, adresser eller produktgrupper, anger du kriterier.</span><span class="sxs-lookup"><span data-stu-id="46127-106">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="46127-107">I sökkriterier kan du använda alla siffror och bokstäver som du normalt kan använda i det specifika fältet.</span><span class="sxs-lookup"><span data-stu-id="46127-107">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="46127-108">Dessutom kan du använda specialtecken som du vill filtrera resultatet ytterligare.</span><span class="sxs-lookup"><span data-stu-id="46127-108">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="46127-109">Det finns två sätt att söka: använda snabbfilter eller kolumn filtren.</span><span class="sxs-lookup"><span data-stu-id="46127-109">There are two ways to search: using the Quick Filter or column filters.</span></span>

## <a name="sorting"></a><span data-ttu-id="46127-110">Sortering</span><span class="sxs-lookup"><span data-stu-id="46127-110">Sorting</span></span>
<span data-ttu-id="46127-111">Med hjälp av sorteringsfunktionen kan du snabbt få en överblick över dina data.</span><span class="sxs-lookup"><span data-stu-id="46127-111">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="46127-112">Om t.ex. har många kunder kan du sortera dem efter **Kundnr.**, **Kundbokföringsmall**, **Valutakod**, **Lands-/regionkod**, eller **Momsregistreringsnr.** för att få den översikt som du behöver.</span><span class="sxs-lookup"><span data-stu-id="46127-112">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="46127-113">Om du vill sortera en lista, kan du välja en kolumn rubriktexten för att växla mellan stigande och fallande ordning, eller välja små listrutor pilen i kolumnrubriken och välj **stigande** eller **fallande**.</span><span class="sxs-lookup"><span data-stu-id="46127-113">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small downs arrow in the column heading, and then choose **Ascending** or **Descending**.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="46127-114">Sortering stöds inte på bilder, BLOB-fält, Flowfilter och fält som inte tillhör samma tabell.</span><span class="sxs-lookup"><span data-stu-id="46127-114">Sorting is not supported images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching-by-using-the-quick-filter"></a><span data-ttu-id="46127-115">Sök genom att använda snabbfiltret</span><span class="sxs-lookup"><span data-stu-id="46127-115">Searching by using the Quick Filter</span></span>
<span data-ttu-id="46127-116">Du kan lägga till filter för alla sidor genom att använda snabbfiltret.</span><span class="sxs-lookup"><span data-stu-id="46127-116">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="46127-117">Snabbfiltret aktiveras genom att välja ikonen med förstoringsglas i det övre högra hörnet av en sida.</span><span class="sxs-lookup"><span data-stu-id="46127-117">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="46127-118">Filtrering av den här typen används för att snabbt ange kriterier.</span><span class="sxs-lookup"><span data-stu-id="46127-118">This filtering type is used for a fast entry of criteria.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="46127-119">Snabbfiltret ger enkelt tillgång till filterdata genom att ange vanlig text, men ger även många alternativet för sökningkriterier.</span><span class="sxs-lookup"><span data-stu-id="46127-119">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="46127-120">Beroende på om du anger vanlig text, eller text inklusive symboler, uppför sig snabbfiltret på olika sätt.</span><span class="sxs-lookup"><span data-stu-id="46127-120">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  

* <span data-ttu-id="46127-121">Om du anger vanlig text i sökkriterierna tolkas sökkriterierna som en skiftlägesokänslig sökning som innehåller viss text.</span><span class="sxs-lookup"><span data-stu-id="46127-121">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
* <span data-ttu-id="46127-122">Om du anger en text inklusive symboler i sökkriterierna tolkas sökkriterierna exakt som du har angett den, och sökningen är skiftlägeskänslig.</span><span class="sxs-lookup"><span data-stu-id="46127-122">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="46127-123">Snabbfilterkriterium</span><span class="sxs-lookup"><span data-stu-id="46127-123">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="46127-124">Sökkriterier</span><span class="sxs-lookup"><span data-stu-id="46127-124">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="46127-125">Tolkat som…</span><span class="sxs-lookup"><span data-stu-id="46127-125">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="46127-126">Returer...</span><span class="sxs-lookup"><span data-stu-id="46127-126">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="46127-127">tillverk</span><span class="sxs-lookup"><span data-stu-id="46127-127">man</span></span></TD>
    <TD><span data-ttu-id="46127-128">@&#42;man&#42;</span><span class="sxs-lookup"><span data-stu-id="46127-128">@&#42;man&#42;</span></span></TD>
    <TD><span data-ttu-id="46127-129">Alla transaktioner som innehåller texten <b>man</b> och är skiftlägesokänsliga.</span><span class="sxs-lookup"><span data-stu-id="46127-129">All records that contain the text <b>man</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="46127-130">sö</span><span class="sxs-lookup"><span data-stu-id="46127-130">se</span></span></TD>
    <TD><span data-ttu-id="46127-131">@&#42;se&#42;</span><span class="sxs-lookup"><span data-stu-id="46127-131">@&#42;se&#42;</span></span></TD>
    <TD><span data-ttu-id="46127-132">Alla transaktioner som innehåller texten <b>se</b> och är skiftlägesokänsliga.</span><span class="sxs-lookup"><span data-stu-id="46127-132">All records that contain the text <b>se</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="46127-133">Man&#42;</span><span class="sxs-lookup"><span data-stu-id="46127-133">Man&#42;</span></span></TD>
    <TD><span data-ttu-id="46127-134">Börjar med <b>Man</b> och är skiftlägeskänsligt.</span><span class="sxs-lookup"><span data-stu-id="46127-134">Starts with <b>Man</b> and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="46127-135">Alla poster som börjar med texten <b>Man</b>.</span><span class="sxs-lookup"><span data-stu-id="46127-135">All records that start with the text <b>Man</b>.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="46127-136">'tillverk'</span><span class="sxs-lookup"><span data-stu-id="46127-136">'man'</span></span></TD>
    <TD><span data-ttu-id="46127-137">En exakt text och är skiftlägeskänsligt.</span><span class="sxs-lookup"><span data-stu-id="46127-137">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="46127-138">Alla poster som matchar <b>man</b> exakt.</span><span class="sxs-lookup"><span data-stu-id="46127-138">All records that match <b>man</b> exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="46127-139">@man*</span><span class="sxs-lookup"><span data-stu-id="46127-139">@man*</span></span> </TD>
    <TD><span data-ttu-id="46127-140">Börjar med och skiftlägesokänsligt.</span><span class="sxs-lookup"><span data-stu-id="46127-140">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="46127-141">Alla poster som börjar med <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="46127-141">All records that start with <b>man</b>.</span></span></TD>
  </TR>
    <TR>
    <TD><span data-ttu-id="46127-142">@&#42;man</span><span class="sxs-lookup"><span data-stu-id="46127-142">@&#42;man</span></span></TD>
    <TD><span data-ttu-id="46127-143">Slutar på och är skiftlägesokänsligt.</span><span class="sxs-lookup"><span data-stu-id="46127-143">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="46127-144">Alla poster som slutar på <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="46127-144">All records that end with <b>man</b>.</span></span></TD>
  </TR>
</TABLE>

> [!NOTE]  
>   <span data-ttu-id="46127-145">Du kan inte använda ett jokertecken när du filtrerar på uppräkningsfält, t.ex fältet **Status** på försäljningsorder.</span><span class="sxs-lookup"><span data-stu-id="46127-145">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="46127-146">För att ange ett filter för den här typen av fält kan du ange det numeriska värdet som en filtreringsparameter.</span><span class="sxs-lookup"><span data-stu-id="46127-146">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="46127-147">Använd till exempel värdena **0**, **1**, **2** och **3** för att filtrera för dessa alternativ i fältet **Status** på en försäljningsorder, som har värdena **Öppna**, **Släppt**, **Väntar på godkännande** och **Väntar på förskottsbetalning**.</span><span class="sxs-lookup"><span data-stu-id="46127-147">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span> 

## <a name="searching-by-using-column-filters"></a><span data-ttu-id="46127-148">Söka med hjälp av kolumnfilter</span><span class="sxs-lookup"><span data-stu-id="46127-148">Searching by using column Filters</span></span>
<span data-ttu-id="46127-149">Du kan lägga till ett filter för en eller flera kolumner i en lista.</span><span class="sxs-lookup"><span data-stu-id="46127-149">You can add a filter on one or more columns in a list.</span></span> <span data-ttu-id="46127-150">Filtrera efter kolumner är mer flexibelt och bättre än snabbfiltret.</span><span class="sxs-lookup"><span data-stu-id="46127-150">Filtering on columns is more flexible and enhanced than the Quick Filter.</span></span> 

### <a name="to-add-a-filter-on-a-column"></a><span data-ttu-id="46127-151">Lägga till ett filter på en kolumn</span><span class="sxs-lookup"><span data-stu-id="46127-151">To add a filter on a column</span></span>
1.  <span data-ttu-id="46127-152">Innan du lägger till ett filter kan du välja ![visa som lista](media/ui_show_as_list_icon.png "Visa som lista VÄNSTERPIL") om du vill ändra i vyn lista.</span><span class="sxs-lookup"><span data-stu-id="46127-152">Before you add a filter, choose ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to change to the list view.</span></span>
2. <span data-ttu-id="46127-153">Välj den nedåt pilen i kolumnrubriken och välj **Filter**.</span><span class="sxs-lookup"><span data-stu-id="46127-153">Choose the downwards arrow in the column heading, and then choose **Filter**.</span></span>
3. <span data-ttu-id="46127-154">Gör något av följande:</span><span class="sxs-lookup"><span data-stu-id="46127-154">Do one of the following:</span></span> 
  -  <span data-ttu-id="46127-155">Välj *...* bredvid rutan Välj ett värde i listan.</span><span class="sxs-lookup"><span data-stu-id="46127-155">Choose *...* next to the box to select a value from a list.</span></span>
  -  <span data-ttu-id="46127-156">Ange filtervillkor i rutan</span><span class="sxs-lookup"><span data-stu-id="46127-156">Enter filter criteria in the box.</span></span> <span data-ttu-id="46127-157">Se avsnittet Mer information.</span><span class="sxs-lookup"><span data-stu-id="46127-157">See the next section for details.</span></span>
4. <span data-ttu-id="46127-158">Välj knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="46127-158">Choose the **OK** button.</span></span>

## <a name="filter-criteria-and-symbols"></a><span data-ttu-id="46127-159">Filterkriterier och symboler</span><span class="sxs-lookup"><span data-stu-id="46127-159">Filter criteria and symbols</span></span>
<span data-ttu-id="46127-160">När du anger kriterier kan du använda alla siffror och bokstäver som du normalt kan använda i fältet.</span><span class="sxs-lookup"><span data-stu-id="46127-160">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="46127-161">Dessutom kan du använda specialtecken som du vill filtrera resultatet ytterligare.</span><span class="sxs-lookup"><span data-stu-id="46127-161">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="46127-162">I tabellen nedan visas de symboler som kan användas i filter.</span><span class="sxs-lookup"><span data-stu-id="46127-162">The following tables show the symbols which can be used in filters.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="46127-163">Det kan finnas fall där fältvärdena innehåller dessa symboler och du vill filtrera efter de.</span><span class="sxs-lookup"><span data-stu-id="46127-163">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="46127-164">Genom att ibland behöva du inkludera det filteruttryck som innehåller symbolen med citattecken (”).</span><span class="sxs-lookup"><span data-stu-id="46127-164">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="46127-165">Om du vill filtrera poster som börjar med texten till exempel *S&R*, är filteruttrycket **S&R*'**.</span><span class="sxs-lookup"><span data-stu-id="46127-165">For example, if you want to filter on records that start with the text *S&R*, the filter expression is **'S&R*'**.</span></span>  
  
### <a name="-interval"></a><span data-ttu-id="46127-166">(..) Intervall</span><span class="sxs-lookup"><span data-stu-id="46127-166">(..) Interval</span></span>  
  
|<span data-ttu-id="46127-167">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-167">Sample Expression</span></span>|<span data-ttu-id="46127-168">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-168">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-169">1100..2100</span><span class="sxs-lookup"><span data-stu-id="46127-169">1100..2100</span></span>|<span data-ttu-id="46127-170">Fr.o.m. 1100 t.o.m. 2100</span><span class="sxs-lookup"><span data-stu-id="46127-170">Numbers 1100 through 2100</span></span>|  
|<span data-ttu-id="46127-171">..2500</span><span class="sxs-lookup"><span data-stu-id="46127-171">..2500</span></span>|<span data-ttu-id="46127-172">Alla t.o.m. 2500</span><span class="sxs-lookup"><span data-stu-id="46127-172">Up to and including 2500</span></span>|  
|<span data-ttu-id="46127-173">..12 31 00</span><span class="sxs-lookup"><span data-stu-id="46127-173">..12 31 00</span></span>|<span data-ttu-id="46127-174">Datum t.o.m. 00-12-31</span><span class="sxs-lookup"><span data-stu-id="46127-174">Dates up to and including 12 31 00</span></span>|  
|<span data-ttu-id="46127-175">P8..</span><span class="sxs-lookup"><span data-stu-id="46127-175">P8..</span></span>|<span data-ttu-id="46127-176">Information för bokföringsperiod 8 och framåt</span><span class="sxs-lookup"><span data-stu-id="46127-176">Information for accounting period 8 and thereafter</span></span>|  
|<span data-ttu-id="46127-177">..23</span><span class="sxs-lookup"><span data-stu-id="46127-177">..23</span></span>|<span data-ttu-id="46127-178">Från startdatumet till den 23 innevarande månad, innevarande år 23:59:59</span><span class="sxs-lookup"><span data-stu-id="46127-178">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|<span data-ttu-id="46127-179">23..</span><span class="sxs-lookup"><span data-stu-id="46127-179">23..</span></span>|<span data-ttu-id="46127-180">Från 23 innevarande månad, innevarande år 0:00:00 till tidsperiodens slut</span><span class="sxs-lookup"><span data-stu-id="46127-180">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|<span data-ttu-id="46127-181">22..23</span><span class="sxs-lookup"><span data-stu-id="46127-181">22..23</span></span>|<span data-ttu-id="46127-182">Från 22 innevarande månad, innevarande år 0:00:00 till 23 innevarande månad, innevarande år 23:59:59</span><span class="sxs-lookup"><span data-stu-id="46127-182">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  
  
### <a name="124-eitheror"></a><span data-ttu-id="46127-183">(&#124;) Antingen/eller</span><span class="sxs-lookup"><span data-stu-id="46127-183">(&#124;) Either/or</span></span>  
  
|<span data-ttu-id="46127-184">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-184">Sample Expression</span></span>|<span data-ttu-id="46127-185">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-185">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-186">1200&#124;1300</span><span class="sxs-lookup"><span data-stu-id="46127-186">1200&#124;1300</span></span>|<span data-ttu-id="46127-187">Nummer med 1200 eller 1300</span><span class="sxs-lookup"><span data-stu-id="46127-187">Numbers with 1200 or 1300</span></span>|  
  
### <a name="-not-equal-to"></a><span data-ttu-id="46127-188">(<>) Inte lika med</span><span class="sxs-lookup"><span data-stu-id="46127-188">(<>) Not equal to</span></span>  
  
|<span data-ttu-id="46127-189">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-189">Sample Expression</span></span>|<span data-ttu-id="46127-190">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-190">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-191"><>0</span><span class="sxs-lookup"><span data-stu-id="46127-191"><>0</span></span>|<span data-ttu-id="46127-192">Alla nummer förutom 0</span><span class="sxs-lookup"><span data-stu-id="46127-192">All numbers except 0</span></span><br /><br /> <span data-ttu-id="46127-193">SQL-serveralternativet låter dig kombinera tecknet med ett jokertecken.</span><span class="sxs-lookup"><span data-stu-id="46127-193">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="46127-194">Till exempel betyder <>A* inte lika med valfri text som börjar med A.</span><span class="sxs-lookup"><span data-stu-id="46127-194">For example, <>A* meaning not equal to any text that starts with A.</span></span>|  
  
### <a name="-greater-than"></a><span data-ttu-id="46127-195">(>) Större än</span><span class="sxs-lookup"><span data-stu-id="46127-195">(>) Greater than</span></span>  
  
|<span data-ttu-id="46127-196">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-196">Sample Expression</span></span>|<span data-ttu-id="46127-197">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-197">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-198">>1200</span><span class="sxs-lookup"><span data-stu-id="46127-198">>1200</span></span>|<span data-ttu-id="46127-199">Nummer större än 1200</span><span class="sxs-lookup"><span data-stu-id="46127-199">Numbers greater than 1200</span></span>|  
  
### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="46127-200">(>=) Större än eller lika med</span><span class="sxs-lookup"><span data-stu-id="46127-200">(>=) Greater than or equal to</span></span>  
  
|<span data-ttu-id="46127-201">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-201">Sample Expression</span></span>|<span data-ttu-id="46127-202">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-202">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-203">>=1200</span><span class="sxs-lookup"><span data-stu-id="46127-203">>=1200</span></span>|<span data-ttu-id="46127-204">Nummer större än eller lika med 1200</span><span class="sxs-lookup"><span data-stu-id="46127-204">Numbers greater than or equal to 1200</span></span>|  
  
### <a name="-less-than"></a><span data-ttu-id="46127-205">(<) Mindre än</span><span class="sxs-lookup"><span data-stu-id="46127-205">(<) Less than</span></span>  
  
|<span data-ttu-id="46127-206">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-206">Sample Expression</span></span>|<span data-ttu-id="46127-207">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-207">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-208"><1200</span><span class="sxs-lookup"><span data-stu-id="46127-208"><1200</span></span>|<span data-ttu-id="46127-209">Nummer mindre än 1200</span><span class="sxs-lookup"><span data-stu-id="46127-209">Numbers less than 1200</span></span>|  
  
### <a name="-less-than-or-equal-to"></a><span data-ttu-id="46127-210">(<=) Mindre än eller lika med</span><span class="sxs-lookup"><span data-stu-id="46127-210">(<=) Less than or equal to</span></span>  
  
|<span data-ttu-id="46127-211">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-211">Sample Expression</span></span>|<span data-ttu-id="46127-212">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-212">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-213"><=1200</span><span class="sxs-lookup"><span data-stu-id="46127-213"><=1200</span></span>|<span data-ttu-id="46127-214">Nummer mindre än eller lika med 1200</span><span class="sxs-lookup"><span data-stu-id="46127-214">Numbers less than or equal to 1200</span></span>|  
  
### <a name="-and"></a><span data-ttu-id="46127-215">(&) och</span><span class="sxs-lookup"><span data-stu-id="46127-215">(&) And</span></span>  
  
|<span data-ttu-id="46127-216">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-216">Sample Expression</span></span>|<span data-ttu-id="46127-217">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-217">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-218">>200&<1200</span><span class="sxs-lookup"><span data-stu-id="46127-218">>200&<1200</span></span>|<span data-ttu-id="46127-219">Nummer som är större än 200 och mindre än 1 200.</span><span class="sxs-lookup"><span data-stu-id="46127-219">Numbers greater than 200 and less than 1200</span></span>|  
  
### <a name="-an-exact-character-match"></a><span data-ttu-id="46127-220">('') En exakt teckenmatchning</span><span class="sxs-lookup"><span data-stu-id="46127-220">('') An exact character match</span></span>  
  
|<span data-ttu-id="46127-221">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-221">Sample Expression</span></span>|<span data-ttu-id="46127-222">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-222">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-223">'tillverk'</span><span class="sxs-lookup"><span data-stu-id="46127-223">'man'</span></span>|<span data-ttu-id="46127-224">Text som matchar man exakt och är skiftlägeskänslig.</span><span class="sxs-lookup"><span data-stu-id="46127-224">Text that matches man exactly and is case sensitive.</span></span>|  
  
### <a name="-case-insensitive"></a><span data-ttu-id="46127-225">(@) Okänslig för skiftläge</span><span class="sxs-lookup"><span data-stu-id="46127-225">(@) Case insensitive</span></span>  
  
|<span data-ttu-id="46127-226">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-226">Sample Expression</span></span>|<span data-ttu-id="46127-227">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-227">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-228">@man*</span><span class="sxs-lookup"><span data-stu-id="46127-228">@man*</span></span>|<span data-ttu-id="46127-229">Text som börjar med man och är skiftlägesokänslig.</span><span class="sxs-lookup"><span data-stu-id="46127-229">Text that starts with man and is case insensitive.</span></span>|  
  
### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="46127-230">(*) Ett obestämt antal okända bokstäver</span><span class="sxs-lookup"><span data-stu-id="46127-230">(*) An indefinite number of unknown characters</span></span>  
  
|<span data-ttu-id="46127-231">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-231">Sample Expression</span></span>|<span data-ttu-id="46127-232">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-232">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-233">*Co*</span><span class="sxs-lookup"><span data-stu-id="46127-233">*Co*</span></span>|<span data-ttu-id="46127-234">Text som innehåller ”Co” och är skiftlägeskänsligt.</span><span class="sxs-lookup"><span data-stu-id="46127-234">Text that contains "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="46127-235">*co</span><span class="sxs-lookup"><span data-stu-id="46127-235">*Co</span></span>|<span data-ttu-id="46127-236">Text som slutar med ”Co” och är skiftlägeskänsligt.</span><span class="sxs-lookup"><span data-stu-id="46127-236">Text that ends with "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="46127-237">co*</span><span class="sxs-lookup"><span data-stu-id="46127-237">Co*</span></span>|<span data-ttu-id="46127-238">Text som börjar med ”Co” och är skiftlägeskänsligt.</span><span class="sxs-lookup"><span data-stu-id="46127-238">Text that begins with "Co" and is case sensitive.</span></span>|  
  
### <a name="-one-unknown-character"></a><span data-ttu-id="46127-239">(?) En okänd bokstav</span><span class="sxs-lookup"><span data-stu-id="46127-239">(?) One unknown character</span></span>  
  
|<span data-ttu-id="46127-240">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-240">Sample Expression</span></span>|<span data-ttu-id="46127-241">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-241">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-242">Hans?n</span><span class="sxs-lookup"><span data-stu-id="46127-242">Hans?n</span></span>|<span data-ttu-id="46127-243">Text som exempelvis Hansen eller Hanson</span><span class="sxs-lookup"><span data-stu-id="46127-243">Text such as Hansen or Hanson</span></span>|  
  
### <a name="combined-format-expressions"></a><span data-ttu-id="46127-244">Kombinerade uttryck</span><span class="sxs-lookup"><span data-stu-id="46127-244">Combined format expressions</span></span>  
  
|<span data-ttu-id="46127-245">Exempel</span><span class="sxs-lookup"><span data-stu-id="46127-245">Sample Expression</span></span>|<span data-ttu-id="46127-246">Poster som visas</span><span class="sxs-lookup"><span data-stu-id="46127-246">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="46127-247">5999&#124;8100..8490</span><span class="sxs-lookup"><span data-stu-id="46127-247">5999&#124;8100..8490</span></span>|<span data-ttu-id="46127-248">Ta med post nummer 5999 och poster med nummer fr.o.m. 8100 t.o.m.</span><span class="sxs-lookup"><span data-stu-id="46127-248">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|<span data-ttu-id="46127-249">..1299&#124;1400..</span><span class="sxs-lookup"><span data-stu-id="46127-249">..1299&#124;1400..</span></span>|<span data-ttu-id="46127-250">Ta med poster med nummer mindre än eller lika med 1299 och nummer större än eller lika med 1400 (d.v.s. alla nummer utom 1300 t.o.m.</span><span class="sxs-lookup"><span data-stu-id="46127-250">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|<span data-ttu-id="46127-251">>50&<100</span><span class="sxs-lookup"><span data-stu-id="46127-251">>50&<100</span></span>|<span data-ttu-id="46127-252">Ta med poster med nummer större än 50 och mindre än 100 (d.v.s. nummer fr.o.m. 51 t.o.m.</span><span class="sxs-lookup"><span data-stu-id="46127-252">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  
 
## <a name="see-also"></a><span data-ttu-id="46127-253">Se även</span><span class="sxs-lookup"><span data-stu-id="46127-253">See Also</span></span>
<span data-ttu-id="46127-254">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="46127-254">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

