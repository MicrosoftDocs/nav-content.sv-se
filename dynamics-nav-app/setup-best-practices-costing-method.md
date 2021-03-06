---
title: "Lägga upp bästa metoder: Värderingsprincip"
description: "**Värderingsprincipen** på artikelkortet anger hur artikelns kostnadsflöde registreras och om ett faktiskt eller budgeterat värde ska kapitaliseras och användas i kostnadsberäkningen."
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
ms.openlocfilehash: a2c25ffc6c2012bac4e86ebbce0f3c33ecaf68fc
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-costing-method"></a>Lägga upp bästa metoder: Värderingsprincip
**Värderingsprincipen** på artikelkortet anger hur artikelns kostnadsflöde registreras och om ett faktiskt eller budgeterat värde ska kapitaliseras och användas i kostnadsberäkningen.  

 Det är viktigt att ange rätt värderingsprincip enligt artikeltyp och affärsmiljö för att garantera ekonomiska lager.  

 I tabellen nedan finns bästa metod för hur du lägger upp fältet **Värderingsprincip**. Mer information finns i [Designdetaljer: Värderingsprinciper](design-details-costing-methods.md).  

|Inställningsalternativ|Best practice|Kommentar|  
|------------------|-------------------|-------------|  
|FIFO|Använd där produktkostnaden är fast.<br /><br /> Använd för artiklar med ett begränsat hållbarhetstid, eftersom den äldsta varor behöver säljas innan deras hållbarhetstid passerat.|En artikels styckkostnad är det verkliga värdet på en mottagen artikel, vald enligt FIFO-regeln.<br /><br /> I lagervärdering antas det att de första artiklarna in i lagret säljs först. **Obs!**  När priser stiger visar balansräkningen ett högre värde Det betyder att skatteskuler ökar, men kreditpoängen och förmåga att låna kontant ökar.|  
|LIFO (Sist in, först ut)|Använd där lagernivåer är konsekvent underhållna eller ökar med tiden.|En artikels styckkostnad är det verkliga värdet på en mottagen artikel, vald enligt LIFO-regeln.<br /><br /> I lagervärdering antas det att de senaste artiklarna in i lagret säljs först. **Obs!**  När priser vill stiger, minskas värdet på resultaträkningen. Det betyder att skatteskuler minskar, men din förmåga att låna kontant försämras. **Viktigt:**  Tillåts inte i många länderregioner, eftersom det kan användas för att dölja vinst.|  
|Genomsnitt|Använd där produktkostnaden inte är fast.<br /><br /> Använd där lager travas eller blandas samman och inte kan åtskiljas, till exempel kemikalier.|En artikels styckkostnad är den exakta kostnaden för mottagandet av den aktuella enheten.|  
|Specifik|Använd i produktionen eller handel med enkelt härledas artiklar med i höga kostnadspris.<br /><br /> Använda för artiklar, som lyder under regler.<br /><br /> Använd för artiklar med serienummer.|En artikels styckkostnad beräknas enligt den genomsnittliga styckkostnaden vid varje tidpunkt efter ett inköp.<br /><br /> För lagervärdering förutsätts att alla lagerartiklar säljs samtidigt.|  
|Standard|Använd där kostnadskontroll är kritisk.<br /><br /> Använd i upprepande produktion för att värdera kostnaderna för direkt material, direkt arbete och produktionsoverheadkostnad.<br /><br /> Använd när det finns funktion och personal som underhåller standarder.|En artikels styckkostnad är förinställd baserad på uppskattning.<br /><br /> När den verkliga kostnaden senare realiseras, måste standardkostnaden justeras med den verkliga kostnaden via skillnadsvärden.|  

## <a name="see-also"></a>Se även  
 [Designdetaljer: Värderingsprinciper](design-details-costing-methods.md)   
 [Designdetaljer: Lagerkalkylering](design-details-inventory-costing.md)   
 [Skapa komplexa moduler med hjälp av bästa metoder](set-up-complex-application-areas-using-best-practices.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

