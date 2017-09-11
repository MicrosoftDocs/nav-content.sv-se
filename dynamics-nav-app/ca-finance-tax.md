---
title: "Omsättningsskatt och moms på varor och tjänster i Kanada"
author: edupont04
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c032a02b545441b927ef5c4facc9f77731f37ab7
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a><span data-ttu-id="0363f-102">Omsättningsskatt och moms på varor och tjänster i Kanada</span><span class="sxs-lookup"><span data-stu-id="0363f-102">Sales Tax and Goods and Services Tax in Canada</span></span>
<span data-ttu-id="0363f-103">I Kanada när en leverantör inte har en företagsnärvaro i regionen som inköpet görs i, debiteras leverantören endast för moms på varor och tjänster (GST) eller harmoniserad försäljningsmoms HST).</span><span class="sxs-lookup"><span data-stu-id="0363f-103">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span></span> <span data-ttu-id="0363f-104">Men om landskapet har en provinsiell omsättningsskatt (PST), måste köparen fortfarande beräkna PST och betala den direkt till regionen.</span><span class="sxs-lookup"><span data-stu-id="0363f-104">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span></span> <span data-ttu-id="0363f-105">När en skatteområdeskod för regionen markeras använder Dynamics NAV den för att beräkna PST och bokföra den så att det finns en skatteskuld både i redovisningen och i skattetransaktionsposten.</span><span class="sxs-lookup"><span data-stu-id="0363f-105">When a Provincial Tax Area Code is selected, Dynamics NAV uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span></span> <span data-ttu-id="0363f-106">Därför bör skatteområdeskoden som markeras här vara en med endast PST och inte GST.</span><span class="sxs-lookup"><span data-stu-id="0363f-106">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span></span>  
<span data-ttu-id="0363f-107">Mer information om omsättningsskatt finns i [Omsättningsskatt och skattegrupper i USA och Kanada](us-finance-setup-sales-tax.md).</span><span class="sxs-lookup"><span data-stu-id="0363f-107">For more information about sales tax, see [Sales Tax and Tax Groups in the US and Canada](us-finance-setup-sales-tax.md).</span></span>  

## <a name="submitting-the-gsthst-file"></a><span data-ttu-id="0363f-108">Skicka GST-/HST-filen</span><span class="sxs-lookup"><span data-stu-id="0363f-108">Submitting the GST/HST File</span></span>
<span data-ttu-id="0363f-109">Skatteinformationen i inköpsdokument används för att generera en GST-/HST-internetfilöverföring som du måste tillhandahålla till skattemyndigheterna.</span><span class="sxs-lookup"><span data-stu-id="0363f-109">The tax information in purchase documents is used to generate a GST/HST internet file transfer that you must  provided to the tax authorities.</span></span> <span data-ttu-id="0363f-110">Den här filen inkluderar moms för varor och tjänster (GST) och harmoniserad försäljningsmoms HST).</span><span class="sxs-lookup"><span data-stu-id="0363f-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span></span> <span data-ttu-id="0363f-111">Arkivet skapas i ett .tax-filformat, som kan överföras via internet.</span><span class="sxs-lookup"><span data-stu-id="0363f-111">The file is created in a .tax file format, which can be transferred via the internet.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0363f-112">Se även</span><span class="sxs-lookup"><span data-stu-id="0363f-112">See Also</span></span>
[<span data-ttu-id="0363f-113">Finans</span><span class="sxs-lookup"><span data-stu-id="0363f-113">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="0363f-114">Konfigurera Ekonomi</span><span class="sxs-lookup"><span data-stu-id="0363f-114">Set Up Finance</span></span>](finance-setup-setup-finance-setup.md)  
[<span data-ttu-id="0363f-115">Omsättningsskatt och momsgrupper i USA och Kanada</span><span class="sxs-lookup"><span data-stu-id="0363f-115">Sales Tax and Tax Groups in the US and Canada</span></span>](us-finance-setup-sales-tax.md)

