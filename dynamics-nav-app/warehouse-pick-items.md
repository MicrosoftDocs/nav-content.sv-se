---
title: Plocka artiklar
description: "Lageraktiviteten att plocka artiklar innan de har levererats eller förbrukats utförs på olika sätt beroende på hur lagerstyrningsfunktionerna har konfigurerats. Hur komplexa [setup](../configure-warehouse-processes.md)-inställningarna är kan sträcka sig från inga lagerfunktioner, till grundläggande lagerkonfigurationer med hantering av order för order i en eller flera aktiviteter samt avancerade konfigurationer där alla lageraktiviteter måste utförs i ett dirigerat arbetsflöde."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a00a6b2740bb55352dfbe8e6ac4fd3d72870608e
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="pick-items"></a>Plocka artiklar
Lageraktiviteten att plocka artiklar innan de har levererats eller förbrukats utförs på olika sätt beroende på hur lagerstyrningsfunktionerna har konfigurerats. Hur komplex det är kan sträcka sig från inga lagerkonfigurationer, till grundläggande lagerstyrning med hantering av order för order i en eller flera aktiviteter samt avancerade konfigurationer där alla lageraktiviteter måste utförs i ett dirigerat arbetsflöde. Mer information finns i [Ställa in Lagerstyrning](warehouse-setup-warehouse.md).

Om du vill organisera och registrera plockningsaktiviteter med distributionslagerdokument, markerar du fältet **Begär plockning** på lagerställekortet. Det indikerar att artiklar som ska plockas för ett utgående källdokument, ska hanteras via, och kontrolleras av systemet. Ett utgående källdokument kan vara en försäljningsorder, en inköpsreturorder, en utgående överföringsorder, en serviceorder eller en produktionsorder med komponenter som ska plockas.

> [!NOTE]
> Även om inställningarna kallas **Begär plockning**, kan du fortfarande bokföra inleveranser och utleveranser direkt från affärskälldokument på platser där du markerar dessa kryssrutor.

Om lagerstället kräver plockningsbearbetning, men inte kräver utleveransbehandling, använder du fönstret **Lagerplockning** om du vill organisera eller skriva ut information om artikelplockning, ange resultat av plockningen eller bokföra plockningsinformation, som i sin tur bokför leverans av artiklarna. Om det gäller att plocka komponenter för en produktionsorder, bokför bokföringen av plockning också förbrukningen.

Om lagerstället kräver både plocknings- och utleveransbearbetning, det vill säga om både fältet **Begär plockning** och fältet **Kräv utleverans** har markerats på lagerställekortet, använder du fönstret **Dist.lager plockning** för att hantera plockningen. Dist.lagerplockning fungerar på samma sätt som lagerplockning, förutom att plockningen registreras i stället för att plockningsinformationen bokförs. I den här registreringsprocessen bokförs inte leveransen, men artiklarna blir tillgängliga för leverans. Du lagerchef kan du använda ett plockningsförslag för att organisera plockninginformation innan du skapar de individuella plockningsinstruktionerna för lager.

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.   

|**Om du vill**|**Gå till**|
|------------|-------------|  
|Bokföra utleveransen av artiklar direkt på det avgående orderdokumentet eftersom det inte finns några lagerfunktioner. (Fungerar på samma sätt för en försäljningsorder, en utgående överföringsorder och returutleveranser.)|[Så här levererar du artiklar](warehouse-how-ship-items.md)|  
|Plocka artiklar order för order och bokföra utleveransen i samma aktivitet, i en grundläggande lagerkonfiguration.|[Så här plockar du artiklar med Lagerplockning](warehouse-how-to-pick-items-with-inventory-picks.md)|
|Plocka artiklar för flera order i en avancerad lagerkonfiguration.|[Så här plockar du artiklar med lagerplockning](warehouse-how-to-pick-items-for-warehouse-shipment.md)|  
|Plocka komponenter för produktion eller montering i en grundläggande eller avancerad lagerkonfiguration.|[Så här: Plocka för produktion eller montering](warehouse-how-to-pick-for-production.md)|  
|Planera optimerade plockinstruktioner för ett antal utleveranser i stället för att låta lagerarbetare agera direkt på bokförda utleveranser.|[Så här planerar du plockningar i förslaget](warehouse-how-to-plan-picks-in-worksheets.md)|  
|Plocka artiklar tekniskt för ett visst syfte, till exempel en produktionsenhet som behöver extra komponenter, så att artiklarna inte lämnar distributionslagret tekniskt.|[Så här: plockning och artikelinförsel utan källdokument](warehouse-how-to-create-put-aways-from-internal-put-aways.md)|
|Förstå hur du automatiskt plockar artiklar enligt deras utgångsdatum, till exempel ömtåliga varor.|[Plockning med FEFO](warehouse-picking-by-fefo.md)|
|En plockningsrad delas upp i flera rader, till exempel eftersom det inte finns tillräckligt många artiklar som ska tas från den bestämda lagerplatsen.|[Så här: Dela Dist.lageraktivitetsrader](warehouse-how-to-split-warehouse-activity-lines.md)|
|Få direkt tillgång till plockningar som tilldelats dig som lagerarbetare.|[Så här: Hitta distributionslagertilldelningar](warehouse-how-to-find-your-warehouse-assignments.md)|  

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

