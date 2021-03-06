---
title: "Ange layouten för en kontroll"
description: "Du kan skapa och skriva ut dina checkar i flera olika format i överensstämmelse med standarder."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 06/15/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d99326be66bf16a4a756d9f78e11f9af37e11fbd
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-define-check-layouts"></a>Så här definierar du checklayouter
Du kan designa dina checkar så att de uppfyller de normer som fastställts av de lokala myndigheterna. Checkbilder kan vara skrivna ut på engelska, franska, eller spanska.

Checkar har utformats för att skrivas ut i både amerikanska och kanadensiska checkbildformat i antingen check-checktalong-check-format eller checktalong-checktalong-check-format.

## <a name="to-define-check-layouts"></a>Om du vill definiera checklayouter
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Rapportval - bankkonto** och välj sedan relaterad länk.
2. I fönstret **Rapportval - bankkonto** i fältet **Användning** väljer du **Check**.
3. Välj något av följande rapport-ID:

| Rapport-ID | Rapportnamn | Beskrivning |
| --- | --- | --- |
| 1401 |Check |Detta är standardrapporten. |
| 10401 |Check (checktalong/checktalong/check) |Den här rapporten är utformad för att skriva ut checkar i formatet checktalong/checktalong/check. |
| 10411 |Check (checktalong/check/checktalong) |Den här rapporten är utformad för att skriva ut checkar i formatet check/checktalong/check. |

När du har upprättat checklayouter, kan du skriva ut checkar från fönstret **utbetalningsjournal**. Mer information finns i [Så här arbetar du med checkar](payables-how-work-checks.md).

## <a name="see-also"></a>Se även
[Hantera Leverantörsreskontra](payables-manage-payables.md)  
[Hantera bankkonton](bank-manage-bank-accounts.md)   
[Slutföra periodslutsprocesser](year-how-complete-period-end-processes.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Allmänna affärsfunktioner](ui-across-business-areas.md)

