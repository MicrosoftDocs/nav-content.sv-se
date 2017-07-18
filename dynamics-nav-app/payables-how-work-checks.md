---
title: "Så här arbetar du med checkar"
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
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a>Så här arbetar du med checkar
Dynamics NAV stödjer elektroniskt och manuellt utfärdande av checkar. För båda metoder används utbetalningsjournalen för att utfärda checkar till leverantörer. Du kan även makulera checkar och granska checktransaktioner.

I processen för att utfärda checkar får du förslag på betalningar, transaktioner skapas och datorcheckar skrivs ut.

Skrivaren måste vara korrekt inställd med checkformulären, och du måste definiera vilken checklayout som ska användas. Mer information finns i [Så här definierar du checklayouter](finance-setup-how-define-check-layouts.md)

## <a name="to-issue-checks"></a>Så här kan du utfärda checkar
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningsjournal** och välj sedan relaterad länk.
2. Fyll i journalen med relevanta utbetalningar, till exempel genom att använda funktionen Betalningsförslag för lev. Mer information finns i [Så här föreslår du leverantörsbetalningar](payables-how-suggest-vendor-payments.md).
3. I fältet **bankbetalningstyp** på journalrader för betalning, som du vill att göra med checkar väljer du ett av följande alternativ:

 - **Datorcheck** Välj alternativet om du vill att programmet ska upprätta, och senare skriva ut, en check på beloppet på utbetalningsjournalens rad. Du måste skriva ut checkarna, innan du kan bokföra journalraderna. Du kan bara välja **Datorcheck** eller **Handskriven check** om **Motkontotyp** eller **Kontotyp** är Bankkonto.

 - **Manuell check** Välj alternativet om du vill skriva en check för hand och vill att programmet ska upprätta en motsvarande checktransaktion för beloppet. Med det här alternativen kan du inte skriva ut checkar från Dynamics NAV. Du kan bara välja **Manuell check** eller **Handskriven check** om **Motkontotyp** eller **Kontotyp** är Bankkonto.

    **Obs!** Du måste skriva ut datorcheckarna, innan du kan bokföra de relaterade journalraderna.
4. Vid datorcheckar väljer du **Skriv ut check**.
5. I fönstret **Check** fyller du i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
6. Välj knappen **Skriv ut**.

**Obs!** Om du vill skriva ut checkar i flera olika valutor från olika bankkonton måste du köra batch-jobbet **Skriv ut check** separat för varje valuta och ange bankkontot.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>Att skriva ut checkar som inte har bokförts
Du kan makulera checkar som inte har bokförts när de har skrivits ut, genom att använda åtgärden **Makulera check** i fönstret **Betalningsjournal**.
1. I fönstret **Betalningsjournal** väljer du **Makulera check** och sedan väljer du checken som ska annulleras.

## <a name="to-void-checks"></a>Så här makulerar du checkar:
När checkbetalning har bokförts, kan du bara ångra (makulera) checkar från de resulterande banktransaktionerna.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.
2. Välj det relevanta bankkontot och välj åtgärden **Redigerat** och välj sedan åtgärden **checktransaktioner**.
3. I fönstret **checktransaktioner** väljer du åtgärden **Makuler check**.
4. Markera kryssrutan **Makulera endast check**.
5. Välj knappen **OK**.

## <a name="see-also"></a>Se även
[Hantera likviditet](payables-manage-payables.md)  
[Konfigurera bank](bank-setup-banking.md)  

