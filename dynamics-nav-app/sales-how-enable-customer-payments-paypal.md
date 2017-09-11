---
title: "Så här aktiverar du kundutbetalning via PayPal"
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
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a><span data-ttu-id="ce211-102">Så här aktiverar du kundutbetalning via PayPal#</span><span class="sxs-lookup"><span data-stu-id="ce211-102">How to: Enable Customer Payments Through PayPal#</span></span>
<span data-ttu-id="ce211-103">Som alternativ till att samla utbetalningar via banköverföring eller kreditkort, kan du erbjuda dina kunder att betala via sina PayPal-konton.</span><span class="sxs-lookup"><span data-stu-id="ce211-103">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span>

<span data-ttu-id="ce211-104">När kunden väljer PayPal-länken på en försäljningsfaktura eller försäljningsorderdokument visar servicesidan för deras PayPal-konto försäljningens betalningsdetaljer.</span><span class="sxs-lookup"><span data-stu-id="ce211-104">When a customer chooses the PayPal link on a sales invoice or sales order document, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="ce211-105">Då kan kunden betala fakturan som en PayPal-betalning.</span><span class="sxs-lookup"><span data-stu-id="ce211-105">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="ce211-106">För att aktivera kundutbetalningar via PayPal måste du göra följande:</span><span class="sxs-lookup"><span data-stu-id="ce211-106">To enable customer payments through PayPal, you must do the following:</span></span>

1. <span data-ttu-id="ce211-107">Skapa PayPal Payments Standard som betalningsservice i fönstret **Betalningstjänst**.</span><span class="sxs-lookup"><span data-stu-id="ce211-107">Set up PayPal Payments Standard as a payment service in the **Payments Services** window.</span></span>
2. <span data-ttu-id="ce211-108">Välj PayPal Payments Standard i fältet **Betalningstjänst** försäljningsdokumentet i fråga.</span><span class="sxs-lookup"><span data-stu-id="ce211-108">Select PayPal Payments Standard in the **Payment Service** field on the sales document in question.</span></span>

<span data-ttu-id="ce211-109">Tjänsten för PayPal Payments Standard har installerats som ett tillägg till Dynamics NAV och är klar att aktiveras.</span><span class="sxs-lookup"><span data-stu-id="ce211-109">The PayPal Payments Standard service is installed as an extension to Dynamics NAV and ready to enabled.</span></span> <span data-ttu-id="ce211-110">Mer information finns i [Anpassa Dynamics NAV ](ui-extensions.md) med tillägg .</span><span class="sxs-lookup"><span data-stu-id="ce211-110">For more information, see [Customizing Dynamics NAV Using Extensions ](ui-extensions.md).</span></span>

## <a name="to-enable-the-paypal-payments-standard-service"></a><span data-ttu-id="ce211-111">Så här aktiverar du Tjänsten för PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="ce211-111">To enable the PayPal Payments Standard service</span></span>
1. <span data-ttu-id="ce211-112">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningstjänst** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="ce211-112">In the top right corner, choose the **Search for Page or Report** icon, **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ce211-113">I fönstret **Betalningstjänst** väljer du åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="ce211-113">In the **Payment Services** window, choose the **New** action.</span></span>
3. <span data-ttu-id="ce211-114">Markera **PayPal-standard** och stäng sedan fönstret.</span><span class="sxs-lookup"><span data-stu-id="ce211-114">Select **PayPal Standard**, and then close the window.</span></span>
4. <span data-ttu-id="ce211-115">I fönstret **Betalningstjänst** väljer du åtgärden **Konfiguration**.</span><span class="sxs-lookup"><span data-stu-id="ce211-115">In the **Payment Services** window, choose the **Setup** action.</span></span>
5. <span data-ttu-id="ce211-116">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="ce211-116">Fill in the fields as necessary.</span></span> <span data-ttu-id="ce211-117">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="ce211-117">Choose a field to read a short description of the field or link to more information.</span></span>

    <span data-ttu-id="ce211-118">**Obs!** Markera kryssrutan **Inkludera alltid på dokument** om hyperlänken för PayPal-betalningstjänsten alltid ska visas på försäljningsdokument där utbetalning via PayPal är aktiverat.</span><span class="sxs-lookup"><span data-stu-id="ce211-118">**Note**: Select the **Always Include on Documents** check box if the hyperlink for the PayPal payment service should always be visible on sales documents where payment through PayPal is enabled.</span></span>

6. <span data-ttu-id="ce211-119">Stäng fönstret.</span><span class="sxs-lookup"><span data-stu-id="ce211-119">Close the window.</span></span>

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a><span data-ttu-id="ce211-120">Om du vill välja PayPal Payments Standard på en försäljningsfaktura</span><span class="sxs-lookup"><span data-stu-id="ce211-120">To select PayPal Payments Standard on a sales invoice</span></span>
1. <span data-ttu-id="ce211-121">Välj åtgärden **Försäljningsfakturor** på startsidan.</span><span class="sxs-lookup"><span data-stu-id="ce211-121">On the Home page, choose **Sales Invoices**.</span></span>
2. <span data-ttu-id="ce211-122">Öppna försäljningsfakturan som du vill aktivera PayPal-betalningar för.</span><span class="sxs-lookup"><span data-stu-id="ce211-122">Open the sales invoice that you want to enable PayPal payments for.</span></span>
3. <span data-ttu-id="ce211-123">I fältet **Betalningtjänst** väljer du PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="ce211-123">In the **Payment Service** field, choose PayPal Payments Standard.</span></span>

<span data-ttu-id="ce211-124">**Obs!** Fältet **Betalningtjänst** visas endast för om Tjänsten för PayPal Payments Standard är aktiverat.</span><span class="sxs-lookup"><span data-stu-id="ce211-124">**Note**: The **Payment Service** field is only visible if the PayPal Payments Standard service is enabled.</span></span>   

## <a name="see-also"></a><span data-ttu-id="ce211-125">Se även</span><span class="sxs-lookup"><span data-stu-id="ce211-125">See Also</span></span>  
[<span data-ttu-id="ce211-126">Ställa in försäljning</span><span class="sxs-lookup"><span data-stu-id="ce211-126">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="ce211-127">Hantera försäljning</span><span class="sxs-lookup"><span data-stu-id="ce211-127">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="ce211-128">Anpassa Dynamics NAV med hjälp av tillägg</span><span class="sxs-lookup"><span data-stu-id="ce211-128">Customizing Dynamics NAV Using Extensions</span></span>](ui-extensions.md)

