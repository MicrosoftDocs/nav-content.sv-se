---
title: "Så här registrerar du försäljningspriser och rabatter"
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
ms.openlocfilehash: 80a0ac1edc994f44795f7f907a647b269578bc47
ms.contentlocale: sv-se
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-record-sales-prices-and-discounts"></a><span data-ttu-id="49bad-102">Så här registrerar du försäljningspriser och rabatter</span><span class="sxs-lookup"><span data-stu-id="49bad-102">How to: Record Sales Prices and Discounts</span></span>
<span data-ttu-id="49bad-103">De olika pris- och rabattavtalen som gäller när du säljer till olika kunder måste definieras så att de överenskomna reglerna och värdena tillämpas på de försäljningsdokument som du skapar för kunden.</span><span class="sxs-lookup"><span data-stu-id="49bad-103">The different price and discount agreements that apply when selling to different customers must be defined so that the agreed rules and values are applied to sales documents that you create for the customers.</span></span>

<span data-ttu-id="49bad-104">När det gäller priser kan du infoga ett särskilt försäljningspris på försäljningsrader, om en viss kombination av kund, artikel, minsta kvantiteten, måttenhet eller start-/slutdatum finns.</span><span class="sxs-lookup"><span data-stu-id="49bad-104">Concerning prices, you can have a special sales price inserted on sales lines if a certain combination of customer, item, minimum quantity, unit of measure, or starting/ending date exists.</span></span>

<span data-ttu-id="49bad-105">När det gäller rabatter kan du ställa in och använda två olika typer av försäljningsrabatter:</span><span class="sxs-lookup"><span data-stu-id="49bad-105">Concerning discounts, you can set up and use two types of sales discounts:</span></span>

|<span data-ttu-id="49bad-106">Rabattyp</span><span class="sxs-lookup"><span data-stu-id="49bad-106">Discount Type</span></span> |<span data-ttu-id="49bad-107">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="49bad-107">Description</span></span> |
|--------------|------------|
|<span data-ttu-id="49bad-108">**Förs.radrabatt**</span><span class="sxs-lookup"><span data-stu-id="49bad-108">**Sales Line Discount**</span></span>|<span data-ttu-id="49bad-109">En beloppsrabatt som infogas på försäljningsrader, om en viss kombination av kund, artikel, minsta kvantiteten, måttenhet eller start-/slutdatum finns.</span><span class="sxs-lookup"><span data-stu-id="49bad-109">An amount discount that is inserted on sales lines if a certain combination of customer, item, minimum quantity, unit of measure, or starting/ending date exists.</span></span> <span data-ttu-id="49bad-110">En procentrabatt som dras av från dokumentets summa om värdebeloppet för alla rader i ett försäljningsdokument överstiger ett viss minimivärde.</span><span class="sxs-lookup"><span data-stu-id="49bad-110">This works in the same way as for sales prices.</span></span>|
|<span data-ttu-id="49bad-111">**Fakturarabatt**</span><span class="sxs-lookup"><span data-stu-id="49bad-111">**Invoice Discount**</span></span>|<span data-ttu-id="49bad-112">En procentrabatt som dras av från dokumentets summa om värdebeloppet för alla rader i ett inköpsdokument överstiger ett viss minimivärde.</span><span class="sxs-lookup"><span data-stu-id="49bad-112">A percentage discount that is subtracted from the document total if the value amount of all lines on a sales document exceeds a certain minimum.</span></span>|

<span data-ttu-id="49bad-113">Eftersom försäljningsradrabatter och försäljningspriser baseras på en kombination av artikel och kund, kan du också utföra den här konfigurationen från artikelkortet för artikeln när reglerna och värdena gäller.</span><span class="sxs-lookup"><span data-stu-id="49bad-113">Because sales prices and sales line discounts are based on a combination of item and customer, you can also perform this configuration from the item card of the item where the rules and values apply.</span></span>

