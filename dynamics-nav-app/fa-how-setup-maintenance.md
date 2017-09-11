---
title: "Så här skapar du underhåll av anläggningstillgångar"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ace0fb13d2be71c7204f16f34f6b65b54ff98230
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-maintenance"></a><span data-ttu-id="243c2-102">Så här skapar du underhåll av anläggningstillgångar</span><span class="sxs-lookup"><span data-stu-id="243c2-102">How to: Set Up Fixed Asset Maintenance</span></span>
<span data-ttu-id="243c2-103">Om du vill hantera underhåll av anläggningstillgångar måste du först ange viss allmän underhållsinformation, ett bokföringskonto för underhållskostnader och underhållskoder för olika typer av arbete, till exempel rutintjänst eller reparation.</span><span class="sxs-lookup"><span data-stu-id="243c2-103">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span></span>

## <a name="to-set-up-general-maintenance-information"></a><span data-ttu-id="243c2-104">Så här ställer du in allmän underhållsinformation</span><span class="sxs-lookup"><span data-stu-id="243c2-104">To set up general maintenance information</span></span>
<span data-ttu-id="243c2-105">Om du skapar fält för underhåll kan du bokföra underhållskostnader från anläggningstillgångsjournalen.</span><span class="sxs-lookup"><span data-stu-id="243c2-105">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span></span>
1. <span data-ttu-id="243c2-106">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="243c2-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="243c2-107">Markera den fasta anläggningstillgång som du definierar täckning av försäkring för välj sedan åtgärden **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="243c2-107">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="243c2-108">Fyll i så många fält som behövs på snabbfliken **Underhåll**.</span><span class="sxs-lookup"><span data-stu-id="243c2-108">On the **Maintenance** FastTab, fill in the fields as necessary.</span></span> <span data-ttu-id="243c2-109">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="243c2-109">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-maintenance-codes"></a><span data-ttu-id="243c2-110">Så här skapar du underhållskoder</span><span class="sxs-lookup"><span data-stu-id="243c2-110">To set up maintenance codes</span></span>  
<span data-ttu-id="243c2-111">När du bokför underhållskostnader (från en redovisningsjournal eller en inköpsfaktura) fyller du i fältet **Underhållskod** för att ange vilken typ av underhåll som har utförts, t.ex. rutinservice eller reparation.</span><span class="sxs-lookup"><span data-stu-id="243c2-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span></span>
1. <span data-ttu-id="243c2-112">Eller välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Underhåll** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="243c2-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Maintenance**, and then choose the related link.</span></span>
2. <span data-ttu-id="243c2-113">Lägg upp koder för andra typer av underhållsarbete i fönstret **Underhåll**.</span><span class="sxs-lookup"><span data-stu-id="243c2-113">In the **Maintenance** window, set up codes for different types of maintenance work.</span></span>

## <a name="to-set-up-maintenance-expense-accounts"></a><span data-ttu-id="243c2-114">Så här skapar du underhållskostnader</span><span class="sxs-lookup"><span data-stu-id="243c2-114">To set up maintenance expense accounts</span></span>  
<span data-ttu-id="243c2-115">Om du vill bokföra underhållskostnader måste du först ange ett kontonummer i fönstret **Anl. bokföringsmallar**.</span><span class="sxs-lookup"><span data-stu-id="243c2-115">To post maintenance costs, you must first enter an account number in the **FA Posting Groups** window.</span></span>
1. <span data-ttu-id="243c2-116">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. bokföringsmall** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="243c2-116">In the top right corner, choose the **Search for Page or Report** icon, enter **FA Posting Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="243c2-117">Fyll i fältet **Underhållskostnader** för varje bokföringsmall.</span><span class="sxs-lookup"><span data-stu-id="243c2-117">Fill in the **Maintenance Expense Account** field for each posting group.</span></span>

<span data-ttu-id="243c2-118">**Obs**: om du vill att underhållskostnaderna ska fördelas på avdelningar och/eller projekt måste du skapa en fördelningsnyckel</span><span class="sxs-lookup"><span data-stu-id="243c2-118">**Note**: To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span></span> <span data-ttu-id="243c2-119">Mer information finns i [Så här ställer du in allmänna funktioner för anläggningstillgångar](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="243c2-119">For more information, see [How to: Set Up General Fixed Assets Features](fa-how-setup-general.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="243c2-120">Se även</span><span class="sxs-lookup"><span data-stu-id="243c2-120">See Also</span></span>
[<span data-ttu-id="243c2-121">Skapa anläggningstillgångar</span><span class="sxs-lookup"><span data-stu-id="243c2-121">Set Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="243c2-122">Hantera anläggningstillgångar</span><span class="sxs-lookup"><span data-stu-id="243c2-122">Manage Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="243c2-123">Finans</span><span class="sxs-lookup"><span data-stu-id="243c2-123">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="243c2-124">Välkommen till Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="243c2-124">Welcome to Dynamics NAV</span></span>](across-get-started.md)

