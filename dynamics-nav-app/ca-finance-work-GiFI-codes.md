---
title: "Så här arbetar du med GIFI-koder i Kanada"
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 695bca0a6836c47610210b759ae48af27484761f
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-work-with-gifi-codes-in-canada"></a><span data-ttu-id="2c860-102">Så här arbetar du med GIFI-koder i Kanada</span><span class="sxs-lookup"><span data-stu-id="2c860-102">How to: Work With GIFI Codes in Canada</span></span>
<span data-ttu-id="2c860-103">Skatteinformation kan inkludera redovisningskonton, rapporter, resultaträkningar, balansräkningar och rapporter över balanserad vinst och förlust.</span><span class="sxs-lookup"><span data-stu-id="2c860-103">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span></span> <span data-ttu-id="2c860-104">Skatteinformation grupperas med hjälp av koder.</span><span class="sxs-lookup"><span data-stu-id="2c860-104">Fiscal information is classified using codes.</span></span> <span data-ttu-id="2c860-105">Hanteringen av koder hjälper regeringen att bearbeta information, förbereda sig för elektronisk arkivering och validera skatteinformation elektroniskt.</span><span class="sxs-lookup"><span data-stu-id="2c860-105">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span></span> <span data-ttu-id="2c860-106">Hanteringen av koder hjälper också statistiska organisationer att arbeta mer effektivt, eftersom den ekonomiska informationen är mer lättillgänglig.</span><span class="sxs-lookup"><span data-stu-id="2c860-106">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span></span> <span data-ttu-id="2c860-107">Mer information finns i [Webbplatsen för Canada Revenue Agency](http://www.cra-arc.gc.ca/).</span><span class="sxs-lookup"><span data-stu-id="2c860-107">For more information, see the [Canada Revenue Agency website](http://www.cra-arc.gc.ca/).</span></span>

<span data-ttu-id="2c860-108">Canada Revenue Agency använder det allmänna indexet av koder för ekonomisk information (GIFI) för att elektroniskt samla, verifiera och bearbeta ekonomisk information och skatteinformation.</span><span class="sxs-lookup"><span data-stu-id="2c860-108">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span></span> <span data-ttu-id="2c860-109">Det är bäst att endast tilldela GIFI-koder för bokföringskonton så att all summering görs av ditt skattförberedelseprogram.</span><span class="sxs-lookup"><span data-stu-id="2c860-109">It is a best practice to assign GIFI codes only to posting accounts, so that all totaling is done by your tax preparation software.</span></span>

<span data-ttu-id="2c860-110">När ett konto är kopplat till en GIFI-kod, rapporteras den till Revenue Agency med den koden.</span><span class="sxs-lookup"><span data-stu-id="2c860-110">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span></span> <span data-ttu-id="2c860-111">Flera konton kan använda samma GIFI-kod, men varje konto kan endast ha en GIFI-kod.</span><span class="sxs-lookup"><span data-stu-id="2c860-111">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span></span>

<span data-ttu-id="2c860-112">Du kan exportera information om saldo per GIFI-kod och spara den exporterade filen i Excel, vilket är användbart för att överföra information till ditt skattförberedelseprogram.</span><span class="sxs-lookup"><span data-stu-id="2c860-112">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span></span>

## <a name="to-set-up-gifi-codes"></a><span data-ttu-id="2c860-113">Så här skapar du GIFI-koder:</span><span class="sxs-lookup"><span data-stu-id="2c860-113">To set up GIFI codes</span></span>
<span data-ttu-id="2c860-114">I Dynamics NAV måste du lägga upp GIFI-koder för redovisningskonton, rapporter, balansräkningar, inkomstark och rapporter över balanserad vinst och förlust.</span><span class="sxs-lookup"><span data-stu-id="2c860-114">In Dynamics NAV, you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span></span>

1. <span data-ttu-id="2c860-115">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **GIFI-koder** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="2c860-115">In the top right corner, choose the **Search for Page or Report** icon, enter **GIFI Codes**, and then choose the related link.</span></span>
2. <span data-ttu-id="2c860-116">I fönstret **GIFI-koder** väljer du åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="2c860-116">In the **GIFI Codes** window, choose the **New** action.</span></span>
3. <span data-ttu-id="2c860-117">Skapa GIFI-koder, genom att fylla i fälten.</span><span class="sxs-lookup"><span data-stu-id="2c860-117">Set up GIFI codes by filling the fields.</span></span> <span data-ttu-id="2c860-118">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="2c860-118">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-associate-gifi-codes-with-gl-accounts"></a><span data-ttu-id="2c860-119">Om du vill koppla GIFI-koder med redovisningskonton</span><span class="sxs-lookup"><span data-stu-id="2c860-119">To associate GIFI codes with G/L accounts</span></span>
<span data-ttu-id="2c860-120">Om du vill rapportera ekonomiska information med GIFI-kod, måste varje GIFI-kod vara kopplad till korrekta konton i kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="2c860-120">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span></span>

1. <span data-ttu-id="2c860-121">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Kontoplan** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="2c860-121">In the top right corner, choose the **Search for Page or Report** icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="2c860-122">Välj ett relevant redovisningskonto och välj sedan åtgärden **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="2c860-122">Select a relevant general ledger account, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="2c860-123">På snabbfliken **Kostnadsredovisning** i fältet **GIFI-kod** väljer du lämplig GIFI-kod.</span><span class="sxs-lookup"><span data-stu-id="2c860-123">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span></span>

## <a name="to-view-account-balances-using-the-gifi-code-report"></a><span data-ttu-id="2c860-124">Om du vill visa kontosaldon som använder GIFI-kodrapport</span><span class="sxs-lookup"><span data-stu-id="2c860-124">To view account balances using the GIFI code report</span></span>
<span data-ttu-id="2c860-125">Du kan granska kontosaldon per GIFI-kod, genom att använda rapporten **kontosaldon per GIFI-kod**.</span><span class="sxs-lookup"><span data-stu-id="2c860-125">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span></span>

1. <span data-ttu-id="2c860-126">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **kontosaldon per GIFI-kod** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="2c860-126">In the top right corner, choose the **Search for Page or Report** icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span></span>
2. <span data-ttu-id="2c860-127">Ange vad som ska ingå i rapporten genom att fylla i fälten.</span><span class="sxs-lookup"><span data-stu-id="2c860-127">Specify what to include in the report by filling the fields.</span></span> <span data-ttu-id="2c860-128">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="2c860-128">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="2c860-129">Välj knappen **Skriv ut** eller **Förhandsgranska**.</span><span class="sxs-lookup"><span data-stu-id="2c860-129">Choose the **Print** or the **Preview** button.</span></span>

## <a name="to-export-balance-information-using-gifi-codes"></a><span data-ttu-id="2c860-130">Så här exporterar du saldoinformation med hjälp av GIFI-koder</span><span class="sxs-lookup"><span data-stu-id="2c860-130">To export balance information using GIFI codes</span></span>
<span data-ttu-id="2c860-131">Du kan exportera saldoinformation med hjälp av GIFI-koder och spara den exporterade filen i Excel.</span><span class="sxs-lookup"><span data-stu-id="2c860-131">You can export balance information using GIFI codes and save the exported file in Excel.</span></span> <span data-ttu-id="2c860-132">Du kan ändra, spara eller ta bort filen.</span><span class="sxs-lookup"><span data-stu-id="2c860-132">You can modify, save, or delete the file.</span></span> <span data-ttu-id="2c860-133">Du kan använda den för att överföra information till ditt skattförberedelseprogram.</span><span class="sxs-lookup"><span data-stu-id="2c860-133">You can use the file to transfer information to your tax preparation software.</span></span>

1. <span data-ttu-id="2c860-134">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Exportera information om GIFI till Excel** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="2c860-134">In the top right corner, choose the **Search for Page or Report** icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span></span>
2. <span data-ttu-id="2c860-135">Ange vad du vill exportera till Excel, genom att fylla i fälten.</span><span class="sxs-lookup"><span data-stu-id="2c860-135">Specify what to export to Excel by filling the fields.</span></span> <span data-ttu-id="2c860-136">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="2c860-136">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="2c860-137">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="2c860-137">Choose the **OK** button.</span></span>

<span data-ttu-id="2c860-138">**Obs!** Excel-filen har följande egenskaper:</span><span class="sxs-lookup"><span data-stu-id="2c860-138">**Note:** The Excel file has the following characteristics:</span></span>

* <span data-ttu-id="2c860-139">Saldot avrundas till den närmaste procentsatsen, men cellvärdet behåller samma procentsats som i redovisningen.</span><span class="sxs-lookup"><span data-stu-id="2c860-139">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span></span>

* <span data-ttu-id="2c860-140">Negativa nummer representeras av positiva nummer i hakparenteser.</span><span class="sxs-lookup"><span data-stu-id="2c860-140">Negative numbers are represented as positive number in brackets.</span></span> <span data-ttu-id="2c860-141">-123 anges därför som (123).</span><span class="sxs-lookup"><span data-stu-id="2c860-141">Accordingly, -123 is represented as (123).</span></span>

## <a name="see-also"></a><span data-ttu-id="2c860-142">Se även</span><span class="sxs-lookup"><span data-stu-id="2c860-142">See Also</span></span>
<span data-ttu-id="2c860-143">[Finans](finance-setup.md) </span><span class="sxs-lookup"><span data-stu-id="2c860-143">[Finance](finance-setup.md) </span></span>  
[<span data-ttu-id="2c860-144">Konfigurera Centrala finansiella processer</span><span class="sxs-lookup"><span data-stu-id="2c860-144">Set Up Core Financial Processes</span></span>](finance-setup-setup-finance-setup.md)

