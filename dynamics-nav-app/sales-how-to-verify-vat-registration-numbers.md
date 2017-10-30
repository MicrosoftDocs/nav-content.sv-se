---
title: "Gör så här: Kontrollera momsregistreringsnummer"
description: "Du kan använda en EU-webbtjänst för att kontrollera att de momsregistreringsnummer som du anger på kund-, leverantörs- eller kontaktkort är giltiga."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8ed345e346ba32a38ebb2738afbe6c12749842ff
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-verify-vat-registration-numbers"></a><span data-ttu-id="5f578-103">Gör så här: Kontrollera momsregistreringsnummer</span><span class="sxs-lookup"><span data-stu-id="5f578-103">How to: Verify VAT Registration Numbers</span></span>
<span data-ttu-id="5f578-104">Du kan använda en EU-webbtjänst för att kontrollera att de momsregistreringsnummer som du anger på kund-, leverantörs- eller kontaktkort är giltiga.</span><span class="sxs-lookup"><span data-stu-id="5f578-104">You can use an EU web service to verify that VAT registration numbers that you enter on customer, vendor, or contact cards are valid.</span></span>  

 <span data-ttu-id="5f578-105">När du ändrar fältet **Momsregistreringsnummer** på ett kort där värdet i **Land-/regionskod** är ett EU-land/-region loggas sedan det nya momsregistreringsnumret och ditt användar-ID i fönstret **Momsregistreringslogg**.</span><span class="sxs-lookup"><span data-stu-id="5f578-105">When you modify the **VAT Registration No.** field on a card where the value in the **Country/Region Code** field is an EU country/region, then the new VAT registration number and your user ID are logged in the **VAT Registration Log** window.</span></span> <span data-ttu-id="5f578-106">Du validerar ett momsregistreringsnummer genom att välja knappen **Kontrollera registreringsnr** i fönstret **momsregistreringslogg**.</span><span class="sxs-lookup"><span data-stu-id="5f578-106">You verify a VAT registration number by choosing the **Verify Registration No.** button in the **VAT Registration Log** window.</span></span> <span data-ttu-id="5f578-107">En ny rad skapas varje gång du använder verifikationsfunktionen.</span><span class="sxs-lookup"><span data-stu-id="5f578-107">A new line is created every time you use the verification function.</span></span> <span data-ttu-id="5f578-108">Om numret kan verifieras innehåller fältet **Status** **Giltigt**.</span><span class="sxs-lookup"><span data-stu-id="5f578-108">If the number could be verified, the **Status** field contains **Valid**.</span></span> <span data-ttu-id="5f578-109">Om numret inte kan verifieras innehåller fältet **Status** **Ogiltig** och du måste då ändra numret i fältet **Momsregistreringsnr** på kortet och starta verifikationsfunktionen igen.</span><span class="sxs-lookup"><span data-stu-id="5f578-109">If the number could not be verified, the **Status** field contains **Invalid**, and you must then change the number in the **VAT Registration No.** field on the card and start the verification function again.</span></span>  

 <span data-ttu-id="5f578-110">Webbadressen för standardwebbtjänsten ställs in i fältet **Validerings-URL för momsreg.nr** i fönstret **Redovisningsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="5f578-110">The URL of the default web service is set up in the **VAT Reg. No. Validation URL** field in the **General Ledger Setup** window.</span></span>  

 <span data-ttu-id="5f578-111">I tabellen **Momsregistreringsnr format** kan du för varje land/region ändra de olika format för momsregistreringsnummer som användare tillåts ange i fältet **Momsregistreringsnr**.</span><span class="sxs-lookup"><span data-stu-id="5f578-111">In the **VAT Registration No. Format** table, you can change for each country/region the different formats of VAT registration number that users are allowed to enter in the **VAT Registration No.** field.</span></span>  

