---
title: "Bokföra inköp"
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
ms.openlocfilehash: 646ea47adfe2f949e0fdf950607e7d246dcb9f59
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="posting-purchases"></a><span data-ttu-id="0e1e4-102">Bokföra inköp</span><span class="sxs-lookup"><span data-stu-id="0e1e4-102">Posting Purchases</span></span>
<span data-ttu-id="0e1e4-103">I **Bokföringsgrupp** i ett inköpsdokument kan du välja mellan följande bokföringsfunktioner:</span><span class="sxs-lookup"><span data-stu-id="0e1e4-103">In the **Posting group** on a purchase document, you can choose between the following posting functions:</span></span>

- <span data-ttu-id="0e1e4-104">**Bokföra**</span><span class="sxs-lookup"><span data-stu-id="0e1e4-104">**Post**</span></span>
- <span data-ttu-id="0e1e4-105">**Förhandsgranska bokföring**</span><span class="sxs-lookup"><span data-stu-id="0e1e4-105">**Preview Posting**</span></span>
- <span data-ttu-id="0e1e4-106">**Bokför och skriv ut**</span><span class="sxs-lookup"><span data-stu-id="0e1e4-106">**Post and Print**</span></span>
- <span data-ttu-id="0e1e4-107">**Testa rapport**</span><span class="sxs-lookup"><span data-stu-id="0e1e4-107">**Test Report**</span></span>
- <span data-ttu-id="0e1e4-108">**Bokför batch-jobb**</span><span class="sxs-lookup"><span data-stu-id="0e1e4-108">**Post Batch**</span></span>

<span data-ttu-id="0e1e4-109">När du har fyllt i alla raderna och skrivit in all information på inköpsordern kan du bokföra den, d.v.s. skapa en inleverans och en faktura.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-109">When you have completed all the lines and entered all the information on the purchase order, you can post it, that is, create a receipt and an invoice.</span></span>

<span data-ttu-id="0e1e4-110">När en inköpsorder bokförs, uppdateras leverantörens konto, redovisningen och artikeltransaktionerna.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-110">When a purchase order is posted, the vendor's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="0e1e4-111">För varje inköpsorder skapas en inköpstransaktion i tabellen **Redovisningstransaktion**.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-111">For each purchase order, a purchase entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="0e1e4-112">Dessutom skapas en transaktion på leverantörens konto i tabellen **Lev.reskontratransaktion** och en redovisningstransaktion på det relevanta kontot för leverantörsskulder.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-112">An entry is also created in the vendor's account in the **Vendor Ledger Entry** table and a G/L entry is created in the relevant payables account.</span></span> <span data-ttu-id="0e1e4-113">Dessutom kan bokföring av inköpsordern resultera i en momstransaktion och en redovisningstransaktion för rabattbeloppet.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-113">In addition, posting the order may result in a VAT entry and a G/L entry for the discount amount.</span></span> <span data-ttu-id="0e1e4-114">Om rabattransaktionen är bokförd eller ej beror på innehållet i fältet **Rabattbokföring** i fönstret **Inköpsinställning**.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-114">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Purchases & Payables Setup** window.</span></span>

<span data-ttu-id="0e1e4-115">För varje inköpsorderrad skapas en artikeltransaktion i tabellen **Artikeltransaktion** (om inköpsraden innehåller artikelnummer) eller en redovisningstransaktion i tabellen **Redovisningstransaktion** (om inköpsraden innehåller ett redovisningskonto).</span><span class="sxs-lookup"><span data-stu-id="0e1e4-115">For each purchase order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the purchase lines contain item numbers) or a G/L entry will be created in the **G/L Entry** table (if the purchase lines contain a G/L account).</span></span> <span data-ttu-id="0e1e4-116">Dessutom registreras inköpsorder alltid i tabellerna **Inleveranshuvud** och **Inköpsfakturahuvud**.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-116">In addition, purchase orders are always recorded in the **Purch. Recpt. Header** and **Purch. Inv. Header** tables.</span></span>

<span data-ttu-id="0e1e4-117">Innan du börjar bokföra kan du välja att skriva ut en testrapport som visar all information på inköpsordern tillsammans med eventuella fel.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-117">Before you start to post, you can print a test report that contains all the information in the purchase order and indicates any errors there.</span></span> <span data-ttu-id="0e1e4-118">Om du vill skriva ut rapporten väljer du **Bokföring** och sedan **Testrapport**.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-118">To print the report, choose **Posting**, and then choose **Test Report**.</span></span>

<span data-ttu-id="0e1e4-119">**Viktigt!** När du bokför en order kan du skapa både en inleverans och en faktura.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-119">**Important**: When you post an order, you can create both a receipt and an invoice.</span></span> <span data-ttu-id="0e1e4-120">Detta kan göras samtidigt eller oberoende av varandra.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-120">These can be done simultaneously or independently.</span></span> <span data-ttu-id="0e1e4-121">Du kan också skapa en delinleverans och en delfaktura genom att fylla i fältet **Ant. att inlevereras** och **Ant. att fakturera** på de enskilda inköpsorderraderna innan du bokför.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-121">You can also create a partial receipt and a partial invoice by completing the **Qty. to Receive** and **Qty. to Invoice** fields on the individual purchase order lines before you post.</span></span> <span data-ttu-id="0e1e4-122">Observera att du inte kan skapa en faktura för något som inte har inlevererats.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-122">Note that you cannot create an invoice for something that has not been received.</span></span> <span data-ttu-id="0e1e4-123">Innan du kan fakturera måste du således ha registrerat en inleverans alternativt välja att inleverera och fakturera samtidigt.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-123">That is, before you can invoice, you must have recorded a receipt, or you must choose to receive and invoice at the same time.</span></span>

<span data-ttu-id="0e1e4-124">Du kan bokföra eller bokföra och skriva ut.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-124">You can either post, or post and print.</span></span> <span data-ttu-id="0e1e4-125">Om du väljer Bokför och Skriv ut, skrivs en rapport ut när ordern bokförs.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-125">If you choose to post and print, a report is printed when the order is posted.</span></span> <span data-ttu-id="0e1e4-126">Du kan även välja funktionen **Bokför batch-jobb** som ger dig möjlighet att bokföra fler fakturor samtidigt.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-126">You can also choose the **Post Batch** function, which lets you post several orders at the same time.</span></span>

<span data-ttu-id="0e1e4-127">När bokföringen är slutförd tas de bokförda inköpsraderna bort från ordern.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-127">When the posting is completed, the posted purchase lines are removed from the order.</span></span> <span data-ttu-id="0e1e4-128">Du får ett meddelande när bokföringen är slutförd.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-128">A message tells you when the posting is completed.</span></span> <span data-ttu-id="0e1e4-129">Sedan kan du se de bokförda transaktionerna i de olika fönster som innehåller bokförda transaktioner, t.ex. fönsterna **Leverantörsreskontratransaktion**, **Redovisningstransaktion**, **Artikeltransaktioner**, **Inleverans** och **Bokförda inköpsfakturor**.</span><span class="sxs-lookup"><span data-stu-id="0e1e4-129">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Vendor Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Purchase Receipts**, and **Posted Purchase Invoices** windows.</span></span>

## <a name="see-also"></a><span data-ttu-id="0e1e4-130">Se även</span><span class="sxs-lookup"><span data-stu-id="0e1e4-130">See Also</span></span>
[<span data-ttu-id="0e1e4-131">Bokför dokument och journaler</span><span class="sxs-lookup"><span data-stu-id="0e1e4-131">Post Documents and Journals</span></span>](ui-post-documents-journals.md)

