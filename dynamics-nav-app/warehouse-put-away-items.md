---
title: "Införa artiklar"
description: "Lageraktiviteten att införa artiklar efter att de har inlevererats eller producerats utförs på olika sätt beroende på hur lagerstyrningsfunktionerna har konfigurerats."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0b68ef1b4c73eef1ac82d59587011a0fcdead096
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="putting-items-away"></a>Införa utflöde från artiklar
Lageraktiviteten att införa artiklar efter att de har inlevererats eller producerats utförs på olika sätt beroende på hur lagerstyrningsfunktionerna har konfigurerats. Hur komplex det är kan sträcka sig från inga lagerkonfigurationer, till grundläggande lagerstyrning med hantering av order för order i en eller flera aktiviteter samt avancerade konfigurationer där alla lageraktiviteter måste utförs i ett dirigerat arbetsflöde. Mer information finns i [Ställa in Lagerstyrning](warehouse-setup-warehouse.md).

Om du vill organisera och registrera införselaktiviteter med distributionslagerdokument markerar du fältet **Begär artikelinförsel** på lagerställekortet. Det indikerar att om du har artiklar som kommer till lagerstället via ett ankommande källdokument, ska införseln av artiklarna hanteras via, och kontrolleras av programmet. Det ankommande källdokumentet kan vara in inköpsorder, en försäljningsreturorder, en ankommande överföringsorder eller en produktionsorder vars utflöde är klart för artikelinförsel.  

Om lagerstället kräver artikelinförselbearbetning, men inte kräver inleveransbearbetning, använder du fönstret **Lagerartikelinförsel** om du vill organisera eller skriva ut information om artikelinförseln, ange resultat av faktisk artikelinförsel eller bokföra artikelinförselinformation. Om du bokför artikelinförselinformation bokförs i sin tur inleveransinformationen för källdokumentet.

Om lagerstället kräver både inleveransbearbetning och artikelinförselbehandling, så att du har placerat markeringar i både **Begär inleveranser** och **Begär artikelinförsel** på lagerställekortet, finns det en annan process som används för att införa artiklar. I det här fallet ska du använda **Dist.lager artikelinförsel** fönstret att hantera artikelinförsel. Dist.lager artikelinförsel fungerar på samma sätt som Lagerartikelinförsel, förutom att du registrerar artikelinförseln istället för att bokföra informationen. Observera att registrering av artikelinförsel inte bokför inleveransen för artiklarna. Den uppdateras bara lagerplatsinnehåll. Du lagerchef kan du använda ett artikelinförselförslag för att organisera artikelinförselinformationen innan du skapar de individuella artikelinförselinstruktionerna.

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.   

|**Om du vill**|**Gå till**|  
|------------|-------------|  
|Bokför inleveransen av artiklar direkt från det ankommande orderdokumentet och därmed registrera införseln, eftersom det finns någon lagerkonfiguration.|[Så här inlevererar du artiklar](warehouse-how-receive-items.md)|  
|Införa artiklar order för order och bokföra inleveransen i samma aktivitet, i en grundläggande lagerkonfiguration.|[Så här: Införa artiklar med lagerartikelinförslar](warehouse-how-to-put-items-away-with-inventory-put-aways.md)|  
|Införa artiklar för flera order i en avancerad lagerkonfiguration.|[Så här: Införa artiklar med dist.lager artikelinförsel](warehouse-how-to-put-items-away-with-warehouse-put-aways.md)|  
|Införa producerade eller monterade artiklar i engrundläggande eller avancerad lagerkonfiguration.|[Så här för du in Produktions- eller monteringsutflöde](warehouse-how-to-put-away-production-output.md)|
|Planera optimerade införselinstruktioner för ett antal bokförda lagerinleveranser i stället för att lagerarbetare agerar direkt på inleveranser.|[Så här: Planera artikelinförsel i förslaget](warehouse-how-to-plan-put-aways-in-worksheets.md)|  
|Lägga tillbaka artiklar som har plockats tekniskt med en intern plockning, till exempel för en produktionsorder som inte förbrukat det förväntade antalet.|[Så här: plockning och artikelinförsel utan källdokument](warehouse-how-to-create-put-aways-from-internal-put-aways.md)|
|Dela upp en införselrad för att placera en del av införselantalet på tillgängliga lagerplatser eftersom den bestämda lagerplatsen är full.|[Så här: Dela Dist.lageraktivitetsrader](warehouse-how-to-split-warehouse-activity-lines.md)|
|Få direkt tillgång till införslar som tilldelats dig som lagerarbetare.|[Så här: Hitta distributionslagertilldelningar](warehouse-how-to-find-your-warehouse-assignments.md)|    

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

