---
title: "Så här lägger du upp fabrikskalendrar"
description: "I en produktionsgruppkalender anger du de arbetsdagar och arbetstimmar, skift, helgdagar och frånvaro som avgör den tillgängliga bruttokapaciteten för produktionsgruppen (mätt i tidsenheter) utifrån de effektivitets- och kapacitetsvärden som har definierats för gruppen. Om du vill skapa och aktivera en produktionsgruppkalender måste du först utföra flera förberedande åtgärder."
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
ms.openlocfilehash: 59131cdded4bf854aed02a7d835e8160342adb36
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-shop-calendars"></a>Så här lägger du upp fabrikskalendrar
I en produktionsgrupp- eller maskingruppkalender anger du de arbetsdagar/arbetstimmar, skift, helgdagar och frånvaro som avgör den tillgängliga bruttokapaciteten för produktionsgruppen (mätt i tidsenheter) utifrån de effektivitets- och kapacitetsvärden som har definierats för gruppen.

Om du vill beräkna en specifik produktionsgrupp- eller maskingruppkalender måste du först skapa en eller flera allmänna fabrikskalendrar. En fabrikskalender innehåller en standardarbetsvecka med start- och sluttider för varje arbetsdag samt en översikt över arbetsskiften. Dessutom kan du i fabrikskalendern se de fasta helgdagarna under året.  

Nedan beskrivs hur du ställer in produktionsgruppskalendrar. Momentet är liknande när du ställer in maksingruppkalender.  

## <a name="to-create-work-shifts"></a>Så här skapar du arbetsskift  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Arbetsskift** och välj sedan relaterad länk.  
2.  På en tom rad anger du ett nummer i fältet **Kod** för att identifiera arbetsskiftet (till exempel **1**).  
3.  Beskriv arbetsskiftet i fältet **Beskrivning**, till exempel **1:a skift**.  
4.  Fyll i raderna för ett andra eller tredje skift, om du vill.  

Även om dina produktionsgrupper inte arbetar i olika skift måste du ange minst en arbetsskiftkod.  

## <a name="to-set-up-a-shop-calendar"></a>Så här skapar du en fabrikskalender  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Arbetsskift** och välj sedan relaterad länk.  
2.  På en tom rad anger du ett nummer i fältet **Kod** för att identifiera fabrikskalendern.  
3.  Beskriv fabrikskalendern i fältet **Beskrivning**.  
4.  Välj åtgärden **arbetsdagar**.
5.  I fönstret **Fabrikskalender arbetsdagar** kan du definiera en fullständig arbetsvecka med start- och sluttider för varje dag.  

    I fältet **Arbetsskiftskod**, markera en av förskjutningarna som du definierade tidigare. Lägg till en rad för varje arbetsdag, samt varje skift. Som exempel:  

    Måndag 07:00 15:00 1   
    Tisdag 07:00 15:00 1  

    Om du behöver en fabrikskalender med två arbetsskift måste du fylla i den på följande sätt:  

    Måndag 07:00 15:00 1   
    Måndag 15:00 23:00 2  
    Tisdag 07:00 15:00 1  
    Tisdag 15:00 23:00 2  

    De veckodagar som du inte definierar i fabrikskalendern, till exempel lördag och söndag, antas vara icke-arbetsdagar och får arbetskapaciteten noll i alla produktionsgruppkalendrar.  

    När du har definierat alla arbetsdagar i veckan kan du stänga fönstret **Fabrikskalender arbetsdagar** och fortsätta med att ange helgdagar.  

6.  I fönstret **fabrikskalender** markerar du fabrikskalendern, och väljer sedan åtgärden **helgdagar**.
7. I fönstret **Fabrikskalender semestrar** anger du helgdagar under året genom att ange startdatum och starttid, sluttid och en beskrivning av varje dag på enskilda rader. Som exempel:  

    04/07/14 0:00:00 23:59:00 Sommarsemester  
    05/07/14 0:00:00 23:59:00 Sommarsemester  
    06/07/14 0:00:00 23:59:00 Sommarsemester  

De angivna helgdagarna får värdet noll för tillgänglig kapacitet i alla produktionsgruppkalendrar.  

Fabrikskalendern kan nu tilldelas en produktionsgrupp så att den produktionsgruppkalender som styr all operationstidsplanering för produktionsgruppen kan beräknas.  

## <a name="to-calculate-a-work-center-calendar"></a>Så här beräknar du en produktionsgruppkalender  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Arbetsskift** och välj sedan relaterad länk.
2. Öppna produktionsgruppen som du vill uppdatera.  
3. I fältet **Fabrikskalenderkod** väljer du vilken fabrikskalender som ska användas som grund för en produktionsgruppkalender.  
4. Välj åtgärden **Kalender**.  
5. I fönstret **Prod.gruppkalender** väljer du åtgärden **Visa matris**.  

    Till vänster i matrisfönstret visas befintliga produktionsgrupper. Till höger visas en tidskalender med värden för tillgänglig kapacitet för varje arbetsdag i den angivna enheten, till exempel **480** minuter. Varje rad motsvarar kalendern för en produktionsgrupp.  

    > [!NOTE]  
    >  Du kan också ange att du vill visa kapacitetsvärdena per vecka eller månad genom att ändra alternativen i fältet **Visa efter** i fönstret **Prod.gruppkalender**.  

    Innan du kan visa den nya fabrikskalendern som en rad på den markerade produktionsgruppen måste den först beräknas.  

6.  Välj åtgärden **Beräkna**.  
7.  På snabbfliken **Produktionsgrupp** kan du ange ett filter så att beräkningen bara utförs för en produktionsgrupp. Om du inte anger något filter beräknas alla befintliga produktionsgruppkalendrar.  
8.  Ange start- och sluttider för kalenderperioden som ska beräknas, till exempel ett år mellan 040101 och 041232.
9. Klicka på **OK** för att beräkna kapacitet.  

Kalendertransaktioner skapas (eller uppdateras), och du ser den tillgängliga kapaciteten per period enligt följande tre uppsättningar standarduppgifter:  

- De arbetsdagar och skift som har angetts i den tilldelade fabrikskalendern.  
- Värdet i fältet **Kapacitet** på produktionsgruppkortet.  
- Värdet i fältet **Effektivitet** på produktionsgruppkortet.  

Den beräknade produktionsgruppkalendern definierar nu när, och hur mycket, som är tillgänglig kapacitet för produktionsgruppen. Detta styr detaljerat planeringen av operationer som utförs i produktionsgruppen.  

## <a name="to-record-work-center-absence"></a>Så här registrerar du frånvaro i produktionsgrupper  
1.  I fönstret **Prod.gruppkalender** väljer du åtgärden **Visa matris**.
2. I fönstret **Prod.gruppkalendermatris** markerar du den produktionsgrupp och den kalenderdag som frånvarotid ska registreras för och väljer åtgärden **Frånvaro**.  
3.  I fönstret **Frånvaro** anger du starttid, sluttid och beskrivning av frånvarotiden. Till exempel:  

    010125 08:00 10:00 Underhåll  

4.  Välj åtgärden **uppdatering** och stäng fönstret **frånvaro**.  

Kapaciteten för den markerade dagen minskas med den registrerade frånvarotiden.  

## <a name="see-also"></a>Se även  
[Så här lägger du upp baskalendrar](across-how-to-assign-base-calendars.md)  
[Så här: ställa in produktionsgrupper och maskingrupper](production-how-to-set-up-work-and-machine-centers.md)  
[Ställa in Produktion](production-configure-production-processes.md)  
[Produktion](production-manage-manufacturing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

