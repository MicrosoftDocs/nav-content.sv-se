---
title: "Så här beräknar du ett orderlöftesdatum"
description: "Orderlöftesfunktionen är ett verktyg för att beräkna det första möjliga datum då en artikel är disponibel för leverans. Funktionen skapar också inköpsförslagsrader för de datum som du accepterar."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5c2167397d95d04c937ddf1820e6e9edff906b2f
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-order-promising-dates"></a>Så här beräknar du ett orderlöftesdatum
Ett företag måste kunna informera sina kunder om orderleveransdatum. Fönstret **Orderlöftesrader** ger dig möjlighet att göra detta från en försäljningsorderrad.  

Baserat på en artikels kända och förväntade dispositionsdatum beräknas utleverans- och leveransdatum omedelbart i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Datum kan sedan utlovas till kund.  

Om du anger ett begärt leveransdatum på försäljningsorderraden används detta datum som utgångspunkt för följande beräkningar.  

- begärt leveransdatum - leveranstid = planerat utleveransdatum  
- planerat utleveransdatum - avgående lagerhanteringstid = utleveransdatum  

Om artiklarna kan plockas på utleveransdatumet kan försäljningsprocessen fortsätta. Om artiklarna inte kan plockas på utleveransdatumet visas en varning om att varan inte finns i lager.  

Om du inte har angett ett begärt leveransdatum på försäljningsorderraden, eller om det begärda leveransdatumet inte kan godtas, beräknas det tidigaste datum då artiklarna är tillgängliga. Detta datum anges automatiskt i fältet **Leveransdatum** på raden. Det datum då du planerar att utleverera artiklarna liksom det datum då varorna kan levereras till kunden beräknas med hjälp av följande beräkningar.  

- planerat utleveransdatum + avgående lagerhanteringstid = planerat utleveransdatum  
- planerat utleveransdatum +- leveranstid = planerat leveransdatum  

## <a name="about-order-promising"></a>Om Orderlöfte
Med funktionen Orderlöfte kan du lova att en order ska levereras på ett visst datum. Det datum då en artikel är disponibel eller kapabel att lova beräknas och orderrader skapas för de datum som du accepterar. Funktionen är ett verktyg för att beräkna det första möjliga datum då en artikel är disponibel för leverans. Funktionen skapar också inköpsförslagsrader, om artiklar måste först vara inköp för de datum som du accepterar.

[!INCLUDE[d365fin](includes/d365fin_md.md)] använder två grundläggande begrepp:  

- Disponibelt att lova (ATP)  
- Kapabel att lova (CTP)  

### <a name="available-to-promise"></a>Disponibelt att lova  
Disponibelt att lova (ATP) beräknar datum baserat på reservationssystemet. Det utför en tillgänglighetskontroll av det icke reserverade antalet i lager med hänsyn till planerad produktion, inköp, överföringar och returer. Baserat på de här uppgifterna beräknas automatiskt kundbeställningens leveransdatum i [!INCLUDE[d365fin](includes/d365fin_md.md)] eftersom artiklarna är disponibla, antingen i lagret eller i planerade inleveranser.  

### <a name="capable-to-promise"></a>Kapabel att lova  
Kapabel att lova (CTP) utgår från vad som händer om t.ex. artikeln inte finns i lager och inga order har planerats. Med hjälp av det här scenariot beräknas i [!INCLUDE[d365fin](includes/d365fin_md.md)] det tidigaste datum då artikeln kan vara tillgänglig, om det ska produceras, köpas in eller överföras.  


### <a name="calculations"></a>Beräkningar  
När kundens leveransdatum beräknas i [!INCLUDE[d365fin](includes/d365fin_md.md)] utförs två uppgifter:  

- Beräkning av tidigast möjliga leveransdatum när kunden inte har begärt ett visst leveransdatum.  
- Kontroll om det leveransdatum som kunden har begärt, eller som har utlovats till kunden, är realistiskt.  

