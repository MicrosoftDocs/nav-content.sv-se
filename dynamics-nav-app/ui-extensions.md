---
title: "Anpassa Dynamics NAV med hjälp av tillägg"
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: cc832772a255c7c801a7b956c74da827caca3765
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# <a name="customizing-dynamics-nav-using-extensions"></a><span data-ttu-id="0ddd9-102">Anpassa Dynamics NAV med hjälp av tillägg</span><span class="sxs-lookup"><span data-stu-id="0ddd9-102">Customizing Dynamics NAV Using Extensions</span></span>
<span data-ttu-id="0ddd9-103">Du kan ändra Dynamics NAV genom att installera tillägg som lägger till funktioner, ändrar beteende eller ger dig tillgång till nya onlinetjänster.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-103">You can change Dynamics NAV by installing extensions that add functionality, change behavior, or give you access to new online services, for example.</span></span>
<span data-ttu-id="0ddd9-104">När du först startar först Dynamics NAV har du dessutom några tillägg installerade.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-104">When you first launch Dynamics NAV, some extensions are already installed for you.</span></span> <span data-ttu-id="0ddd9-105">Med tiden kan fler tillägg göras tillgängliga till dig, och du kan då välja om du vill använda tillägg eller inte.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-105">Over time, more extensions can be made available to you, and you can then choose if you want to use the extension or not.</span></span>

<span data-ttu-id="0ddd9-106">Till exempel ger Microsoft ett tillägg som ger integrering med PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-106">For example, Microsoft provides an extension that provides integration with PayPal Payments Standard.</span></span> <span data-ttu-id="0ddd9-107">Detta tillägg instalelras dessutom som standard.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-107">This extension is installed by default.</span></span>
<span data-ttu-id="0ddd9-108">Men om ett annat tillägg är tillgängligt som erbjuder integrering med en annan utbetalningtjänst, kan du installera det nya tillägget och sedan välja vilka av de två tjänsterna som ska användas.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-108">But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.</span></span>  

<span data-ttu-id="0ddd9-109">Du hanterar tilläggen i fönstret **Tilläggshantering**.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-109">You manage the extensions in the **Extension Management** window.</span></span> <span data-ttu-id="0ddd9-110">Du kan öppna det här fönstret från startsidan.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-110">You can access this window from Home.</span></span> <span data-ttu-id="0ddd9-111">Alternativt kan du välja ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Tillägg** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-111">Alternatively, choose the **Search for Page or Report** icon in the top right corner, enter **Extension**, and then choose the related link.</span></span>   

## <a name="installing-an-extension"></a><span data-ttu-id="0ddd9-112">Installerar tillägg</span><span class="sxs-lookup"><span data-stu-id="0ddd9-112">Installing an Extension</span></span>
<span data-ttu-id="0ddd9-113">Om nya tillägg görs tillgängliga till dig eftersom de har publicerats till din server kommer de att visas i fönstret **Tilläggshantering**.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-113">If new extensions are made available to you because they have been published to your server, they will be shown in the **Extension Management** window.</span></span> <span data-ttu-id="0ddd9-114">Härifrån kan du välja att installera och avinstallera tillägg.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-114">From here, you can choose to install and uninstall extensions.</span></span>  

<span data-ttu-id="0ddd9-115">Om du väljer ett tillägg kan du läsa om vad tillägget används till och du kan få mer information om tillägget.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-115">If you choose an extension, you can read about what the extension does, and you can access Help for the extension to learn more.</span></span> <span data-ttu-id="0ddd9-116">När du väljer att få ett tillägg, måste du godkänna användningsvillkoret.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-116">When you choose to get an extension, you must agree to the terms of use.</span></span>  

<span data-ttu-id="0ddd9-117">När du installerar tillägget kanske du behöver måste konfigurera det, till exempel ange ett konto för användning med tillägget **PayPal Payments Standard för Dynamics NAV**.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-117">When you install an extension, you might have to set it up, such as specifying an account for use with the **PayPal Payments Standard for Dynamics NAV** extension.</span></span>
<span data-ttu-id="0ddd9-118">Andra tillägg lägger bara till i fält på en befintlig sida, eller lägger till en ny sida, till exempel.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-118">Other extensions simply add fields to an existing page, or they add a new page, for example.</span></span>   

<span data-ttu-id="0ddd9-119">Om du avinstallerar tillägget och du sedan ändrar dig kan du installera det på nytt.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-119">If you uninstall an extension, and you then change your mind, you can install it again.</span></span> <span data-ttu-id="0ddd9-120">När du avinstallerar tillägg som du har använt, bevaras data så att de är tillgängliga om du installerar tillägget igen.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-120">When you uninstall an extension that you have been using, the data is preserved so that if you install the extension again, your data is still available.</span></span>  

<span data-ttu-id="0ddd9-121">Microsoft ger även följande tillägg:</span><span class="sxs-lookup"><span data-stu-id="0ddd9-121">Microsoft provides the following extensions:</span></span>  
- [<span data-ttu-id="0ddd9-122">PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="0ddd9-122">PayPal Payments Standard</span></span>](ui-extensions-paypal-payments-standard.md)  
- [<span data-ttu-id="0ddd9-123">Prognos för försäljning och lager</span><span class="sxs-lookup"><span data-stu-id="0ddd9-123">Sales and Inventory Forecast</span></span>](ui-extensions-sales-forecast.md)  

<span data-ttu-id="0ddd9-124">Andra tillägg är även tillgängliga som standard, beroende på ditt land/region.</span><span class="sxs-lookup"><span data-stu-id="0ddd9-124">Other extensions are also available by default, depending on your country/region.</span></span>

## <a name="see-also"></a><span data-ttu-id="0ddd9-125">Se även</span><span class="sxs-lookup"><span data-stu-id="0ddd9-125">See Also</span></span>  
[<span data-ttu-id="0ddd9-126">Så här aktiverar du kundutbetalning via PayPal</span><span class="sxs-lookup"><span data-stu-id="0ddd9-126">How to: Enable Customer Payment Through PayPal</span></span>](sales-how-enable-customer-payments-paypal.md)  
[<span data-ttu-id="0ddd9-127">Välkommen till Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0ddd9-127">Welcome to Dynamics NAV</span></span>](across-get-started.md)  

