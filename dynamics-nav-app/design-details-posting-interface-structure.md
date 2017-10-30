---
title: "Designdetaljer - Bokföringsgränssnittsstruktur"
description: "Det här avsnittet innehåller en översikt över de globala procedurerna i bokföringsgränssnittsstruktur."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cc5efca8087bc24ab988ae592a9ba60e4caf46bb
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="de35c-103">Designdetaljer: Bokföringsgränssnittsstruktur</span><span class="sxs-lookup"><span data-stu-id="de35c-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="de35c-104">I gränssnittstrukturen för bokföring i [!INCLUDE[d365fin](includes/d365fin_md.md)] finns det flera globala processer som använder samma struktur:</span><span class="sxs-lookup"><span data-stu-id="de35c-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="de35c-105">RunWithCheck och RunWithoutCheck anropar procedurkod – generiskt bokföringsgränssnitt för standardredovisningsjournalrad.</span><span class="sxs-lookup"><span data-stu-id="de35c-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span></span>  
* <span data-ttu-id="de35c-106">CustPostApplyCustLedgEntry – bokför kundapplikation, anropad från kodmodul 226 CustEntry - koppla bokförda transaktioner.</span><span class="sxs-lookup"><span data-stu-id="de35c-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="de35c-107">VendPostApplyVendLedgEntry – bokför koppling av leverantörsapplikation, anropad från kodmodul 227 VendEntry – koppla bokförda transaktioner.</span><span class="sxs-lookup"><span data-stu-id="de35c-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="de35c-108">UnapplyCustLedgEntry – bokför borttagning av koppling av kundapplikation, anropad från kodmodul 226 CustEntry - koppla bokförda transaktioner</span><span class="sxs-lookup"><span data-stu-id="de35c-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="de35c-109">UnapplyVendLedgEntry – bokför borttagning av koppling av leverantörsapplikation, anropad från kodmodul 227 VendEntry - koppla bokförda transaktioner</span><span class="sxs-lookup"><span data-stu-id="de35c-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="de35c-110">Se även</span><span class="sxs-lookup"><span data-stu-id="de35c-110">See Also</span></span>  
[<span data-ttu-id="de35c-111">Designdetaljer: Bokföringsmotorstruktur</span><span class="sxs-lookup"><span data-stu-id="de35c-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)
