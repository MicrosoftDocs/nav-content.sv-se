---
title: "Så här: Ställa in grundläggande dist.lager med operationsområden"
description: "Om internt operationsområde till exempel produktion eller tillverkning finns i grundläggande distributionslagerkonfiguration, där lagerställen använder **Lagerplats ska finnas** inställningar, och eventuellt fälten **Begär plockning** och **Begär artikelinförsel**, kan du använda följande grundläggande dokument för att registrera lageraktiviteter för internt operationsområde:"
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d141fcb9f5357355272f6a34d71b88f50129985b
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-basic-warehouses-with-operations-areas"></a>Så här: Ställa in grundläggande dist.lager med operationsområden
Om internt operationsområde till exempel produktion eller tillverkning finns i grundläggande distributionslagerkonfiguration, där lagerställen använder **Lagerplats ska finnas** inställningar, och eventuellt fälten **Begär plockning** och **Begär artikelinförsel**, kan du använda följande grundläggande dokument för att registrera lageraktiviteter för internt operationsområde:  

- **lagerförflyttning** fönster.  
- Fönstret **Lagerplockning**.  
- Fönstret **Lagerinförsel**.

> [!NOTE]
> Även om inställningarna kallas **Begär plockning** och **Begär artikelinförsel**, kan du fortfarande bokföra inleveranser och utleveranser direkt från affärskälldokument på platser där du markerar dessa kryssrutor.  

Att använda dessa fönster med intern operation t.ex för att plocka komponenter och flytta till produktionen, måste du följa några eller alla följande steg, beroende på hur mycket kontrollerar du behöver:  

- Aktivera lagerplockningen, flytta och artikelinför dokumenten.  
- Definiera standardlagerplatsstrukturer för komponenter och artiklar, flöde till och från åtgärdsresurser.  
- Göra till- och frånlagerplatser som är avsedda för åtgärdsresurser för att förhindra att artiklarna plockas för utgående dokument.

Lagerplatskoder som definierats på lagerställekort anger ett standardlagerflöde för vissa aktiviteter, till exempel komponenter i en monteringsavdelning. Ytterligare funktioner finns för att se till att artiklar inte kan plockas eller flyttas till andra aktiviteter när de placerats på en viss lagerplats. Mer information finns i avsnittet ”Så här skapar du särskilda komponentlagerplatser”.

Procedurerna baseras på att ställa in grundläggande av lageraktiviteter kring en produktionsområde. Momentet är liknande för andra operationsområden, t.ex montering, servicehantering och projekt.  

> [!NOTE]  
>  I följande procedur här fältet **Lagerplats ska finnas** på lagerställekort markeras som ett villkor, eftersom det betraktas som grund för en nivå i lagerstyrningen.  

## <a name="to-enable-inventory-documents-for-internal-operation-activities"></a>Om du vill aktivera lagerdokument för intern operation aktiviteter  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.
2. Öppna lagerställekortet som du vill ställa in.  
3.  Välj kryssrutan **Dist.lager**, fältet **Begär artikelinförsel** för att visa att när ett ankommande eller en internt källdokument med en lagerplatskod släpps, en lagerartikelinförsel eller en lagertransportdokument kan skapas.  
4.  Välj **Begär plockning** för att visa att när ett utgående eller en internt källdokument med en lagerplatskod skapas, en lagerplockning eller en lagertransportdokument måste skapas.  

## <a name="to-define-a-default-bin-structure-in-the-production-area"></a>Så här definierar du en standardlagerplatsstruktur i produktionsområdet  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.
2. Öppna lagerstället som du vill ställa in.  
3.  På Snabbfliken **Lagerplatser** , i **Öppen prod.lagerplats kod** fältet, ange koden för lagerplatsen i produktionsområdet med överflöd av komponenter som maskinoperatören kan använda utan att begära en lageraktivitet om att ta dem till lagerplatsen. Artiklar som placeras på denna lagerplats, används vanligtvis för automatisk bokföring. Det innebär att **Bokföringsmetod** fältet, innehåller **Framåt** eller **Bakåt**.  
4. I fältet **Till prod.-lagerplats - kod** anger du koden för lagerstället i produktionen där komponenter, som plockas för produktion i denna plats, placeras som standard, innan de kan förbrukas. Artiklar som placeras på denna lagerplats, används vanligtvis för förbrukningsbokföring. Det innebär att **Bokföringsmetod** fältet innehåller **Manuell** eller **Plocka + framåt** eller **Plocka + bakåt** för dist.lager plockning och lagerförflyttningar.  

    > [!NOTE]  
    >  Om du använder lagerplockningar definierar fältet **Lagerplatskod** på en produktionsorderkomponentrad lagerplatsen *ta* från vilken antalet komponenter minskas när konsumtionen bokförs. Om du använder lagerförflyttningar definierar fältet **Lagerplatskod** på en produktionsorderkomponentrad, lagerplatsen *plats* i operationsområdet från vilken antalet lagerarbetare måste placera komponenter.  

