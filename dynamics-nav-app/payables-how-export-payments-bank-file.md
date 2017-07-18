---
title: "Så här exporterar du betalningar till en bankfil"
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
ms.openlocfilehash: 09bdf56b3d5e76b12d868091e89232ce9c08e215
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-export-payments-to-a-bank-file"></a>Så här exporterar du betalningar till en bankfil
När du är redo att göra betalningar till leverantörer med hjälp av **Betalningsjournal** fönster, kan du exportera en fil med betalningsinformation på journalraderna. Du kan sedan överföra filen till den elektroniska banken att bearbeta relaterade pengaöverföringar.

I den generiska versionen av Dynamics NAV ställs en global tjänstleverantör in och ansluts för att konvertera bankdata till valfritt filformat som din bank kräver.

**Obs!** Innan du kan exportera från en utbetalningsjournal måste du aktivera export på den relaterade journalen. Dessutom måste ditt bankkonto och leverantörens bankkonto ställas in för elektronisk betalning. Mer information finns i [Så här konfigurerar du bankdatakonverteringstjänsten](bank-how-setup-bank-data-conversion-service.md).

Du använder fönstret **Kreditöverföringsregister** för att visa de betalningsfiler som har exporterats från betalningsjournalen. I det här fönstret kan du också återexportera betalningfiler i händelse av tekniska fel, eller om filen ändras.

## <a name="to-export-payments-to-a-bank-file"></a>Exportera betalningar till en bankfil
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningsjournal** och välj sedan relaterad länk.
2. Fyll i betalningsjournalen med relevanta utbetalningar, till exempel genom att använda funktionen **Betalningsförslag för lev.**. Mer information finns i [Så här föreslår du leverantörsbetalningar](payables-how-suggest-vendor-payments.md).  
3. När du har gjort alla betalningsjournalrader, väljer du **Exportera betalning till fil**.

    Felmeddelanden visas i faktaboxen **Fel i betalningsfil** där du kan även välja ett felmeddelande om du vill se detaljerad information. Du måste lösa alla fel innan betalningsfilen kan exporteras.

    **Tips** När du använder tjänsten för bankdatakonvertering visas ett vanligt felmeddelande som berättar att bankkontonumret inte har den längd som din bank kräver. För att undvika eller åtgärda felet, måste du ta bort värdet i fältet **IBAN** i fönstret **Bankkontokort** och sedan i **Bankkontonr.** anger du ett bankkonto i formatet som din bank krävs.
4. I fönstret **Spara som** anger du var filen ska exporteras till och välj sedan **Spara**.

Bankbetalningsfilen exporteras till den plats som du anger, och du kan fortsätta att föra över den till ditt elektroniska bankkonto och göra de faktiska beloppen.

När du tar emot en bekräftelse på att betalningarna har behandlats korrekt i banken kan du bokföra de exporterade utbetalningsjournalraderna.

## <a name="to-plan-when-to-post-exported-payments"></a>Så här planerar du när du vill bokföra exporterad betalning
Om du inte vill bokföra en utbetalningsjournalrad för en exporterad betalning, till exempel eftersom du väntar på en bekräftelse att transaktionen har behandlats av banken, kan du bara ta bort journalraden. När du senare skapar en utbetalningsjournal för att betala återstående belopp på fakturan kan du i fältet **Totalt exporterat belopp** se hur mycket av beloppet som redan har exporterats. Du kan också söka efter detaljerad information om det exporterade totalbeloppet genom att välja knappen **Transaktioner i kreditöverföringsregister** för att visa detaljer om exporterade betalningsfiler.

Om du följer en process där du inte vill bokföra utbetalningar, tills du har bekräftelsemeddelande att de har behandlats i banken, kan du använda detta två sätt.

* I en utbetalningsjournal med föreslagna betalningsrader kan du sortera på antingen kolumnen **Exporterat till betalningsfil** eller **Totalt exporterat belopp** och sedan ta bort betalningsförslag för öppna fakturor för vilka betalningar som redan har gjorts och du inte vill göra betalningar för.
* På liknande sätt kan du i batchjobbet **Betalningsförslag för lev.**, där du anger vilka betalningar som ska infogas i utbetalningsjournalen, markera kryssrutan **Hoppa över exporterade betalningar** om du inte vill infoga journalrader för betalningar som redan har exporterats.

Om du vill visa information om exporterade betalningar väljer du åtgärden **Betalningsexporthistorik**.

## <a name="to-re-export-payments-to-a-bank-file"></a>Så här återexporterar du betalningar till en bankfil
Du kan återexportera betalningsfiler till en bankfil från fönstret **Kreditöverföringsregister**. Innan du tar bort eller bokför utbetalningsjournalrader kan du också återexportera betalningsfilen från fönstret **Betalningsjournal** genom att helt enkelt exportera den på nytt.

Om du har tagit bort eller bokfört rader i utbetalningsjournalen efter att du har exporterat dem kan du återexportera samma betalningsfil från fönstret **Kreditöverföringsregister**. Markera raden för batchen med kreditöverföringar du vill återexportera och välj sedan åtgärden **Återexportera betalningar till fil**.

## <a name="see-also"></a>Se även
[Leverantörsreskontra](payables-manage-payables.md)  
[Hantera inköp](purchasing-manage-purchasing.md)  
[Konfigurera inköp](purchasing-setup-purchasing.md)

