---
title: "Om kostnader för färdiga produktionsorder"
description: "Att färdigställa produktionsordern är en viktig uppgift när det gäller att slutföra livscykeln för kostnadsberäkning för artikeln som tillverkas. Slutkostnader (avvikelser i standardkostnad, faktiska värden i en FIFO, genomsnittskostnader eller LIFO-kostnader) beräknas med hjälp av batch-jobbet **Justera kost. - artikeltrans**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6b6fd4fe1ba4bd279aacbca38bf953bce5a996fc
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="about-finished-production-order-costs"></a>Om kostnader för färdiga produktionsorder
Att färdigställa produktionsordern är en viktig uppgift när det gäller att slutföra livscykeln för kostnadsberäkning för artikeln som tillverkas. Slutkostnader, inklusive avvikelser i standardkostnad, faktiska värden i en FIFO, genomsnittlig eller LIFO-kostnad, beräknas med hjälp av batch-jobbet **Justera kostnad - artikeltransaktioner** som används för avstämning av kostnaderna för produktionsartiklar. Om kostnadsjustering ska genomföras för en produktionsorder måste statusen vara **Färdig**. Det är därför viktigt att vid slutförande ändra statusen för en produktionsorder till **Färdig**.  

## <a name="example"></a>Exempel  
 Vid standardkostnad, när du t.ex. förbrukar material för att producera en artikel, överförs förenklat kostnaden för artikeln plus arbets- och overheadkostnader till PIA. När artikeln tillverkas minskar PIA med beloppet för standardkostnaden för artikeln. De här kostnaderna får vanligtvis inte nollnetto. För att dessa kostnader inte ska få nollnetto måste du köra batchjobbet **Justera kostnad - artikeltransaktiner** och notera att endast produktionsorder med statusen **Färdig** ska beaktas för justering.  

## <a name="see-also"></a>Se även  
[Hantera lagerkostnader](finance-manage-inventory-costs.md)  
[Produktion](production-manage-manufacturing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