5. På Snabbfliken **Lagerplatser** , i **Från prod.lagerplats - kod** fältet, ange koden för lagerplatsen i produktionsområdet där färdiga slutartiklar tas från som standard, när processen omfattar lageraktiviteter. I grundläggande lagerkonfigurationer registreras aktiviteten som en lagerartikelinförsel eller en lagerförflyttning.  

Nu kräver produktionsorderkomponentrader med standardlagerplatskoden att framåtriktade komponenter placeras där. Dock tills komponenterna förbrukas från den lagerplats kan andra komponentbehov väljas eller förbrukas från den lagerplatsen eftersom de är fortfarande tillgängligt lagerplatsinnehåll. Se till att lagerplatsinnehållet är bara tillgänglig för det komponentbehov som använder den till produktion-lagerplats genom att välja fältet **Dedikerad** på raden för den lagerplatskoden i **Lagerplatser**-fönstret som du öppnar från lagerställekortet.

Diagrammet visar hur **Lagerplatskod** på produktionsorderkomponentraderna fylls enligt inställningen.  

![Flödesschema för lagerplats](media/binflow.png "BinFlow")    

## <a name="to-define-a-default-bin-structure-in-the-assembly-area"></a>Så här definierar du en standardlagerplatsstruktur i monteringsområdet
Komponenter för monteringsorder kan inte plockas eller bokföras med lagerplockningar. Med **lagerförflyttning** fönstret. För mer informatio, se [Så här: Flytta komponenter till ett operationsområde i grundläggande lagerstyrning](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)

Om plockning- och leveransförsäljningsradantal läggs till i order ska du följa vissa regler när du skapar lagerplockningsraderna. Mer information finns i avsnittet ”hantera artiklar för montering mot kundorder i lagerplockningar” i [Så här plockar du artiklar med Lagerplockning](warehouse-how-to-pick-items-with-inventory-picks.md).

Mer information finns i [Monteringshantering](assembly-assemble-items.md).

### <a name="to-set-up-that-an-inventory-movement-is-automatically-created-when-the-inventory-pick-for-the-assembly-item-is-created"></a>För att ställa in automatiskt skapa en lagertransport, när monteringsartikeln för lagerplockningen skapas.
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Monteringsinställningar** och välj sedan relaterad länk.
2. Markera kryssrutan **Skapa transporter automatiskt**.

### <a name="to-set-up-the-bin-in-the-assembly-area-where-components-are-placed-by-default-before-they-can-be-consumed-in-assembly"></a>Anger lagerplatsen i monteringsområdet där komponenter placeras som standard innan de kan förbrukas vid montering.
Värdet i det här fältet infogas automatiskt i fältet **Lagerplatskod** på monteringsorderrader när lagerstället anges i fältet **Platskod** på monteringsorderraden.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.
2. Öppna lagerstället som du vill ställa in.
3. Fyll i fältet **Till monteringsplats - kod**.

### <a name="to-set-up-the-bin-in-the-assembly-area-where-finished-assembly-items-are-posted-to-when-they-are-assembled-to-stock"></a>Anger lagerplatsen i monteringsområdet där slutförda monteringsartiklar bokförs när de monteras mot lager.
Värdet i det här fältet infogas automatiskt i fältet **Lagerplatskod** på monteringsorderhuvuden när platskod anges i fältet **Platskod** på monteringsorderhuvudet.

Lagerplatskoder som definierats på lagerställekort anger ett standardlagerflöde för vissa lageraktiviteter, till exempel konsumtion i en monteringsavdelning. Ytterligare funktioner finns för att se till att artiklar inte kan plockas eller flyttas till andra aktiviteter när de placerats på en standardlagerplats.

