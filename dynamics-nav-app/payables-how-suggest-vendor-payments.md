---
title: "Så här använder du betalningsförslag för leverantörer"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 11bfba9f279f6bd84c5d169f6f97fd48759bc6df
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-suggest-vendor-payments"></a>Så här använder du betalningsförslag för leverantörer
I fönstret **Utbetalningsjournal** kan du använda en funktion för att föreslå betalningsrader enligt dina inställningar, till exempel betalningar som förfaller snart eller betalningar där en kassarabatt är tillgänglig.

För att dra helt nytta av funktionen Betalningsförslag för lev. måste du först prioritera leverantörerna. Mer information finns i [Så här prioriterar du leverantörer](purchasing-how-prioritize-vendors.md).

Leverantörstransaktioner som inte har en markering **Stoppad** tas inte med i batch-jobbet.  

**Viktigt!** Om du vill utnyttja kassarabatterna och har angett ett disponibelt belopp, används beloppet först för prioriterade leverantörstransaktioner som förfallit, ordnade efter prioritet, därefter för förfallna leverantörstransaktioner som inte prioriterats, och till sist för öppna leverantörstransaktioner berättigade till kassarabatter, ordnade efter leverantörsnummer.

## <a name="to-use-the-suggest-vendor-payments-function"></a>Om du vill använda funktionen Betalningsförslag för lev.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningsjournal** och välj sedan relaterad länk.
2. Öppna den relevanta journalen och välj sedan åtgärden **Betalningsförslag för lev.**.
3. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
4. Välj **OK**.

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>Så här infogar du förfallodatum som bokföringsdatum på betalningsjournalrader
När du använder **Betalningsförslag för lev.**-batchjobbet för att skapa betalningsrader för leverantörer, kan du fylla två specialfält så att de genererade raderna använder förfallodatumet för att beräkna bokföringsdatumet. Dessa fält är **Beräkna bokföringsdatum från dokumentets förfallodatum** och **Dokumentets förfallodatum är förskjutet**.

**Viktigt!** Du kan inte använda fältet **Beräkna bokföringsdatum från dokumentets förfallodatum** tillsammans med fältet **Utnyttja kassarabatter** eller fältet **Summering per leverantör**. Anledningen är att om bokföringsdatumet baseras på förfallodatum, så kan en kassarabatt kanske inte beräknas korrekt eftersom bokföringsdatumet kan inträffa efter kassarabattdatumet.
Om det beräknade bokföringsdatum inträffar tidigare flyttas bokföringsdatumet fram till arbetsdatumet, och en varning visas.

Du kan även skapa betalningsrader manuellt genom att använda förfallodatum för att beräkna bokföringsdatum När du har kopplat leverantörsreskontratransaktioner kan du använda åtgärden **Beräkna bokföringsdatum**. Detta upptaerar bokföringsdatumet på journalraden till förfallodatum på den relaterade inköpsfakturan. Mer information finns i [Så här kopplar du inköpstransaktioner manuellt](payables-how-apply-purchase-transactions-manually.md).  

**Obs!** Om inköpsfakturan har förfallit kommer bokföringsdatum att anges till arbetsdatumet, och teckensnittet på raden ändras till röd färg.

## <a name="see-also"></a>Se även
[Hantera likviditet](payables-manage-payables.md)  
[Gör utbetalningar](payables-make-payments.md)  
[Arbeta med redovisningsjournaler](ui-work-general-journals.md)

