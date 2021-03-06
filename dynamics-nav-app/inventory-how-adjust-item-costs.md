---
title: "Så här justerar du kostnader för artiklar manuellt"
description: "Du kan justera lagervärderingen för en artikel som använder FIFO eller genomsnittliga värderingsprinciper, till exempel när artikelkostnader ändras av andra skäl än transaktioner."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost adjustment, cost forwarding, costing method, inventory valuation, costing
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 40647e0263b7c21c1f085cd6dde449f8210ede10
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-adjust-item-costs"></a>Så här justerar du artikelkostnader
Kostnaden för en artikel (lagervärde) som du köper och senare säljer kan ändras under dess livstid, eftersom till exempel en fraktkostnad läggs till dess inköpkostnad när du har sålt artikeln. Kostnadsjustering är speciellt relevant i situationer där du säljer varor, innan du fakturerar inköpet av dessa varor. För att alltid ha rätt lagervärde måste artikelkostnader därför regelbundet justeras. Detta säkerställer att försäljnings- och vinststatistiken är aktuell och ekonomiska KPI-er är korrekta. Mer information finns i [Designdetaljer: kostnadsjustering](design-details-cost-adjustment.md).

Som regel beräknas värdet i fältet **Styckkostnad** på artikelkortet enligt standardkostnaden för artiklar där värderingsprincipen Standard används. För artiklar där någon annan värderingsprincip används, beräknas värdet baserat på beräkningen av lagersaldot (fakturerade kostnader och förväntade kostnader) dividerat med lagersaldot. Mer information finns i avsnittet "Förstå Styckkost. beräkningstyp".

I [!INCLUDE[d365fin](includes/d365fin_md.md)] justera artikelkostnaderna automatiskt varje gång en lagertransaktion uppstår till exempel när bokföring av en faktura för en artikel.

Du kan också använda en funktion för att justera kostnaderna för en eller flera artiklar. Detta är användbart när du vet att artikelkostnader har ändrats av andra orsaker än artikeltransaktioner.

Artikelkostnaderna justeras av FIFO eller metoden Genomsnittskostnad beroende på ditt val i assisterad konfiguration för **Konfigurera mitt företag** på fältet **Värderingsprincip** på artikelkortet. Mer information finns i [Så här registrerar du nya artiklar](inventory-how-register-new-items.md).  

Om du använder en FIFO-kostnadsmetod är artikelns enhetskostnad det verkliga värdet på en inleverans av artikeln. Lager värders genom att anta att de första artiklarna in i lagret säljs först.

Om du använder metoden Genomsnittskostnad beräknas en artikels enhetskostnad som den genomsnittliga styckkostnaden vid varje tidpunkt efter ett inköp. Lager värderas med förutsättningen att alla lagerartiklar säljs samtidigt. För artiklar som avänder den här värderingsprincipen kan du välja fältet **Styckkostnad** på artikelkortet för att visa tidigare transaktioner som genomsnittskostnaden beräknas från.

Funktionen Kostnadsjustering bearbetar endast värdetransaktioner som inte ännu har justerats. Om en funktion påträffas där ankommande kostnader behöver flyttas fram till kopplade avgående kostnader, görs detta genom att nya justeringsvärdetransaktioner skapas som baseras på informationen i de ursprungliga värdetransaktionerna, men som innehåller justeringsbeloppet. Funktionen Kostnadsjustering använder bokföringsdatumet för den ursprungliga värdetransaktionen om inte det datumet infaller i en avslutad lagerperiod. Om så är fallet används startdatumet för nästa öppna lagerperiod. Om lagerperioder inte används definieras datumet i fältet **Tillåt bokföring fr.o.m.** i fönstret **Redovisningsinställningar** när justeringstransaktionerna bokförs.

## <a name="to-adjust-item-costs-manually"></a>Så här justerar du artikelkostnader manuellt
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Justera kost. - artikeltrans** och välj sedan relaterad länk.
2. I fönstret **Justera kost. - artikeltrans** kan du ange vilka artiklar som du vill justera kostnader för.
3. Välj knappen **OK**.

