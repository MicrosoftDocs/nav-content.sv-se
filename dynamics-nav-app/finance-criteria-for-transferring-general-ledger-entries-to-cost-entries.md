---
title: "Villkor för överföring av redovisningstransaktioner till kostnadstransaktioner"
description: "Det är viktigt att förstå kriterier för överföring av redovisningstransaktioner mot kostnadstransaktioner. Under överföringen använder batchjobbet **Överför redovisningstransaktioner** till kostnadsredovisning följande kriterier för att bestämma om och hur redovisningstransaktionerna överförs."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 99b18cee56b6300cb1852265eed6d56206a2eaab
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="criteria-for-transferring-general-ledger-entries-to-cost-entries"></a>Villkor för överföring av redovisningstransaktioner till kostnadstransaktioner
Det är viktigt att förstå kriterier för överföring av redovisningstransaktioner mot kostnadstransaktioner. Under överföringen använder batchjobbet **Överför redovisningstransaktioner till kostnadsredovisning** följande kriterier för att bestämma om och hur redovisningstransaktionerna överförs.  

Redovisningstransaktioner överförs om:  

-   Transaktionerna har dimensionsvärden som motsvarar antingen ett kostnadsställe eller en kostnadsbärare.  
-   Transaktionerna har dimensionsvärden som motsvarar ett kostnadsställe och en kostnadsbärare. För dessa verifikationer har kostnadsstället prioritet. Det gör att det går att undvika en situation där en kostnadstyp visas både i en kostnadsbärare och ett kostnadsställe och därigenom räknas två gånger i statistiken.  
-   Verifikationsnumret i transaktionerna är tomt, så att visas med verifikationsnumret 0000 i kostnadstransaktionerna.  
-   Transaktionerna överförs till en kostnadstyp som används för kombinerade transaktioner, och dessa transaktioner överförs som en kombinerad transaktionen antingen månatligt eller dagligen.  

Redovisningstransaktioner överförs inte om:  

-   Transaktionerna har dimensionsvärden som inte motsvarar ett kostnadsställe eller en kostnadsbärare.  
-   Transaktionerna har ett belopp på noll.  
-   Transaktionerna har ett redovisningskonto som har tagits bort.  
-   Transaktionerna har ett redovisningskonto som inte är av typen **Resultaträkning**.  
-   Transaktionerna har ett redovisningskonto som inte har kopplats till en kostnadstyp.  
-   Transaktionerna har ett bokföringsdatum före startdatum för **Startdatum för överföring till redovisning**.  
-   Transaktionerna har bokförts med ett stängningsdatum. Dessa är vanliga transaktioner som nollställer saldot i resultaträkningen i slutet av året.  

## <a name="see-also"></a>Se även  
[Redovisa kostnader](finance-manage-cost-accounting.md)  
 [Så här: Överföra redovisningstransaktioner till kostnadstransaktioner](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
 [Överföra och bokföra kostnadstransaktioner](finance-transfer-and-post-cost-entries.md)   
 [Om kostnadsredovisning](finance-about-cost-accounting.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

