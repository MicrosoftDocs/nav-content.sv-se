---
title: "Servicebokföring"
description: "Funktionen för servicebokföring gör att du kan behandla dokumenten mer effektivt och upprätthålla en bra service till kunderna. Du kan skapa och uppdatera bokförda dokument och skapa transaktioner i modulen Service och i andra moduler så att informationen alltid är korrekt uppdaterad."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ab0d57c960b0568c1da1896914f1a1ce939d0ea
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="service-posting"></a>Servicebokföring
Funktionen för servicebokföring gör att du kan behandla dokumenten mer effektivt och upprätthålla en bra service till kunderna. Du kan skapa och uppdatera bokförda dokument och skapa transaktioner i modulen Service och i andra moduler så att informationen alltid är korrekt uppdaterad.  

> [!NOTE]  
>  Nedan beskrivs servicebokföring oavsett hur artiklar ska hanteras fysiskt i distributionslagret.  
>   
>  I ett lagerställe som inte har konfigurerats med krav på lagerhantering, utför du bokföringsåtgärder direkt från fönstret **Servicerader**. I lagerställen som omfattar lagerhantering utförs de beskrivna bokföringsåtgärderna, utom förbrukning, indirekt via varierande lagerleveransfunktioner beroende på konfiguration. För mer information, se [så här: Plocka artiklar med lagerplockningar](warehouse-how-to-pick-items-with-inventory-picks.md).  

## <a name="ship"></a>Leverera  
Med det här leveransalternativet kan du registrera alla relevanta artiklar och tidpunkter som har angetts på raderna i en serviceorder efter att servicen har slutförts. En bokförd utleverans skapas och uppdateringar sker i modulen Lager och i andra moduler i [!INCLUDE[d365fin](includes/d365fin_md.md)] för att visa att artiklarna har tagits från lagret och skickats till kunden. Mer specifikt skapas artikeltransaktioner, värdetransaktioner, servicetransaktioner och garantitransaktioner.  

Om lagerstället kräver distributionslagerhantering sker leverans och flytt av serviceradartiklar av artiklar på samma sätt som för övriga källdokument. Den enda skillnaden är att serviceradartiklar kan förbrukas antingen externt eller internt, vilket kräver två olika släppfunktioner.

## <a name="invoice"></a>Fakturera  
Det här alternativet måste användas om du vill skicka en faktura till kunden som ska debiteras för servicen. Vanligtvis är det skillnaden mellan det levererade antal som har registrerats med funktionen **Bokför utleverans** och det förbrukade antal som har registrerats med funktionen **Bokför förbrukning** som ska faktureras. Det går inte att fakturera artiklar som inte har levererats. När du kör funktionen **Bokför fakturor** skapas en bokförd servicefaktura och tidigare bokförda dokument uppdateras så att de blir konsekventa med antalet på fakturan. Precis som vid andra bokföringsprocedurer skapas alla relevanta transaktioner, innefattande redovisningstransaktioner.  

## <a name="ship-and-invoice"></a>Leverera och fakturera  
Med alternativet leverera och fakturera kan du skapa både en serviceleverans och en faktura samtidigt.  

## <a name="ship-and-consume"></a>Leverera och förbruka  
Med det här leverans- och förbrukningsalternativet kan du registrera och bokföra artiklar, kostnader eller timmar som har använts för service men som inte kan tas med i fakturan till kunden. Ingen faktura skapas, men du kan skapa en serviceutleverans och en serviceförbrukning samtidigt om du vill visa att kunden har fått en del artiklar eller timmar utan kostnad. Motsvarande transaktioner skapas också för att registrera förbrukningen.  

> [!NOTE]  
>  Med funktionen för servicebokföring kan du välja att utföra bokföringen delvis. Du kan skapa en delleverans eller en delfaktura genom att fylla i fältet **Ant. att utleverera** och **Ant. att fakturera** på var och en av  serviceraderna på dina serviceorder innan du bokför. Observera att det inte går att skapa en faktura för något som inte har levererats. Innan du fakturerar måste du alltså ha registrerat en leverans, eller så måste du leverera och fakturera samtidigt.  

När bokföringen har slutförts kan du visa de bokförda servicedokumenten från motsvarande fönster **Bokförd serviceutleverans** och **Bokförd servicefaktura**. De bokförda transaktionerna som har skapats visas i de fönster som innehåller bokförda transaktioner, t.ex. **Redovisningstransaktioner**, **Artikeltransaktioner**, **Dist.lager transaktioner**, **Servicetransaktioner**, **Projekttransaktioner** och **Garantitransaktioner**.  

## <a name="to-view-information-about-a-posted-service-document"></a>Så här visar du information om bokförda servicedokument  
När du bokför en servicefaktura, en serviceleverans eller en servicekreditnota överförs informationen i dokumentet till fönstret  **Bokförd servicefaktura**,  **Bokförd serviceleverans** eller  **Bokförd servicekreditnota**. Det går inte att ange, ändra eller ta bort något i de här fönstren. Du kan skriva ut en leverans, faktura eller kreditnota från fönstren.  

I proceduren nedan används en bokförd servicefaktura som exempel, men samma procedur kan koppla till den bokförda serviceleveransen och bokförda kreditnotor.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Bokförda försäljningsfaktura** och välj sedan relaterad länk.  
2. Öppna den bokförda servicefaktura som du vill visa.  
3. Om du vill få en översikt över den bokförda fakturan, väljer du åtgärden **statistik**.  

    Fönstret **Serviceorderstatistik** öppnas. Här visas information som antal, belopp, moms, kostnad, TB och kundkreditlimit för det bokförda dokumentet.

## <a name="see-also"></a>Se även  
[Så här bokför du serviceorder](service-how-to-post-service-orders.md)   
[Så här skapar du serviceorder](service-how-to-create-service-orders.md)

