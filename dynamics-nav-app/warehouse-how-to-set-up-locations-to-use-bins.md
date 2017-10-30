---
title: "Så här: Lägger du upp lagerställen för att använda lagerplatser"
description: "Lagerplatser representerar den grundläggande lagerstrukturen och används för att göra förslag om artiklarnas specifika placering av artiklar. När du har skapat lagerplatserna kan du definiera det innehåll som du vill placera på respektive lagerplats, eller så kan lagerplatsen fungera som en flytande lagerplats utan att något särskilt innehåll har angetts."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 95b36b6eed79da868c1e41905110788c90f24829
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-locations-to-use-bins"></a>Så här: Lägger du upp lagerställen för att använda lagerplatser
Lagerplatser representerar den grundläggande lagerstrukturen och används för att göra förslag om artiklarnas specifika placering av artiklar. När du har skapat lagerplatserna kan du definiera det innehåll som du vill placera på respektive lagerplats, eller så kan lagerplatsen fungera som en flytande lagerplats utan att något särskilt innehåll har angetts.  

Om du vill använda lagerplatsfunktionerna på ett lagerställe måste du först aktivera dessa på kortet **Lagerställe**. Sedan designar du artikelflödet på lagerstället, genom att ange inställningar för lagerplatskoder i fältet som representerar de olika flödena.  

> [!NOTE]  
>  Innan du kan ange lagerplatskoder på lagerställekortet, måste lagerplatskoderna skapas. Mer information finns i [Så här: Skapa lagerplatser](warehouse-how-to-create-individual-bins.md).  

## <a name="to-set-up-a-location-to-use-bins"></a>Så här lägger du upp ett lagerställe för att använda lagerplatser  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.  
2.  Välj lagerstället där du vill använda lagerplatser.  
3.  Välj åtgärden **Redigera**.  
4.  Markera fältet **Lagerplats ska finnas** på kryssrutan **Dist.lager**.  
5.  Om du inte använder dirigerad artikelinförsel och plockning för ett lagerställe fyller du i fältet **Standard lagerplatsval** med den metod som ska användas för att tilldela en standardlagerplats till en artikel.  
6.  Öppna kortet för den plats som du vill ställa in lagerplatser för.
7.  På snabbfliken **Lagerplatser** väljer du de lagerplatser som du vill använda som standard för inleveranser, utleveranser samt ankommande, avgående och öppna produktionslagerplatser.  
8.  De lagerplatskoder som du fyller i här visas automatiskt i huvudena och på raderna för olika distributionslagerdokument. Standardlagerplatserna definierar alla start- och slutplaceringar av artiklar i distributionslagret.  
9.  Om du använder dirigerad artikelinförsel och plockning väljer du en lagerplats för distributionslagerjusteringarna. Lagerplatskoden i **Justering lagerplatskod** fältet anger den virtuella lagerplats där avvikelser i lagret registreras, när du registrerar antingen observerade avvikelser som har registrerats i dist.lagerartikeljournalen, eller avvikelser beräknade när du registrerar en fysiskt dist.lager.  
10. Fyll i fälten på snabbfliken **Lagerplatsprinciper** om de är relevanta för distributionslagret. De viktigaste fälten är **Lagerplats kapacitetsprincip**, **Tillåt brytenhet** och **Artikelinförsel mallkod**.  
11. På snabbfliken **Dist.lager** fyller du i fälten **Avgående lagerhanteringstid**, **Ankommande lagerhanteringstid** och **Baskalenderkod**. Mer information finns i [Så här lägger du upp baskalendrar](across-how-to-assign-base-calendars.md).

## <a name="filling-the-consumption-bin"></a>Fylla förbrukningslagerplatsen
Diagrammet visar hur **Lagerplatskod** på produktionsorderkomponentraderna fylls enligt platsinställningen.

![Flödesschema för lagerplats](media/binflow.png "BinFlow")  

## <a name="see-also"></a>Se även
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

