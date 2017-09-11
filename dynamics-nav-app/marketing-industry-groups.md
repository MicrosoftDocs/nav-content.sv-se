---
title: "Skapa Branschgrupper för kontaktföretag"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 5d0a8f8f8f1e5b50671911d6bfba3da00f2d7ae2
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---
# <a name="set-up-industry-groups-for-contact-companies"></a><span data-ttu-id="f3821-102">Skapa Branschgrupper för kontaktföretag</span><span class="sxs-lookup"><span data-stu-id="f3821-102">Set Up Industry Groups for Contact Companies</span></span>
<span data-ttu-id="f3821-103">Branschgrupper används för att visa vilken bransch kontakterna tillhör, exempelvis detaljhandel eller bilBransch.</span><span class="sxs-lookup"><span data-stu-id="f3821-103">You use industry groups to indicate the type of industry to which your contacts belong, for example, the retail industry or the automobile industry.</span></span>

<span data-ttu-id="f3821-104">Att använda Branschgrupper på kontakter är en två-stegsprocess.</span><span class="sxs-lookup"><span data-stu-id="f3821-104">Using industry groups on contacts is a two-step process.</span></span> <span data-ttu-id="f3821-105">Först definierar du Branschgruppkoden.</span><span class="sxs-lookup"><span data-stu-id="f3821-105">First, you define the industry group code.</span></span> <span data-ttu-id="f3821-106">Du måste bara utföra den här steget en gång för varje Branschgrupp.</span><span class="sxs-lookup"><span data-stu-id="f3821-106">You only have to perform this step one time for each industry group.</span></span> <span data-ttu-id="f3821-107">När du har en Branschgrupp kan du börja koppla koden till kontaktföretag.</span><span class="sxs-lookup"><span data-stu-id="f3821-107">Once you have an industry group code, you can start to assign the code to contact companies.</span></span>

<span data-ttu-id="f3821-108">**Obs!** Om du tänker synkronisera kontakterna med leverantörer, kunder eller bankkonton i andra delar av programmet vill du kanske skapa en affärsrelation för dem.</span><span class="sxs-lookup"><span data-stu-id="f3821-108">**Note:** If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="define-an-industry-group-code"></a><span data-ttu-id="f3821-109">Definiera en Branschgruppskod</span><span class="sxs-lookup"><span data-stu-id="f3821-109">Define an Industry Group Code</span></span>
<span data-ttu-id="f3821-110">Koden för branschgruppen definierar typen eller kategorin för den gruppen, till exempel ANNONS för annonsering eller PRESS för TV och radio.</span><span class="sxs-lookup"><span data-stu-id="f3821-110">The industry group code defines the type or category of the group, such as ADVERT for advertising, or PRESS, for TV and radio.</span></span> <span data-ttu-id="f3821-111">Du kan ha flera branschgruppkoder.</span><span class="sxs-lookup"><span data-stu-id="f3821-111">You can have several industry group codes.</span></span> <span data-ttu-id="f3821-112">För att definiera branschgrupperna använder du fönstret **branschgrupper**.</span><span class="sxs-lookup"><span data-stu-id="f3821-112">To define the industry groups, you use the **Industry Groups** window.</span></span>

1. <span data-ttu-id="f3821-113">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **branschgrupper** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="f3821-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Industry Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="f3821-114">Välj åtgärden **Ny** och fyll i en kod och en beskrivning.</span><span class="sxs-lookup"><span data-stu-id="f3821-114">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="f3821-115">Koden kan bestå av högst 11 tecken, både siffror och bokstäver.</span><span class="sxs-lookup"><span data-stu-id="f3821-115">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="assign-industry-groups-to-a-contact"></a><span data-ttu-id="f3821-116">Så här tilldelar du industrigrupper till en kontakt</span><span class="sxs-lookup"><span data-stu-id="f3821-116">Assign Industry Groups to a Contact</span></span>
<span data-ttu-id="f3821-117">Du kan inte tilldela branschgrupper till en kontaktperson, endast företag.</span><span class="sxs-lookup"><span data-stu-id="f3821-117">You cannot assign industry groups to a contact person - only companies.</span></span>

1. <span data-ttu-id="f3821-118">Öppna kontakten .</span><span class="sxs-lookup"><span data-stu-id="f3821-118">Open the contact.</span></span>
2. <span data-ttu-id="f3821-119">Välj åtgärden **företag** och sedan **branschgrupper**.</span><span class="sxs-lookup"><span data-stu-id="f3821-119">Choose the **Company** action, and then the **Industry Groups** action.</span></span> <span data-ttu-id="f3821-120">Fönstret **Kontakt branschgrupper** öppnas.</span><span class="sxs-lookup"><span data-stu-id="f3821-120">The **Contact Industry Groups** window opens.</span></span>
3. <span data-ttu-id="f3821-121">I fältet **branschgruppkod**, markera den branschgrupp du vill tilldela.</span><span class="sxs-lookup"><span data-stu-id="f3821-121">In the **Industry Groups Code** field, select the industry groups you want to assign.</span></span>

<span data-ttu-id="f3821-122">Upprepa stegen för varje branschgrupp du vill skapa.</span><span class="sxs-lookup"><span data-stu-id="f3821-122">Repeat these steps to assign as many industry groups as you want.</span></span> <span data-ttu-id="f3821-123">Branschgrupper kan också tilldelas i Kontaktlista på samma sätt.</span><span class="sxs-lookup"><span data-stu-id="f3821-123">You can also assign industry groups from the contact list by following the same procedure.</span></span>

<span data-ttu-id="f3821-124">Antalet branschgrupper som du har tilldelat kontakter anges automatiskt i fältet **Antal branschgrupper** på avnisttet **Segmentering** på **Kontakt**-fönstret.</span><span class="sxs-lookup"><span data-stu-id="f3821-124">The number of industry groups that you have assigned to the contact is displayed in the **No. of Industry Groups** field on the **Segmentation** section of the **Contact** window.</span></span>

<span data-ttu-id="f3821-125">När du har tilldelat kontakterna branschgrupper kan du använda dessa uppgifter för urval av kontakter till segmenten.</span><span class="sxs-lookup"><span data-stu-id="f3821-125">After you have assigned industry groups to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="f3821-126">Mer information finns i [Så här lägger du till kontakter i segment](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="f3821-126">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="f3821-127">Se även</span><span class="sxs-lookup"><span data-stu-id="f3821-127">See Also</span></span>
[<span data-ttu-id="f3821-128">Skapa kontaktföretag</span><span class="sxs-lookup"><span data-stu-id="f3821-128">Create Contact Companies</span></span>](marketing-create-contact-companies.md)

