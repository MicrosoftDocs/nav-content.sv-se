---
title: "Så här ändrar du vilken layout som används i en rapport för närvarande"
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
ms.openlocfilehash: a97caf4b123ffcb21099d73044370bcb20ea1750
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-change-which-layout-is-currently-used-on-a-report"></a><span data-ttu-id="8ac0c-102">Så här ändrar du vilken layout som används i en rapport för närvarande</span><span class="sxs-lookup"><span data-stu-id="8ac0c-102">How to: Change Which Layout is Currently Used on a Report</span></span>
<span data-ttu-id="8ac0c-103">En rapport kan ställas in med fler än en rapportlayout som du kan växla mellan.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-103">A report can be set up with more than one report layout, which you can then switch among as needed.</span></span>

<span data-ttu-id="8ac0c-104">Beroende på layouterna som finns tillgängliga för en rapport kan du välja att använda en inbyggd RDLC-rapportlayout, en inbyggd Word-rapportlayout eller en anpassad layout.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-104">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span></span> <span data-ttu-id="8ac0c-105">Mer information om RDLC- och Word-rapportlayouter, inbyggda och anpassade layouter och mer finns i [Hantera rapportlayouter](ui-manage-report-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="8ac0c-105">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span></span>

## <a name="to-change-the-layout-that-is-used-on-a-report"></a><span data-ttu-id="8ac0c-106">Så här ändrar du layout som används i en rapport</span><span class="sxs-lookup"><span data-stu-id="8ac0c-106">To change the layout that is used on a report</span></span>
1. <span data-ttu-id="8ac0c-107">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Val av rapportlayout** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-107">In the top right corner, choose the **Search for Page or Report** icon, enter **Report Layout Selection**, and then choose the related link.</span></span>  
<span data-ttu-id="8ac0c-108">I fönstret **Val av rapportlayout** visas alla rapporter som är tillgängliga i företaget som har angetts i fältet Företag högst upp i fönstret.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-108">The **Report Layout Selection** window lists all the reports that are available for the company that is specified in the Company field at the top of the window.</span></span> <span data-ttu-id="8ac0c-109">Fältet Vald layout anger den layout som används i rapporten för närvarande.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-109">The Selected Layout field specifies the layout that is currently used on the report.</span></span>
2. <span data-ttu-id="8ac0c-110">Ange fältet **Företag** fältet högst upp i fönstret till företaget som inkluderar rapporten.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-110">Set the **Company** field at the top of the window to the company that includes the report.</span></span>
3. <span data-ttu-id="8ac0c-111">I raden för rapporten i listan och anger du fältet **Vald layout** till ett av följande alternativ för att ändra layouten som används för en rapport:</span><span class="sxs-lookup"><span data-stu-id="8ac0c-111">To change the layout that is used by a report, in the row for the report in the list, set the **Selected Layout** field to one of the following options:</span></span>
    - <span data-ttu-id="8ac0c-112">RDLC (inbyggd), använder den inbyggda RDLC-rapportlayouten i rapporten.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-112">RDLC (built-in), uses the built-in RDLC report layout on the report.</span></span>
    - <span data-ttu-id="8ac0c-113">Word (inbyggd), använder den inbyggda Word-rapportlayouten i rapporten.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-113">Word (built-in), uses the built-in Word report layout on the report.</span></span>
    - <span data-ttu-id="8ac0c-114">Anpassad använder en anpassad layout i rapporten.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-114">Custom, uses a custom layout on the report.</span></span>  
    <span data-ttu-id="8ac0c-115">Du kan se vilka anpassade layouter som är tillgängliga för rapporten i faktaboxen Rapportlayoutdelar.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-115">You can see which custom layouts are available for the report in the Report Layouts Part FactBox.</span></span> <span data-ttu-id="8ac0c-116">Om det inte finns några anpassade layouter för rapporten, måste du skapa en först.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-116">If there are no custom layouts for the report, then you will have to create one first.</span></span> <span data-ttu-id="8ac0c-117">Om du väljer det här alternativet, gå vidare till nästa procedur för att ange den anpassade layout som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-117">If you choose this option, go to the next procedure to specify the custom layout that you want to use.</span></span>
<span data-ttu-id="8ac0c-118">**Obs!** Om du väljer **RDLC (inbyggt)** eller **Word (inbyggt)** och du får ett felmeddelande att rapporten inte har en layout för den angivna typen, måste du välja ett annat layoutalternativ eller skapa en anpassad rapportlayout av den typ som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-118">**Note**: If you choose **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span></span>

<span data-ttu-id="8ac0c-119">Om du har valt en inbyggd RDLC- eller Word-rapportlayout krävs ingen mer åtgärd och layouten används i när rapporten körs nästa gång.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-119">If you selected a built-in RDLC or Word report layout, then no further action is required and the layout will be used the next time the report is run.</span></span>

## <a name="to-specify-a-custom-layout-on-a-report"></a><span data-ttu-id="8ac0c-120">Så här anger du en anpassad layout på en rapport</span><span class="sxs-lookup"><span data-stu-id="8ac0c-120">To specify a custom layout on a report</span></span>
1. <span data-ttu-id="8ac0c-121">Du anger vilken anpassad layout som ska användas i rapporten i fönstret **Anpassad rapportlayout**.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-121">You specify which custom layout to use on the report from the **Custom Report Layouts** window.</span></span> <span data-ttu-id="8ac0c-122">Om fönstret **Anpassad rapportlayout** inte är öppet väljer du sökknappen i fältet **Rapportlayoutbeskrivning**.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-122">If the **Custom Report Layouts** window is not open, then in the **Report Layout Description** field, choose the lookup button.</span></span>
2. <span data-ttu-id="8ac0c-123">I fönstret **Rapportlayoutbeskrivning** markera raden för anpassad layout som du vill använda, och välj sedan knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-123">In the **Custom Report Layouts** window, select the row for custom layout that you want to use, and then choose the **OK** button.</span></span>

<span data-ttu-id="8ac0c-124">Du återgår till fönstret **Val av rapportlayout**.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-124">You return to the **Report Layout Selection** window.</span></span> <span data-ttu-id="8ac0c-125">Namnet på den valda anpassade layouten visas i fältet **Anpassad layoutbeskrivning**.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-125">The name of the selected custom layout displays in the **Custom Layout Description** field.</span></span> <span data-ttu-id="8ac0c-126">Den anpassade layouten används nästa gången som du kör rapporten.</span><span class="sxs-lookup"><span data-stu-id="8ac0c-126">The custom layout will be used the next time that you run the report.</span></span>

## <a name="see-also"></a><span data-ttu-id="8ac0c-127">Se även</span><span class="sxs-lookup"><span data-stu-id="8ac0c-127">See Also</span></span>
[<span data-ttu-id="8ac0c-128">Hantera rapportlayouter</span><span class="sxs-lookup"><span data-stu-id="8ac0c-128">Manage Report Layouts</span></span>](ui-manage-report-layouts.md)

