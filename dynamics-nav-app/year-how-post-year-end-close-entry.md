---
title: "Så här bokför du årsslutstransaktionen"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a8fdb459a2b98066bb93bb47cc0bd9721b992d94
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---
# <a name="how-to-post-year-end-closing-entry"></a>Så här bokför du årsslutstransaktionen
Som en del av att avsluta böckerna för ett räkenskapsår kommer du att köra batch-jobbet och flyttaöver årets resultat flyttas till ett konto i balansräkningen och avsluta resultaträkningskontona. När du har kört batch-jobbet Avslut av resultatkonton måste du öppna den journal du har angett i batch-jobbet och sedan granska och bokföra transaktionerna.

## <a name="to-post-the-year-end-closing-entry"></a>Så här bokför du årsslutstransaktionen
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournal** och välj sedan relaterad länk.
2. I fönstret **Redovisningsjournal** i fältet **Batch-namn** väljer du den batch som innehåller årsavslutstransaktionerna.
3. Granska transaktionerna.
4. Om du vill bokföra journalen väljer du åtgärden **Bokför**.

**Obs!** Om ett fel påträffas visas ett felmeddelande. Om bokföringen utförs tas de bokförda transaktionerna bort från journalen. Efter bokföringen bokförs en transaktion på varje resultatkonto så att saldot blir noll och årets resultat överförs till balansräkningen.

## <a name="see-also"></a>Se även
[Avsluta böcker](year-close-books.md)  
[Avslut av resultatkonton](year-close-income-statement.md)  
[Så här avslutar du bokföringsperioder](year-close-account-periods.md)  
