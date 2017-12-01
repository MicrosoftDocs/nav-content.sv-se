---
title: "Så här skapar du arbetsflöden från arbetsflödesmallar"
description: "Du kan spara tid när du skapar nya arbetsflöden genom att skapa arbetsflöden från arbetsflödesmallar."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 9aa8ef38212360ed14dfef86f32afd8bfcb098dc
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-create-workflows-from-workflow-templates"></a><span data-ttu-id="e0829-103">Så här skapar du arbetsflöden från arbetsflödesmallar</span><span class="sxs-lookup"><span data-stu-id="e0829-103">How to: Create Workflows from Workflow Templates</span></span>
<span data-ttu-id="e0829-104">Du kan spara tid när du skapar nya arbetsflöden genom att skapa arbetsflöden från arbetsflödesmallar.</span><span class="sxs-lookup"><span data-stu-id="e0829-104">To save time when creating new workflows, you can create workflows from workflow templates.</span></span>  

 <span data-ttu-id="e0829-105">Arbetsflödesmallar representerar icke-redigerbara arbetsflöden som finns i den generiska versionen av [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e0829-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e0829-106">Koderna för arbetsflödesmallar som läggs till av Microsoft har prefixet ”MS-”.</span><span class="sxs-lookup"><span data-stu-id="e0829-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span>  

 <span data-ttu-id="e0829-107">Ett annat sätt att snabbt att skapa ett arbetsflöde är att importera ett befintligt arbetsflöde som du har i en fil utanför [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e0829-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e0829-108">Mer information finns i [Gör så här: Exportera och importera arbetsflöden](across-how-to-export-and-import-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="e0829-108">For more information, see [How to: Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span></span>  

<span data-ttu-id="e0829-109">I fönstret **arbetsflöde** skapar du ett arbetsflöde genom att ange de berörda stegen på raderna.</span><span class="sxs-lookup"><span data-stu-id="e0829-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="e0829-110">Varje steg består av en arbetsflödehändelse, modifierad av händelsevillkor, och ett arbetsflödesvar som modifieras av svarsalternativ.</span><span class="sxs-lookup"><span data-stu-id="e0829-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="e0829-111">Du definierar arbetsflödesstegen genom att fylla i fält på arbetsflödesrader från fasta listor med händelse- och svarsvärden som representerar de scenarier som stöds av programkoden.</span><span class="sxs-lookup"><span data-stu-id="e0829-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="e0829-112">(Mer information finns i [Så här skapar du arbetsflöde](across-how-to-create-workflows.md).)</span><span class="sxs-lookup"><span data-stu-id="e0829-112">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-create-a-workflow-from-workflow-template"></a><span data-ttu-id="e0829-113">Så här skapar du ett arbetsflöde från en arbetsflödesmall</span><span class="sxs-lookup"><span data-stu-id="e0829-113">To create a workflow from workflow template</span></span>  
1.  <span data-ttu-id="e0829-114">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "Söka efter sida eller rapport") gå till **Arbetsflöden** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="e0829-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e0829-115">Välj åtgärd **skapa arbetsflödet från mallen**.</span><span class="sxs-lookup"><span data-stu-id="e0829-115">Choose the **Create Workflow from Template** action.</span></span> <span data-ttu-id="e0829-116">Fönstret **arbetsflödesmallar**.</span><span class="sxs-lookup"><span data-stu-id="e0829-116">The **Workflow Templates** window opens.</span></span>  
3.  <span data-ttu-id="e0829-117">Markera en arbetsflödesmall och välj sedan knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="e0829-117">Select a workflow template, and then choose the **OK** button.</span></span>  

     <span data-ttu-id="e0829-118">Fönstret **Arbetsflöde** öppnas för ett nytt arbetsflöde som innehåller all information för den valda mallen.</span><span class="sxs-lookup"><span data-stu-id="e0829-118">The **Workflow** window opens for a new workflow containing all the information of the selected template.</span></span> <span data-ttu-id="e0829-119">Värdet i fältet **Kod** utökas med till exempel ”-01" för att ange att det är det första arbetsflödet som skapas från arbetsflödesmallen.</span><span class="sxs-lookup"><span data-stu-id="e0829-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span></span>  
4.  <span data-ttu-id="e0829-120">Fortsätt med att skapa arbetsflödet genom att redigera arbetsflödesstegen, eller lägg till nya steg.</span><span class="sxs-lookup"><span data-stu-id="e0829-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span></span> <span data-ttu-id="e0829-121">(Mer information finns i [Så här skapar du arbetsflöde](across-how-to-create-workflows.md).)</span><span class="sxs-lookup"><span data-stu-id="e0829-121">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="e0829-122">Se även</span><span class="sxs-lookup"><span data-stu-id="e0829-122">See Also</span></span>  
 <span data-ttu-id="e0829-123">[Så här skapar du arbetsflöden](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="e0829-123">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="e0829-124">[Gör så här: Exportera och importera arbetsflöden](across-how-to-export-and-import-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="e0829-124">[How to: Export and Import Workflows](across-how-to-export-and-import-workflows.md) </span></span>  
 <span data-ttu-id="e0829-125">[Så här visar du arkiverade instanser för arbetsflödessteg](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="e0829-125">[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="e0829-126">[Så här tar du bort arbetsflöden](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="e0829-126">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="e0829-127">[Genomgång: Konfigurera och använda ett arbetsflöde för godkännande av inköp](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="e0829-127">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="e0829-128">[Konfigurera arbetsflöden](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="e0829-128">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="e0829-129">[Använda arbetsflöden](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="e0829-129">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="e0829-130">Arbetsflöde</span><span class="sxs-lookup"><span data-stu-id="e0829-130">Workflow</span></span>](across-workflow.md)   

