---
title: "Så här använder du resurser för projekt"
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: cced4bca42b74c2664fd18770f1616c57286e1c3
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-resources-for-jobs"></a>Så här använder du resurser för projekt
Du registrerar förbrukning av resurser i projektjournalen för att hålla reda på kostnader, priser och de specifika projekttyper som är kopplade till projekt. Mer information finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).

Du kan även bokföra förbrukningen av en resurs i en resursjournal eller projektjournal. Transaktioner bokförda i resursjournaler påverkar inte redovisningen.

## <a name="to-assign-resources-to-jobs"></a>Så här tilldelar du resurser till projekt
Du tilldelar resurser till projekt genom att skapa planeringsrader för projektet. Mer information finns i [Så här skapar du Projekt](projects-how-create-jobs.md).

## <a name="to-record-resource-usage-for-a-job"></a>Registrera resursförbrukning för ett projekt

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projektjournaler** och välj sedan relaterad länk.
2. Öppna den relevanta projektjournalen och fyll sedan i fälten som behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. När journalen är slutförd väljer du åtgärden **Bokföra**.

## <a name="to-adjust-resource-prices"></a>Justera resurspriser  
Om du vill ändra kostnader eller priser för många resurser på en gång kan du använda ett batch-jobb .  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Justera resurskost./-priser** och välj sedan relaterad länk.
2. Fyll i fälten på en rad efter behov och välj sedan knappen **OK**.

**Obs**! Batch-jobbet varken skapar eller justerar alternativa kostnader eller priser för resurser. Detta ändrar bara innehållet i fältet på resurskortet för fältet **Justeringsfält** som du har valt i batch-jobbet. Justeringarna börjar gälla direkt för resurser så kontrollera justeringsfaktorerna innan du kör batch-jobbet.

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a>Så här får du förslag till resursprisändringar enligt befintliga alternativa priser:  
Om du redan har skapat alternativa priser för några resurser kan du använda batch-jobbet för att skapa flera alternativa resurspriser.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resursprisändringar** och välj sedan relaterad länk.
2. Välj åtgärden **Föreslå res.prisändring (pris)** och fyll sedan i fälten efter behov.
3. Välj **OK**.  
4. När batch-jobbet har avslutats visar fönstret **Resursprisändringar** resultatet av batch-jobbet.

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a>Så här får du förslag till resursprisändringar enligt standardpriser  
Om du vill skapa flera alternativa resurspriser baserat på standardpriserna på resurskorten kan du använda ett batch-jobb .  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resursprisändringar** och välj sedan relaterad länk.
2. Välj åtgärden **Föreslå res.prisändring (res)** och fyll sedan i fälten efter behov.  
3. Välj **OK**.  
4. När batch-jobbet har avslutats öppnar du fönstret **Resursprisändringar** för att visa resultatet av batch-jobbet.

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a>Så här får du förslag till resursprisändringar baserat på alternativa priser  
Om du redan har skapat alternativa priser för några resurser kan du använda batch-jobbet för att skapa flera alternativa resurspriser.

1. I rutan **Sök** anger du **Föreslå res.prisändring (pris)** och väljer sedan relaterad länk.  
2. Fyll i fälten om det behövs.
3. Välj **OK**.  
4. När batch-jobbet har avslutats öppnar du fönstret **Resursprisändringar** för att visa resultatet av batch-jobbet.

## <a name="see-also"></a>Se även
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)     
[Arbeta med Dynamics NAV](ui-work-product.md)  