> [!WARNING]  
>  <span data-ttu-id="5f578-112">Den här webbtjänsten använder http-protokoll, vilket betyder att data som har överförts via tjänsten inte har krypteras.</span><span class="sxs-lookup"><span data-stu-id="5f578-112">This web service uses the http protocol, which means that data transferred through the service is not encrypted.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5f578-113">Du kan drabbas av stilleståndstid, vilket inte är Microsofts ansvar, för den här tjänsten eftersom den ingår i ett omfattande EU-nätverk av nationella mervärdeskattregister.</span><span class="sxs-lookup"><span data-stu-id="5f578-113">You may experience downtime for this service for which Microsoft is not responsible, as the service is part of a broad EU network of national VAT registers.</span></span>  

## <a name="to-verify-a-vat-registration-number-from-a-customer-card"></a><span data-ttu-id="5f578-114">Så här verifierar du ett momsregistreringsnummer från ett kundkort</span><span class="sxs-lookup"><span data-stu-id="5f578-114">To verify a VAT registration number from a customer card</span></span>  
<span data-ttu-id="5f578-115">Nedan beskrivs hur du kontrollerar momsregistreringsnummer för en kund.</span><span class="sxs-lookup"><span data-stu-id="5f578-115">The following describes how to verify a VAT registration number for a customer.</span></span> <span data-ttu-id="5f578-116">Momenten är liknande för en leverantör och en kontakt.</span><span class="sxs-lookup"><span data-stu-id="5f578-116">The steps are similar for a vendor and a contact.</span></span>   
1.  <span data-ttu-id="5f578-117">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kunder** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="5f578-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="5f578-118">Öppna kortet för en kund du vill kontrollera momsregistreringsnumret för.</span><span class="sxs-lookup"><span data-stu-id="5f578-118">Open the card of a customer where you want to verify the VAT registration number.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="5f578-119">Fältet **Lands-/regionkod** på kundkortet måste innehålla ett land/en region i EU.</span><span class="sxs-lookup"><span data-stu-id="5f578-119">The **Country/Region Code** field on the customer card must contain an EU country/region.</span></span>  
3.  <span data-ttu-id="5f578-120">På snabbfliken **Fakturering** väljer du knappen **Momsregistreringsnr**.</span><span class="sxs-lookup"><span data-stu-id="5f578-120">On the **Invoicing** FastTab, choose the DrillDown button next to the **VAT Registration No.** field.</span></span>  

    <span data-ttu-id="5f578-121">Fönstret **Momsregistreringslogg** öppnas och visar en rad där fältet **Status** innehåller **Ej verifierad**.</span><span class="sxs-lookup"><span data-stu-id="5f578-121">The **VAT Registration Log** window opens showing one line where the **Status** field contains **Not Verified**.</span></span>  
4.  <span data-ttu-id="5f578-122">Välj åtgärd **Kontrollera registreringsnr**.</span><span class="sxs-lookup"><span data-stu-id="5f578-122">Choose the **Verify Registration No.** action.</span></span>  

     <span data-ttu-id="5f578-123">En ny rad skapas när fältet **Status** antingen innehåller **Giltigt** eller **Ogiltigt**.</span><span class="sxs-lookup"><span data-stu-id="5f578-123">A new line is created where the **Status** field contains either **Valid** or **Invalid**.</span></span>  
5.  <span data-ttu-id="5f578-124">Om fältet **Status** innehåller **Ogiltig**, ändrar du numret i fältet **Momsregistreringsnr.** på kortet och upprepar sedan steg 3 till 4.</span><span class="sxs-lookup"><span data-stu-id="5f578-124">If the **Status** field contains **Invalid**, change the number in the **VAT Registration No.** field on the card, and then repeat steps 3 through 4.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5f578-125">Se även</span><span class="sxs-lookup"><span data-stu-id="5f578-125">See Also</span></span>  
[<span data-ttu-id="5f578-126">Ekonomi</span><span class="sxs-lookup"><span data-stu-id="5f578-126">Finance</span></span>](finance.md)  
[<span data-ttu-id="5f578-127">Så här registrerar du nya kunder</span><span class="sxs-lookup"><span data-stu-id="5f578-127">How to: Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="5f578-128">Så här registrerar du nya leverantörer</span><span class="sxs-lookup"><span data-stu-id="5f578-128">How to: Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
<span data-ttu-id="5f578-129">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5f578-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

