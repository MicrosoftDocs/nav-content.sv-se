---
title: "Så här konfigurerar du Inkommande dokument"
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
ms.openlocfilehash: d55329b571e4c59d4821a86a39362ea58480b86a
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="9432b-102">Så här konfigurerar du Inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="9432b-102">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="9432b-103">Om du skapar redovisningsjournalrader från inkommande dokumentposter måste du ange vilken journalmall och batch som ska användas i fönstret **Inställning av inkommande dokument**.</span><span class="sxs-lookup"><span data-stu-id="9432b-103">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="9432b-104">Om du inte vill att användare ska skapa fakturor eller redovisningsjournalrader från inkommande dokumentposter om inte dokumenten har godkänts först, måste du konfigurera godkännare i fönstret **Godkännare för inkommande dokument**.</span><span class="sxs-lookup"><span data-stu-id="9432b-104">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="9432b-105">För att omvandla PDF- och bildfiler till elektroniska dokument som du kan konverteras till, till exempel,inköpsfakturor inne i Dynamics NAV måste du först konfigurera OCR-funktionen och aktivera tjänsten.</span><span class="sxs-lookup"><span data-stu-id="9432b-105">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside Dynamics NAV, you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="9432b-106">När funktionen för Inkommande dokument är inställd, kan du använda olika funktioner för att förhandsgranska utgiftskvitton, hantera OCR-uppgifter och konvertera inkommande dokumentfiler, manuellt eller automatiskt, till relevanta dokument eller journalrader i .</span><span class="sxs-lookup"><span data-stu-id="9432b-106">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="9432b-107">De externa filerna kan kopplas till något processteg, inklusive till bokförda dokument och till resulterande leverantörs-, kund- och redovisningstransaktioner.</span><span class="sxs-lookup"><span data-stu-id="9432b-107">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="9432b-108">Mer information finns i [Så här bearbetar du inkommande dokument](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="9432b-108">For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="9432b-109">Så här konfigurerar du funktionen för inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="9432b-109">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="9432b-110">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inställning av inkommande dokument** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9432b-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="9432b-111">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="9432b-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="9432b-112">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="9432b-112">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="9432b-113">Så här konfigurerar du godkännare för inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="9432b-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="9432b-114">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inställning av inkommande dokument** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9432b-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9432b-115">I fönstret **Inställning av inkommande dokument** väljer du åtgärden **Godkännare**.</span><span class="sxs-lookup"><span data-stu-id="9432b-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="9432b-116">Fönstret **Godkännare för inkommande dokument** visar alla användare som är inställda i Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="9432b-116">The **Incoming Document Approvers** window shows all users that are set up in your Dynamics NAV .</span></span>  
3. <span data-ttu-id="9432b-117">Markera en eller flera användare som kan godkänna ett inkommande dokument, innan en relaterat dokumentet eller journalrad kan skapas.</span><span class="sxs-lookup"><span data-stu-id="9432b-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="9432b-118">När godkännare har konfigurerats i fönstret **Godkännare för inkommande dokument** kan endast dessa användare godkänna ett inkommande dokument om kryssrutan **Kräv godkännande för att skapa** i fönstret **Inställning av inkommande dokument** är markerad.</span><span class="sxs-lookup"><span data-stu-id="9432b-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

<span data-ttu-id="9432b-119">**Obs!** Denna inställning av godkännande är inte relaterad till arbetsflöden för godkännande.</span><span class="sxs-lookup"><span data-stu-id="9432b-119">**Note**: This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="9432b-120">Mer information finns i [Så här använder du arbetsflöden för godkännande](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="9432b-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="9432b-121">Så här konfigurerar du en OCR-tjänst</span><span class="sxs-lookup"><span data-stu-id="9432b-121">To set up an OCR service</span></span>
1. <span data-ttu-id="9432b-122">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **OCR-serviceinställningar** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9432b-122">In the top right corner, choose the **Search for Page or Report** icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="9432b-123">Fyll i fälten om det behövs.</span><span class="sxs-lookup"><span data-stu-id="9432b-123">Fill in the fields as necessary.</span></span> <span data-ttu-id="9432b-124">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="9432b-124">Choose a field to read a short description of the field or link to more information.</span></span>


## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="9432b-125">Så här kan du kryptera dina inloggningsuppgifter</span><span class="sxs-lookup"><span data-stu-id="9432b-125">To encrypt your login information</span></span>
<span data-ttu-id="9432b-126">Du rekommenderas att skydda de inloggningsuppgifter som du anger i fönstret **OCR-serviceinställningar**.</span><span class="sxs-lookup"><span data-stu-id="9432b-126">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="9432b-127">Du kan kryptera data på servern genom att skapa nya eller importera befintliga krypteringsnycklar som aktiverar på serverinstansen med anslutningen till databasen.</span><span class="sxs-lookup"><span data-stu-id="9432b-127">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="9432b-128">I fönstret **OCR-serviceinställningar** väljer du åtgärden **Krypteringshantering**.</span><span class="sxs-lookup"><span data-stu-id="9432b-128">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="9432b-129">Aktivera krypteringen av dina data i fönstret **Datakrypteringshantering**.</span><span class="sxs-lookup"><span data-stu-id="9432b-129">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="9432b-130">Se även</span><span class="sxs-lookup"><span data-stu-id="9432b-130">See Also</span></span>  
[<span data-ttu-id="9432b-131">Bearbeta inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="9432b-131">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="9432b-132">Inkommande dokument</span><span class="sxs-lookup"><span data-stu-id="9432b-132">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="9432b-133">Hantera inköp</span><span class="sxs-lookup"><span data-stu-id="9432b-133">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="9432b-134">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="9432b-134">Work With Dynamics NAV</span></span>](ui-work-product.md)

