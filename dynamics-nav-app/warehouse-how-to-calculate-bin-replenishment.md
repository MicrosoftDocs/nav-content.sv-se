---
title: "Så här Beräkna du lagerplatsåteranskaffning"
description: "Om lagerstället är inställt på dirigerad artikelinförsel och plockning, beaktas artikelinförsel prioriteter av mallen för lagerstället när införsel av inleveranser."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3a6ff833aad54cf98720857a8ae67492abe9af4f
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-bin-replenishment"></a>Så här Beräkna du lagerplatsåteranskaffning
Om lagerstället är inställt på dirigerad artikelinförsel och plockning, beaktas artikelinförsel prioriteter av mallen för lagerstället när införsel av inleveranser. Prioriteter innehåller minimal och maximal kvantitet av lagerplatsinnehåll, som har kopplats till en viss lagerplats, och lagerplatsordningarna. Om artiklar anländer i fast takt fylls därför de plocklagerplatser på som används mest allt eftersom de töms.  

Inleveranser anländer dock inte alltid i en stadig takt. Ibland köps artiklar in i större kvantiteter så att företaget kan få rabatt, eller så att produktionsenheten kan producera mycket av en artikel för att få en låg styckkostnad. Då kan det ta ett tag innan artiklarna inlevereras på nytt i distributionslagret, och distributionslagret behöver regelbundet transportera artiklar till plocklagerplatser från volymlagret.  

Det kan även vara så att ett nytt parti förväntas inom kort och därför behöver volymlagret tömmas på artiklar innan de nya varorna anländer.  

Slutligen gäller att om du har definierat volymlagerplatser med enbart lagerplatstypåtgärden **Artikelinförsel**, d.v.s. åtgärden **Plocka** inte är markerad, måste du alltid fylla på plocklagerplatserna eftersom lagerplatser av artikelinförseltyp inte föreslås för en plockning från lager.  

## <a name="to-replenish-pick-bins"></a>Så här fyller du på plocklagerplatser  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Transportförslag**, och välj sedan relaterad länk.  
2.  Välj åtgärden **Beräkna lagerplatsåteranskaffning** för att öppna sidan för rapportbegäran.  
3.  Fyll i fönstret för begäran om batch-jobb för att begränsa omfattningen av de påfyllningsförslag som kommer beräknas. Du kanske är mest intresserad av särskilda artiklar, zoner eller lagerplatser.  
4.  Välj **OK**. Rader skapas för de påfyllningstransporter som måste utföras enligt de regler som har angetts för lagerplatserna och lagerplatsinnehållet, d.v.s. artiklar på lagerplatser.  
5.  Om du vill utföra alla påfyllningsförslag klickar du på åtgärden **Skapa transport**. Lagerpersonalen kan nu hitta instruktionerna under menyobjektet **Transport**, utföra dem och registrera dem.  
6.  Om du endast vill utföra vissa förslag tar du bort de rader som är mindre viktiga och skapar sedan en transport.  

Nästa gång som du beräknar lagerplatspåfyllning återskapas de förslag som du har tagit bort, om de fortfarande är aktuella.  

> [!NOTE]  
>  Om följande villkor är uppfyllda för en artikel:  
>   
>  -   artikeln har ett utgångsdatum,  
> -   Fältet **Plocka enligt FEFO** på lagerställekortet är markerat och  
> -   Du använder funktionen **Beräkna lagerplatsåteranskaffning**  
>   
>  då innehåller fälten **Från zon** och **Från lagerplats** inga värden. Detta beror på att algoritmen som används för att beräkna varifrån artiklarna ska transporteras endast utlöses när du aktiverar funktionen **Skapa transport**.  

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Plockning med FEFO](warehouse-picking-by-fefo.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

