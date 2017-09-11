---
title: Skapa nummerserier
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a><span data-ttu-id="9ad72-102">Skapa nummerserier</span><span class="sxs-lookup"><span data-stu-id="9ad72-102">Create Number Series</span></span>

<span data-ttu-id="9ad72-103">För varje företag som du lägger upp måste du tilldela unika ID-koder till exempelvis redovisningskonton, kund- och leverantörskonton, fakturor och dokument.</span><span class="sxs-lookup"><span data-stu-id="9ad72-103">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and documents.</span></span> <span data-ttu-id="9ad72-104">Numrering är viktigt inte enbart för identifiering.</span><span class="sxs-lookup"><span data-stu-id="9ad72-104">Numbering is important not only for identification.</span></span> <span data-ttu-id="9ad72-105">Ett adekvat numreringssystem gör också företaget mer hanterbart och enkelt att analysera, och kan minska antalet fel som uppstår vid datainmatning.</span><span class="sxs-lookup"><span data-stu-id="9ad72-105">A well-designed numbering system also makes the company more manageable and easy to analyze, and can reduce the number of errors that occur in data entry.</span></span>

<span data-ttu-id="9ad72-106">Du kan lägga upp ett komplett numreringssystem med ett obegränsat antal nummerserier.</span><span class="sxs-lookup"><span data-stu-id="9ad72-106">You can set up a complete numbering system with an unlimited number of number series.</span></span> <span data-ttu-id="9ad72-107">Du kan använda nummerserier för alla typer av dokument och journaler, samt för huvuddata som kunder, artiklar och projekt.</span><span class="sxs-lookup"><span data-stu-id="9ad72-107">You can use number series for all types of documents and journals, as well as for master data such as customers, items, and jobs.</span></span>

<span data-ttu-id="9ad72-108">Du kan kombinera och använda nummerserier vid manuell numrering.</span><span class="sxs-lookup"><span data-stu-id="9ad72-108">You can combine the use of number series with manual numbering.</span></span>

<span data-ttu-id="9ad72-109">Du skapar ett numreringssystem genom att skapa en eller flera koder för varje typ av huvuddata eller dokument.</span><span class="sxs-lookup"><span data-stu-id="9ad72-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span></span> <span data-ttu-id="9ad72-110">Du kan till exempel skapa en kod för numrering av kunder, en annan för numrering av försäljningsfakturor och en annan för numrering av dokument i redovisningsjournaler.</span><span class="sxs-lookup"><span data-stu-id="9ad72-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span></span>

<span data-ttu-id="9ad72-111">När du har skapat en kod måste du skapa minst en nummerserierad.</span><span class="sxs-lookup"><span data-stu-id="9ad72-111">After you have set up a code, you set must set up at least one number series line.</span></span> <span data-ttu-id="9ad72-112">Nummerserieraden innehåller information som första och sista nummer i serien och startdatum.</span><span class="sxs-lookup"><span data-stu-id="9ad72-112">The number series line contains information such as the first and last number in the series and the starting date.</span></span> <span data-ttu-id="9ad72-113">Du kan registrera flera nummerserierader per nummerseriekod, med olika startdatum på varje rad.</span><span class="sxs-lookup"><span data-stu-id="9ad72-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span></span> <span data-ttu-id="9ad72-114">Nummerserierna används löpande, med början på respektive startdatum.</span><span class="sxs-lookup"><span data-stu-id="9ad72-114">The series will be used consecutively, starting each series on the respective starting date.</span></span>

<span data-ttu-id="9ad72-115">Om du vill använda mer än en nummerseriekod för en typ av huvuddata, till exempel om du vill använda olika nummerserier för olika kategorier med artiklar, kan du använda nummerseriesamband.</span><span class="sxs-lookup"><span data-stu-id="9ad72-115">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span></span>

<span data-ttu-id="9ad72-116">Förutom de nummer som du tilldelar manuellt eller med hjälp av numreringssystemet, tilldelas alla transaktioner automatiskt löpnummer.</span><span class="sxs-lookup"><span data-stu-id="9ad72-116">In addition to the numbers that you assign manually or by use of the numbering system, all transactions (ledger entries) are automatically assigned consecutive numbers.</span></span> <span data-ttu-id="9ad72-117">Dessa nummer visas i **Löpnr.**</span><span class="sxs-lookup"><span data-stu-id="9ad72-117">These numbers can be seen in the **Entry No.**</span></span> <span data-ttu-id="9ad72-118">fält i alla transaktionsfönster.</span><span class="sxs-lookup"><span data-stu-id="9ad72-118">field in all the ledger entry windows.</span></span> <span data-ttu-id="9ad72-119">Du kan inte ändra eller ta bort dessa nummer.</span><span class="sxs-lookup"><span data-stu-id="9ad72-119">You cannot modify or delete these numbers.</span></span>

## <a name="to-create-relationships-between-number-series"></a><span data-ttu-id="9ad72-120">Så här skapar du samband mellan nummerserier</span><span class="sxs-lookup"><span data-stu-id="9ad72-120">To create relationships between number series</span></span>
<span data-ttu-id="9ad72-121">Om du har definierat mer än en nummerseriekod för samma typ av allmän information eller transaktioner kan du skapa samband mellan koderna.</span><span class="sxs-lookup"><span data-stu-id="9ad72-121">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span></span> <span data-ttu-id="9ad72-122">Den här funktionen gör det enklare för dig att välja bland koderna när du använder ett nummer.</span><span class="sxs-lookup"><span data-stu-id="9ad72-122">This feature can assist you in deciding among the codes when you use a number.</span></span>

1. <span data-ttu-id="9ad72-123">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Nr-serier** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="9ad72-123">In the top right corner, choose the **Search for Page or Report** icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="9ad72-124">Markera raden med de nummerserier som du vill skapa relationer för och välj sedan **Relationer**.</span><span class="sxs-lookup"><span data-stu-id="9ad72-124">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span></span>
3. <span data-ttu-id="9ad72-125">I fältet **Seriekod** anger du koden för nummerserien som du vill koppla till serien du valde i steg 2.</span><span class="sxs-lookup"><span data-stu-id="9ad72-125">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span></span>
4. <span data-ttu-id="9ad72-126">Lägg till en rad för varje kod som du vill koppla till den valda nummerserien.</span><span class="sxs-lookup"><span data-stu-id="9ad72-126">Add a line for each code that you want to relate to the selected number series.</span></span>
5. <span data-ttu-id="9ad72-127">Stäng fönstret.</span><span class="sxs-lookup"><span data-stu-id="9ad72-127">Close the window.</span></span>

<span data-ttu-id="9ad72-128">När du hädanefter definierar något för vilket ett nummer krävs kan du använda sambanden som har skapats för att välja bland de kopplade nummerserierna.</span><span class="sxs-lookup"><span data-stu-id="9ad72-128">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span></span>

## <a name="see-also"></a><span data-ttu-id="9ad72-129">Se även</span><span class="sxs-lookup"><span data-stu-id="9ad72-129">See Also</span></span>
[<span data-ttu-id="9ad72-130">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="9ad72-130">Work with Dynamics NAV</span></span>](ui-work-product.md)

