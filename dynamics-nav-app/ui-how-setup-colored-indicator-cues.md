---
title: "Så här skapar du en färglagd indikator på stack-ikoner"
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
ms.openlocfilehash: 38cd904d0cf22374eac430d035e6ea6d205bcab8
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---
    
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="f6f5d-102">Så här skapar du en färglagd indikator på stack-ikoner</span><span class="sxs-lookup"><span data-stu-id="f6f5d-102">How to: Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="f6f5d-103">Du kan skapa stack-ikoner som visas på **Startsidan** för att inkludera en indikator som ändrar färg baserat på datavärdena i stack-ikonerna.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-103">You can set up Cues that appear on the **Home** page to include an indicator that changes color based on the data values in the Cues.</span></span> 

<span data-ttu-id="f6f5d-104">Indikatorn visas som en kulört stapel längs den övre kanten på stack-ikon-panelen.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-104">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="f6f5d-105">Den ger en visuell signal över statusen för stack-ikonaktivitet, som kan ange gynnsamma eller ofördelaktiga förhållanden för att meddela användaren att vidta åtgärd.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-105">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="f6f5d-106">Om t.ex. en stack-ikon visar pågående försäljningsfakturor kan du ställa in indikatorn för att visa grönt (positivt) när totala antalet pågående försäljningsfakturor är under 10, och röd (negativt) när antalet är större än 20.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-106">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="f6f5d-107">Från fönstret **Inställning av stack-ikon** ställer du in indikatorer för alla stack-ikoner som är tillgängliga i företagsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-107">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="f6f5d-108">För att ställa in indikatorn, anger du upp till två tröskelvärden som definierar tre intervall av datavärden (låg, medel och hög) som du kan koppla en annan färg (eller stil).</span><span class="sxs-lookup"><span data-stu-id="f6f5d-108">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="f6f5d-109">Så här ställer du in kulörta indikatorer på stack-ikoner</span><span class="sxs-lookup"><span data-stu-id="f6f5d-109">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="f6f5d-110">Under **Aktiviteter** på din **Startsida** väljer du **Inställning av stack-ikon**.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-110">Under **Activities** on your **Home** page, choose **Set Up Cues**.</span></span>  
<span data-ttu-id="f6f5d-111">Fönstret **Inställning av stack-ikon** visas.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-111">The **Cue Setup** window appears.</span></span> <span data-ttu-id="f6f5d-112">I fönstret anges indikatorerna som för närvarande är inställda på stack-ikoner.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-112">The window lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="f6f5d-113">För att ändra en indikator redigerar du fälten och för att ändra till exempel,värdena för de olika trösklarna.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-113">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="f6f5d-114">Efterföljande tabeller listar de bakgrundsfärger som motsvarar alternativen för fälten **Lågt intervallformat**, **Medelintervallformat** och **Högt intervallformat**.</span><span class="sxs-lookup"><span data-stu-id="f6f5d-114">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

|<span data-ttu-id="f6f5d-115">Alternativ</span><span class="sxs-lookup"><span data-stu-id="f6f5d-115">Option</span></span>|<span data-ttu-id="f6f5d-116">Färg</span><span class="sxs-lookup"><span data-stu-id="f6f5d-116">Color</span></span>|
|------|-----|
|<span data-ttu-id="f6f5d-117">**Ingen**</span><span class="sxs-lookup"><span data-stu-id="f6f5d-117">**None**</span></span>|<span data-ttu-id="f6f5d-118">Ingen färg (samma färg som stack-ikonen</span><span class="sxs-lookup"><span data-stu-id="f6f5d-118">No color (same color as the Cue tile</span></span>|
|<span data-ttu-id="f6f5d-119">**Positiv**</span><span class="sxs-lookup"><span data-stu-id="f6f5d-119">**Favorable**</span></span>|<span data-ttu-id="f6f5d-120">Grön</span><span class="sxs-lookup"><span data-stu-id="f6f5d-120">Green</span></span>|
|<span data-ttu-id="f6f5d-121">**Negativ**</span><span class="sxs-lookup"><span data-stu-id="f6f5d-121">**Unfavorable**</span></span>|<span data-ttu-id="f6f5d-122">Röd</span><span class="sxs-lookup"><span data-stu-id="f6f5d-122">Red</span></span>|
|<span data-ttu-id="f6f5d-123">**Tvetydigt**</span><span class="sxs-lookup"><span data-stu-id="f6f5d-123">**Ambiguous**</span></span>|<span data-ttu-id="f6f5d-124">Gul</span><span class="sxs-lookup"><span data-stu-id="f6f5d-124">Yellow</span></span>|
|<span data-ttu-id="f6f5d-125">**Underordnad**</span><span class="sxs-lookup"><span data-stu-id="f6f5d-125">**Subordinate**</span></span>|<span data-ttu-id="f6f5d-126">Grått</span><span class="sxs-lookup"><span data-stu-id="f6f5d-126">Gray</span></span>|

## <a name="see-also"></a><span data-ttu-id="f6f5d-127">Se även</span><span class="sxs-lookup"><span data-stu-id="f6f5d-127">See Also</span></span>
[<span data-ttu-id="f6f5d-128">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="f6f5d-128">Work with Dynamics NAV</span></span>](ui-work-product.md)