Om kunden inte begär ett visst leveransdatum anges leveransdatum till arbetsdatum, och tillgänglighet baseras sedan på det datumet. Om artikeln finns i lager beräknar [!INCLUDE[d365fin](includes/d365fin_md.md)] framåt i tiden för att kunna bestämma när ordern kan levereras. Det utförs med hjälp av följande formler:  

- Utleveransdatum + Tid för avgående lagerhantering + Planerat utleveransdatum + Hanteringstid = Datum  
- Planerat utleveransdatum + Leveranstid = Planerat leveransdatum  

[!INCLUDE[d365fin](includes/d365fin_md.md)] verifierar sedan om beräknat leveransdatum är realistiskt. Det beräknar bakåt i tiden så att det blir möjligt att fastställa när artikeln måste vara tillgänglig på det utlovade datumet. Det utförs med hjälp av följande formler:  

- Planerat leveransdatum - Leveranstid = Planerat utleveransdatum  
- Planerat utleveransdatum - Tid för avgående lagerhantering = Utleveransdatum  

Utleveransdatum används för att göra tillgänglighetskontrollen. Om artikeln är tillgänglig på detta datum bekräftar [!INCLUDE[d365fin](includes/d365fin_md.md)] bekräftar att den begärda/utlovade leveransen kan ske. Det görs genom att ange det planerade leveransdatum på samma dag som det begärda/utlovade leveransdatum. Om artikeln är inaktiverad returneras ett tomt datum och orderhandläggaren kan då använda CTP-funktionen.  

Baserat på nya datum och tider beräknas alla relaterade datum enligt de formler som definierats tidigare i det här avsnittet. CTP-beräkningen tar längre tid, men den ger det exakta datumet för när kunden kan vänta sig leverans av artikeln. De datum som beräknas från CTP presenteras i **planerat leveransdatum** och **tidigaste leveransdatum** i fönstret **Orderlöftesrader**.  

Orderhandläggaren slutför CTP-processen genom att acceptera datum. Det innebär att en planeringsrad och en reservationstransaktion har skapats för artikeln före beräknade datum så att ordern kan uppfyllas.  

Förutom ett externt orderlöfte som du kan utföra i fönstret **Orderlöftesrader** kan du också utlova interna eller externa leveransdatum för strukturartiklar. Mer information finns i [så här: Visa tillgängliga objekt ](inventory-how-availability-overview.md).

## <a name="to-set-up-order-promising"></a>Så här skapar du orderlöfte  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Orderlöfte inställning** och välj sedan relaterad länk.  
2. Ange ett nummer och en tidsenhetskod i fältet **Offset (tid)**. Välj en av följande koder.  

    |Kod|Beskrivning|  
    |----------|-----------------|  
    |**d**|Kalenderdag|  
    |**a**|Vecka|  
    |**m**|Månad|  
    |**q**|Kvartal|  
    |**y**|År|  

    "3v" anger till exempel att offset-tiden är tre veckor. Använd "c" som ett prefix för alla de här koderna när du ska ange aktuell period. Om du t.ex. vill att offset-tiden ska vara den aktuella månaden skriver du **cm**.  
3. Ange en nummerserie i fältet **Orderlöfte nr-serie** genom att markera en rad från listan i fönstret **Nr-serier**.  
4. Ange en orderlöftesmall i fältet **Orderlöftesmall** genom att välja en rad från listan i fönstret **Inköpsförslagsmallista**.  
5. Ange ett inköpsförslag i fältet **Orderlöftesförslag** genom att markera en rad från listan i fönstret **Inköpsförslagsnamn**.

### <a name="to-enter-inbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Så här anger du ankommande lagerhanteringstid i lagerinställningarna  
Om du vill ange en ankommande lagerhanteringstid som ska tas med i orderlöftesberäkningen på inköpsraden, kan du ange tiden som standard för lagret och för lagerstället.    
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerinställningar** och välj sedan relaterad länk.  
2. I fältet **Ankommande lagerhanteringstid** på snabbfliken **Allmänt** anger du det antal dagar som ska tas med i orderlöftesberäkningen.  

