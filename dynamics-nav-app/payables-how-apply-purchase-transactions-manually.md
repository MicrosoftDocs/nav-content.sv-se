---
title: "Så här kopplar du leverantörsbetalningar manuellt"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d3aaafc9ac3dcfd1fba3802b1158bde890e09110
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-apply-vendor-payments-manually"></a>Så här kopplar du leverantörsbetalningar manuellt

När du skickar ett betalningskvitto till, eller tar emot en återbetalning från, en leverantör måste du bestämma om du ska koppla betalningen eller återbetalningen till en eller flera öppna debet- eller kreditposter. Du kan ange det exakta beloppet som ska kopplas till betalningsinleveransen eller återbetalningen och därmed endast delvis koppla leverantörsreskontratransaktioner. Du måste koppla alla leverantörsreskontratransaktioner för att leverantörsstatistik och rapporter över kontoutdrag och finansavgifter ska bli korrekta.

**Obs!** Leverantörer föredrar ibland återbetalning framför en kreditnota som ska användas mot framtida fakturor, särskilt om du returnerar artiklar som du redan har betalt eller om du har betalat för mycket för en faktura.

Du kan koppla leverantörsreskontratransaktioner på tre olika sätt:

- Genom att ange information i det dedikerade fönstret som till exempel fönstret **Utbetalningsjournal** och fönstret **Betalningsavstämningsjournal**.
- Från inköpskreditnotor.
- Från leverantörsreskontratransaktioner efter att inköpsdokument har bokförts men inte har kopplats.

**Obs!** Om fältet **Avräkningsmetod** på leverantörskortet innehåller **Koppla till äldsta faktura**, kommer betalningen att kopplas automatiskt till den äldsta öppna kredittransaktionen om du inte manuellt anger vilken transaktion som ska kopplas till. Om avräkningsmetoden för en kund är **Manuell** måste du koppla transaktioner manuellt.

Du kan koppla leverantörsbetalningar manuellt till dess relaterade inköpsdokument, när du bokför utbetalningarna i fönstret **Utbetalningsjournal**. Mer information om att fylla i utbetalningsjournalen finns i [Så här gör du betalningar](payables-make-payments.md).

Du kan också koppla leverantörsbetalningar och kundutbetalningar när utbetalningarna visas som negativa banktransaktioner på banken. I fönstret **Betalningsavstämningsjournal** kan du använda funktioner för import av kontoutdrag, automatisk koppling och bankkontoavstämning. Mer information finns i [Stämma av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md).

## <a name="to-apply-a-payment-to-a-single-or-multiple-vendor-ledger-entries"></a>Så här kopplar du en betalning till en enskild eller flera leverantörsreskontratransaktioner
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Utbetalningsjournal** och välj sedan relaterad länk.
2. Ange information om betalningstransaktionen på den första journalraden i fönstret **Utbetalningsjournal**.
3. Så här kopplar du en enskild leverantörsreskontratransaktion:
4. I fältet **Kopplas till ver.nr.** väljer du fältet för att öppna fönstret **Koppla leverantörstrans.**.
5. I fönstret **Koppla leverantörstrans.** markerar du transaktionen som du vill koppla betalningen till.
6. På raden i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten.
7. Eller så här kopplar du flera leverantörsreskontratransaktioner:
8. Välj åtgärden **Koppla transaktioner**.
9. I fönstret **Koppla leverantörstrans.** markerar du raden med transaktioner som du vill koppla betalningen till.
10. Välj åtgärden **Koppla till ID**.  
11. På varje rad i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten.

    Om du inte anger något belopp kopplas automatiskt det maximala beloppet. Längst ned i fönstret **Koppla leverantörstransaktioner** kan du se beloppet i fältet Kopplat belopp och om kopplingen balanserar.
12. Välj **OK**.
13. Om du vill bokföra utbetalningsjournalen väljer du åtgärden **Bokför**.

## <a name="to-apply-a-credit-memo-to-a-single-or-multiple-vendor-ledger-entries"></a>Så här kopplar du en kreditnota till en enskild eller flera leverantörsreskontratransaktioner:
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inköpskreditnota** och välj sedan relaterad länk.
2. Öppna den kreditnota som du vill koppla.
3. Fyll i relevant information i huvudet.
4. Så här kopplar du en enskild leverantörsreskontratransaktion:
5. På snabbfliken **Koppling** i fältet **Kopplas till ver.nr.** markerar du transaktionen som krediteringen ska kopplas till.
6. På raden i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten.
7. Eller så här kopplar du flera leverantörsreskontratransaktioner:
8. Välj åtgärden **Koppla transaktioner**.
9. Markera raderna med transaktioner som du vill koppla kreditnotan till.
10. Välj åtgärden **Koppla till ID**.  
11. På varje rad i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten.

    Om du inte anger något belopp kopplas automatiskt det maximala beloppet. Längst ned i fönstret **Koppla leverantörstransaktioner** kan du se beloppet i fältet **Kopplat belopp** och om kopplingen balanserar.