## <a name="to-make-general-changes-in-the-direct-unit-cost"></a>Så här gör du generella ändringar i inköpspris
Om du vill ändra inköpspriset för flera olika artiklar kan du använda batchjobbet **Justera artikelkost./priser**.  

 När batch-jobbet körs ändras innehållet i fältet **Inköpspris** på artikelkortet. Innehållet i fältet ändras på samma sätt för alla artiklar eller för de artiklar du valt. Värdet i fältet multipliceras med en justeringsfaktor som du anger.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Justera artikelkost./-priser** och välj sedan relaterad länk.  
2. I fältet **Justeringsfält** anger du vilket artikelfält eller lagerställeskortfält du vill justera.  
3. I fältet **Justeringsfaktor** anger du den faktor som ska justera värdet. Ange t.ex. **1,5** för att minska värdet med 50 %.  
4. På snabbfliken **Artikel** ställer du in filter för att ange till exempel vilka artiklar som ska hanteras med batch-jobbet.  
5. Välj knappen **OK**.  

## <a name="understanding-unit-cost-calculation"></a>Förstå beräkning av styckkostnad
Som regel beräknas värdet i fältet **Styckkostnad** på artikelkortet enligt standardkostnaden för artiklar där värderingsprincipen Standard används. För artiklar där någon annan värderingsprincip används, beräknas värdet baserat på beräkningen av lagersaldot (fakturerade kostnader och förväntade kostnader) dividerat med lagersaldot.  

 I de avsnitt som följer beskrivs hur innehållet i fältet **Värderingsprincip** påverkar beräkningen av styckkostnaden vid inköp och försäljningar.  

## <a name="unit-cost-calculation-for-purchases"></a>Beräkna styckkostnad vid inköp  
 När du köper in artiklar kopieras alltid värdet i fältet **Senaste direkt kostnad** på artikelkortet till fältet **Inköpspris** på en inköpsrad eller till raden A-pris på en artikeljournalrad.  

 Ditt val i fältet **Värderingsprincip** påverkar hur [!INCLUDE[d365fin](includes/d365fin_md.md)] beräknar innehållet i fältet **Styckkostnad** på raderna.  

### <a name="costing-method-fifo-lifo-specific-or-average"></a>Värderingsprincip FIFO, LIFO, Serienr eller Genomsnitt  
 [!INCLUDE[d365fin](includes/d365fin_md.md)] beräknar innehållet i fältet **Styckkostnad (BVA)** på inköpsraden eller innehållet i fältet **Styckkostnad** på artikeljournalraden enligt följande formel:  

 Styckkostnad (BVA) = (Inköpspris – (Rabattbelopp/Antal)) x (1 + Indirekt kostnad %/100) + Overheadkostnad  

### <a name="costing-method-standard"></a>Värderingsprincip Standard  
 Fältet **Styckkostnad (BVA)** på inköpsraden, eller fältet **Styckkostnad** på artikeljournalraden, fylls i med värdet i fältet **Styckkostnad** på artikelkortet. Med värderingsprincipen som Standard beräknas detta värde alltid enligt standardkostnaden.  

 När du bokför inköpet kopieras styckkostnaden från inköpsraden eller artikeljournalraden till en transaktionsrad för den inköpta artikeln. Styckkostnaden visas på artikelns transaktionslista.  

### <a name="all-costing-methods"></a>Samtliga värderingsprinciper  
 Innehållet i fältet Kost.belopp aktuellt, eller i vissa fall fältet **Kost.belopp (faktisk)** eller, om tillämpligt, fältet **Kost.belopp (förväntat)** för den här artikeltransaktionen, beräknas alltid enligt styckkostnaden från raden i källdokumentet, oavsett vilken värderingsprincip som används för artikeln.  

## <a name="unit-cost-calculation-for-sales"></a>Beräkning av styckkostnad vid försäljning  
 När du säljer artiklar, kopieras styckkostnaden från fältet Styckkostnad på artikelkortet till försäljnings- eller artikeljournalraden.  

 När du bokför, kopieras styckkostnaden till en rad på försäljningsfakturan. Styckkostnaden visas på artikelns transaktionslista. [!INCLUDE[d365fin](includes/d365fin_md.md)] använder styckkostnaden från källdokumentraden för att beräkna innehållet i **Kost.belopp (aktuellt)** eller, om tillämpligt, fältet **Kost.belopp(förväntat)** oavsett vilken värderingsprincip som används för artikeln.  

## <a name="see-also"></a>Se även
[Hantera lagerkostnader](finance-manage-inventory-costs.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Försäljning](sales-manage-sales.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