## <a name="to-set-up-a-sales-price-for-a-customer"></a><span data-ttu-id="49bad-114">Så här skapar du försäljningspriser för en kund:</span><span class="sxs-lookup"><span data-stu-id="49bad-114">To set up a sales price for a customer</span></span>
1. <span data-ttu-id="49bad-115">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Kunder** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="49bad-115">In the top right corner, choose the **Search for Page or Report** icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="49bad-116">Öppna det relevanta kundkortet och välj sedan åtgärden **Priser.**.</span><span class="sxs-lookup"><span data-stu-id="49bad-116">Open the relevant customer card, and then choose the **Prices** action.</span></span>

    <span data-ttu-id="49bad-117">Fältet **Förs.typ** är ifyllt med aktuell **kund** och fältet **Förs.kod** innehåller kundnumret.</span><span class="sxs-lookup"><span data-stu-id="49bad-117">The **Sales Type** field is prefilled with **Customer**, and the **Sales Code** field is prefilled with the customer number.</span></span>
3. <span data-ttu-id="49bad-118">Fyll i fälten på den första raden.</span><span class="sxs-lookup"><span data-stu-id="49bad-118">Fill in the fields on the line as necessary.</span></span> <span data-ttu-id="49bad-119">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="49bad-119">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="49bad-120">Fyll i en rad för varje kombination som ska bevilja ett speciellt försäljningspris till kunden.</span><span class="sxs-lookup"><span data-stu-id="49bad-120">Fill a line for each combination that will grant a special sales price to the customer.</span></span>

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a><span data-ttu-id="49bad-121">Så här skapar du försäljningsradrabatter för en kund</span><span class="sxs-lookup"><span data-stu-id="49bad-121">To set up a sales line discount for a customer</span></span>
1. <span data-ttu-id="49bad-122">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Kunder** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="49bad-122">In the top right corner, choose the **Search for Page or Report** icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="49bad-123">Öppna det relevanta kundkortet och välj sedan åtgärden **Radrabatter.**.</span><span class="sxs-lookup"><span data-stu-id="49bad-123">Open the relevant customer card, and then choose the **Line Discounts** action.</span></span>

    <span data-ttu-id="49bad-124">Fältet **Förs.typ** är ifyllt med aktuell **kund** och fältet **Förs.kod** innehåller kundnumret.</span><span class="sxs-lookup"><span data-stu-id="49bad-124">The **Sales Type** field is prefilled with **Customer**, and the **Sales Code** field is prefilled with the customer number.</span></span>
3.  <span data-ttu-id="49bad-125">Fyll i fälten på den första raden.</span><span class="sxs-lookup"><span data-stu-id="49bad-125">Fill in the fields on the line as necessary.</span></span> <span data-ttu-id="49bad-126">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="49bad-126">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="49bad-127">Fyll i en rad för varje kombination som ska bevilja en speciell försäljningsradrabatt till kunden.</span><span class="sxs-lookup"><span data-stu-id="49bad-127">Fill a line for each combination that will grant a sales line discount to the customer.</span></span>

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a><span data-ttu-id="49bad-128">Så här definierar du radrabatt för en kund</span><span class="sxs-lookup"><span data-stu-id="49bad-128">To set up an invoice discount for a customer</span></span>
<span data-ttu-id="49bad-129">När du har bestämt vilka kunder som är aktuella för fakturarabatter, skriver du fakturarabattkoderna på kundkorten och lägger upp villkoren för respektive kod.</span><span class="sxs-lookup"><span data-stu-id="49bad-129">When you have decided which customers are eligible for invoice discounts, enter the invoice discount code on the customer cards and set up the terms for each code.</span></span>

