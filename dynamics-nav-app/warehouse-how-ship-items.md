---
title: "Så här utlevererar du artiklar"
description: "Beroende på konfigurationen av lagret, kan du antingen registrera utleverans på relaterade avgående affärsdokumentet, till exempel försäljningsorder, direkt eller använda distributionslagerutleveransdokument som följer ett arbetsflöde och integreras i olika lageraktiviteter."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 121f1e32d1fa265d4e059dc0ee43fad22f732472
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-ship-items"></a>Så här utlevererar du artiklar
När artiklarna utlevereras från ett distributionslager som har ställts in för utleveransbearbetning kan du bara registrera utleveransen med relaterade dokument, till exempel en försäljningsorder, en serviceorder, inköpsreturorder eller en order för avgående överföringar.

När du utlevererar artiklar från ett distributionslagret som har ställt in utleveransbearbetning kan du bara leverera artiklar baserat på källdokument som andra företagsenheter har släppt till distributionslagret för åtgärder.

> [!NOTE]
> Om distributionslagret använder direktutleveranser och lagerplatser, kan du för varje rad visa hur många artiklar som har placerats i direktutleveranslagerplatserna. Programmet beräknar antalet automatiskt när fälten i utleveransen uppdateras. Om det rör sig om de artiklar som ingår i den utleverans du förbereder, kan du skapa en plockning för alla raderna och därefter färdigställa utleveransen. För mer information finns i [Så här Direktutleverans av artiklar](warehouse-how-to-cross-dock-items.md).

## <a name="to-ship-items-with-a-sales-order"></a>För att utleverera artiklar med en försäljningsorder.
Nedan beskrivs hur du inlevererar artiklar med en inköpsorder. Stegen är liknande för inköpsreturorder, serviceorder och utgående överföringsorder.  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningsorder** och välj sedan relaterad länk.
2. Öppna en befintlig försäljningsorder eller skapa en ny. Mer information finns i [Så här säljer du produkter](sales-how-sell-products.md).
3. Ange hur många enheter som har inlevererats i fältet **Ant. att utleverera**.

    Värdet i fältet **Utlevererat antal** uppdateras i enlighet därmed. Om detta är en delutleverans och värdet är lägre än värdet i fältet **antal**.
4. Välj åtgärden **Bokföra**.

## <a name="to-ship-items-with-a-warehouse-shipment"></a>För att utleverera artiklar med en lagerutleverans.
Först kan du skapa ett utleveransdokument från ett källdokument för företag. Sedan kan du välja de angivna artiklarna för utleverans.

### <a name="to-create-a-warehouse-shipment"></a>Skapa en distributionslagerutleverans.
Medarbetare som är ansvarig för utleveransen skapar en distributionslagerutleverans.
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerutleveranser**, och välj sedan relaterad länk.  
2.  Välj åtgärden **Ny**.  

    Fyll i fälten på snabbfliken **Allmänt**. När du hämtar källdokumentrader, kopieras delar av informationen i huvudet till varje rad.  

    För dirigerad artikelinförsel och plockning: om lagerstället har en standardzon och standardlagerplats för utleveranser fylls fälten **Zonkod** och **Lagerplatskod** i automatiskt. Du kan dock ändra fälten vid behov.  

    > [!NOTE]  
    >  Om du vill utleverera artiklar med klasskoder för distributionslager som skiljer sig från klasskoderna för lagerplatsen i fältet **Lagerplatskod** i dokumenthuvudet, måste du ta bort innehållet i fältet **Lagerplatskod** i huvudet innan du hämtar källdokumentets rader för artiklarna.  
