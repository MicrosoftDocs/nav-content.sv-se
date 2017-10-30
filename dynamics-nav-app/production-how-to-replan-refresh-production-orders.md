---
title: Omplanera eller uppdatera produktionsorder direkt
description: "Produktionsorderraderna innehåller de artiklar som ska produceras i produktionsordern."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 424fddfb1f92f426badec5477267be7477c3be22
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-replan-or-refresh-production-orders-directly"></a>Omplanera eller uppdatera produktionsorder direkt
Funktionen **Omplanera** på produktionsorder används vanligtvis när du har lagt till eller ändrat komponenter som utgör underliggande produktionsorder. Funktionen beräknar de ändringar som gjorts på komponent- och operationsföljdsrader, och artiklar på lägre produktionsstrukturnivåer beaktas. Detta innebär att nya produktionsorder kan skapas för dessa artiklar.  

Funktionen Omplanera utgår ifrån de ändringar som du har gjort på komponent- och operationsföljdsrader, och beräknar och planerar för eventuella nya behov för produktionsordern.  

Funktioen **uppdatera** för produktionsorder används vanligtvis när du har gjort något av följande:

- Skapat ett produktionsorderhuvud manuellt för att beräkna och skapa radinformation för första gången.
- Gjort ändringar i produktionsorderhuvudet för att beräkna om all radinformation.

Uppdateringsfunktionen beräknar de ändringar som gjorts i ett produktionsorderhuvud, och produktionsstrukturnivåer beaktas inte. Funktionen beräknar och initierar värdena på komponent- och operationsföljdsrader utifrån de standarduppgifter som har angetts i den tilldelade produktionsstrukturen och operationsföljden, och enligt den orderkvantitet och förfallodatum som har angetts i produktionsorderhuvudet.

Du kan antingen infoga produktionsorderraderna manuellt eller använda en funktion som beräknar produktionsorderraderna från huvudet.  

> [!NOTE]
 Om du använder funktionen Uppdatera för att omberäkna produktionsorderraderna kommer de gamla produktionsorderraderna tas bort och nya beräknas.  

## <a name="to-replan-a-production-order"></a>Så här planerar du om en produktionsorder  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Fasta planerade prod.order** och välj sedan relaterad länk.  
2.  Öppna den produktionsorder som du vill omplanera.  
3.  På snabbfliken **Rader** väljer du åtgärden **Rader** och väljer sedan åtgärden **Komponenter**.  
4.  Lägg till en komponent som är en producerad artikel eller halvfabrikat.  
5.  Från produktionsordern väljer du åtgärden **Omplanera**.  

    I fönstret **Omplanera produktionsorder** anger du vad som ska omplaneras och hur:  
6.  I fältet **Planeringsriktning**, välj ett av följande alternativ.  

    |Alternativ|Description|  
    |----------------------------------|---------------------------------------|  
    |**Tillbaka**|Beräknar operationssekvensen baklänges från det tidigaste möjliga slutdatumet, som definieras genom förfallodatumet och/eller andra planerade ordrar, till det senaste möjliga startdatumet. **Obs!**  Det här är standardalternativet, som fungerar i de flesta situationer.|  
    |**Framåt**|Beräknar operationssekvensen framåt från det senaste möjliga startdatumet, som definieras genom förfallodatumet och/eller andra planerade ordrar, till det tidigaste möjliga slutdatumet. **Obs!**  Detta alternativ fungerar endast för snabborder.|  

7.  I fältet **Planera** anger du om produktionsbehov för producerade artiklar i produktionsstrukturen ska beräknas:  

    |Alternativ|Description|  
    |----------------------------------|---------------------------------------|  
    |**Inga nivåer**|Produktion på lägre nivåer beaktas inte. Detta innebär att endast artikelns plan uppdateras (som vid en uppdatering).|  
    |**En nivå**|Planera för produktionsbehov på en nivå. Produktionsorder kan skapas på första nivån.|  
    |**Alla nivåer**|Planera för produktionsbehov på alla nivåer. Produktionsorder kan skapas på alla nivåer.|  

8.  Välj **En nivå** och klicka på **OK** om du vill omplanera produktionsordern samt beräkna och skapa en ny underliggande produktionsorder för det nya halvfabrikatet, om det inte är helt tillgängligt.  

> [!NOTE]  
>  De ändringar som genomförs via funktionen **Omplanering** ändrar förmodligen kapacitetsbehovet i produktionsordern, och du kan därför behöva planera om operationer när du har uppdaterat.  

## <a name="to-refresh-a-production-order"></a>Så här uppdaterar du en produktionsorder  
Om du har ändrat produktionsorderrader, komponenter eller operationsföljdrader måste du också uppdatera informationen i produktionsordern. I följande procedur beräknas komponenterna för en fast planerad produktionsorder. Momenten är liknande för operationsföljdsrader.

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Fast planerad prod.order** och välj sedan relaterad länk.  
2.  Välj åtgärden **Ny**. Mer information finnsi [Så här skapar du ett produktionsorder](production-how-to-create-production-orders.md).  
3.  Välj åtgärden **Uppdatera**.
4. Du kan välja en av följande alternativ i fönstret **Uppdatera produktionsorder**:

    |Alternativ|Description|  
    |----------------------------------|---------------|---------------------------------------|  
    |**Planeringsriktning**|**Framåt**|Planeringen börjar vid startdatumet och fortsätter framåt till slutdatumet. Du måste fylla i startdatumet om du vill använda det här alternativet.|  
    ||**Bakåt**|Planeringen börjar vid slutdatumet och fortsätter bakåt till startdatumet.|  
    |**Beräkna**|**Rader**|Markera det här fältet om du vill beräkna produktionsorderrader.|  
    ||**Operationsföljder**|Det här fältet påverkar inte beräkningen av produktionsrader.|  
    ||**Komponentbehov**|Det här fältet påverkar inte beräkningen av produktionsrader.|  
    |**Dist.lager**|**Skapa ingående rekvisition**|Det här fältet påverkar inte beräkningen av produktionsrader.|  

5. Klicka på knappen **OK** för att bekräfta ditt val. Nu har produktionsorderraderna beräknats.

> [!NOTE]  
>  När du beräknar produktionsorderkomponenter tas tidigare gjorda ändringar i komponenterna bort.

## <a name="see-also"></a>Se även  
[Planerad](production-planning.md)  
[Ställa in Produktion](production-configure-production-processes.md)  
[Produktion](production-manage-manufacturing.md)    
[Lagersaldo](inventory-manage-inventory.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Designdetaljer: Leveransplanering](design-details-supply-planning.md)   
[Skapa metodtips: leveransplanering](setup-best-practices-supply-planning.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

