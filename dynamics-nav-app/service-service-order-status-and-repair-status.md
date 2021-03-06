---
title: Serviceorderstatus och reparationsstatus
description: "Fältet **Status** i fönstret **Serviceorder** och serviceartikelns reparationsstatus som visas i fältet **Reparationsstatuskod** i fönstret **Serviceorder** har ett visst samband i modulen Servicehantering. Serviceorderstatus visar reparationsstatus för alla serviceartiklar i serviceordern."
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
ms.openlocfilehash: 6e2edc1cde66b49c3961cf4c93820f056d230dc8
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="service-order-status-and-repair-status"></a>Serviceorderstatus och reparationsstatus
Fältet **Status** i fönstret **Serviceorder** och serviceartikelns reparationsstatus som visas i fältet **Reparationsstatuskod** i fönstret **Serviceorder** har ett visst samband i modulen Service. Serviceorderstatus visar reparationsstatus för alla serviceartiklar i serviceordern.  
  
> [!NOTE]  
>  De två statusfälten är inte kopplade till fältet **Släppningsstatus** i huvudet på serviceordern, som styr lagerhanteringen av serviceartiklar.  
  
 När du ändrar en serviceartikels reparationsstatus på serviceordern uppdateras serviceorderns status. För att se den status som anger den generella reparationsstatusen för enskilda serviceartiklar måste du ange följande:  
  
* Den serviceorderstatus som respektive reparationsstatus är länkad till. Mer information finns i Serviceorderstatus.  
* Prioritetsnivå för varje serverorderstatusalternativ. Mer information finns i Prioritet.  
  
 När du omvandlar en serviceoffert till en serviceorder ändras reparationsstatus för alla serviceartiklar i ordern till **Initial** och serviceorderstatusen till **Förestående**.  
  
## <a name="specifying-service-order-status-for-repair-status"></a>Ange serviceorderstatus för reparationsstatus  
Varje reparationsstatus är länkad till en viss serviceorderstatus. Alternativen för serviceorderstatus är **Förestående**, **På gång**, **Stoppad** och **Avslutad**. Det finns nio olika alternativ för reparationsstatus: **Initial**, **På gång**, **Hänvisad**, **Delvis servad**, **Offert avslutad**, **Väntar på kund**, **Beställt reservdelar**, **Reservdelar inlevererade** och **Avslutad**.  
  
### <a name="pending"></a>Förestående  
Serviceorderstatusen **Förestående** anger att servicen kan inledas eller fortsätta när som helst. Därför kan fyra av alternativen för reparationsstatus, nämligen **Initial**, **Hänvisad**, **Delvis servad** och **Reservdelar inlevererade**, alla länkas till den här serviceorderstatusen.  
  
### <a name="in-process"></a>Pågående  
Serviceorderstatusen **På gång** anger att servicen pågår. Därför kan två av alternativen för reparationsstatus, nämligen **På gång** och **Beställt reservdelar**, länkas till den här serviceorderstatusen. Om du länkar statusen **Beställt reservdelar** till servicestatusen **På gång** måste du även länka statusen **Beställt reservdelar** till den här serviceorderstatusen.  
  
### <a name="on-hold"></a>Stoppad  
Serviceorderstatusen **Stoppad** anger att servicen tillfälligt har stoppats i väntan på svar från kunden eller reservdelar innan servicen kan inledas. Därför kan tre av alternativen för reparationsstatus, nämligen **Offert avslutad**, **Beställt reservdelar** och **Väntar på kund**, alla länkas till den här serviceorderstatusen.  
  
### <a name="finished"></a>Avslutad  
Serviceorderstatusen **Avslutad** anger att servicen har slutförts. Därför är reparationsstatusen **Avslutad** länkad till den här statusen.  
  
## <a name="assigning-priority-to-service-order-status"></a>Tilldela en serviceorderstatus prioritet  
När du ändrar reparationsstatus för en serviceartikel identifieras de serviceorderstatusalternativ som är länkade till olika reparationsstatusalternativ för alla serviceartiklar i ordern. Om serviceartiklarna är kopplade till två eller fler serviceorderstatusalternativ väljs den serviceorderstatus som har högst prioritet.  
  
Du måste välja vilken serviceorderstatus som innehåller viktigast information om serviceorderstatusen och tilldela den högst prioritet o.s.v.  
  
### <a name="example"></a>Exempel  
En typisk tilldelning av prioritetsnivå kan se ut så här:  
  
* Pågående – hög  
* Förestående – medelhög  
* Stoppad – medellåg  
* Färdig – låg  
  
Om t.ex. en serviceartikel har reparationsstatus **Initial**, länkad till serviceorderstatus **Förestående**, en annan har **På gång**, länkad till servicestatus **På gång**, och en tredje har **Beställt reservdelar**, länkad till servicestatus **Stoppad**, blir den resulterande serviceorderstatus **På gång** eftersom den har högst prioritet.  
  
## <a name="see-also"></a>Se även  
[Så här: ställa in status för serviceorder och reparationer](service-order-repair-status.md)  
[Ställa in servicehantering](service-setup-service.md)  