> [!NOTE]  
>  Om du har fyllt i fältet **Ankommande lagerhanteringstid** på **lagerställekortet** för lagerstället, används värdet i detta fält som standard för ankommande lagerhanteringstid.  

### <a name="to-enter-inbound-warehouse-handling-time-on-location-cards"></a>Så här anger du ankommande lagerhanteringstid på lagerställekort  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställe** och välj sedan relaterad länk.  
2.  Öppna önskat lagerställekort.  
3.  I fältet **Ankommande lagerhanteringstid** på snabbfliken **Lager** anger du det antal dagar som ska tas med i orderlöftesberäkningen.  

> [!NOTE]  
>  Om du lämnar fältet **Ankommande Lagerhanteringstid. Lagerhanteringstid** tomt använder beräkningen värdet i fönstret **Lagerinställningar**.

### <a name="to-enter-outbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Så här anger du avgående lagerhanteringstid i lagerinställningarna  
Om du vill ange en avgående lagerhanteringstid som ska tas med i orderlöftesberäkningen på försäljningsraden, kan du ange tiden som standard för lagret.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerinställningar** och välj sedan relaterad länk.  
2. I fältet **Avgående lagerhanteringstid** på snabbfliken **Allmänt** anger du det antal dagar som ska tas med i orderlöftesberäkningen.  

> [!NOTE]  
>  Om du har fyllt i fältet **Avgående lagerhanteringstid** på lagerställekortet för lagerstället, används värdet i detta fält som standard för avgående lagerhanteringstid.  

### <a name="to-enter-outbound-warehouse-handling-time-on-location-cards"></a>Så här anger du avgående lagerhanteringstid på lagerställekort  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.  
2.  Öppna önskat lagerställekort.  
3.  I fältet **Avgående lagerhanteringstid** på snabbfliken **Lager** anger du det antal dagar som ska tas med i orderlöftesberäkningen.  

> [!NOTE]  
>  Om du lämnar fältet **Avgående lagerhanteringstid** tomt används värdet i fönstret **Lagerinställningar** för beräkning.

## <a name="to-make-an-item-critical"></a>Så här gör du en artikel kritisk  
Innan ett objekt kan tas med i orderlöftesberäkningen, måste den markeras som kritisk. Den här inställningen ser till att icke-kritiska objekt inte orsakar orderlöftesberäkningar.   
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Artiklar** och välj sedan relaterad länk.  
2.  Öppna relevant artikelkort.  
3.  Välj **Kritiskt** på snabbfliken **Planering**.  

## <a name="to-calculate-an-order-promising-date"></a>Så här beräknar du ett orderlöftesdatum  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningsorder** och välj sedan relaterad länk.  
2.  Öppna relevant försäljningsorder och markera de försäljningsorderrader som ska beräknas.  
3.  Välj åtgärden **Orderlöfte** och klicka på åtgärden **Orderlöftesrader**.  
4.  Välj en ny rad och välj sedan ett av följande alternativ.  

    - Markera **Disponibelt att lova** om du vill beräkna det tidigaste datum då artikeln är disponibel avseende lager, planenlig inleverans och bruttobehov.  
    - Markera **Kapabel att lova** om du vet att artikeln för närvarande är slut på lagret och vill beräkna det tidigaste datum då artikeln kan vara disponibel genom att skicka ut nya påfyllningsrekvisitioner.  
5.  Välj **Acceptera** om du accepterar det tidigaste leveransdatum som är tillgängligt.  

## <a name="see-also"></a>Se även  
[Försäljning](sales-manage-sales.md)  
[Datumberäkning för inköp](purchasing-date-calculation-for-purchases.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

