---
title: "Så här: Omstrukturera distributionslager"
description: Du kanske vill omstrukturera distributionslagret med nya lagerplatskoder och nya lagerplatsegenskaper.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 852aa1a36b150d13d763e2c398265b9eaec5c3ea
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-restructure-warehouses"></a>Så här: Omstrukturera distributionslager
Du kanske vill omstrukturera distributionslagret med nya lagerplatskoder och nya lagerplatsegenskaper. Den typen av aktivitet utförs inte särskilt ofta, men det kan uppstå situationer när en omgruppering är nödvändig för att åstadkomma en effektivare drift. Som exempel:  

- Du kanske vill växla till lagerplatskoder som stöder automatisk datainsamling, exempelvis med handenheter.  
- Distributionslagret kanske har köpt in nya ställningar som ger andra möjligheter att lagra artiklar.  
- Företaget kanske har ändrat sitt artikelsortiment och flyttat distributionslagret till en ny plats för att kunna hantera förändringen.  

Om distributionslagret är inställt på lagerplatser, men inte dirigerad artikelinförsel och plockning, strukturera om distributionslagret genom att skapa nya lagerplatser du vill använda.  

## <a name="to-restructure-a-basic-warehouse-that-uses-bins-only"></a>Om du vill omstrukturera en vanlig dist.lager som använder lagerplatser bara  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.  
2.  På snabbfliken **lager** anger du fältet **Standardlagerplatsval** till **Senaste lagerplats**.  
3.  Flytta allt innehåll på de nuvarande lagerplatserna till de nya lagerplatserna som du precis har skapat.  

    1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Artikelgrupperingsjournal** och välj sedan relaterad länk.  
    2.  Markera en rad och välj sedan åtgärden **Hämta lagerplatsinnehåll**.  
    3.  På Snabbfliken **Lagerplatsinnehåll** , ställer du in filter i **Lagerställekod**, **Lagerplatskod**, och **Artikelnr** fältet för att ange innehållet som du vill flytta.  
    4.  Välj den **OK** på för att fylla i en journalrad.  
    5.  Markera den lagerplats till vilken artiklarna ska flyttas i fältet **Ny lagerplatskod**.  
    6.  Upprepa steg b till e för allt lagerplatsinnehåll som du vill flytta.  
    7.  Välj åtgärden **Bokföra**.  

Du har nu tömt lagerplatser där artiklarna användes. Standardlagerplatserna för artiklarna har nu ändrats till de nya lagerplatser.  

## <a name="to-restructure-an-advanced-warehouse-that-uses-directed-put-away-and-pick"></a>Omstrukturera en avancerad lager som använder dirigerad artikelinförsel och plockning  

1.  Ska de nya lagerplatserna som du vill använda i framtiden. Mer information finns i [Så här: Skapa lagerplatser](warehouse-how-to-create-individual-bins.md).  
2.  Flytta allt innehåll på de nuvarande lagerplatserna till de nya lagerplatserna som du precis har skapat.  

    1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lageromgrupperingsjournal** och välj sedan relaterad länk.  
    2.  För de lagerplatser där det inte sker någon transport av artiklar skapar du en rad för varje aktuell lagerplats i **Dist.lager omgrupperingsjnl** med den gamla lagerplatskoden, **Från lagerplatskod** och den nya lagerplatskoden, **Till lagerplatskod**.  
    3.  Om vissa transporter innefattar fysiska transporter som du vill att lagerpersonalen ska utföra använder du **Transportförslag** för att förbereda transportinstruktioner i stället för att använda lagergrupperingsjournalen. För mer information, se [Så här: Flytta artiklar avancerad distributionslagerkonfiguration](warehouse-how-to-move-items-in-advanced-warehousing.md).  

3.  När de gamla lagerplatserna är tomma gruppera om dem som **KS** typ av lagerplatsen, för att se till att de inte inkluderas i artikelflöden.  

    1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.  
    2.  Markera raden med lagerstället, och välj sedan åtgärden **Lagerplatser**.  
    3.  I **Lagerplatser** fönstret i **Lagerplatstyp kod** fältet, ange **KS** för var och en av de gamla lagerplatserna som du tömde i steg 3 i föregående process.  

Du har nu tagit bort lagerplatserna från lagerflödet och har omklassificerat dem, som KS-lagerplatser. KS-lagerplatser har inte några av aktivitetsfälten i fältet **Lagerplatstyper** valda och därför inte beaktas av objektflödet. (Mer information finns i [Så här: Skapa Lagerplatstyper](warehouse-how-to-set-up-bin-types.md).)  

## <a name="to-delete-a-bin"></a>Så här tar du bort en lagerplats  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.  
2.  Markera lagerstället där du vill ta bort lagerplatser väljer du åtgärden **Lagerplatser**.  
3.  Markera raderna för de lagerplatser som du vill ta bort.  
4.  Välj åtgärden **Radera**.  

Om du klickar på **Ja** tas lagerplatsen bort för framtida användning, men lagerplatskoden finns kvar i alla distributionslagertransaktioner.  

Om du vill byta namn på en lagerplats så att alla poster som tillhör lagerplatsen också får det nya namnet kan du göra det i fönstret **Lagerplatser**, inklusive lagerplatsinnehåll, aktivitetsrader för distributionslager, registrerade aktivitetsrader för distributionslager, förslagsrader för distributionslager, inleveransrader för distributionslager, bokförda inleveransrader för distributionslager, utleveransrader för distributionslager, bokförda utleveransrader för distributionslager och distributionslagertransaktioner.  

## <a name="to-rename-a-bin-and-change-the-bin-code-in-all-records"></a>Så här byter du namn på en lagerplats och ändrar lagerplatskoden i alla poster  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.  
2.  Välj lagerstället där du vill byta namn på en lagerplats eller ändra lagerplatskoden och klicka på åtgärden **Lagerplatser**.  
3.  I **Kod** fältet, ange lagerplatsen du vill ändra och ange en ny lagerplatskod.  
4.  Välj **Ja**.  

> [!NOTE]  
>  Om du väljer **ja** , och det finns många transaktioner som rör den här lagerplatsen, till exempel, eftersom du inte har tagit bort de dokument för en tid, kan det ta en stund byta namn på samtliga transaktioner. Använd batch-jobbet **Ta bort reg. dist.lagerdok.** innan du startar bytanamnprocessen, om du använder den här metoden. Observera också att det enda dokumenten som tas bort i det här batch-jobbet är artikelinförsel, plockning och transport.  
>   
>  Om du byter namn på en inleveranslagerplats eller en leveranslagerplats, alla bokförd inleveranser och utleveranser som gäller för lagerplatsen, byts namn på.  

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

