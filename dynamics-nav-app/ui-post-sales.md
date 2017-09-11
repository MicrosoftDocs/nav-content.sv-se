---
title: "Bokföra försäljning"
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
ms.openlocfilehash: e87dd5faf7713aecfbe7209d00bb8076fcae9d25
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="posting-sales"></a><span data-ttu-id="76cca-102">Bokföra försäljning</span><span class="sxs-lookup"><span data-stu-id="76cca-102">Posting Sales</span></span>
<span data-ttu-id="76cca-103">I **Bokföringsgrupp** i ett försäljningsdokument kan du välja mellan följande bokföringsfunktioner:</span><span class="sxs-lookup"><span data-stu-id="76cca-103">In the **Posting group** on a sales document, you can choose between the following posting functions:</span></span>

- <span data-ttu-id="76cca-104">**Bokföra**</span><span class="sxs-lookup"><span data-stu-id="76cca-104">**Post**</span></span>
- <span data-ttu-id="76cca-105">**Testa rapport**</span><span class="sxs-lookup"><span data-stu-id="76cca-105">**Test Report**</span></span>
- <span data-ttu-id="76cca-106">**Bokför och skicka**</span><span class="sxs-lookup"><span data-stu-id="76cca-106">**Post and Send**</span></span>
- <span data-ttu-id="76cca-107">**Bokför och skriv ut**</span><span class="sxs-lookup"><span data-stu-id="76cca-107">**Post and Print**</span></span>
- <span data-ttu-id="76cca-108">**Bokför och e-posta**</span><span class="sxs-lookup"><span data-stu-id="76cca-108">**Post and Email**</span></span>
- <span data-ttu-id="76cca-109">**Bokför batch-jobb**</span><span class="sxs-lookup"><span data-stu-id="76cca-109">**Post Batch**</span></span>
- <span data-ttu-id="76cca-110">**Förhandsgranska bokföring**</span><span class="sxs-lookup"><span data-stu-id="76cca-110">**Preview Posting**</span></span>

<span data-ttu-id="76cca-111">När du har fyllt i alla raderna och skrivit in all information på försäljningsordern kan du bokföra den.</span><span class="sxs-lookup"><span data-stu-id="76cca-111">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="76cca-112">Här skapas en leverans och en faktura.</span><span class="sxs-lookup"><span data-stu-id="76cca-112">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="76cca-113">När en försäljningsorder bokförs, uppdateras kundens konto, redovisningen och artikeltransaktionerna.</span><span class="sxs-lookup"><span data-stu-id="76cca-113">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="76cca-114">För varje försäljningsorder skapas en försäljningstransaktion i tabellen **Redovisningstransaktion**.</span><span class="sxs-lookup"><span data-stu-id="76cca-114">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="76cca-115">Dessutom skapas en transaktion på kundens konto i tabellen **Kundreskontra** och en redovisningstransaktion på det relevanta kontot för leverantörsreskontra.</span><span class="sxs-lookup"><span data-stu-id="76cca-115">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="76cca-116">Dessutom kan bokföring av inköpsordern resultera i en momstransaktion och en redovisningstransaktion för rabattbeloppet.</span><span class="sxs-lookup"><span data-stu-id="76cca-116">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="76cca-117">Huruvida rabattransaktionen bokförs eller inte beror på innehållet i fältet **Rabattbokföring** i fönstret **Försäljningsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="76cca-117">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Sales & Receivables Setup** window.</span></span>

<span data-ttu-id="76cca-118">För varje orderrad skapas en artikeltransaktion i tabellen **Artikeltransaktion** (om försäljningsraden innehåller artikelnummer) eller en redovisningstransaktion i tabellen **Redovisningstransaktion** (om försäljningsraden innehåller ett redovisningskonto).</span><span class="sxs-lookup"><span data-stu-id="76cca-118">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="76cca-119">Därutöver registreras order alltid i tabellerna **Utleveranshuvud** och **Försäljningsfakturahuvud**.</span><span class="sxs-lookup"><span data-stu-id="76cca-119">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

<span data-ttu-id="76cca-120">**Viktigt!** När du bokför en order kan du skapa både en utleverans och en faktura.</span><span class="sxs-lookup"><span data-stu-id="76cca-120">**Important**: When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="76cca-121">Detta kan göras samtidigt eller oberoende av varandra.</span><span class="sxs-lookup"><span data-stu-id="76cca-121">These can be done at the same time or independently.</span></span> <span data-ttu-id="76cca-122">Du kan också skapa en delutleverans och en delfaktura genom att fylla i fältet **Ant. att utleverera** och **Ant. att fakturera** på de enskilda försäljningsorderraderna innan du bokför.</span><span class="sxs-lookup"><span data-stu-id="76cca-122">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="76cca-123">Observera att du inte kan skapa en faktura för något som inte har utlevererats.</span><span class="sxs-lookup"><span data-stu-id="76cca-123">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="76cca-124">D.v.s. innan du kan fakturera måste du ha registrerat en leverans alternativt välja att leverera och fakturera samtidigt.</span><span class="sxs-lookup"><span data-stu-id="76cca-124">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span> 

<span data-ttu-id="76cca-125">När bokföringen är slutförd tas de bokförda försäljningsraderna bort från ordern.</span><span class="sxs-lookup"><span data-stu-id="76cca-125">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="76cca-126">Du får ett meddelande när bokföringen är slutförd.</span><span class="sxs-lookup"><span data-stu-id="76cca-126">A message tells you when the posting is completed.</span></span> <span data-ttu-id="76cca-127">Sedan kan du se de bokförda transaktionerna i de olika fönstren som innehåller bokförda transaktioner, t.ex. fönsterna **Leverantörsreskontratransaktion**, **Redovisningstransaktion**, **Artikeltransaktion**, **Bokförda försäljningsutleveranser** och **Bokförda försäljningsfakturor**.</span><span class="sxs-lookup"><span data-stu-id="76cca-127">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** windows.</span></span>

## <a name="see-also"></a><span data-ttu-id="76cca-128">Se även</span><span class="sxs-lookup"><span data-stu-id="76cca-128">See Also</span></span>
[<span data-ttu-id="76cca-129">Så här skickar du dokument som e-post</span><span class="sxs-lookup"><span data-stu-id="76cca-129">How to: Send Documents by Email</span></span>](ui-how-send-documents-email.md)