12. Välj **OK**.  
I fönstret **Inköpskreditnota** visas nu transaktionen som du har valt i fältet **Kopplas till dokumenttyp** och **Kopplas till ver.nr.** . Fönstret innehåller nu också beloppet på den kreditnota som ska bokföras justerat med eventuell kassarabatt.
13. Klicka på knappen **Bokför** för att bokföra inköpskreditnotan.

## <a name="to-apply-posted-vendor-ledger-entries"></a>Så här kopplar du bokförda leverantörsreskontratransaktioner:

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Leverantörer** och välj sedan relaterad länk.
2. Öppna relevant leverantör med poster som redan bokförts.
3. Välj åtgärden **Transaktioner** och välj sedan åtgärden **Koppla transaktioner**.
4. I fönstret **Koppla leverantörstrans.** visas leverantörens öppna transaktioner.
5. Markera raden med den transaktion som ska kopplas.
6. Välj åtgärden **Koppla till ID**.
7. I fältet **Koppla till ID** visas tre asterisker (***) om du arbetar i ett enanvändarsystem, eller ditt användar-id om du arbetar i ett fleranvändarsystem.  
8. På varje rad i fältet **Belopp att koppla** anger du det belopp som du vill koppla till posten.

    Om du inte anger något belopp kopplas automatiskt det maximala beloppet. Längs ned i fönstret **Koppla leverantörstrans.** kan du se beloppet i fältet **Kopplat belopp**.
9. Välj åtgärden **Bokför kopplade trans.**.  
Fönstret **Bokför kopplade trans.** öppnas med dokumentnumret för den kopplade transaktionen och bokföringsdatumet för den post som har det senaste bokföringsdatumet.
10. Klicka på **OK** för att bokföra kopplingen.

## <a name="to-apply-vendor-ledger-entries-in-different-currencies-to-one-another"></a>Så här kopplar du leverantörsreskontratransaktioner i olika valutor till varandra:
Om en valuta används vid inköp från en leverantör och en annan vid betalning kan du ändå koppla fakturan till betalningen.

Om du kopplar en post (post 1) i en valuta till en post (post 2) i en annan valuta används bokföringsdatumet för post 1 för att söka efter rätt valutakurs att omvandla belopp efter i post 2. Rätt valutakurs hittas i fönstret **Valutakurser**.

Koppla leverantörsreskontratransaktioner i olika valutor till varandra måste vara aktiverad. Mer information finns i [Så här aktiverar du koppling av kundreskontratransaktioner till olika valutor](finance-setup-how-enable-application-ledger-entries-different-currencies.md)

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Utbetalningsjournal** och välj sedan relaterad länk.
2. Öppna den journal som du vill ha och fyll i första tomma journalrad med en valutakod.
3. Välj åtgärden **Koppla transaktioner**.
4. Välj raden med den post som du vill koppla till posten i utbetalningsjournalen. Klicka sedan på åtgärden **Koppla till ID** och välj den post som du vill koppla till.
5. Välj knappen **OK** om du vill återvända till utbetalningsjournalen.
6. Bokför utbetalningsjournalen.

**Viktigt!** När du kopplar poster i olika valutor till varandra omvandlas posterna till USD. Även om valutakurserna är fasta för de två aktuella valutorna, t.ex. mellan USD och EUR, kan det uppstå ett litet restbelopp när beloppen i utländsk valuta omvandlas till USD. Dessa små restbelopp bokförs som vinster och förluster på kontot som har angetts i fältet **Kursvinster konstaterade** eller i fältet **Kursförluster konstaterade** i fönstret **Valutor**. Fältet **Belopp (USD)** justeras också i de aktuella leverantörsreskontratransaktionerna.

## <a name="to-unapply-an-application-of-vendor-entries"></a>Så här tar du bort en koppling av leverantörstransaktioner
När du tar bort en felaktig koppling skapas och bokförs korrigeringstransaktioner som är identiska med den ursprungliga transaktionen, men med motsatt tecken i beloppsfältet för alla transaktioner, inklusive all redovisningsbokföring som gjorts i redovisningen till följd av kopplingen, t.ex. kassarabatter och valutakursvinster/-förluster. Alla transaktioner som stängdes av kopplingen öppnas på nytt.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Leverantörer** och välj sedan relaterad länk.
2. Öppna relevant leverantörskort.
3. Välj åtgärden **Transaktioner**.
4. Välj aktuell transaktion och klicka på åtgärden **Ta bort koppling på trans.**.
5. Välj alternativt åtgärden **Detaljerad transaktion**.
6. Välj aktuell koppling och klicka på åtgärden **Ta bort koppling på trans.**.
7. Fyll i fälten i huvudet och välj sedan åtgärden **Ta bort koppling**.

**Viktigt!** Om en post har använts i flera kopplingar måste du ta bort den senaste kopplingen först.

## <a name="see-also"></a>Se även
[Leverantörsreskontra](payables-manage-payables.md)  
[Hantera inköp](purchasing-manage-purchasing.md)
