<properties
                pageTitle="Så här omvärderar du lager | Dynamics NAV"
                description="Beskriver hur du uppskattar eller skriver av värdet av en eller flera artiklar i lager genom att bokföra deras faktiska, beräknade värde."
                services="project-madeira"
                documentationCenter=""
                authors="SorenGP"
/>
<tags
    ms.service="project-madeira"
    ms.topic="article"
    ms.devlang="na"
    ms.tgt_pltfrm="na"
    ms.workload="na"
    ms.date="11/07/2016"
    ms.author="SorenGP" />


# <a name="how-to-revalue-inventory"></a><span data-ttu-id="0cc26-103">Så här omvärderar du lager</span><span class="sxs-lookup"><span data-stu-id="0cc26-103">How to: Revalue Inventory</span></span>   
<span data-ttu-id="0cc26-104">Om du vill öka eller minska värdet för en artikel eller en viss artikeltransaktion, använder du omvärderingsjournalen.</span><span class="sxs-lookup"><span data-stu-id="0cc26-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="0cc26-105">Omvärdera lager</span><span class="sxs-lookup"><span data-stu-id="0cc26-105">To revalue inventory</span></span>
1. <span data-ttu-id="0cc26-106">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Omvärderingsjournal** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="0cc26-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="0cc26-107">Välj åtgärden **Beräkna lagervärde**.</span><span class="sxs-lookup"><span data-stu-id="0cc26-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="0cc26-108">I fönstret **Beräkna lagervärde** fyller du i fälten efter behov.</span><span class="sxs-lookup"><span data-stu-id="0cc26-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span></span> <span data-ttu-id="0cc26-109">Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.</span><span class="sxs-lookup"><span data-stu-id="0cc26-109">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="0cc26-110">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="0cc26-110">Choose the **OK** button.</span></span>
5. <span data-ttu-id="0cc26-111">På varje rad i fönstret **Omvärderingsjournal** i fältet **Styckkostnad (omvärderad)** anger du den nya styckkostnaden.</span><span class="sxs-lookup"><span data-stu-id="0cc26-111">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="0cc26-112">Du kan alternativt ange det nya totalbeloppet i fältet **Lagervärde (omvärderad)**.</span><span class="sxs-lookup"><span data-stu-id="0cc26-112">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="0cc26-113">Relevanta fält uppdateras automatiskt.</span><span class="sxs-lookup"><span data-stu-id="0cc26-113">The relevant fields are automatically updated.</span></span> <span data-ttu-id="0cc26-114">Lägg märke till att den faktiska förändringen av lagervärdet för den aktuella artikeltransaktionen visas i fältet **Belopp**.</span><span class="sxs-lookup"><span data-stu-id="0cc26-114">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="0cc26-115">Detta belopp utgör skillnaden mellan värdena i fälten **Lagervärde (beräknat)** och **Lagervärde (omvärderat)**.</span><span class="sxs-lookup"><span data-stu-id="0cc26-115">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>

6. <span data-ttu-id="0cc26-116">När du har slutfört alla rader i omvärderingsjournalen väljer du åtgärden **Bokför**.</span><span class="sxs-lookup"><span data-stu-id="0cc26-116">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="0cc26-117">Nya värdetransaktioner skapas nu för att visa omvärderingarna som du har bokfört.</span><span class="sxs-lookup"><span data-stu-id="0cc26-117">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="0cc26-118">Du kan se de nya värdena på respektive artikelkort.</span><span class="sxs-lookup"><span data-stu-id="0cc26-118">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="0cc26-119">Se även</span><span class="sxs-lookup"><span data-stu-id="0cc26-119">See Also</span></span>
[<span data-ttu-id="0cc26-120">Hantera lager</span><span class="sxs-lookup"><span data-stu-id="0cc26-120">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0cc26-121">Hantera försäljning</span><span class="sxs-lookup"><span data-stu-id="0cc26-121">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="0cc26-122">Hantera inköp</span><span class="sxs-lookup"><span data-stu-id="0cc26-122">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="0cc26-123">Arbeta med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0cc26-123">Work With Dynamics NAV</span></span>](ui-work-product.md)

