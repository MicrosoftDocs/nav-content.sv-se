---
title: "Datumberäkning för inköp"
description: "Programmet beräknar automatiskt det datum då du måste beställa en artikel som du vill ha i lager på ett visst datum. Det är detta datum då du kan förvänta dig att artiklar som beställts ett visst datum ska vara tillgängliga för plockning."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f3f87311f0971b2901852a9aa0c766c6c806190
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="date-calculation-for-purchases"></a>Datumberäkning för inköp
I [!INCLUDE[d365fin](includes/d365fin_md.md)] beräknas automatiskt det datum då du måste beställa en artikel som du vill ha i lager på ett visst datum. Det är detta datum då du kan förvänta dig att artiklar som beställts ett visst datum ska vara tillgängliga för plockning.  

Om du anger ett begärt inleveransdatum i en inköpsorderhuvud, är det beräknade orderdatumet det datum då ordern måste placeras för inleverans av artiklarna på datumet som du valde. Då beräknas datumet då artiklarna är tillgängliga för plockning och visas i fältet **Förväntat inleveransdatum**.  

Om inget begärt inleveransdatum anges används orderdatumet på raden som utgångspunkt när programmet beräknar det datum då du kan förvänta dig att ta emot artiklarna och det datum då artiklarna kommer att vara tillgängliga för plockning.  

## <a name="calculating-with-a-requested-receipt-date"></a>Beräkna med ett begärt inleveransdatum  
Om ett begärt inleveransdatum angetts på inköpsorderraden används detta datum som utgångspunkt i följande beräkningar:  

- begärt inleveransdatum – ledtidsberäkning = orderdatum  
- begärt inleveransdatum + ankommande lagerhanteringstid + säkerhetsledtid = förväntat inleveransdatum  

Om du angett ett begärt inleveransdatum i inköpsorderhuvudet kopieras detta datum till motsvarande fält på alla raderna. Du kan ändra datumet på raderna eller ta bort datumet på raden.  

## <a name="calculating-without-a-requested-delivery-date"></a>Beräkna utan begärt leveransdatum  
Om du skriver in en inköpsorderrad utan ett begärt leveransdatum fylls fältet **Orderdatum** i automatiskt med datumet i fältet **Orderdatum** i inköpshuvudet. Detta datum är antingen det datum du angett eller arbetsdatumet. Därefter utförs följande datumberäkningar för inköpsorderraden, med utgångspunkt från orderdatumet:  

- orderdatum + ledtidsberäkning = planerat inleveransdatum.  
- planerat inleveransdatum + ankommande lagerhanteringstid + säkerhetsledtid = förväntat inleveransdatum  

Om du ändrar orderdatumet på raden, t.ex. om artiklarna inte är tillgängliga hos leverantören förrän vid ett senare datum, beräknas de aktuella datumen automatiskt om på raden.  

Om du ändrar orderdatumet i huvudet kopieras detta datum till fältet **Orderdatum** på samtliga rader, varefter alla relaterade datumfält beräknas om.  

## <a name="see-also"></a>Se även  
 [Datumberäkning för försäljning](sales-date-calculation-for-sales.md)   
 [Så här beräknar du ett orderlöftesdatum](sales-how-to-calculate-order-promising-dates.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

