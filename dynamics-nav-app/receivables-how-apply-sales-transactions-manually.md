---
title: "Koppla kundreskontratransaktioner för att manuellt stämma av kundbetalningar"
description: "Beskriver hur du använder inbetalningar eller återbetalningar för kunder till en eller flera öppna kundreskontratransaktioner och stämma av kundbetalningar."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, cash receipt
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bf6be6c1e4130396210555a394f39f0ce4b54f5a
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-reconcile-customer-payments-manually"></a>Så här stämmer du av kundbetalningar rabatter manuellt
När du får en inbetalning av en kund eller när du gör en kontant återbetalning måste du bestämma om inbetalningen eller återbetalningen ska kopplas till en eller flera öppna debet- eller kredittransaktioner. Du kan ange det belopp som du vill koppla. Du kan till exempel använda delbetalningar till kundreskontratransaktioner. Att avsluta kundreskontratransaktioner ser till att informationen som t.ex. kundstatistik och kontoutdrag och dröjsmålsräntor är korrekta.

> [!NOTE]  
>   I fönstret **kundreskontratransaktioner** betyder rött teckensnittet att den relaterade betalningen kommer efter dess förfallodatum.

Du kan koppla kundreskontratransaktioner på olika sätt:

* Genom att ange information i det dedikerade fönstret som till exempel fönstret **Inbetalningsjournal** och fönstret **Betalningsavstämningsjournal**.
* Från försäljningskreditnotor.
* Från kundreskontratransaktioner efter att försäljningsdokument har bokförts men inte har kopplats.

> [!NOTE]  
>   Om fältet **Avräkningsmetod** på kundkortet innehåller **Koppla till äldsta faktur**, kommer betalningen att kopplas till den äldsta öppna kredittransaktionen om du inte manuellt anger en transaktion. Om avräkningsmetoden för en leverantör är **Manuell** måste du alltid koppla transaktioner manuellt.

Du kan tillämpa kundbetalningar manuellt i fönstret **Inbetalningsjournal**. En inbetalningsjournal är en sorts redovisningsjournal, så du kan använda den för att bokföra transaktioner på redovisningskonton, bankkonton, kundkonton, leverantörskonton och anläggningstillgångskonton. Du kan koppla betalningen till en eller flera debettransaktioner när du bokför betalningen, eller så kan du koppla från de bokförda transaktionerna senare.

Du kan också tillämpa kundbetalningar och leverantörsbetalningar i fönstret **Betalningsavstämningsjournal** med hjälp av funktioner för bankutdragsimport, automatiskt koppling och bankkontoavstämning. Mer information finns i [Stämma av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md). Alternativt kan du stämma av kundutbetalningar utifrån en lista över obetalda försäljningsdokument i fönstret **Betalningsregistrering**. Mer information finns i [Så här stämmer du av kundutbetalningar manuellt från en lista med obetalda försäljningsdokument](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)

## <a name="to-fill-and-post-a-cash-receipt-journal"></a>Så här fyller du i och bokför en inbetalningsjournal:
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inbetalningsjournal**, och välj sedan relaterad länk.
2. Välj åtgärden **Redigera journal**.
3. Välj önskat namn i fältet **Journalnamn**.
4. Fyll i fältet **Bokföringsdatum**.  
5. I fältet **Dokumenttyp** väljer du **Betalning**.

    Fältet **Dokumentnr** fylls i av den nummerserie som har tilldelats journalen.  
6. Använd fältet **Externt verifikationsnr** om du lagrat ett ID t.ex kundens checknummer.
7. I fältet **Kontotyp** väljer du **Kund**.
8. I fältet **bankkontonr.** väljer du relevant redovisningskonto.
9. Gör något av följande om du vill bokföra kopplingen samtidigt som du bokför journalen.
10. I fältet **Motkontotyp** väljer du **Redovisningskonto** för kontantbetalningar eller **Bankkonto** för andra typer av betalningar.
11. Välj kontantkontot för kontantbetalningar eller rätt bankkonto för andra typer av betalningar i fältet **Motkonto**.
12. Bokför journalen.

## <a name="to-apply-a-payment-to-a-single-customer-ledger-entry"></a>Så här kopplar du en betalning till en enskild kundreskontratransaktion
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inbetalningsjournal**, och välj sedan relaterad länk.
2. Välj åtgärden **Redigera journal**.
3. Ange information om den transaktion som ska kopplas på den första journalraden.
4. I fältet **Dokumenttyp** anger du **Betalning**.
5. I fältet **Kontotyp** anger du **Kund**.
6. I fältet **Motkontotyp** anger du **Bankkonto.**
7. I fältet **Kopplas till ver.nr** väljer du fältet för att öppna fönstret **Koppla kundtransaktioner**.
8. I fönstret **Koppla kundtransaktioner** markerar du transaktionen som du vill koppla betalningen till.
9. I fältet **Belopp att koppla** anger du det belopp som du vill koppla till transaktionen. Om du inte anger något belopp kopplas det maximala beloppet.

    Längst ned i fönstret **Koppla kundtransaktioner** kan du se beloppet i fältet **Kopplat belopp** och om kopplingen balanserar.  
