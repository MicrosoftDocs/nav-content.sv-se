---
title: "Så här skapar du lagerställeenheter"
description: "Du kan använda lagerställeenheter för att registrera artikelinformation som rör ett visst lagerställe eller en viss variantkod."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b52cfedfa7e5d6b375ef3040764ba74a151d3550
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-stockkeeping-units"></a>Så här skapar du lagerställeenheter
Du kan använda lagerställeenheter för att registrera artikelinformation som rör ett visst lagerställe eller en viss variantkod.  

 Lagerplatsenheter fungerar som komplement till artikelkort. De ersätter dem inte även om de är relaterade till dem. Med lagerställeenheter kan du ha olika information om en artikel på ett visst lagerställe (t.ex. ett distributionslager eller ett distributionscenter) eller om en särskild variant, (t.ex. olika hyllnummer och olika återanskaffningsinformation) av samma artikel.  

## <a name="to-set-up-a-stockkeeping-unit"></a>Så här skapar du lagerställeenheter  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställeenheter**, och välj sedan relaterad länk.  
2.  Välj åtgärden **Ny**.  
3.  Fyll i fälten på kortet. Följande fält är obligatoriska: **Artikelnr**, **Lagerställekod**och/eller **Variantkod**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

När du har skapat den första lagerställeenheten för en artikel, markeras kryssrutan **Lagerställeenhet finns** på **artikelkortet**.  

Om du vill skapa flera lagerställeenheter för en artikel, kan du använda batch-jobbet **Skapa lagerställeenhet**.  

> [!NOTE]  
>  Informationen på **lagerställeenhetskortet** har högre prioritet än informationen på **artikelkortet**.  

## <a name="see-also"></a>Se även  
[Så här registrerar du nya objekt](inventory-how-register-new-items.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

