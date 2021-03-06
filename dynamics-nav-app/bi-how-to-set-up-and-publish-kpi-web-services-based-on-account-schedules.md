---
title: "Så här skapar och publicerar du KPI-webbtjänster som är baserade på kontouppställningar"
description: "I fönstret **Installation av webbtjänst för KPI för kontouppställning**, kan du konfigurera hur du visar kontouppställnings-kpi-data och vilka specifika kontouppställningar som du vill basera KPI-erna på."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b45fe6e1e5d4e5be00a6e8a34b7b4fea39b5d75b
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules"></a>Så här: Skapar och publicerar du KPI-webbtjänster som är baserade på kontouppställningar
I fönstret **Installation av webbtjänst för KPI för kontouppställning** kan du konfigurera hur du visar kontouppställnings-kpi-data och vilka specifika kontouppställningar som du vill basera KPI-erna på. När du väljer knappen **Publicera webbtjänst** läggs det angivna kontouppställning-kpi-data till listan över publicerade webbtjänster i fönstret **Webbtjänster**.  

## <a name="to-set-up-and-publish-a-kpi-web-service-that-is-based-on-account-schedules"></a>Så här: Skapar och publicerar du en KPI-webbtjänst som är baserad på kontouppställningar  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Installation av webbtjänst för KPI för kontouppställning** och välj sedan relaterad länk.  
2.  Fyll i fälten enligt beskrivningen i följande tabell på snabbfliken **Allmänt**.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Start för prognostiserade värden**|Ange vid vilken tidpunkt i prognosen som värden visas på kontouppställning-kpi-grafiken.<br /><br /> De prognostiserade värdena hämtas från redovisningsbudgeten som du väljer i fältet **Redov.budgetnamn**. **Obs!**Om du vill få KPI:er att visar prognossiffror efter ett visst datum och den verkliga siffror före datumet, kan du ändra fältet **Tillåt bokföring fr.o.m.** i fönstret **Redovisningsinställningar**. Mer information finns också i Tillåt bokföring fr.o.m..|  
    |**Redov.budgetnamn**|Ange namnet på den redovisningsbudget som ger prognostiserade värden till kontouppställning-kpi-webbtjänsten.|  
    |**Period**|Ange perioden som kontouppställning-KPI-webbtjänsten baseras på.|  
    |**Visa per**|Ange vid vilket tidsintervall kontouppställning-KPI visas i.|  
    |**Webbtjänstnamn**|Ange namnet på kontouppställningen-KPI-webbtjänsten.<br /><br /> Det här namn visas i fältet **Servicenamn** i fönstret **Webbtjänster**.|  

    Fortsätt genom att ange en eller flera kontouppställningar som du vill publicera som en KPI webbtjänst enligt inställningarna, som du gjorde i föregående tabellen.  

3.  Fyll i fälten enligt beskrivningen i följande tabell på snabbfliken **kontouppställningar**.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Kontouppställningsnamn**|Ange kontouppställningen som KPI-webbtjänsten baseras på.|  
    |**Beskrivning av kontouppställning**|Ange beskrivningen av kontouppställningen som KPI webbtjänsten baseras på.|  

4.  Upprepa moment 3 för alla kontouppställningar som du vill basera kontouppställningswebbtjänsten för kpi på.  
5.  Välj åtgärden **Redigera kontouppställning** på snabbfliken **Kontouppställning** för att visa eller redigera den valda kontouppställningen.  
6.  Om du vill visa kontouppställning-kpi-data som du har upprättat väljer du åtgärden **Webbtjänst för KPI för kontouppställning**.  
7.  Om du vill publicera kontouppställningens KPI-webbtjänst väljer du åtgärden **Publicera webbtjänst**. Webbtjänsten läggs till i listan över publicerade webbtjänster i fönstret **Webbtjänster**.  

    > [!NOTE]  
    >  Du kan också publicera KPI webbtjänsten genom att peka på sidobjektet **KPI Web Service kontouppställningsinställning** från fönstret **Webbtjänster**. Mer information finns i [Så här: Publicerar du en webbtjänst](https://msdn.microsoft.com/en-us/library/dd338978.aspx) på MSDN.  

## <a name="see-also"></a>Se även  
[Affärsstöd](bi.md)  
[Ekonomi](finance.md)  
[Ställa in Finance](finance-setup-finance.md)  
[Redovisningen och kontoplanen](finance-general-ledger.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

