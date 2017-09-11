---
title: "Ange skrivarval för rapporter"
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
ms.openlocfilehash: 56a5c1428651162293e56d71e2369fe55d291594
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---
    
# <a name="specify-printer-selection-for-reports"></a><span data-ttu-id="3d49a-102">Ange skrivarval för rapporter</span><span class="sxs-lookup"><span data-stu-id="3d49a-102">Specify Printer Selection for Reports</span></span>
<span data-ttu-id="3d49a-103">Du kan ställa in rapporter så att de måste skrivas ut på en viss skrivare.</span><span class="sxs-lookup"><span data-stu-id="3d49a-103">You can set up reports so that they must be printed on a specific printer.</span></span> <span data-ttu-id="3d49a-104">Följande är några användningsområden för skrivarurvalet:</span><span class="sxs-lookup"><span data-stu-id="3d49a-104">The following are some uses of printer selection:</span></span> 

- <span data-ttu-id="3d49a-105">Du kan skriva ut rapporter på ett särskilt företagsbrevhuvud.</span><span class="sxs-lookup"><span data-stu-id="3d49a-105">You can print reports on special company letterhead.</span></span>
- <span data-ttu-id="3d49a-106">Du kan skriva ut rapporter i olika pappersstorlekar.</span><span class="sxs-lookup"><span data-stu-id="3d49a-106">You can print reports on different paper sizes.</span></span>
- <span data-ttu-id="3d49a-107">Du kan skriva ut rapporter på standardskrivaren för en viss anställd.</span><span class="sxs-lookup"><span data-stu-id="3d49a-107">You can print reports on the default printer of a specified employee.</span></span>

<span data-ttu-id="3d49a-108">Du använder fönstret **Skrivarval** för att ange olika värden för att få olika utflöden.</span><span class="sxs-lookup"><span data-stu-id="3d49a-108">You use the **Printer Selections** window to set different values to obtain different output.</span></span> <span data-ttu-id="3d49a-109">Om du anger ett visst skrivarval, får det sedan företräde framför mer allmänna skrivarval.</span><span class="sxs-lookup"><span data-stu-id="3d49a-109">If you set a specific printer selection, then it takes precedence over a more general printer selection.</span></span> <span data-ttu-id="3d49a-110">Du kan till exempel ange ett skrivarval som har värdena i fälten **Användar-ID**, **Rapport-ID**, och **Skrivarnamn**.</span><span class="sxs-lookup"><span data-stu-id="3d49a-110">For example, you can set a printer selection that has values in the **User ID**, **Report ID**, and **Printer Name** fields.</span></span> <span data-ttu-id="3d49a-111">Det här skrivarvalet åsidosätter det skrivarval som har tomma transaktioner i fälten **Användar-ID** , eller **Rapport-ID**.</span><span class="sxs-lookup"><span data-stu-id="3d49a-111">This printer selection takes precedence over a printer selection that has blank entries in the **User ID** or **Report ID** fields.</span></span> 

<span data-ttu-id="3d49a-112">I följande tabell beskrivs kombinationen av värdena för att ange när du lägger upp skrivarval för en rapport.</span><span class="sxs-lookup"><span data-stu-id="3d49a-112">The following table describes the combination of values to specify when you set up printer selections for a report.</span></span>

|<span data-ttu-id="3d49a-113">Om du vill</span><span class="sxs-lookup"><span data-stu-id="3d49a-113">To</span></span>                                                 |<span data-ttu-id="3d49a-114">Ange följande värden</span><span class="sxs-lookup"><span data-stu-id="3d49a-114">Set the following values</span></span>                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|<span data-ttu-id="3d49a-115">Skriva ut en rapport till en viss skrivare för alla användare</span><span class="sxs-lookup"><span data-stu-id="3d49a-115">Print a report to a specific printer for all users</span></span> |<span data-ttu-id="3d49a-116">Ange värden i fälten **Rapport-ID**, och **Skrivarnamn** och lämna fältet **Användar-ID** tomt.</span><span class="sxs-lookup"><span data-stu-id="3d49a-116">Specify values in the **Report ID** and **Printer Name** fields and leave the **User ID** field blank.</span></span>|
|<span data-ttu-id="3d49a-117">Skriva ut alla rapporter till en viss skrivare för en specifik användare</span><span class="sxs-lookup"><span data-stu-id="3d49a-117">Print all reports to a specific printer for a specific user</span></span>|<span data-ttu-id="3d49a-118">Ange värden i fälten **Användar-ID**, och **Skrivarnamn** och lämna fältet **Rapport-ID** tomt.</span><span class="sxs-lookup"><span data-stu-id="3d49a-118">Specify values in the **User ID** and **Printer Name** fields and leave the **Report ID** field blank.</span></span>|
|<span data-ttu-id="3d49a-119">Ange standardskrivaren för alla rapporter</span><span class="sxs-lookup"><span data-stu-id="3d49a-119">Set the default printer for all reports</span></span>|<span data-ttu-id="3d49a-120">Ange ett värde i fälten **Skrivarnamn** och lämna fältet **Användar-ID** och **Rapport-ID** tomma.</span><span class="sxs-lookup"><span data-stu-id="3d49a-120">Specify a value in the **Printer Name** field and leave the **User ID** and **Report ID** fields blank.</span></span>|
|<span data-ttu-id="3d49a-121">Skriva ut en viss rapport till användarens standardskrivare</span><span class="sxs-lookup"><span data-stu-id="3d49a-121">Print a specific report to the user’s default printer</span></span>|<span data-ttu-id="3d49a-122">Ange ett värde i fälten **Rapport-ID** och lämna fältet **Skrivarnamn** och **Användar-ID** tomma.</span><span class="sxs-lookup"><span data-stu-id="3d49a-122">Specify a value in the **Report ID** field and leave the **Printer Name** and **User ID** fields blank.</span></span>|
|<span data-ttu-id="3d49a-123">Skriva ut en viss rapport till en viss skrivare till en viss användare</span><span class="sxs-lookup"><span data-stu-id="3d49a-123">Print a specific report to a specific printer for a specific user</span></span>|<span data-ttu-id="3d49a-124">Ange värden i samtliga tre fält.</span><span class="sxs-lookup"><span data-stu-id="3d49a-124">Specify values in all three fields.</span></span>|

## <a name="see-also"></a><span data-ttu-id="3d49a-125">Se även</span><span class="sxs-lookup"><span data-stu-id="3d49a-125">See Also</span></span>
[<span data-ttu-id="3d49a-126">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="3d49a-126">Work with Dynamics NAV</span></span>](ui-work-product.md)

