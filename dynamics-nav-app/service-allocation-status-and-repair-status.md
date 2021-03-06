---
title: "Fördelningsstatus och reparationsstatus"
description: "Lär dig mer om sambandet mellan reparationsstatus för serviceartiklar och fördelningsstatus för fördelningsposterna för dessa."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resources, allocation, status, repairs
ms.date: 08/28/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b57b237ea527ad7a163c0bd65cb08e8b285ef644
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="allocation-status-and-repair-status-of-service-items"></a>Fördelningsstatus och reparationsstatus för serviceartiklar
Det finns ett visst samband mellan serviceartiklarnas reparationsstatus och fördelningsstatus för fördelningsposterna till serviceartiklarna i modulen Service. Fördelningsstatusen ändras när du ändrar serviceartikelns reparationsstatus till **Avslutad** eller **Delvis servad** och när du omvandlar en serviceoffert till en serviceorder. En serviceartikels reparationsstatus ändras när du avbryter fördelningen av serviceartiklar eller flyttar serviceartikeln till en annan resurs. Du kan visa serviceartiklarnas reparationsstatus i fönstret **Serviceuppgifter** och uppdatera reparationsstatus i fältet **Reparationsstatuskod** i fönstret **Serviceartikeldokument**. Du kan visa fördelningsstatus i fältet **Status** i fönstret **Resursfördelningar**.  
  
## <a name="changing-repair-status"></a>Ändra reparationsstatus  
När du ändrar en serviceartikels reparationsstatus på en serviceartikelrad, görs en sökning efter motsvarande fördelningspost för serviceartikeln som har statusen **Aktiv**. Om en sådan fördelningspost hittas uppdateras dess status på något av följande sätt:  
  
* Om du ändrar reparationsstatus till **Avslutad** ändras fördelningsstatus från **Aktiv** till **Avslutad**.  
* Om du ändrar reparationsstatus till **Delvis servad** (viss service har avslutats) eller **Hänvisad** (ingen service har utförts) ändras fördelningsstatus i programmet från **Aktiv** till **Omfördelning nödvändig**.  
* När en fördelningstransaktion för en serviceorder skapas, vilket innebär att ingen resurs har fördelats, anges värdet **Ej aktiv** för fältet **Status** i fönstret **Resursfördelning**.  
* Fördelningstransaktionens status blir **Avbruten** när du omfördelar den serviceartikel som nämns i fördelningstransaktionen för serviceordern, vilket innebär att den fördelade resursen eller resursgruppen inte har använts för serviceuppgiften.  
  
Fördelningsstatusen visar därmed när serviceprocessen är avslutad eller när en annan resurs krävs för att avsluta service av serviceartikeln.  
  
## <a name="converting-service-quotes-to-service-orders"></a>Omvandla serviceofferter till serviceorder  
När du omvandlar en serviceoffert till en serviceorder uppdateras serviceordern, serviceartiklarna i ordern och deras fördelningsposter så här:  
  
* Serviceartiklarnas reparationsstatus ändras till **Initial**.  
* Serviceorderstatus ändras till **Förestående**.  
* En sökning görs efter fördelningstransaktioner för alla serviceartiklar i serviceordern som har statusen **Aktiv**. Om sådana fördelningsposter hittas ändras deras fördelningsstatus från **Aktiv** till **Omfördelning nödvändig**.  
  
## <a name="canceling-allocations"></a>Rätta fördelningar  
När du avbryter fördelningen av en serviceartikel uppdaterar [!INCLUDE[d365fin](includes/d365fin_md.md)] fördelningsstatusen för motsvarande fördelningspost från **Aktiv** till **Omfördelning nödvändig**.

Reparationsstatus uppdateras för serviceartikeln i fördelningsposten så här:  
  
* Om fördelningsstatus är **Initial** ändras reparationsstatus till **Hänvisad** (ingen service har inletts).  
* Om reparationsstatus är **Pågående** ändras reparationsstatus till **Delvis servad** (viss service har utförts).  
  
## <a name="reallocating-an-active-allocation-entry"></a>Omfördela en fördelningspost som är aktiv  
När du omfördelar en serviceartikel i en fördelningspost som är **Aktiv** uppdateras fördelningsposten så här:  
  
* Om servicen startade när fördelningen var **Aktiv** (det vill säga om serviceartikelns reparationsstatus ändrats till **Pågående**), ändras fördelningsstatus från **Aktiv** till **Avslutad**.  
* Om servicen inte påbörjades när fördelningen var **Aktiv**, ändras fördelningsstatus från **Aktiv** till **Inställt**.  
  
Reparationsstatus för serviceartikeln i fördelningsposten uppdateras på samma sätt som om du hade ställt in fördelningen:  
  
* Om fördelningsstatus är **Initial** ändras reparationsstatus till **Hänvisad** (ingen service har inletts).  
* Om reparationsstatus är **Pågående** ändras reparationsstatus till **Delvis servad** (viss service har utförts).  
  
En ny fördelningspost skapas som innehåller den nya resursen med statusen **Aktiv**.  
  
## <a name="reallocating-a-service-item"></a>Omfördela en serviceartikel  
När du omfördelar en serviceartikel i en fördelningspost med statusen **Omfördelning nödvändig** uppdateras fördelningsposten så här:  
  
* Om servicen startade när fördelningen var **Aktiv**, dvs. om serviceartikelns reparationsstatus ändrats till **Pågående**, ändras fördelningsstatus från **Omfördelning nödvändig** till **Avslutad**.  
* Om servicen inte påbörjades när fördelningen var **Aktiv**, ändras fördelningsstatus från **Omfördelning nödvändig** till **Inställt**.  
  
En ny fördelningspost skapas som innehåller den nya resursen med statusen **Aktiv**.  
  
## <a name="see-also"></a>Se även  
[Så här kan du ställa in resursfördelningar](service-how-setup-resource-allocation.md)  
[Så här fördelar du resurser:](service-how-to-allocate-resources.md)  