10. Välj **OK**. I fönstret **Inbetalningsjournal** visas nu transaktionen som du har valt i fälten **Kopplas till dokumenttyp** och **Kopplas till ver.nr.**
11. Bokför inbetalningsjournalen.

## <a name="to-apply-a-payment-to-multiple-customer-ledger-entries"></a>Så här kopplar du en betalning till flera kundreskontratransaktioner
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inbetalningsjournal**, och välj sedan relaterad länk.
2. Välj åtgärden **Redigera journal**.
3. Ange information om den transaktion som ska kopplas på den första journalraden.
4. I fältet **Dokumenttyp** anger du **Betalning**.
5. I fältet **Kontotyp** anger du **Kund**.
6. I fältet **Motkontotyp** anger du **Bankkonto.**
7. I fältet **Belopp** anger du den fullständiga betalningen som ett negativt belopp.
8. Om du vill koppla betalningen till flera kundreskontratransaktioner vid bokföringen väljer du åtgärden **Koppla transaktioner**.  
9. Markera raderna med de poster som du vill koppla transaktionen till och väljer sedan åtgärden **Koppla till ID**.  
10. På varje rad i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten. Om du inte anger något belopp kopplas det maximala beloppet.

    Längst ned i fönstret **Koppla kundtransaktioner** kan du se beloppet i fältet **Kopplat belopp** och om kopplingen balanserar.  
11. Välj **OK**.
12. Bokför inbetalningsjournalen.

## <a name="to-apply-a-credit-memo-to-a-single-customer-ledger-entry"></a>Så här kopplar du en kreditnota till en enskild kundreskontratransaktion
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningskreditnotor** och välj sedan relaterad länk.
2. Öppna relevant försäljningskreditnota.
3. Om du vill koppla kreditnotan till en enskild kundreskontratransaktion vid bokföring klickar du på snabbfliken **Kopplas till ver.nr** och väljer den transaktion som du vill koppla betalningen till.
4. På raden i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten.  

    Om du inte anger något belopp kopplas automatiskt det maximala beloppet. Längst ned i fönstret **Koppla kundtransaktioner** kan du se beloppet i fältet **Kopplat belopp** och om kopplingen balanserar.    
5. Välj **OK**. I fönstret **Försäljningskreditnota** visas nu transaktionen som du har valt i fälten **Kopplas till dokumenttyp** och **Kopplas till ver.nr.** Och beloppet på den kreditnota som ska bokföras justerat för eventuell kassarabatt.
6. Bokför kreditnotan.

## <a name="to-apply-a-credit-memo-to-multiple-customer-ledger-entries"></a>Så här kopplar du en kreditnota till flera kundreskontratransaktioner
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningskreditnotor** och välj sedan relaterad länk.
2. Öppna relevant försäljningskreditnota.
3. Om du vill koppla kreditnotan till flera kundreskontratransaktioner vid bokföringen väljer du åtgärden **Koppla transaktioner**.
4. Markera raderna med de poster som du vill koppla transaktionen till och väljer sedan åtgärden **Koppla till ID**.
5. På varje rad i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten. Om du inte anger något belopp kopplas det maximala beloppet.  

    Längst ned i fönstret **Koppla kundtransaktioner** kan du se beloppet i fältet **Kopplat belopp** och om kopplingen balanserar.  
6. Välj **OK**. Fönstret **Förs.kreditnota** innehåller nu beloppet på den kreditnota som ska bokföras justerat med eventuell kassarabatt.
7. Bokför kreditnotan.

## <a name="to-apply-posted-customer-ledger-entries"></a>Så här kopplar du bokförda kundreskontratransaktioner
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kunder** och välj sedan relaterad länk.
2. Öppna kundkortet för kunden med transaktionerna som du vill koppla.
3. Välj åtgärden **Transaktioner** och välj sedan raden med transaktionen som ska vara kopplingstransaktionen.
4. Välj åtgärden **Koppla transaktioner**. Fönstret **Koppla kundtransaktioner** öppnas där du kan se de öppna transaktionerna för kunden.
5. Markera raderna med de poster som du vill koppla transaktionen till och väljer sedan åtgärden **Koppla till ID**. .
6. På varje rad i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten. Om du inte anger något belopp kopplas det maximala beloppet.  

    Längs ned i fönstret **Kopplat belopp** kan du se det specifika beloppet i fältet **Koppla kundtransaktioner**.  
