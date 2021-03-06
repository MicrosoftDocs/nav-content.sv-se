---
title: Analysera data efter dimensioner
description: "Beskriver hur du kan analysera olika affärsdata per dimension."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/13/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 2ea54861f8203406cf6c9d110ad2317b8f883dde
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
#  <a name="how-to-analyze-data-by-dimensions"></a>Så här: Analysera data efter dimensioner
Inom ekonomisk analys är en dimension data som du kan lägga till en transaktion som en sorts markör. Dessa data används för att gruppera transaktioner med liknande egenskaper, till exempel kunder, regioner, produkter och säljare, och enkelt hämta dessa grupper för analys. Dimensioner kan användas på transaktioner i journaler, dokument och budgetar. Termen dimension används för att beskriva hur analyser utförs. Ett exempel på en tvådimensionell analys är försäljning per område. Om du använder fler än två dimensioner när du skapar en transaktion kan du utföra mer komplexa analyser, exempelvis försäljning per försäljningskampanj per kundgrupp per område. Mer information finns i [Arbeta med](finance-dimensions.md).

Att analyera data efter dimensioner ger dig bättre inblick i din verksamhet, så att du kan utvärdera information, till exempel hur väl verksamheten fungerar, inom vilka områden det går riktigt bra och inom vilka det går sämre samt var det krävs mer resurser.

> [!TIP]
> Som ett snabbt sätt att analysera transaktionsdata med dimensioner kan du filtrera summorna i kontoplanen och posterna i alla fönstrer för **Transaktioner** per dimension. Sök efter åtgärden **Ange dimensionsfilter**.

## <a name="to-set-up-an-analysis-view"></a>Så här definierar du en analysvy  
En analys per dimension visar en vald kombination av dimensioner. Du kan lagra och hämta alla analyser som har definierats. Informationen som används för att skapa en analys lagras på **analysvykortet** för att underlätta framtida analyser.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Analysvyer** och välj sedan relaterad länk.  
2. I fönstret **Analysvylista** väljer du åtgärden **Ny**.
3. Fyll i fälten om det behövs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Om du vill lägga till ytterligare dimensionskoder förutom de fyra koderna väljer du på snabbfliken **Dimensioner**, åtgärden **Filter**, fyller i fälten och klickar på **OK**.  
5. Om du vill uppdatera vyn, väljer du åtgärden **uppdatera**.

## <a name="to-analyze-by-dimensions"></a>Analysera efter dimensioner
Du kan använda matrisen **Analys per dimension** för att visa beloppen i redovisningen med hjälp av de analysvyer som du har definierat. Du fyller i fönstret **Analys per dimension** för att definiera vad som ska visas i matrisen och klickar sedan på **Visa matris** för att visa matrisen.  

- Kolumnen till vänster innehåller information baserad på vad du valt i fältet **Visa som rader** i huvudet.  
- Kolumnen till höger innehåller information baserad på vad du valt i fältet **Visa som kolumner** i huvudet.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Analysvyer** och välj sedan relaterad länk.  
2. Välj lämplig analysvy och klicka på **Redigera analysvy**.
3. Högst upp i fönstret **Analys efter dimensioner** fyller du i fälten för att definiera vad som ska visas.
4. 5. Om du vill visa en specifikation av ett belopp som visas i matrisfönstret väljer du beloppet.  

> [!IMPORTANT]  
>   Du kan inte välja en period som är kortare än perioden som angetts för datumkomprimeringen på **Analysvy**-kortet. Kommandona **Nästa period** och **Föregående period** är inaktiverade om du har valt **Period** i **Visa som rader** eller **Visa som kolumner**.  

> [!NOTE]  
>   Du kan använda rapporten **Dimensioner - detaljerad** om du vill visa en detaljerad klassificering av hur dimensionerna har använts på transaktioner under en vald period. Du använder rapporten **Dimensioner - total** om du bara vill visa totalbeloppen.  

> [!TIP]  
>   Du kan också ändra vyn genom att ändra innehållet i fältet **Visa som rader** och fältet **Visa om kolumner**. Om du vill ändra vyinställningen, väljer du åtgärden **Byt plats på rader och kolumner**.

## <a name="to-update-an-analysis-view"></a>Så här uppdaterar du en analysvy  
Beloppen som visas i fönstret **Analys per dimension** ger dig en bild av företagets status vid tidpunkten för den sista uppdateringen. Om du vill få en bild av den aktuella situationen måste du uppdatera analysvyn genom att köra funktionen Uppdatera.

Nedanstående procedur beskriver hur du uppdaterar en analysvy från fönstret **Analys per dimension**. Momentet är liknande från den **Analysvykort** och **Analysvylista** windows.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Analysvyer** och välj sedan relaterad länk.  
2. I fönstret **analys per dimension** väljer du fältet **Analysvykod** för att visa alternativen.  
3. Välj raden med önskad analysvy.  
4. Välj åtgärden **Uppdatera**.  

> [!TIP]  
>   Om du väljer kryssrutan **Uppdatera vid bokföring** på ett analysvykort, uppdateras vyn automatiskt när du bokför en transaktion som berörs.

> [!NOTE]  
>   Om du vill uppdatera några eller alla analysvyer samtidigt måste du använda batchjobbet **Uppdatera analysvyer**.  

## <a name="see-also"></a>Se även
[Affärsstöd](bi.md)  
[Ekonomi](finance.md)  
[Ställa in Finance](finance-setup-finance.md)  
[Redovisningen och kontoplanen](finance-general-ledger.md)  
[Arbeta med dimensioner](finance-dimensions.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

