---
title: "Så här: Planera lagertransporter i förslag"
description: "Planera transporter i förslaget med hjälp av Återanskaffningsfunktionen eller manuellt planera de rader som du vill skapa som transportinstruktioner."
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
ms.openlocfilehash: fcf44a681e597df1bd50e94e851810fa00656a96
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-warehouse-movements-in-worksheets"></a>Så här: Planera lagertransporter i förslag
Planera transporter i förslaget med hjälp av Återanskaffningsfunktionen eller manuellt planera de rader som du vill skapa som transportinstruktioner.  

## <a name="to-calculate-a-replenishment-movement"></a>Så här beräknar du återanskaffningstransporter:  
Allt eftersom artiklarna i distributionslagret levereras till kunderna innehåller lagerplatser med högst lagerplatsordning allt färre artiklar. Om du vill fylla på plocklagerplatserna med högst lagerplatsordning med artiklar från andra lagerplatser kan du köra funktionen **Beräkna lagerplatsåteranskaffning** i fönstret **Transportförslag**

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Transportförslag**, och välj sedan relaterad länk.  
2.  Välj åtgärden **Beräkna lagerplatsåteranskaffning**.  

    [!INCLUDE[d365fin](includes/d365fin_md.md)] skapar rader som anger exakt hur du ska flytta artiklar från lagerplatser med låg lagerplatsordning till lagerplatser med högre lagerplatsordning.  

    > [!NOTE]  
    >  Föreslår en transport enligt FEFO när du aktiverar **Skapa transport** operationen, om följande villkor är uppfyllda för en artikel:  
    >   
    >  -   artikeln har ett utgångsdatum,  
    > -   Fältet **Plocka enligt FEFO** på lagerställekortet är markerat och  
    > -   På lagerställekortet måste kryssrutan **Lagerplats ska finnas** vara markerad.  
    > -   fälten **Från zon** och **Från lagerplats** innehåller inga värden.  

    Mer information finns i [Plocka enligt FEFO](warehouse-picking-by-fefo.md).  

3.  Titta igenom raderna och ändra dem vid behov, eller ta bort vissa av raderna om du inte har tillräckligt med tid att utföra alla.  
4.  Välj åtgärden **Skapa transport** för att skapa en distributionslagerinstruktion till lagerpersonalen.  

## <a name="to-move-the-entire-contents-of-one-or-more-bins-by-using-the-get-bin-content-function"></a>Du kan flytta hela innehållet i en eller flera lagerplatser med funktionen Hämta lagerplatsinnehåll:  
Du kan även använda Transportförslag för att planera andra lagertransporter inom distributionslagret. När du till exempel vill placera artiklar på en lagerplats för kvalitetskontroll kan du använda transportförslaget för att planera den åtgärden och sedan skapa en transportinstruktion för en anställd.  

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Transportförslag**, och välj sedan relaterad länk.  
2.  Välj åtgärden **Hämta lagerplatsinnehåll**. Du använder fönstret för begäran för att filtrera vilka lagerplatser och artiklar som ska visas på transportförslagets rader.  
3.  Fyll i de relevanta fälten i fönstret för begäran av batch-jobb. Om du till exempel vill visa lagerplatsinnehållet för alla lagerplatser i en viss zon på lagerstället fyller du i fältet **Zonkod**. Om du vill hämta rader för alla lagerplatser som innehåller en viss artikel fyller du i fältet **Artikelnr**.  

    > [!NOTE]  
    >  Du kan inte manuellt flytta artiklar in och ut ur en lagerplats av typen RECEIVE. Detta beror på att artiklar som finns i en lagerplats av RECEIVE-typ måste registreras som införda innan de blir en del av det tillgängliga lagret.  

4.  Om du hämtar många rader väljer du **Sortera** för att välja en sorteringsmetod som du kan använda för att bestämma den ordning som raderna ska visas med i förslaget och klickar sedan på **OK**.  

    > [!NOTE]  
    >  Förflyttningsrader hämtas enligt FEFO när du aktiverar **Hämta lagerplatsinnehåll** operationen, om följande villkor är uppfyllda för en artikel:  
    >   
    >  -   artikeln har ett utgångsdatum,  
    > -   Fältet **Plocka enligt FEFO** på lagerställekortet är markerat och  
    > -   På lagerställekortet måste kryssrutan **Lagerplats ska finnas** vara markerad.  
    > -   fälten **Från zon** och **Från lagerplats** innehåller inga värden.  

5.  Fyll i en del av de hämtade raderna för att spegla de ändringar som du vill utföra. För varje artikel som du vill flytta måste du fylla i fälten **Artikelnr**, **Från lagerplatskod**, **Till lagerplatskod** och **Antal**.  
6.  Ta bort ofullständiga rader som du bara använde i informationssyfte.  
7.  När raderna i transportförslaget korrekt speglar hur transporten ska utföras av lagerpersonalen klickar du på åtgärden **Skapa transport** för att skapa instruktionerna för personalen.  

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