7. Välj åtgärden **Bokför kopplade trans.**. Fönstret **Bokför kopplade trans.** visas med dokumentnumret för den kopplade transaktionen och bokföringsdatumet för den post som har det senaste bokföringsdatumet.  
8. Klicka på **OK** för att bokföra kopplingen.

    Om den bokförda kopplingen har medfört avslutade kundreskontratransaktioner finns det inte längre någon sådan markering i fältet **Öppen**.    
9. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningskreditnotor** och välj sedan relaterad länk. Bläddra till kortet för att den relevanta kunden ska se de redovisningstransaktioner.  

I transaktionslistan på raden som innehåller transaktionen som helt kopplades till kan du se att kryssrutan **Öppen** inte är markerad.  

> [!NOTE]  
>   När du har valt en post i fönstret **Koppla kundtransaktioner** eller flera poster genom att anger **Koppla till ID** kommer fältet **Kopplat belopp** på journalraden att innehålla summan av de återstående beloppen för de bokförda poster som du har valt, om inte fältet redan innehåller något värde. Om du väljer **Koppla till äldsta trans.** i fältet **Avräkningsmetod** på kundkortet utförs kopplingen automatiskt.

## <a name="to-apply-customer-ledger-entries-in-different-currencies-to-one-another"></a>Så här kopplar du kundreskontratransaktioner i olika valutor till varandra
Om du säljer i en valuta och får betalt i en annan kan du ändå koppla fakturan till betalningen.  

Om du kopplar en post (post 1) i en valuta till en post (post 2) i en annan valuta används bokföringsdatumet för post 1 för att söka efter rätt valutakurs att omvandla belopp efter i post 2. Rätt valutakurs hittas i fönstret **Valutakurser**.  

Koppla kundreskontratransaktioner i olika valutor till varandra måste vara aktiverad. Mer information finns i [Så här aktiverar du koppling av kundreskontratransaktioner till olika valutor](finance-how-enable-application-ledger-entries-different-currencies.md).  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inbetalningsjournal**, och välj sedan relaterad länk.
2. Öppna den journal som du vill ha och fyll i första tomma journalrad med en valutakod.
3. Välj åtgärden **Koppla transaktioner**.
4. Välj raden med den post som du vill koppla till posten i inbetalningsjournalen. Klicka sedan på åtgärden **Koppla till ID** och välj den post som du vill koppla till.
5. Välj knappen **OK** om du vill återvända till inbetalningsjournalen.
6. Bokför försäljningsjournalen.  

> [!IMPORTANT]  
>   När du kopplar poster i olika valutor till varandra omvandlas posterna till USD. Även om valutakurserna är fasta för de två aktuella valutorna, t.ex. mellan USD och EUR, kan det uppstå ett litet restbelopp när beloppen omvandlas till USD. Dessa små restbelopp bokförs som vinster och förluster på kontot som har angetts i fältet **Kursvinster konstaterade** eller i fältet **Kursförluster konstaterade** i fönstret **Valutor**. Fältet **Belopp (USD)** justeras också i de aktuella leverantörsreskontratransaktionerna.  

## <a name="to-correct-an-application-of-customer-entries"></a>Så här rättar du en koppling av kundtransaktioner
När du rättar en koppling skapas och bokförs korrigeringstransaktioner som är identiska med den ursprungliga transaktionen, men med motsatt tecken i beloppsfältet för alla transaktioner, inklusive all redovisningsbokföring som gjorts i redovisningen till följd av kopplingen, t.ex. kassarabatter och valutakursvinster/-förluster. Alla transaktioner som stängdes av kopplingen öppnas på nytt.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kunder** och välj sedan relaterad länk.
2. Öppna relevant kundkort.
3. Välj åtgärden **Transaktioner**.
4. Välj aktuell transaktion och klicka på åtgärden **Ta bort koppling på trans.**.
5. Välj alternativt åtgärden **Detaljerad transaktion**.
6. Välj aktuell koppling och klicka på åtgärden **Ta bort koppling på trans.**.
7. Fyll i fälten i huvudet och välj sedan åtgärden **Ta bort koppling**.  

> [!IMPORTANT]  
>   Om en post har använts i flera kopplingar måste du ta bort den senaste kopplingen först.  

## <a name="see-also"></a>Se även
[Hantera kundreskontra](receivables-manage-receivables.md)  
[Försäljning](sales-manage-sales.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

