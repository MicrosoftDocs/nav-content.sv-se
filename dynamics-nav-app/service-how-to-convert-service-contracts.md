---
title: "Så här: Omvandla servicekontrakt"
description: "Eftersom ändringsverktyget för momssats inte kan omvandla servicekontrakt, måste dessa konverteras manuellt. I det här avsnittet beskrivs flera alternativa metoder som du kan använda för konvertering av servicekontrakt."
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
ms.openlocfilehash: 2ae15fef88b10072a5c1dffa8e2673fe9413dd27
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-convert-service-contracts-that-include-vat-amounts"></a>Så här: omvandla servicekontrakt som innehåller momsbelopp
Eftersom ändringsverktyget för momssats inte kan omvandla servicekontrakt, måste dessa konverteras manuellt. I det här avsnittet beskrivs flera alternativa metoder som du kan använda för konvertering av servicekontrakt.  

> [!NOTE]  
>  Det här avsnittet innehåller arbetsflöde på hög nivå.  

 Nedan beskrivs hur du uppdaterar en faktura för ett förutbetald servicekontakt som har skapats ett år i förväg.  

> [!NOTE]  
>  För det här exemplet måste du ändra arbetsdatum till 01.01.2017.  

### <a name="to-correct-an-invoice-for-a-prepaid-service-contract"></a>Så här korrigerar du en faktura för ett förskottsbetalt servicekontrakt  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kontraktshantering** och välj sedan relaterad länk.  
2. Välj **Servicekontrakt** under **Listor**.  
3. Skapa ett nytt förutbetalt servicekontrakt. Ange startdatumet **01.01.2017** och fakturaperiodåret för kunden **20000**.  
4. Det kontrakt måste undertecknas. På fliken **Start** i gruppen **Process** väljer du **Signera kontrakt**.  
5. Skapa en servicefaktura.
6. Fakturera anges som en ej bokförda servicefaktura. Välj **Service**, välj **Kontraktshantering**och välj sedan **Servicefakturor** för att visa servicefakturan.  
7. Bokför servicefakturan.  

> [!NOTE]  
>  Ändra inte den ej bokförda servicefakturan. Eftersom servicetransaktioner skapas när fakturan skapas, ändrar en ändring av den ej bokförda fakturan inte de redan skapade servicetransaktionerna. Dock skapas momstransaktionerna när fakturan bokförs. Detta gör att du kan ändra den allmänna produktbokföringsmallen och GSP-produktbokföringsmallen på den ej bokförda servicefakturan.  

### <a name="to-create-a-credit-memo-for-vat-difference"></a>Så här skapar du en kreditnota för momsdifferens  
Nedan beskrivs hur du skapar en kreditnota som bara innehåller momsavvikelsen för den redan fakturerade perioden som börjar **01.07.2017**. I det här exemplet bokförs momsbeloppet endast i modulen för ekonomihantering, inte i modulen för servicehantering. Momstransaktionerna som är kopplade till servicetransaktionen kommer inte rättas.  

1. Skapa ett nytt redovisningskonto för momsdifferensen. Det här kontot ska användas för direkt bokföring av momsrättningstransaktion.  
2. Lägg till en ny rad i momsbokföringsinställningen.  

### <a name="to-create-contract-expiration-dates-in-contract-lines"></a>Så här skapar du utgångsdatum på kontraktsrader  
Nedan beskrivs hur du skapar nya kontrakt genom att arbeta med kontaktsutgångsdatum på servicekontraktsrader.  

1. I fönstret **Servicekontrakt** anger du kontraktsutgångsdatumet till **30.06.2017**.  
2. Välj åtgärden **Skapa kreditnota** för att automatiskt skapa en kreditnota för juli 2017 till december 2017.  
3. Eftersom kontraktet har löpt ut, måste du skapa ett nytt kontrakt för perioden med den nya momssatsen för 1 juli 2017 till 31 december 2017.  

### <a name="to-create-a-new-credit-memo"></a>Så är skapar du en ny kreditnota  
Nedan beskrivs hur du skapar en ny kreditnota med hjälp av batchjobbet **Hämta förutbetalda kont.trans.**. Transaktioner som du inte vill korrigera från januari 2017 till juni 2017 kommer att tas bort.  

1. Kör ändringsverktyget för momssats på 1 juli 2017.  Allmän produktbokföringsmall eller momsproduktbokföringsmallen ändras. För mer information, se [Så här arbetar du med moms för försäljning och inköp](finance-work-with-vat.md).  
2. När du har kört ändringsverktyget för momssats, anger du ett utgångsdatum för servicekontraktet. Nu kan du ta bort servicekontraktsraden och skapa en ny rad som är identisk med den gamla.  
3. Skapa en ny faktura för perioden för januari 2017 till december 2012 med den nya momssatsen.  
4. Skapa en annan kreditnota genom att, i fönstret **Servicekreditnotor**, välja **Ny** för att skapa en ny servicekreditnota.  
5. Välj åtgärden **Hämta förutbetalda kont.trans**.  
6. Efter konverteringen rättas moms- och servicetransaktioner.  

## <a name="see-also"></a>Se även  
[Så här arbetar du med servicekontrakt och servicekontraktsofferter](service-how-to-create-service-contracts-and-service-contract-quotes.md)  
[Ekonomi](finance.md)  
[Så här: rapportera moms till skattemyndigheterna](finance-how-report-vat.md)  
[Så här arbetar du med moms på försäljning och inköp](finance-work-with-vat.md)  

