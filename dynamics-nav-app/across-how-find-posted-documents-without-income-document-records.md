---
title: "Så här söker du efter bokförda dokument utan inkommande dokumentposter"
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
ms.openlocfilehash: eca38d238361a9ac50aac117199fa97fbba4374f
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="8bb91-102">Så här söker du efter bokförda dokument utan inkommande dokumentposter</span><span class="sxs-lookup"><span data-stu-id="8bb91-102">How to: Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="8bb91-103">Från fönstren **Kontoplan** och **Redovisningstransaktioner** kan du använda en sökfunktion för att hitta redovisningsposter för bokförda inköps- och försäljningsdokument som inte har inkommande dokumentposter och sedan länka dem till befintliga poster eller skapa nya centralt med bifogade dokumentfiler.</span><span class="sxs-lookup"><span data-stu-id="8bb91-103">From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="8bb91-104">Söka efter bokförda dokument utan inkommande dokumentposter</span><span class="sxs-lookup"><span data-stu-id="8bb91-104">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="8bb91-105">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Kontoplan** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="8bb91-105">In the top right corner, choose the **Search for Page or Report** icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="8bb91-106">Välj en rad för ett redovisningskonto för vilka redovisningstransaktioner du vill se bokförda inköps- och försäljningsdokument utan inkommande dokumentpost och välj sedan **Bokförda dokument utan inkommande dokument**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-106">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="8bb91-107">Välj alternativt åtgärden **Transaktioner**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-107">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="8bb91-108">I fönstret **Redovisningstransaktioner** väljer du åtgärden **Bokförda dokument utan inkommande dokument**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-108">In the **General Ledger Entries** window, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="8bb91-109">Fönstret **Dokförda dokument utan inkommande dokument** öppnas med visning av bokförda inköps- och försäljningsdokument utan inkommande dokumentposter som representeras av redovisningstransaktioner på det redovisningskonto som du öppnade fönstret för.</span><span class="sxs-lookup"><span data-stu-id="8bb91-109">The **Posted Documents without Incoming Document** window opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the window for.</span></span> <span data-ttu-id="8bb91-110">Fönstret kan innehålla högst 1000 rader.</span><span class="sxs-lookup"><span data-stu-id="8bb91-110">The window can show a maximum of 1000 lines.</span></span> <span data-ttu-id="8bb91-111">Som standard innehåller fältet **Datumfilter** därför ett filter som begränsar raderna till poster med bokföringsdatum från början av bokföringsperioden till arbetsdatumet.</span><span class="sxs-lookup"><span data-stu-id="8bb91-111">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="8bb91-112">Koppla hittade dokument till befintliga inkommande dokumentposter</span><span class="sxs-lookup"><span data-stu-id="8bb91-112">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="8bb91-113">I fönstret **Bokförda dokument utan inkommande dokument** väljer du raden för ett bokfört dokument som du vill koppla till en befintlig inkommande dokumentpost och väljer sedan åtgärden **Välj inkommande dokument**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-113">In the **Posted Documents without Incoming Document** window, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="8bb91-114">I fönstret **Inkommande dokument** väljer du den inkommande dokumentpost som du vill koppla till det hittade bokförda dokumentet och klickar sedan på knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-114">In the **Incoming Documents** window, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="8bb91-115">Nu är den valda inkommande dokumentposten kopplad till det bokförda dokumentet i fönstret **Bokförda dokument utan inkommande dokument**, som du kan se i faktaboxen **Inkommande dokumentfiler**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-115">In the **Posted Documents without Incoming Document** window, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="8bb91-116">Om en relevant inkommande dokumentpost inte finns i fönstret **Inkommande dokument** kan du skapa den.</span><span class="sxs-lookup"><span data-stu-id="8bb91-116">If a relevant incoming document record does not exist in the **Incoming Documents** window, then you can create it.</span></span> <span data-ttu-id="8bb91-117">Mer information finns i [Så här skapar du inkommande dokumentposter](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="8bb91-117">For more information, see [How to: Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="8bb91-118">Se även</span><span class="sxs-lookup"><span data-stu-id="8bb91-118">See Also</span></span>  
[<span data-ttu-id="8bb91-119">Bearbeta inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="8bb91-119">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="8bb91-120">Inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="8bb91-120">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="8bb91-121">Hantera inköp</span><span class="sxs-lookup"><span data-stu-id="8bb91-121">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="8bb91-122">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="8bb91-122">Work With Dynamics NAV</span></span>](ui-work-product.md)

