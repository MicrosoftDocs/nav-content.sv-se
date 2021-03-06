---
title: 'Skapa metodtips: partiformningsmetoder'
description: "Fältet **Partiformningsmetod** på artikelkort erbjuder fyra olika planeringsmetoder som bestämmer hur de enskilda planeringsparametrarna kommunicerar."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b96fc662f741bd705e673f7d17b2467b4e6dc846
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-reordering-policies"></a>Skapa metodtips: partiformningsmetoder
**Partiformningsmetod**-fältet på artikelkort erbjuder fyra olika planeringsmetoder som bestämmer hur de enskilda planeringsparametrarna kommunicerar.  

En grund för bästa metod för val av en partiformningsmetod är artikelns ABC-klassificering. När du använder ABC-klassificeringen för lagerkontroll och leveransplanering, artiklar hanteras enligt tre olika indelningar beroende på deras värden och volym, i förhållande till summan i lager. Volymfördelning av de tre indelningar visas i följande tabell.

|Klass|Procent av totala antalet i lagervolym|Procent av totala antalet i lagervärde|
|-----|-----------------------------|----------------------------|
|A|10-20|50-70|
|B|20|20|
|L|60-70|10-30|

ABC-klassificeringen anger att insats och pengar kan sparas genom lösare kontroll av artiklar med låg värdevolym, än av artiklar med hög värdevolym. Illustrationen visar vilken partiformningsmetod i [!INCLUDE[d365fin](includes/d365fin_md.md)] som är bättre lämpade för A-, B- och C-objekt, respektive.

![ABC-klassificering](media/abc_classification.png "abc_classification")

I följande tabell visas bästa metod för att välja mellan de fyra regler.  

|Inställningsalternativ|Best practice|Kommentar|  
|------------------|-------------------|-------------|  
|**Order**|Använd för a-artiklar.<br /><br /> Använd för tillverka-mot-order-artiklar.<br /><br /> Använd för artiklar på den högsta nivån och för dyra komponenter och halvfabrikat i produktionen.<br /><br /> Använd för artikel som köps, som direktutleveranser och specialorder.<br /><br /> Använd inte, om du inte accepterar automatisk reservation.|A-artiklar, till exempel lädersoffor i ett möbler lager, är högvärderade artiklar med låg, och ojämnt orderomsättning där lagret är oacceptabelt, eller de obligatoriska attributen varierar. Den bästa partiformningsmetoden är därför en som planerar specifikt för varje behov.|  
|**Parti-för-parti**|Använd för B-artiklar.<br /><br /> Använd för komponenter som finns i flera strukturer i produktionen. Detta säkerställer att inköpsorder kombineras för samma leverantör, så bättre pris kan förhandlas.<br /><br /> Använd om du inte vet om vilken partiformningsmetoden som ska väljas.|B-artiklar, till exempel matsalsmöbelstolar, har en regelbunden och relativt hög orderomsättning men innebär också höga lagerhållningskostnader. Den bästa partiformningsmetoden för B-objekt är därför ett som är ekonomisk, genom att sammanföra behov i Beställningscykeln.<br /><br /> 80 procent av artiklar kan använda den här principen.<br /><br /> Kan användas, utan planeringsparametrar.|  
|**Fast orderkvantitet**|Använd för C-artiklar.<br /><br /> Kombinera med beställningspunktparametrar.<br /><br /> Använd för låg-nivå komponenter i produktionen.<br /><br /> Använd inte, om artikeln har reserverats ofta.|C-objekt, till exempel tekoppar, är låg-värde artiklar med hög, och regelbunden orderomsättning. Den bästa partiformningsmetoden för C-objekt är därför ett som garanterar konstant tillgänglighet, genom att alltid hålla sig över en beställningspunkt.<br /><br /> Om användaren reserveras ett antal för något avlägset behov, störs planeringsgrunden. Även om den planerade distributionslagernivån är accepterad av ordermottagaren med hänsyn till beställningspunkten, kan det hända att antalet inte är tillgängligt på grund av reservation.|  
|**Maximalt antal**|Använd för C-objekt med höga lagerhållningskostnader eller lagringsbegränsningar.<br /><br /> Kombinera tillsammans med en eller flera orderändringar (lägsta/max partistorlek eller Partistorleksmultipel).|C-objekt, till exempel tekoppar, är låg-värde artiklar med hög, och regelbunden orderomsättning. Den bästa partiformningsmetoden för C-objekt är därför ett som garanterar konstant tillgänglighet, genom att alltid hålla sig över en beställningspunkt, men under en maximal lagerkvantitet.<br /><br /> Om du vill ändra den föreslagna order, kan du behöva minska partistorleken till en angiven maximal partistorlek, öka till en angiven minimal partistorlek eller avrundad uppåt för att uppfylla en viss partistorleksmultipel. **Obs!** Lagret stannar då mellan beställningspunkt och högsta antal, om använd med en beställningspunkt.|  

## <a name="see-also"></a>Se även  
 [Skapa metodtips: leveransplanering](setup-best-practices-supply-planning.md)   
 [Designdetaljer: Partiformningsmetoder](design-details-reordering-policies.md)   
 [Designdetaljer: Order](design-details-order.md)   
 [Designdetaljer: Parti-för-parti](design-details-lot-for-lot.md)   
 [Designdetaljer: Fast orderkvantitet](design-details-fixed-reorder-qty.md)   
 [Designdetaljer: Maximalt antal](design-details-maximum-qty.md)   
 [Skapa komplexa moduler med hjälp av bästa metoder](set-up-complex-application-areas-using-best-practices.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

