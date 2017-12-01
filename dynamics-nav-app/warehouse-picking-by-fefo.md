---
title: "Så här: Aktivera plockning med FEFO"
description: "FEFO-metoden (First-Expired-First-Out) är en sorteringsmetod som säkerställer att de äldsta artiklar, de med de tidigaste utgångsdatumen, plockas först."
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
ms.openlocfilehash: d3977cd235293d685490464e51aec16a95d01e9d
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-picking-items-by-fefo"></a>Så här: Aktivera plockning av artiklar med FEFO
FEFO-metoden (First-Expired-First-Out) är en sorteringsmetod som säkerställer att de äldsta artiklar, de med de tidigaste utgångsdatumen, plockas först.  

 Den här funktionen fungerar bara, när dessa villkor är uppfyllt:  

-   Artikel måste ha en serie-/partinummer.  
-   På artikelns artikelspårningskod har angetts, fältet **SN specifik spårning för dist.lager** , eller **Parti specifik spårning distr.lager** måste väljas.  
-   Artikeln måste bokföras till lagret med ett utgångsdatum.  
-   På lagerställekortet måste kryssrutan **Begär plockning** vara markerad.  
-   Kryssrutan **Plocka enligt FEFO** på lagerställekortet måste vara markerat.  
-   På lagerställekortet måste kryssrutan **Lagerplats ska finnas** vara markerad.  

 När alla kriterier uppfylls, sorteras serie-/partinumrerade artiklar som ska plockas med de äldsta första alla plockningar och transporter, utom artiklar som använder SN-närmare visst eller partispecifik spårning.  

> [!NOTE]  
>  Om någon serie-/partinumrerade artiklar använder specifik spårning, är de respekterade först och under dem, listas de återstående, icke-specifika serie-/partinummer enligt FEFO.  

 Om två serie-/partinumrerade artiklar har samma utgångsdatum, väljs artikeln med det lägsta serie - eller partinummer. Om serie - eller partinummer är samma, väljs artikeln som registrerades först.  

> [!NOTE]  
>  -   När du plockar serie-/partinumrerade artiklar på lagerplatser som har ställs in för dirigerad artikelinförsel och plockning, plockas bara kvantiteter på lagerplatser av typen *Plock* enligt FEFO.  
> -   Om du vill aktivera transporter enligt FEFO antingen i **lagerförflyttning** fönster eller **Transportförslag** fönstret, måste du lämna **Från binge** fältet tomt.  
> -   Om fältet **Endast utgångsbokföring** är markerat kommer endast artiklar som inte har förfallit att tas med i plockningen. Detta gäller även om du inte använder plockning enligt FEFO.  

## <a name="see-also"></a>Se även  
[Plocka artiklar](warehouse-pick-items.md)   
[Så här: plocka artiklar för Dist.lager utleverans](warehouse-how-to-pick-items-for-warehouse-shipment.md)   
[Så här plockar du artiklar med Lagerplockning](warehouse-how-to-pick-items-with-inventory-picks.md)   
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