3.  Välj åtgärden **Hämta källdokument**. Fönstret **Källdokument** öppnas.

    Från en ny eller öppen lagerutleverans kan du använda fönstret **Filter att hämta ursprungsdok..** för att hämta de släppta källdokumentraderna som anger vilka artiklar som ska utlevereras.

    1. Välj åtgärden **Filter för att hämta urspr.dok.**.  
    2. Du skapar ett nytt filter genom att ange en beskrivande kod i fältet **Kod** och väljer sedan åtgärden **Ändra**.  
    3. Definiera vilken typ av källdokumentrader som du vill hämta genom att fylla i relevanta filterfält.  
    4. Välj åtgärden **Kör**.  

    Alla relaterat källdokumentrader, som uppfyller filterkriterierna, infogas nu i fönstret **Dist.lager utleverans** som du aktiverade från filterfunktionen.  

    Filterkombinationerna, vilka du definierar, sparas i fönstret **Filter att hämta ursprungsdok.** tills nästa gång du behöver den. Du kan skapa ett obegränsat antal filterkombinationer. Du kan ändra kriterier när som helst, genom att välja åtgärden **Ändra**.

4.  Välj det källdokument som du vill utleverera artiklar för och klicka på knappen **OK**.  

Raderna i källdokumentet visas i fönstret **Dist.lager utleverans** fönstret. **Ant. att utlevereras** är ifyllt med utestående antal på respektive rad, men du kan ändra antalet som behövs. Om du tar bort innehållet i fältet **Lagerplatskod** på snabbfliken **Allmänt** innan du hämtar raderna måste du fylla i en lämplig lagerplatskod på varje utleveransrad.  

> [!NOTE]  
>  Det går inte att utleverera fler artiklar än antalet, i **Utestående ant.** på källdokumentraden. Om du vill utleverera fler artiklar, hämtar du ett annat källdokument som innehåller en rad för artikeln, genom att använda filterfunktionen för att hämta källdokument med aktuell artikel.  

När du har alla rader som ska utlevereras kan du skicka raderna som lagerpersonalen ska plocka.

### <a name="to-pick-and-ship"></a>Så här plockar och utlevererar du artiklar
Vanligtvis skapar en lagerarbetare ansvarig för plockning ett plockningsdokument eller öppnar ett redan skapat plockningsdokument.
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerutleveranser**, och välj sedan relaterad länk.
2. Välj dist.lager utleverans som du vill plocka för och välj sedan åtgärden **Skapa plockning**.
3. Fyll i fälten i fönstret och sedan välj **OK** knappen. De angivna dokumenten för distributionslagertransport har skapats.

    Du kan också öppna en befintlig dist.lager plockning.
4. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Plockningar**, och välj sedan relaterad länk. Välj Dist.lager plockning som du vill arbeta med.

    Om distributionslagret är konfigurerat att använda lagerplatser har plockningsraderna omvandlats till åtgärdsrader för Ta och Placera.

    Du kan sortera raderna, tilldela en anställd plockningen, använda ett brytenhetsfilter, om du använder dirigerad artikelinförsel och plockning, samt skriva ut plockningsinstruktionerna.

5. Utför den faktiska plockningen av artiklarna och placera dem på angiven utleveranslagerplats, eller i utleveransområdet, om du inte använder lagerplatser.
6. Välj **Registrera plockning**.

    Fälten **Ant. att utleverera** och **Dokumentstatus** i leveransdokumentets huvud uppdateras. De artiklar som du har plockat är inte längre tillgängliga för plockning för andra utleveranser eller för interna operationer.
7. Skriv ut leveransdokumenten, förbered godspaketen och bokför utleveransen.

Mer information om hur du plockar för utleveranser finns i [Så här: plocka artiklar för Dist.lager utleverans](warehouse-how-to-pick-items-for-warehouse-shipment.md).

Du kan också använda plockningsförslaget för att kombinera flera plockningsinstruktioner till en enda instruktion (för flera utleveranser) och på så sätt optimera plockningen i distributionslagret. Mer information finns i [Så här planerar du plockningar i förslaget](warehouse-how-to-plan-picks-in-worksheets.md).

> [!NOTE]
> Om du väntar på att vissa artiklar ska anlända till distributionslagret, och du använder funktionerna för direktutleverans, beräknar [!INCLUDE[d365fin](includes/d365fin_md.md)] det antal artiklar som finns på lagerplatsen för direktutleverans för varje utleverans- eller plockningsförslagsrad. Det här fältet uppdateras varje gång du lämnar och öppnar utleveransdokumentet eller förslaget. För mer information finns i [Så här Direktutleverans av artiklar](warehouse-how-to-cross-dock-items.md).

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

