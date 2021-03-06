---
title: "Datumberäkning för försäljning"
description: "Programmet beräknar automatiskt det datum då du måste beställa en artikel som du vill ha i lager på ett visst datum. Det är detta datum då du kan förvänta dig att artiklar som beställts ett visst datum ska vara tillgängliga för plockning."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 72e8f2a2f1d2d6427c716205da7ecee58b85bcc6
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="date-calculation-for-sales"></a>Datumberäkning för försäljning
I [!INCLUDE[d365fin](includes/d365fin_md.md)] beräknas automatiskt tidigast möjliga leveransdatum för en artikel på en försäljningsorderrad.

Om kunden har begärt ett särskilt leveransdatum beräknas det datum då artiklarna måste vara tillgängliga för plockning så att varorna faktiskt ska kunna levereras på angiven dag.

Om inget bestämt leveransdatum begärts beräknas det datum då artiklarna kan levereras, med utgångspunkt från det datum då artiklarna är tillgängliga för plockning.

## <a name="calculating-a-requested-delivery-date"></a>Beräkna ett begärt leveransdatum
Om du anger ett begärt leveransdatum på försäljningsorderraden används detta datum som utgångspunkt för följande beräkningar.

- begärt leveransdatum - leveranstid = planerat utleveransdatum
- planerat utleveransdatum - avgående lagerhanteringstid = utleveransdatum

Om artiklarna kan plockas på utleveransdatumet kan försäljningsprocessen fortsätta.

Om artiklarna inte kan plockas på utleveransdatumet visas en varning om att varan inte finns i lager.

## <a name="calculating-the-earliest-possible-delivery-date"></a>Beräkna tidigaste möjliga leveransdatum
Om du inte har angett ett begärt leveransdatum på försäljningsorderraden, eller om det begärda leveransdatumet inte kan godtas, beräknas det tidigaste datum då artiklarna är tillgängliga. Detta datum anges automatiskt i fältet Leveransdatum på raden. Det datum då du planerar att utleverera artiklarna liksom det datum då varorna kan levereras till kunden beräknas med hjälp av följande formler.

- planerat utleveransdatum + avgående lagerhanteringstid = planerat utleveransdatum
- planerat utleveransdatum +- leveranstid = planerat leveransdatum


## <a name="see-also"></a>Se även  
 [Datumberäkning för inköp](purchasing-date-calculation-for-purchases.md)   
 [Så här beräknar du ett orderlöftesdatum](sales-how-to-calculate-order-promising-dates.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

