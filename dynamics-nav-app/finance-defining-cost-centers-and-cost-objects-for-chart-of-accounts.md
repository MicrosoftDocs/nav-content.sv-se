---
title: "Definiera kostnadsställen och kostnadsbärare för kontoplanen"
description: "Du kan automatiskt överföra kostnads- och intäktstransaktioner från redovisningen till kostnadsredovisningen antingen för varje redovisningsbokföring eller med ett batch-jobb. När du gör överföringen överför systemet endast de transaktioner som redan är länkade till ett kostnadsställe eller en kostnadsbärare. Om du vill skapa en meningsfullt överföring måste du kontrollera att kostnadsställena och kostnadsbärarna definierats korrekt."
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
ms.openlocfilehash: d034d2ab8f772ecd4a7b8db2ddf99720113948e3
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="defining-cost-centers-and-cost-objects-for-chart-of-accounts"></a>Definiera kostnadsställen och kostnadsbärare för kontoplanen
Du kan automatiskt överföra kostnads- och intäktstransaktioner från redovisningen till kostnadsredovisningen antingen för varje redovisningsbokföring eller med ett batch-jobb. När du gör överföringen överför, [!INCLUDE[d365fin](includes/d365fin_md.md)] endast de transaktioner som redan är länkade till ett kostnadsställe eller en kostnadsbärare. Om du vill skapa en meningsfullt överföring måste du kontrollera att kostnadsställena och kostnadsbärarna definierats korrekt.  

## <a name="defining-default-dimension-values-for-general-ledger-accounts"></a>Ange standarddimensionsvärden för redovisningskonton  
För varje redovisningskonto kan du ange standarddimensionsvärden i tabellen **Standarddimension**. Följande exempel visar hur du anger att det alltid ska finnas ett kostnadsställe för avdelningen, men aldrig är en kostnadsbärare för ett projekt när du bokför på ett redovisningskonto.  

|**Dimensionskod**|**Bokförs med**|  
|------------------------------------------|-----------------------------------------|  
|Avdelning|Kod alltid|  
|Objekt|Ingen kod|  

## <a name="defining-dimension-values-for-overhead-costs-and-direct-costs"></a>Definiera dimensionsvärden för omkostnader och direkta kostnader  
 Du kan överföra omkostnader till ett kostnadsställe och direkta kostnader till en kostnadsbärare. Följande tabell visar den optimala kombinationen av installationsvärden för dimensioner.  

|Överför till|Kostnadsställebokföring|Kostnadsbärarbokföring|  
|-----------------|-------------------------|-------------------------|  
|Kostnadsställe|Kod alltid|Ingen kod|  
|Kostnadsbärare|Ingen kod|Kod alltid|  

> [!NOTE]  
>  Markera kryssrutan **Kontrollera redovisningsbokföringar** för att se till att de fördefinierade kostnadsställena och kostnadsbärarna som du skapar i redovisningen automatiskt överförs till kostnadsredovisningen.  

## <a name="see-also"></a>Se även  
[Redovisa kostnader](finance-manage-cost-accounting.md)  
[Så här: Skapa kostnadsställen](finance-how-to-set-up-cost-centers.md)   
[Så här: Skapa kostnadsbärare](finance-how-to-set-up-cost-objects.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

