---
title: "Så här justerar du artikelkostnader"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 59db38c159dd2810656edc668ee431c6414b9d90
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-adjust-item-costs"></a>Så här justerar du artikelkostnader   
Kostnaden för en artikel (lagervärde) som du köper och senare säljer kan ändras under dess livstid, eftersom till exempel en fraktkostnad läggs till dess inköpkostnad när du har sålt artikeln. För att alltid ha rätt lagervärde måste artikelkostnader därför regelbundet justeras.
Detta säkerställer att försäljnings- och vinststatistiken är aktuell och ekonomiska KPI-er är korrekta.

**Obs**! Artikelkostnader justeras endast av FIFO-principen. Det betyder att en artikels styckkostnad är det faktiska värdet av alla inleveranser av artikeln och att lagret värderas med antagandet om att de första artiklarna som finns i lager säljs först.

Funktionen Kostnadsjustering bearbetar endast värdetransaktioner som inte ännu har justerats. Om en funktion påträffas där ankommande kostnader behöver flyttas fram till kopplade avgående kostnader, görs detta genom att nya justeringsvärdetransaktioner skapas som baseras på informationen i de ursprungliga värdetransaktionerna, men som innehåller justeringsbeloppet. Funktionen Kostnadsjustering använder bokföringsdatumet för den ursprungliga värdetransaktionen om inte det datumet infaller i en avslutad lagerperiod. Om så är fallet används startdatumet för nästa öppna lagerperiod. Om lagerperioder inte används definieras datumet i fältet **Tillåt bokföring fr.o.m.** i fönstret **Redovisningsinställningar** när justeringstransaktionerna bokförs.

**Obs!** När artikelkostnader har justerats, måste lagerkostnaden bokföras i redovisningen, antingen automatiskt eller manuellt. Mer information finns i [Så här bokför du lagerkostnader i redovisningen](inventory-how-post-inventory-cost-gl.md).

Du kan justera artikelkostnader på två sätt:
 - Automatiskt genom att ställa in systemet till att justera för alla kostnadsändringar varje gång du som lagertransaktioner inträffar.
 - Manuellt genom att köra batch-jobbet **Justera kost. - artikeltrans** för en eller flera artiklar, när du vet att motsvarande kostnader har ändrat.  

## <a name="to-adjust-item-costs-automatically"></a>Så här justerar du artikelkostnader automatiskt
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Lagerinställningar** och välj sedan relaterad länk.
2. Välj ett av följande värden i fönstret **Lagerinställningar** i fältet **automatisk kostnadsjustering**.

|Alternativ |Beteende |
|-------|---------|
|Aldrig|Kostnaderna justeras inte vid bokföringen|
|Dag|Kostnaderna justeras om bokföringen sker inom ett dygn från arbetsdatumet.|
|Vecka|Kostnaderna justeras om bokföringen sker inom en vecka från arbetsdatumet.|
|Månad|Kostnaderna justeras om bokföringen sker inom en månad från arbetsdatumet.|
|Kvartal|Kostnaderna justeras om bokföringen sker inom ett kvartal från arbetsdatumet.|
|År|Kostnaderna justeras om bokföringen sker inom ett år från arbetsdatumet.|
|Alltid|Kostnaderna justeras vid bokföringen, oavsett bokföringsdatum.|

## <a name="to-adjust-item-costs-manually"></a>Så här justerar du artikelkostnader manuellt
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Justera kost. - artikeltrans.** och välj sedan relaterad länk.
2. I fönstret **Justera kost. - artikeltrans.** anger du vilka artiklar att justera kostnaderna för och om den justerade kostnaden ska bokföras i redovisningen samtidigt

## <a name="see-also"></a>Se även
[Hantera lager](inventory-manage-inventory.md)  
[Så här kan du bokföra lagerkostnader i redovisningen](inventory-how-post-inventory-cost-gl.md)  
[Hantera försäljning](sales-manage-sales.md)  
[Hantera inköp](purchasing-manage-purchasing.md)