1. <span data-ttu-id="49bad-130">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Kunder** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="49bad-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="49bad-131">Öppna kundkortet för en kund som är aktuell för fakturarabatter.</span><span class="sxs-lookup"><span data-stu-id="49bad-131">Open the customer card for a customer that will be eligible for invoice discounts.</span></span>
3. <span data-ttu-id="49bad-132">Välj i fältet  **Fakturarabattkod** koden för den fakturarabatt som ska användas vid beräkning av fakturarabatter för kunden.</span><span class="sxs-lookup"><span data-stu-id="49bad-132">In the **Invoice Disc. Code** field, select a code for the relevant invoice discount terms to use to calculate invoice discounts for the customer.</span></span>

    <span data-ttu-id="49bad-133">**Obs!** Fakturarabattkoder representeras av befintliga kundkort.</span><span class="sxs-lookup"><span data-stu-id="49bad-133">**Note**: Invoice discount codes are represented by existing customer cards.</span></span> <span data-ttu-id="49bad-134">Detta aktiverar dig att snabbt tilldela fakturarabattvillkor till kunder, genom att välja namnet på en andra kunder som ska ha dessa villkor.</span><span class="sxs-lookup"><span data-stu-id="49bad-134">This enables you to quickly assign invoice discount terms to customers by picking the name of another customer who will have the same terms.</span></span>

    <span data-ttu-id="49bad-135">Så här definierar du fakturarabattvillkor för försäljning:</span><span class="sxs-lookup"><span data-stu-id="49bad-135">Proceed to set up new the sales invoice discount terms.</span></span>
4. <span data-ttu-id="49bad-136">I fönstret **Kundkort** väljer du åtgärden **Fakturarabatter**.</span><span class="sxs-lookup"><span data-stu-id="49bad-136">In the **Customer Card** window, choose the **Invoice Discounts** action.</span></span> <span data-ttu-id="49bad-137">Fönstret **Kundfakturarabatter** öppnas.</span><span class="sxs-lookup"><span data-stu-id="49bad-137">The **Cust. Invoice Discounts** window opens.</span></span>
5. <span data-ttu-id="49bad-138">Ange valutakoden som du vill definiera fakturarabattvillkor för i fältet **Valutakod**.</span><span class="sxs-lookup"><span data-stu-id="49bad-138">In the **Currency Code** field, enter the code for a currency that the invoice discount terms on the line applies to.</span></span> <span data-ttu-id="49bad-139">Lämna det här fältet tomt om du vill ange fakturarabattvillkor i USD.</span><span class="sxs-lookup"><span data-stu-id="49bad-139">Leave the field blank to set up invoice discount terms in USD.</span></span>
6. <span data-ttu-id="49bad-140">Ange i fältet **Minimibelopp** det minsta belopp som en faktura måste vara på för att komma i fråga för rabatt.</span><span class="sxs-lookup"><span data-stu-id="49bad-140">In the **Minimum Amount** field, enter the minimum amount that an invoice must have to be eligible for the discount.</span></span>
7. <span data-ttu-id="49bad-141">Fakturarabatten beräknas som en procentandel av fakturabeloppet i fältet **Rabatt %**.</span><span class="sxs-lookup"><span data-stu-id="49bad-141">In the **Discount %** field, enter the invoice discount as a percentage of the invoice amount.</span></span>
8. <span data-ttu-id="49bad-142">Upprepa steg 5 till och med 7 för varje valuta som kunden ska ta emot en annan fakturarabatt för.</span><span class="sxs-lookup"><span data-stu-id="49bad-142">Repeat steps 5 through 7 for each currency that the customer will receive a different invoice discount for.</span></span>

<span data-ttu-id="49bad-143">Fakturarabatten ställs nu in i fältet och fördelas till kunden i fråga.</span><span class="sxs-lookup"><span data-stu-id="49bad-143">The invoice discount is now set up and assigned to the customer in question.</span></span> <span data-ttu-id="49bad-144">När du väljer kundkoden i fältet **Fakturarabattkod** på andra kundkort, kopplas samma fakturarabatt till dessa kunder.</span><span class="sxs-lookup"><span data-stu-id="49bad-144">When you select the customer code in the **Invoice Disc. Code** field on other customer cards, the same invoice discount is assigned to those customers.</span></span>

## <a name="see-also"></a><span data-ttu-id="49bad-145">Se även</span><span class="sxs-lookup"><span data-stu-id="49bad-145">See Also</span></span>  
[<span data-ttu-id="49bad-146">Ställa in försäljning</span><span class="sxs-lookup"><span data-stu-id="49bad-146">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="49bad-147">Hantera försäljning</span><span class="sxs-lookup"><span data-stu-id="49bad-147">Manage Sales</span></span>](sales-manage-sales.md)

