---
title: "Så här registrerar du nya produkter"
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
ms.openlocfilehash: df84a4d3e15035cd956c7612a12069844f5601d2
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-products"></a><span data-ttu-id="ec02d-102">Så här registrerar du nya produkter</span><span class="sxs-lookup"><span data-stu-id="ec02d-102">How to: Register New Products</span></span>

<span data-ttu-id="ec02d-103">Produkter utgör basen för ditt arbete, varorna eller tjänster som du handlar med.</span><span class="sxs-lookup"><span data-stu-id="ec02d-103">Products are the basis of your business, the goods or services that you trade in.</span></span> <span data-ttu-id="ec02d-104">Varje produkt måste registreras som ett artikelkort.</span><span class="sxs-lookup"><span data-stu-id="ec02d-104">Each product must be registered as an item card.</span></span>

<span data-ttu-id="ec02d-105">**Obs!** I Dynamics NAV  refereras en produkt till termen “item”.</span><span class="sxs-lookup"><span data-stu-id="ec02d-105">**Note**: In Dynamics NAV, a product is referred to using the term “item”.</span></span>

<span data-ttu-id="ec02d-106">Artikelkort innehåller den information som behövs för att köpa, lagra, sälja, leverera och informera om produkter.</span><span class="sxs-lookup"><span data-stu-id="ec02d-106">Item cards hold the information that is required to buy, store, sell, deliver, and account for products.</span></span>