> [!NOTE]
> Den här konfigurationen är endast möjlig för lagerplatser där fältet Lagerplats ska finnas är markerat.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.
2. Öppna lagerstället som du vill ställa in.
3. Fyll i fältet **Från monteringsplats - kod**.

### <a name="to-set-up-the-bin-where-finished-assembly-items-are-posted-to-when-they-are-assembled-to-a-linked-sales-order"></a>Anger lagerplatsen där slutförda monteringsartiklar bokförs när de monteras mot en kopplad försäljningsorder.
Från den här lagerplatsen levereras monteringsartiklarna omedelbart, via en lagerplockning, för att uppfylla försäljningsordern.

> [!NOTE]
> Fältet kan inte användas om dirigerad artikelinförsel och plockning används på lagerstället.

Lagerplatskoden kopieras från försäljningsorderraden till monteringsorderhuvudet för att meddela monteringsarbetarna om var utflödet ska placeras inför leveransen. Den kopieras även till lagerplockningsraden för att ange för lagerarbetarna var det ska tas från för leverans.

> [!NOTE]
> Utleveranslagerplatsen för montering mot kundorder är alltid tom. När du bokför en försäljningsrad för montering mot kundorder justeras lagerplatsinnehållet först positivt med monteringsutflödet. Direkt efter justeras det negativt med det levererade antalet.

Värdet i fältet infogas automatiskt i fältet Lagerplatskod på försäljningsorderrader som innehåller ett antal i fältet **Antal att montera mot kundorder** eller om den artikel som ska säljas har **Montering mot kundorder** i fältet **Återanskaffningssystem**.

Om **Lagerpl.kod för mont. mot lev.** är tomt, används fältet **från monteringsplats-kod** i stället. Om båda konfigurationsfälten är tomma används den sista använda lagerplatsen med innehåll i fältet **Lagerplatskod** på försäljningsorderrader.

Samma lagerplatskod kopieras i sin tur till fältet **Lagerplatskod** på lagerplockningsraden som hanterar utleveransen av antalet för montering mot kundorder. Mer information finns i avsnittet ”hantera artiklar för montering mot kundorder i lagerplockningar” i [Så här plockar du artiklar med Lagerplockning](warehouse-how-to-pick-items-with-inventory-picks.md).

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.
2. Öppna lagerstället som du vill ställa in.
3. Fyll i fältet **Lagerpl.kod för mont. mot lev.**.

## <a name="to-create-dedicated-component-bins"></a>För att du ska kunna göra dedikerade komponentlagerplatser
Du kan ange att kvantiteter på lagerplatser skyddas från plockning för andra krav än krav från det aktuella syftet.

Antalet i lagerplatserna kan fortfarande reserveras. Därmed ingår antalet i dedikerade lagerplatser i fältet **Totalt disponibelt antal** i fönstret **Reservation**.

Till exempel skapas en produktionsgrupp med en lagerplatskod i fältet **Till prod.-lagerplats - kod**. Produktionsorderkomponentrader med den här lagerplatskoden kräver att framåtriktade komponenter placeras där. Dock tills komponenterna förbrukas från den lagerplats kan andra komponentbehov väljas eller förbrukas från den lagerplatsen eftersom de är fortfarande tillgängligt lagerplatsinnehåll. Se till att lagerplatsinnehållet är bara tillgänglig för det komponentbehov som använder den till produktion-lagerplats genom att välja fältet **Dedikerad** på raden för den lagerplatskoden i **Lagerplatser**-fönstret som du öppnar från lagerställekortet.

Att dedikera en lagerplats påminner om funktionen att använda lagerplatstyper, som endast finns i avancerade distributionslager. (Mer information finns i [Så här: Skapa Lagerplatstyper](warehouse-how-to-set-up-bin-types.md).)

> [!Caution]
> Artiklar på dedikerade lagerplatser skyddas inte när de plockas och förbrukas som produktionskomponenter med fönstret Lagerplockning.

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk. Välj lagerstället som du vill uppdatera.  
2.  Välj åtgärden **Lagerplatser**.  
3.  Välj **Dedikerad**-fältet för varje Lagerplats som du vill använda exklusivt för vissa interna operationer och där kvantiteten på lagerplatsen ska reserveras för den interna åtgärd som placerats där.  

> [!NOTE]  
>  Lagerplatsen måste vara tom, innan du kan välja eller ta bort **Dedikerad** fältet.

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

