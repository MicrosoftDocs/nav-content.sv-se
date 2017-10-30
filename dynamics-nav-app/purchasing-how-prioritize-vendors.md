---
title: "Tilldela en leverantör till en prioritetsnivå"
description: "Du kan tilldela nummer till leverantörer eller för att prioritera dem och underlätta betalningsförslag i Dynamics NAV."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 79458c1372c9f696a8331f2e7c83179dd42fb905
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-prioritize-vendors"></a>Så här prioriterar du leverantörer
[!INCLUDE[d365fin](includes/d365fin_md.md)] används för att ta fram olika betalningsförslag, t.ex. betalningar som snart förfaller eller betalningar för vilka en rabatt kan erhållas. Mer information finns i [Så här föreslår du leverantörsbetalningar](payables-how-suggest-vendor-payments.md).

Först måste du prioritera leverantörerna genom att tilldela nummer till dem.

## <a name="to-prioritize-vendors"></a>Så här prioriterar du leverantörer:
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Leverantör** och välj sedan relaterad länk.
2. Välj lämplig leverantör och sedan **Redigera**.
3. Ange ett nummer i fältet **Prioritet**.

I [!INCLUDE[d365fin](includes/d365fin_md.md)] räknas lägst nummer (förutom 0) som högst prioritet. Om du t.ex. använder 1, 2 och 3 har alltså 1 högst prioritet.

Om du inte vill prioritera en leverantör lämnar du fältet **Prioritet** tomt. Om du sedan använder funktionen för betalningsförslag visas den här leverantören sist i listan, efter de leverantörer som har tilldelats ett prioritetsnummer. Du kan ange valfritt antal prioritetsnivåer alltefter behov.

## <a name="see-also"></a>Se även
[Ställa in inköp](purchasing-setup-purchasing.md)  
[Hantera Leverantörsreskontra](payables-manage-payables.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