<span data-ttu-id="ec02d-107">Artikelkortet kan vara av typen Lager eller Service för att ange om produkten är en fysisk enhet eller en arbetstidsenhet.</span><span class="sxs-lookup"><span data-stu-id="ec02d-107">The item card can be of type Inventory or Service to specify if the product is a physical unit or labor time unit.</span></span> <span data-ttu-id="ec02d-108">Förutom vissa fält som är knutna till de fysiska aspekterna av en artikel, fungerar alla fält på ett artikelkort på samma sätt för lagerartiklar och tjänster.</span><span class="sxs-lookup"><span data-stu-id="ec02d-108">Apart from some fields that relate to the physical aspects of an item, all fields on an item card function in the same way for inventory items and services.</span></span> <span data-ttu-id="ec02d-109">Mer information om att sälja en artikel finns i [Så här säljer du produkter](sales-how-sell-products.md) eller [Så här fakturerar du försäljning](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="ec02d-109">For more information about selling an item, see [How to: Sell Products](sales-how-sell-products.md) or [How to: Invoice Sales](sales-how-invoice-sales.md).</span></span>

<span data-ttu-id="ec02d-110">**Obs!** Om artikelmallar finns för olika artikeltyper, visas ett fönster när du skapar ett nytt artikelkort där du kan välja en lämplig mall.</span><span class="sxs-lookup"><span data-stu-id="ec02d-110">**Note**: If item templates exist for different item types, then a window appears when you create a new item card from where you can select an appropriate template.</span></span> <span data-ttu-id="ec02d-111">Om endast en artikelmall finns, då använder nya artikelkort alltid den mallen.</span><span class="sxs-lookup"><span data-stu-id="ec02d-111">If only one item template exists, then new item cards always use that template.</span></span>

## <a name="to-create-a-new-item-card"></a><span data-ttu-id="ec02d-112">Skapa ett nytt artikelkort</span><span class="sxs-lookup"><span data-stu-id="ec02d-112">To create a new item card</span></span>
1. <span data-ttu-id="ec02d-113">På startsidan väljer du åtgärden **Artiklar** för att öppna listan över befintliga artiklar.</span><span class="sxs-lookup"><span data-stu-id="ec02d-113">On the Home page, choose the **Items** action to open the list of existing items.</span></span>  
2. <span data-ttu-id="ec02d-114">I fönstret **Artiklar** väljer du åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="ec02d-114">In the **Items** window, choose the **New** action.</span></span>

    <span data-ttu-id="ec02d-115">Om endast en artikelmall finns, då öppnas ett nytt artikelkort med fält ifyllda med information från mallen.</span><span class="sxs-lookup"><span data-stu-id="ec02d-115">If only one item template exists, then a new item card opens with some fields filled with information from the template.</span></span>
3. <span data-ttu-id="ec02d-116">Välj den mall som du vill använda för den nya artikelkortet i fönstret **Välj en mall för en ny artikel**.</span><span class="sxs-lookup"><span data-stu-id="ec02d-116">In the **Select a template for a new item** window, choose the template that you want to use for the new item card.</span></span>
4. <span data-ttu-id="ec02d-117">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="ec02d-117">Choose the **OK** button.</span></span> <span data-ttu-id="ec02d-118">Ett nytt artikelkort öppnas med ifyllda fält med information från mallen.</span><span class="sxs-lookup"><span data-stu-id="ec02d-118">A new item card opens with some fields filled with information from the template.</span></span>
5. <span data-ttu-id="ec02d-119">Fortsätt att fylla i eller ändra fält på artikelkortet vid behov.</span><span class="sxs-lookup"><span data-stu-id="ec02d-119">Proceed to fill or change fields on the item card as necessary.</span></span> <span data-ttu-id="ec02d-120">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="ec02d-120">Choose a field to read a short description of the field or link to more information.</span></span>

<span data-ttu-id="ec02d-121">På snabbfliken **Försäljningspriser** ser du specialpriser eller rabatter som du beviljar för artikeln om vissa kriterier uppfylls, till exempel kund, lägsta partistorlek eller slutdatum</span><span class="sxs-lookup"><span data-stu-id="ec02d-121">On the **Sales Prices** FastTab, you can view special prices or discounts that you grant for the item if certain criteria are met, such as customer, minimum order quantity, or ending date.</span></span> <span data-ttu-id="ec02d-122">Varje rad representerar ett speciellt pris eller radrabatt.</span><span class="sxs-lookup"><span data-stu-id="ec02d-122">Each row represents a special price or line discount.</span></span> <span data-ttu-id="ec02d-123">Varje kolumn representerar ett kriterium som måste gälla för att garantera specialpriset som du anger i fältet **Enhetspris** eller radrabatten som du anger i fältet **Radrabatt %**.</span><span class="sxs-lookup"><span data-stu-id="ec02d-123">Each column represents a criterion that must apply to warrant the special price that you enter in the **Unit Price** field, or the line discount that you enter in the **Line Discount %** field.</span></span> <span data-ttu-id="ec02d-124">Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="ec02d-124">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>

<span data-ttu-id="ec02d-125">Artikeln är nu registrerad, och artikelkortet är klart att användas i försäljningsdokument.</span><span class="sxs-lookup"><span data-stu-id="ec02d-125">The item is now registered, and the item card is ready to be used on purchase and sales documents.</span></span>

<span data-ttu-id="ec02d-126">Om du vill använda detta artikelkort som en mall när du skapar nya artikelkort, så fortsätt med att spara den som en mall.</span><span class="sxs-lookup"><span data-stu-id="ec02d-126">If you want to use this item card as a template when you create new item cards, you can save it as a template.</span></span> <span data-ttu-id="ec02d-127">Mer information finns i följande avsnitt:</span><span class="sxs-lookup"><span data-stu-id="ec02d-127">For more information, see the following section.</span></span>

## <a name="to-save-the-item-card-as-a-template"></a><span data-ttu-id="ec02d-128">Om du vill spara artikelkortet som en mall</span><span class="sxs-lookup"><span data-stu-id="ec02d-128">To save the item card as a template</span></span>
1. <span data-ttu-id="ec02d-129">I fönstret **artikelkort** väljer du åtgärden **Spara som mall**.</span><span class="sxs-lookup"><span data-stu-id="ec02d-129">In the **Item Card** window, choose the **Save as Template** action.</span></span> <span data-ttu-id="ec02d-130">Det **artikelmall** fönstret öppnas uppvisar artikelkortet som mall.</span><span class="sxs-lookup"><span data-stu-id="ec02d-130">The **Item Template** window opens showing the item card as a template.</span></span>
2. <span data-ttu-id="ec02d-131">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="ec02d-131">Fill in the fields as necessary.</span></span> <span data-ttu-id="ec02d-132">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="ec02d-132">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="ec02d-133">Om du vill återanvända dimensioner i mallar väljer du fönstret **Dimensioner**.</span><span class="sxs-lookup"><span data-stu-id="ec02d-133">To reuse dimensions in templates, choose the **Dimensions** action.</span></span> <span data-ttu-id="ec02d-134">Fönstret **Dimensionsmallar** öppnas och visar de dimensionskoder som ställts in för artikeln.</span><span class="sxs-lookup"><span data-stu-id="ec02d-134">The **Dimension Templates** window opens showing any dimension codes that are set up for the item.</span></span>
4. <span data-ttu-id="ec02d-135">Ändra eller ange dimensionskoder som ska kopplas till nya artikelkort som skapas med hjälp av mallen.</span><span class="sxs-lookup"><span data-stu-id="ec02d-135">Edit or enter dimension codes that will apply to new item cards created by using the template.</span></span>
5. <span data-ttu-id="ec02d-136">Välj **OK** när du har slutfört den nya artikelmallen.</span><span class="sxs-lookup"><span data-stu-id="ec02d-136">When you have completed the new item template, choose the **OK** button.</span></span>

<span data-ttu-id="ec02d-137">Artikelmallen läggs till listan över artikelmallar, så att du kan använda det för att skapa nya artikelkort.</span><span class="sxs-lookup"><span data-stu-id="ec02d-137">The item template is added to the list of item templates, so that you can use it to create new item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="ec02d-138">Se även</span><span class="sxs-lookup"><span data-stu-id="ec02d-138">See Also</span></span>
  [<span data-ttu-id="ec02d-139">Hantera lager</span><span class="sxs-lookup"><span data-stu-id="ec02d-139">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="ec02d-140">  [Hantera inköp](purchasing-manage-purchasing.md)</span><span class="sxs-lookup"><span data-stu-id="ec02d-140">  [Manage Purchasing](purchasing-manage-purchasing.md)</span></span>  
<span data-ttu-id="ec02d-141">  [Hantera försäljning](sales-manage-sales.md)</span><span class="sxs-lookup"><span data-stu-id="ec02d-141">  [Manage Sales](sales-manage-sales.md)</span></span>

