---
title: "Så här importerar och exporterar du data i SIE-format (Standard Import Export)"
description: Du kan importera och exportera redovisningsdata i SIE-format (Standard Import Export).
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 970ceede1d3619b9d7994a408baaec28f758ac6b
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-import-and-export-data-in-standard-import-export-format"></a>Så här importerar och exporterar du data i SIE-format (Standard Import Export)
Du kan importera och exportera redovisningsdata i SIE-format (Standard Import Export). Genom att ange SIE-dimensioner och -filtyper kan du ange vilken detaljnivå import- eller exporttransaktionerna ska ha. Mer information finns i [SIE-grupp](http://go.microsoft.com/fwlink/?LinkID=164870&clcid=0x41d).  

## <a name="to-import-data-in-sie-format"></a>Så här importerar du data i SIE-format  

1.  Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **SIE-import** och välj sedan relaterad länk.  
2.  Fyll i fälten enligt beskrivningen i följande tabell.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Filnamn**|Ange namnet på och sökvägen till filen du vill importera.|  
    |**Redovisningsjournalmall**|Välj en redovisningsjournalmall.|  
    |**Redovisningsjournal**|Välj en redovisningsjournal.|  
    |**Dimensioner**|Markera SIE-dimensionerna du vill importera.|  
    |**Infoga redovisningskonto**|Välj det här alternativet om redovisningskontot i importfilen saknas i kontoplanen och måste skapas under importprocessen.|  
    |**Använd nummerserie för dok.nr**|Välj det här alternativet om det inte finns något dokumentnummer i importfilen.|  

3.  Välj **OK**.  

## <a name="to-export-data-in-sie-format"></a>Så här exporterar du data i SIE-format  

1.  Välj ikonen ![Söka efter sida eller rapport](../../media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **SIE-import** och välj sedan relaterad länk.  
2.  Välj lämpliga filter på snabbfliken **Redovisningskonto**.  
3.  Fyll i fälten enligt beskrivningen i följande tabell på snabbfliken **Alternativ**.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Filtyp**|Välj typen av fil du vill skapa. Välj något av följande alternativ:<br /><br /> -   **År - Slutsaldon** - Innehåller årligt utgående saldo för alla konton i kontoplanen.<br />-   **Periodiska saldon** - Innehåller årligt utgående saldo och månatliga förändringar för alla konton i kontoplanen.<br />-   **Objektsaldon** - Innehåller årligt utgående kontosaldo, månatliga förändringar och saldon på objektnivån, till exempel kostnadsenheter och projekt, för alla konton i kontoplanen.<br />-   **Transaktioner** - Innehåller alla redovisningstransaktioner för perioden.|  
    |**Filnamn**|Ange namnet på och sökvägen till filen du vill skapa.|  
    |**Kontakt**|Ange kontaktperson. Fältet är ett tillval.|  
    |**Kommentarer**|Beskriv filens innehåll.|  
    |**Dimensioner**|Markera dimensionerna du vill exportera.|  
    |**Räkenskapsår**|Ange räkenskapsåret.|  

4.  Välj knappen **OK**.  

## <a name="see-also"></a>Se även  
 [SIE-grupp](http://go.microsoft.com/fwlink/?LinkID=164870&clcid=0x41d)   
 [Lokal funktionalitet för Sverige](sweden-local-functionality.md)

