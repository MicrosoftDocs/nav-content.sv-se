---
title: "Automatisk överföring och kombinerade transaktioner"
description: "I kostnadsredovisningen kan du överföra redovisningstransaktioner till en kostnadstyp, genom att använda en kombinerad bokföring. Du kan ange om en kostnadstyp tar emot kombinerade transaktioner i fältet **Kombinera transaktioner** i kostnadstypsdefinitionen. Alternativen beskrivs i tabellen nedan."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 638fc123d4113695d70102a94b9fce0bff6b43fa
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="automatic-transfer-and-combined-entries"></a>Automatisk överföring och kombinerade transaktioner
I kostnadsredovisningen kan du överföra redovisningstransaktioner till en kostnadstyp, genom att använda en kombinerad bokföring. Du kan ange om en kostnadstyp tar emot kombinerade transaktioner i fältet **Kombinera transaktioner** i kostnadstypsdefinitionen. Alternativen beskrivs i tabellen nedan.  

|Kombinera transaktioner|Beskrivning|  
|---------------------|-----------------|  
|Ingen|Varje redovisningstransaktion överförs individuellt till motsvarande kostnadstyp.|  
|Dag|Redovisningstransaktioner med samma bokföringsdatum överförs som en post till motsvarande kostnadstyp.|  
|Månad|Alla redovisningstransaktioner i samma kalendermånad överförs som en post till motsvarande kostnadstyp.|  

> [!IMPORTANT]  
>  Om du har markerat kryssrutan **Automatisk överföring från redovisning** i fönstret **Inställningar för kostnadsredovisning**, [!INCLUDE[d365fin](includes/d365fin_md.md)] uppdaterar kostnadsredovisningen efter varje bokföring i redovisningen. Kombinerade transaktioner är inte möjliga.  

## <a name="see-also"></a>Se även  
 [Så här: Överföra redovisningstransaktioner till kostnadstransaktioner](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
 [Villkor för överföring av redovisningstransaktioner till kostnadstransaktioner](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
 [Resultat av överföringen](finance-results-of-the-transfer.md)   
 [Överföra och bokföra kostnadstransaktioner](finance-transfer-and-post-cost-entries.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

