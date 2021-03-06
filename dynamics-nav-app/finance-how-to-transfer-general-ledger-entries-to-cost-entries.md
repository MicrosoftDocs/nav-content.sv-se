---
title: "Så här: Överföra redovisningstransaktioner till kostnadstransaktioner"
description: "Du kan överföra redovisningstransaktioner till kostnadstransaktioner."
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
ms.openlocfilehash: b7a78fb1023e8b664fd866eb1a8b5e42ff0de265
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-transfer-general-ledger-entries-to-cost-entries"></a>Så här: Överföra redovisningstransaktioner till kostnadstransaktioner
Du kan överföra redovisningstransaktioner till kostnadstransaktioner.  

Innan du kör processen för att överföra redovisningstransaktioner till kostnadstransaktioner, måste du förbereda överföringen för att undvika manuella rättningsbokföringar.  

## <a name="to-prepare-the-transfer"></a>Så här förbereder du överföringen  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inställningar för kostnadsredovisning** och välj sedan relaterad länk.  
2.  I fönstret **Inställningar för kostnadsredovisning** kontrollerar du att fältet **startdatum för överföring till redovisning** anges till rätt värde.  
3.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lista över kostnadstyper** och välj sedan relaterad länk.  
4.  I fönstret **Kostnadstypkort** kontrollerar du att fältet **Redovisningskontointervall** är korrekt länkat för alla kostnadstyper som tar transaktioner från redovisningen.  
5.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kontoplan** och välj sedan relaterad länk.  
6.  För varje relevant redovisningskonto i fönstret **Redovisningskontokort** kontrollerar du att fältet **Kostnadstypsnr.** är korrekt länkat till en kostnadstyp. För mer information, se [Definiera relationen mellan kostnadstyper och redovisningskonton](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)  
7.  Kontrollera att alla relevanta redovisningstransaktioner har dimensionsvärden som motsvarar ett kostnadsställe och en kostnadsbärare.  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a>Så här överför du redovisningstransaktioner till kostnadstransaktioner  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Överför redovisningstransaktioner till kostnadsredovisning** och välj sedan relaterad länk.  
2.  Välj **Ja** för att starta överföringen. Processen överför alla redovisningstransaktioner som inte redan har överförts.  

    Under överföringen skapar processen anslutningar i transaktionerna i tabellerna **Kostnadstransaktion** och **Bokförd journal för kostnad**. Det gör det möjligt att spåra ursprunget till kostnadstransaktionerna.  

## <a name="see-also"></a>Se även  
 [Villkor för överföring av redovisningstransaktioner till kostnadstransaktioner](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
 [Automatisk överföring och kombinerade transaktioner](finance-automatic-transfer-combined-entries.md)   
 [Resultat av överföringen](finance-results-of-the-transfer.md)   
 [Överföra och bokföra kostnadstransaktioner](finance-transfer-and-post-cost-entries.md)   
 [Definiera relationen mellan kostnadstyper och redovisningskonton](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   

