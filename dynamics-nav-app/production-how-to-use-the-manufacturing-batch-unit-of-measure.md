---
title: "Så här kan du använda enheten för produktionsbatch"
description: "Om en artikel lagerförs med en enhet men tillverkas med en annan, måste produktionsordern använda en enhet för produktionsbatch för att beräkna rätt antal komponenter. Ett exempel på beräkning med en enhet för produktionsbatch är när tillverkade artiklar lagerförs styckvis, men tillverkas tonvis."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cf0c91b076f473c12e61ce82d870a66e352c1920
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-manufacturing-batch-units-of-measure"></a>Så här kan du arbeta med enheter för produktionsbatch
Om en artikel lagerförs med en enhet men tillverkas med en annan, kan du skapa en produktionsorder som använder enheten för produktionsbatch för att beräkna rätt antal komponenter under batch-jobbet **Uppdatera produktionsorder**. Ett exempel på beräkning med en enhet för produktionsbatch är när tillverkade artiklar lagerförs styckvis, men tillverkas tonvis.  

## <a name="to-create-a-production-bom-using-a-batch-unit-of-measure"></a>Så här skapar du en produktionsstruktur med hjälp av en batchenhet  
1.  Enheten för produktionsbatchen anges som en alternativ enhet i fönstret **Artikelenheter** för den artikel som ska tillverkas. Batchenheten kommer inte att ersätta basenheten för artikeln.  
2.  Skapa en produktionsstruktur för den artikel som har angetts med enheten för produktionsbatch. För mer information, se [Så här skapar du produktionsstrukturer](production-how-to-create-production-boms.md).  
3.  Markera enhetskod för produktionsbatch i fältet **Enhetskod**.  
4.  I fältet **Antal per** anger du det antal av komponentartikeln som krävs för att skapa den här batchenheten för varje produktionsstrukturrad.  
5.  Öppna **Artikelkort** för den kopplade artikeln.  

    Klicka på snabbfliken **Återanskaffning**. I fältet **Prod.struktursnr** väljer du den produktionsstruktur som skapades ovan.  
6.  Skapa ett produktionsorderhuvud med hjälp av den artikel som har angetts med enheten för produktionsbatch. Mer information finnsi [Så här skapar du ett produktionsorder](production-how-to-create-production-orders.md).  
7.  Välj åtgärden **Uppdatera** och sedan knappen **OK**.  

På snabbfliken **Rader** väljer du åtgärden **Rad** och väljer sedan åtgärden **Komponenter** för att visa resultatet. I programmet beräknas det rätta antalet komponenter som krävs för att uppfylla produktionsstrukturen baserat på enheten för produktionsbatch.  

## <a name="to-calculate-a-manufacturing-batch-unit-of-measure-on-a-production-order"></a>Så här beräknar du en enhet för produktionsbatch i en produktionsorder  
1.  Skapa ett produktionsorderhuvud med hjälp av den artikel som har angetts med enheten för produktionsbatch.  
2.  I fältet **Artikelnr** på produktionsorderraden anger du samma artikelnummer som användes i huvudet.  
3.  I fältet **Antal** anger du samma antal som användes i huvudet.  
4.  Markera enhetskod för produktionsbatch i fältet **Enhetskod**.  
5.  Välj åtgärden **Uppdatera**.
6.  På snabbfliken **Beräkna** avmarkerar du kryssrutan **Rader**.  
7.  Välj knappen **OK**.  
8.  På snabbfliken **Rader** väljer du åtgärden **Rad** och väljer sedan åtgärden **Komponenter** för att visa resultatet. Det rätta antalet komponenter som krävs för att uppfylla produktionsstrukturen beräknas baserat på enheten för produktionsbatch.  

## <a name="see-also"></a>Se även  
[Så här skapar du operationsföljder](production-how-to-create-routings.md)  
[Så här skapar du nya produktionsstrukturer](production-how-to-create-production-boms.md)     
[Ställa in Produktion](production-configure-production-processes.md)  
[Produktion](production-manage-manufacturing.md)    
[Planerad](production-planning.md)   
[Lagersaldo](inventory-manage-inventory.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

