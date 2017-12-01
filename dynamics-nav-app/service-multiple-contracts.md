---
title: Flera kontrakt
description: "Beroende på dina servicenivåavtal med en kund kan du bli tvungen att hantera en serviceartikel på fler än ett servicekontrakt."
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
ms.openlocfilehash: ecb02a00a23f183dfa5fa34e1aba8d5fe899f069
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="multiple-contracts"></a>Flera kontrakt
Beroende på dina servicenivåavtal med en kund kan du bli tvungen att hantera en serviceartikel på fler än ett servicekontrakt.  
  
Genom att hantera en serviceartikel i flera kontrakt, kan du göra följande:  
  
* Utfärda olika kontrakt för samma serviceartikel.  
* Utföra service på olika delar separat.  
* Ta hänsyn till vilka behov som krävs för att utföra service på en serviceartikel, till exempel olika mekaniska komponenter och mjukvara.  
* Specificera olika svarstider och frekvenser för service på olika delar av en serviceartikel.  
* Hantera olika typer av aktiviteter som ska utföras på en serviceartikel när den kräver olika typer av service vid olika tidpunkter.  
* Välja och tilldela en serviceartikelrad ett korrekt kontraktsnummer när du skapar en serviceorder.  
* Hantera relevant ekonomisk information för serviceartiklar och servicenivåavtal.  
  
Titta på följande exempel som visar hur du kan använda funktionen för flera kontrakt.  
  
## <a name="creating-multiple-contracts-per-service-item"></a>Skapa flera kontrakt per serviceartikel  
Du kan manuellt skapa ett servicekontrakt eller en kontraktsoffert för serviceartiklar som redan har registrerats i icke-annullerade kontrakt som ägs av samma kund. Följ standardprocessen där du skapar servicekontrakt och servicekontraktsofferter om du vill göra detta. Mer information finns i [så här: arbeta med servicekontrakt och servicekontraktsofferter](service-how-to-create-service-contracts-and-service-contract-quotes.md).  
  
När du lägger till en serviceartikel på en kontraktsrad som är registrerad i andra servicekontrakt eller kontraktsofferter, visas ett varningsmeddelande med texten att serviceartikeln redan tillhör ett eller flera servicekontrakt eller kontraktsofferter. Om du bekräftar meddelandet kommer all relevant serviceartikelinformation att kopieras till en ny kontraktsrad.  
  
## <a name="copying-documents"></a>Kopiera dokument  
Du kan automatiskt skapa ett servicekontrakt eller en kontraktsoffert för serviceartiklar som redan har registrerats i andra servicekontrakt eller kontraktsofferter med hjälp av åtgärden **Kopiera dokument**.  
  
## <a name="creating-service-orders-for-multiple-contracts"></a>Skapa serviceorder för flera kontrakt  
Du kan skapa en serviceorder manuellt för en serviceartikel som är registrerad i flera aktiva kontrakt. Ett servicekontrakt är aktivt när det är signerat och inte utgånget.  
  
## <a name="see-also"></a>Se även  
[Uppfylla servicekontrakt](service-fulfill-service-contracts.md)  
[Så här skapar du serviceorder](service-how-to-create-service-orders.md)  

