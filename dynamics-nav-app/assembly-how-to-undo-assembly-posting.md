---
title: "Så här: Ångra monteringbokning"
description: "Ibland kan du behöva ångra en bokförd monteringsorder, t.ex då ordern har bokförts med ett misstag som måste rättas, eller eftersom det inte bör både ha bokförts i första omgången och måste återställas."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3ba93dd182aa1591f5d24398d4b749942d38bb4b
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-undo-assembly-posting"></a>Så här: Ångra monteringbokning
Ibland kan du behöva ångra en bokförd monteringsorder, t.ex då ordern har bokförts med ett misstag som måste rättas, eller eftersom det inte bör både ha bokförts i första omgången och måste återställas.

När du återställer en bokförd monteringsorder, skapas en uppsättning korrigerande artikeltransaktioner för att återföra de ursprungliga transaktionerna. Varje positivt utflödestransaktion för monteringsartikeln återförs av en negativ utflödestransaktion. Varje negativ förbrukningstransaktion för en monteringskomponent återförs av en positiv förbrukningstransaktion. Fast kostnad-koppling skapas automatiskt mellan korrigerande och ursprungliga transaktionerna som visas för att garantera exakt kostnadsåterställning.  

När du helt återställer en bokförd monteringsorder, kan du välja att skapa monteringsorder på nytt till den ursprungliga statusen, till exempel för att göra korrigeringar, innan du ombokför det. Du kan också välja att inte skapa monteringsorder på nytt.  

När du återställer delvis bokförda monteringsorder, påverkas alla antalfält, till exempel **Monterad kvantitet**, **Förbrukat antal** och **Återstående antal**, som återställs till värdena de hade innan bokföringen i fråga.  

Om du skapar om eller återställer monteringsorder, följande villkor måste gälla för monteringsartikeln som tillverkades i den ursprungliga bokföring:  

-   Den återstår ändå finnas i lager, d.v.s, det är inte sålt eller förbrukat av avgående transaktioner.  
-   Det får inte reserveras.  
-   Det måste finnas på lagerplatsen som den tillverkades till.  

Dessutom kan befintliga monteringsorder endast återställs, om antalet rader och sekvensen av rader på den ursprungliga monteringsorder inte ändras.  

> [!TIP]  
>  För att lösa konflikter på grund av radändringar, kan du manuellt återföra ändringar på raderna i fråga, innan du återställer den relaterade bokförda monteringsorder. Alternativt kan du bokföra monteringsorder fullständigt och sedan välja att skapa den på nytt, när du ångra bokföringen.  

Nedan beskrivs hur du återställ bokförda monteringsorder där artiklar monteras mot lager. Om du vill ångra bokförda monteringsorder där artiklar monteras till en försäljningsorder, måste du använda **Återställ utleverans** funktionen på en bokförd utleverans som avser bokförda monteringsorder. Mer information finns i [Så hör: Återföra bokföringar](finance-how-reverse-journal-posting.md). Ångra av den bokförda monteringsordern sker sedan automatiskt på samma sätt som beskrivs i det här avsnittet.  

## <a name="to-undo-posting-of-an-assembly-order"></a>Om du vill ångra bokföring av en monteringsorder  
1.  Om du vill ångra en helt eller delvis bokförd monteringsorder, väljer du ikonen ![Sök efter sidan eller rapporten](media/ui-search/search_small.png "ikonen Sök efter sidan eller rapporten"), anger **Bokförda monteringsorder** och väljer sedan relaterad länk.  

    **Bokförda monteringsorder** fönstret öppnas med en eller flera bokförda monteringsorder som bokförts från monteringsorder i fråga. Varje delbokföringstyp skapar en separat bokförda monteringsorder.  
2.  Öppna den bokförda monteringsordern som du vill ångra och välj sedan åtgärden **Ångra montering**.  

    Om den bokförda monteringsorder som du vill ångra, avser helt en bokförd monteringsorder som tas bort nu, får du välja att skapa den på nytt, vanligtvis, eftersom du vill process den igen.  
3.  Om du vill skapa monteringsorder på nytt, välj **ja** knappen. Välj **nej** om du vill ångra bokföringen, utan att skapa den kopplade monteringsordern på nytt.  

Fältet **Återförd** på monteringsorderhuvudet ändras till **Ja**. Monteringsorderbokföringen återförs nu, och du kan fortsätta att bearbeta hela monteringsordern, om du har valt att skapa den på nytt, eller den öppna monteringsorder som du har återställt till den ursprungliga status.  

> [!NOTE]  
>  Om du vill återställa antal från flera delbokföringar i en monteringsorder måste du ångra alla bokförda monteringsorder i fråga genom att följa steg 1 till 3 ovan för varje bokförd monteringsorder.  

## <a name="see-also"></a>Se även  
[Monteringshantering](assembly-assemble-items.md)  
[Så här: Återföra en bokning](finance-how-reverse-journal-posting.md)  
[Så här behandlar du försäljningreturer eller annulleringar](sales-how-process-sales-returns-cancellations.md)    
[Så här arbetar du med strukturer](inventory-how-work-BOMs.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

