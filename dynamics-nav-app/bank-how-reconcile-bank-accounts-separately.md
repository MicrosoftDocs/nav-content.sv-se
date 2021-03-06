---
title: "Stämma av bankkonton separat"
description: "Beskriver hur ditt lagervärde stäms av med redovisningen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account balance, bank statement
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9742569e97f8b2ad5546b364d76edb702f1a0c1c
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-reconcile-bank-accounts-separately"></a>Så här stämmer du av bankkonton separat
För att stämma av bankkonton i [!INCLUDE[d365fin](includes/d365fin_md.md)] med utdrag från banken måste du först fylla i raderna i fönstret **Bankkontoavstämning**.

> [!NOTE]  
>   Du kan också stämma av bankkonton i fönstret **Betalningsavstämningsjournal**. Eventuella öppna bankkontotransaktioner som relateras till kopplade kund- eller leverantörsreskontratransaktionerna kommer att avslutas när du väljer **Bokför betalningar och stäm av bankkonton**. Detta betyder att bankkontot stäms av automatiskt för betalningar som du bokför med journalen. Mer information finns i [Så här stämmer du av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md).

Om du vill importera ett bankutdrag som bankfeed måste du först ställa in och aktivera tjänsten bankdatakonvertering. Mer information finns i [Så här konfigurerar du bankdatakonverteringstjänsten](bank-how-setup-bank-data-conversion-service.md).

Raderna i fönstret **Bankkontoavstämning** är uppdelade i två rutor. Rutan **Bankkontoavstämning** visar antingen importerade banktransaktioner eller transaktioner med utestående utbetalningar. Rutan **Bankkontotransaktioner** visar transaktionerna på bankkontot.

Aktiviteten att hitta och koppla transaktioner som ska stämmas av benämns som *matchning*. Du kan välja att utföra matchning automatiskt genom att använda funktionen **Matcha automatiskt**. Alternativt kan manuellt välja rader i båda fönster för att koppla varje kontoutdragrad till en eller flera motsvarande bankkontotransaktioner och sedan använda **Matcha manuellt** funktionen. Kryssrutan **Kopplad** markeras på rader där transaktioner matchas.

Du kan fylla i rutan **Kontoutdragrader** i fönstret **Bankkontoavstämning** på följande sätt:

* Automatiskt, genom att använda funktionen **Importera bankutdrag** för att fylla i raderna enligt faktiska bankkontotransaktioner som baseras på en fil som tillhandahålls i banken.
* Manuellt genom att använda funktionen **Föreslå rader** för att fylla i raderna med transaktioner för fakturor som har utestående utbetalningar.

När värdet i fältet **Totalt saldo** i rutan **Bankutdragsrader** är lika med värdet i fältet **Saldo att stämma av** i rutan **Bankkontotransaktioner** kan du välja åtgärden **Bokför** för att stämma av de kopplade bankkontotransaktionerna. Alla icke godkända bankkontotransaktioner kommer att stå kvar i fönstret vilket innebär att betalningar som ska bearbetas för bankkonto inte återspeglas i det senaste bankkontoutdraget eller att några betalningar mottogs via checkar.

> [!NOTE]  
>   Om kontoutdragrader hör till checktransaktioner, kan du inte använda de matchningsfunktionerna. I stället måste du välja åtgärden **Koppla trans.** och sedan välja den relevanta checktransaktionen att matcha kontoutdragraden med.

## <a name="to-fill-bank-reconciliation-lines-by-importing-a-bank-statement"></a>Så här fyller du i bankavstämningrader genom att importera ett kontoutdrag
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Bankkontoavstämningar** och välj sedan relaterad länk.
2. Välj åtgärden **Ny**.
3. Välj ett bankkonto i fältet **Bankkontonr**. Bankkontotransaktionerna som finns på bankkonto, visas i rutan **Bankkontotransaktioner**.
4. Ange datumet på kontoutdraget från banken i fältet **Kontoutdragets datum**.
5. Ange saldot på kontoutdraget från banken i fältet **Kontoutdragets slutsaldo**.
6. Om du har en bankutdragsfil väljer du åtgärden **Importera bankutdrag**.
7. Leta upp filen och välj sedan knappen **Öppna** för att importera banktransaktionerna till raderna i fönstret **Bankkontoavstämning**.

