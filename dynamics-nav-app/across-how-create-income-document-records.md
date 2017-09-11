---
title: "Så här skapar du inkommande dokumentposter"
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
ms.openlocfilehash: e91c4570ff60d991974ac6afd16ba3bc3e73e44f
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-create-incoming-document-records"></a><span data-ttu-id="be7a3-102">Så här skapar du inkommande dokumentposter</span><span class="sxs-lookup"><span data-stu-id="be7a3-102">How to: Create Incoming Document Records</span></span>
<span data-ttu-id="be7a3-103">I fönstret **Inkommande dokument** använder du olika funktioner för att förhandsgranska utgiftskvitton, hantera OCR-uppgifter och konvertera inkommande dokumentfiler, manuellt eller automatiskt, till relevanta dokument eller journalrader i .</span><span class="sxs-lookup"><span data-stu-id="be7a3-103">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="be7a3-104">De externa filerna kan kopplas till något processteg, inklusive till bokförda dokument och till resulterande leverantörs-, kund- och redovisningstransaktioner.</span><span class="sxs-lookup"><span data-stu-id="be7a3-104">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="be7a3-105">Om du vill registrera ett externt dokument i | Dynamics NAV måste du först skapa eller slutföra en inkommande dokumentpost.</span><span class="sxs-lookup"><span data-stu-id="be7a3-105">To record an external document in Dynamics NAV, you must first create or complete an incoming document record.</span></span> <span data-ttu-id="be7a3-106">Du kan göra detta manuellt eller så kan du ta ett foto på det externa dokumentet och sedan skapa en inkommande dokumentpost med bildfilen bifogad.</span><span class="sxs-lookup"><span data-stu-id="be7a3-106">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="be7a3-107">Innan du kan använda funktionen för inkommande dokument måste du utföra de nödvändiga inställningarna.</span><span class="sxs-lookup"><span data-stu-id="be7a3-107">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="be7a3-108">Mer information finns i [Så här skapar du inkommande dokument](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="be7a3-108">For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="be7a3-109">Så här Godkänn eller avvisa ett inkommande dokument.</span><span class="sxs-lookup"><span data-stu-id="be7a3-109">To approve or reject an incoming document</span></span>
<span data-ttu-id="be7a3-110">Om du inte vill att användare ska skapa fakturor eller redovisningsjournalrader från inkommande dokumentposter om inte dokumenten har godkänts först kan du konfigurera godkännare som måste godkänna transaktionerna innan de kan behandlas.</span><span class="sxs-lookup"><span data-stu-id="be7a3-110">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="be7a3-111">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inkommande dokument** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="be7a3-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="be7a3-112">Markera raden med dokumentet som du vill godkänna eller avvisa, och välj sedan åtgärden **godkänna** eller **avvisa**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-112">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="be7a3-113">Om du godkänner den inkommande dokumentposten markeras kryssrutan **Släppt** på den inkommande dokumentraden.</span><span class="sxs-lookup"><span data-stu-id="be7a3-113">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="be7a3-114">Användaren som ansvarar för att skapa t.ex inköpsfakturor kan fortsätta med att bearbeta transaktionen.</span><span class="sxs-lookup"><span data-stu-id="be7a3-114">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="be7a3-115">Så här skapar du en inkommande dokumentpost genom att ta ett foto</span><span class="sxs-lookup"><span data-stu-id="be7a3-115">To create an incoming document record by taking a photo</span></span>
<span data-ttu-id="be7a3-116">**Obs!**: Följande proceduren gäller endast Dynamics NAV för surfplatte- och telefonklienter.</span><span class="sxs-lookup"><span data-stu-id="be7a3-116">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="be7a3-117">Välj panelen **Skapa inkommande dokument från kamera** i appfältet och gå sedan till steg 4.</span><span class="sxs-lookup"><span data-stu-id="be7a3-117">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="be7a3-118">Välj annars alternativknappen på appfältet, välj **Inkommande dokument** och välj sedan **Alla**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-118">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="be7a3-119">I fönstret **Inkommande dokument** väljer du ellipsknappen och sedan **Skapa från kamera**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-119">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="be7a3-120">Kameran på Tablet PC:n eller telefonen aktiveras.</span><span class="sxs-lookup"><span data-stu-id="be7a3-120">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="be7a3-121">Ta ett foto av ett dokument, t.ex. ett inköpskvitto, som du vill bearbeta som ett inkommande dokument, och välj sedan knappen **OK** .</span><span class="sxs-lookup"><span data-stu-id="be7a3-121">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="be7a3-122">En ny inkommande dokumentpost skapas med bilden bifogad.</span><span class="sxs-lookup"><span data-stu-id="be7a3-122">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="be7a3-123">Så här bifogar du en bild till en inkommande dokumentpost genom att ta ett foto</span><span class="sxs-lookup"><span data-stu-id="be7a3-123">To attach an image to an incoming document record by taking a photo</span></span>
<span data-ttu-id="be7a3-124">**Obs!**: Följande proceduren gäller endast Dynamics NAV för surfplatte- och telefonklienter.</span><span class="sxs-lookup"><span data-stu-id="be7a3-124">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="be7a3-125">Välj alternativknappen på appfältet, välj **Inkommande dokument** och välj sedan **Alla**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-125">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="be7a3-126">Öppna kortet för en befintlig inkommande dokumentpost.</span><span class="sxs-lookup"><span data-stu-id="be7a3-126">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="be7a3-127">I fönstret **Inkommande dokument** väljer du ellipsknappen och sedan **Bifoga fil från kamera**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-127">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="be7a3-128">Kameran på Tablet PC:n eller telefonen aktiveras.</span><span class="sxs-lookup"><span data-stu-id="be7a3-128">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="be7a3-129">Ta ett foto av ett dokument, t.ex. ett inköpskvitto, som du vill bearbeta som ett inkommande dokument, och välj sedan knappen **OK** .</span><span class="sxs-lookup"><span data-stu-id="be7a3-129">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="be7a3-130">Bilden har bifogats till den inkommande dokumentposten.</span><span class="sxs-lookup"><span data-stu-id="be7a3-130">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="be7a3-131">Så här skapar du en inkommande dokumentpost manuellt</span><span class="sxs-lookup"><span data-stu-id="be7a3-131">To create an incoming document record manually</span></span>
1. <span data-ttu-id="be7a3-132">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inkommande dokument** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="be7a3-132">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="be7a3-133">Välj åtgärden **Skapa från fil**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-133">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="be7a3-134">Välj en fil och välj sedan **Öppna** i fönstret **Infoga fil**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-134">In the **Insert File** window, select a file, and then choose **Open**.</span></span>

    <span data-ttu-id="be7a3-135">Filen kopplas automatiskt.</span><span class="sxs-lookup"><span data-stu-id="be7a3-135">The file is automatically attached.</span></span>
4. <span data-ttu-id="be7a3-136">Välj alternativt åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-136">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="be7a3-137">För att bifoga en fil väljer du åtgärden **Bifoga fil**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-137">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="be7a3-138">Markera filen som representerar det inkommande dokumentet i fråga och välj sedan knappen **Öppna** i fönstret **Infoga fil**.</span><span class="sxs-lookup"><span data-stu-id="be7a3-138">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="be7a3-139">I fönstret **Inkommande dokument** fyller du i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="be7a3-139">In the **Incoming Document** window, fill in the fields as necessary.</span></span> <span data-ttu-id="be7a3-140">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="be7a3-140">Choose a field to read a short description of the field or link to more information.</span></span>

##<a name="see-also"></a><span data-ttu-id="be7a3-141">Se även</span><span class="sxs-lookup"><span data-stu-id="be7a3-141">See Also</span></span>  
[<span data-ttu-id="be7a3-142">Bearbeta inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="be7a3-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="be7a3-143">Inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="be7a3-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="be7a3-144">Hantera inköp</span><span class="sxs-lookup"><span data-stu-id="be7a3-144">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="be7a3-145">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="be7a3-145">Work With Dynamics NAV</span></span>](ui-work-product.md)

