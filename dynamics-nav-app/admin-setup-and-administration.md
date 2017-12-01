---
title: Administrativa uppgifter i Dynamics NAV
description: "Vissa uppgifter i [!INCLUDE[d365fin](includes/d365fin_md.md)] kräver central administration och inställningar. Se vad de är och lär dig vad du ska göra."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 873c8e6f9887ef49d8639851bb64013d985e640e
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="setup-and-administration-in-dynamics-nav"></a>Installation och administration i Dynamics NAV
Central administration utförs vanligtvis av en roll i företaget. Omfattningen av dessa uppgifter kan vara beroende av företagets storlek och administratörens ansvarsområden. Dessa uppgifter kan omfatta att hantera databassynkronisering av projekt och e-postköer, konfigurera användare, anpassa användargränssnittet och hantera krypteringsnycklar.  

Det är viktigt att ange rätt inställningsvärden från början för att en ny verksamhetsprogramvara ska fungera effektivt. [!INCLUDE[d365fin](includes/d365fin_md.md)] innehåller ett antal assisterade installationer som hjälper dig att ställa in grundläggande information. Mer information finns i [Skapa Dynamics NAV](setup.md).

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

En superanvändare eller administratör kan konfigurera ramverket för datautbyte så att användare kan exportera och importera data i bank- och lönesystemfiler, till exempel för olika processer av likviditetsstyrning.  

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.   

|**Om du vill**|**Gå till**|  
|------------|-------------|  
|Lägg till användargrupper och hantera behörigheter, åtkomst till data, tilldela roller.|[Användare, profiler och rollcenter i Dynamics NAV](admin-users-profiles-roles.md)|  
|Spåra alla direkta ändringar som användarna gör av data i databasen för att kunna identifiera var fel och dataändringar härrör från.|[Logga ändringar i Dynamics NAV](across-log-changes.md)|  
|Stöd inställningsalternativ med rekommendationer för valda fält som eventuellt orsakar att lösningen är ineffektiv, om fältet felaktigt inställt|[Skapa komplexa moduler med hjälp av bästa metoder](set-up-complex-application-areas-using-best-practices.md)|  
|Visa sidor, kodenheter och frågor som webbtjänster.|[Så här: Publicerar du en webbtjänst](across-how-publish-web-service.md)|  
|Skapa en SMTP-server för att aktivera e-postkommunikation i och utanför Dynamics NAV| [Så här: Konfigurera e-post manuellt eller med hjälp av Assisterad konfiguration](madeira-how-setup-email.md)|  
|Ange enstaka eller återkommande begäranden om att köra rapporter eller kodenheter.|[Använd jobbköer för att schemalägga uppgifter](admin-job-queues-schedule-tasks.md)|  
|Hantera, ta bort eller komprimera dokument|[Hantera dokument](admin-manage-documents.md)|  

## <a name="see-also"></a>Se även
[Översikt över affärsfunktioner](madeira-business-functionality.md)  
[Allmänna affärsfunktioner](ui-across-business-areas.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Välkommen till [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)  