## <a name="to-fill-bank-reconciliation-lines-with-the-suggest-lines-function"></a>Så här fyller du i bankavstämningrader med funktionen Föreslå rader
1. I fönstret **Bankkontoavstämning** väljer du åtgärden **Föreslå rader**.
2. Ange det tidigaste bokföringsdatumet för transaktionsavstämningen i fältet **Startdatum**.
3. Ange det senaste bokföringsdatumet för transaktionsavstämningen i fältet **Slutdatum**.
4. Om du vill att föreslå checktransaktion istället för bankkontotransaktioner markerar du kryssrutan **Ta med checkar**.
5. Välj **OK**.

## <a name="to-match-bank-statement-lines-with-bank-account-ledger-entries-automatically"></a>Så här matchar du automatiskt kontoutdragrader med bankkontotransaktioner
1. I fönstret **Bankkontoavstämning** väljer du åtgärden **Matcha automatiskt**. Fönstret **Matcha banktransaktioner** öppnas.
2. Ange antalet dagar före och efter bankkontotransaktionbokföringsdatumet som funktionen ska söka i för att matcha bokföringsdatum i bankkontoutdraget i fältet **Bokföringsdatumtolerans (dagar)**.

    Om du anger 0 eller lämnar fältet tomt kommer funktionen **Matcha automatiskt** endast söka efter matchande bokföringsdatum på bankkontotransaktionbokföringsdatumet.
3. Välj **OK**.

    Alla kontoutdragrader och bankkontotransaktioner som kan matchas ändrar till grönt teckensnitt och **Kopplat** kryssrutan markeras.
4. Markera kontoutdragraden och välj sedan åtgärden **Ta bort matchning**.

## <a name="to-match-bank-statement-lines-with-bank-account-ledger-entries-manually"></a>Så här matchar du manuellt bankutdragsrader med bankkontotransaktioner
1. I fönstret **Bankkontoavstämning** markerar du en okopplad rad i rutan **Kontoutdragrader**.
2. I rutan **Bankkontotransaktioner** markerar du en eller flera bankkontotransaktioner som kan matchas med den valda kontoutdragraden. Om du vill välja flera rader, tryck och håll ned CTRL-tangenten.
3. Välj åtgärden **Matcha manuellt**.

    Den valda kontoutdragraden och de valda bankkontotransaktionerna ändrar till grönt teckensnitt och **Kopplat** kryssrutan i det högra fönstret markeras.
4. Upprepa moment 1 till och med 3 för alla kontoutdragrader som inte matchas.
5. Markera kontoutdragraden och välj sedan åtgärden **Ta bort matchning**.

## <a name="to-create-missing-ledger-entries-to-match-bank-transactions-with"></a>Så här skapar du saknade transaktioner för att matcha med banktransaktioner
Ibland kan det hända att ett kontoutdrag från banken innehåller belopp som motsvarar en avgift eller räntekostnad. Sådana banktransaktioner kan inte matchas, eftersom inga relaterade transaktioner finns i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Du måste sedan bokföra en journalrad för varje transaktion för att skapa en artikelrelaterad transaktion som den kan matchas med.

1. I fönstret **Bankkontoavstämning** väljer du åtgärden **Överföring till redovisningsjournal**.  
2. I fönstret **Bankavst. trans. åt redov.jnl** anger du vilka redovisningsjournalen om du vill använda och klickar på knappen **OK**.

    Fönstret **Redovisningsjournal** öppnas med nya journalrader för alla bankrapportrader med saknade transaktioner.
3. Fyll i journalraden med information, till exempel motkonton. Mer information finns i [Arbeta med Redovisningsjournaler](ui-work-general-journals.md).  
4. Välj åtgärden **Bokföra**.

    När transaktionen har bokförts går du vidare och matchar bankkontotransaktionen med den.
5. Uppdatera eller öppna fönstret **Bankkontoavstämning** igen. Den nya transaktionen ska visas i fönstret **Bankkontotransaktioner**.
6. Matcha kontoutdragraden till bankkontotransaktionen, antingen manuellt eller automatiskt.

## <a name="see-also"></a>Se även
[Hantera bankkonton](bank-manage-bank-accounts.md)  
[Ställa in bankverksamhet](bank-setup-banking.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

