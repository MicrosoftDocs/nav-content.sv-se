---
title: Hantera likviditet
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
ms.openlocfilehash: 50a68e1eaf0d6057420635f85b473639e39caa5a
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="manage-payables"></a>Hantera likviditet
En central aktivitet, i hanteringen av leverantörsreskontratransaktioner, är att betala dina leverantörer. Du kan använda funktioner för att automatiskt fylla i fönstret **Betalningsjournal** med betalningrader för förfallna inköpsfakturor. För att snabbt utföra de berörda banktransaktionerna kan du exportera åtskilliga betalningsjournalrader till en fil, som du överför till din bank för att bearbetas. Du kan också göra betalningar med check som inkluderar att överföra checkar som elektronisk betalning.

En annan typisk aktivitet är att koppla utgående betalningar till deras relaterade på kund- eller leverantörsreskontratransaktioner och därmed avsluta de relaterade inköpsfakturorna eller inköpskreditnotorna som betalda. Du kan utföra denna aktivitet i fönstret **Betalningsavstämningsjournal** genom att importera ett kontoutdrag för att snabbt registrera utbetalningarna i Dynamics NAV. En automatisk kopplingsfunktion gäller betalningar till deras relaterade öppna kund- eller leverantörsreskontratransaktioner som baseras på datamatchningar mellan utbetalningtext och transaktionsinformation. Du kan använda olika funktioner för att granska och ändra automatiska kopplingar, innan du bokför journalen. Du kan välja att avsluta alla öppna bankkontotransaktioner som relateras till kopplade transaktioner, när du bokför journalen. Det betyder att bankkontot avstäms automatiskt, när alla utbetalningar kopplas.

Du kan också koppla utgående betalningar manuellt i fönstret **Betalningsjournal** eller från relaterade leverantörsreskontraposterna.

I följande tabell beskrivs en serie uppgifter inom Leverantörsskulder med länkar till de avsnitt där de beskrivs.

|Om du vill |Gå till |
|---|----|
|Generera förfallna leverantörsbetalningar som prioriteras enligt kassarabatter och förseningsavgifter. Exportera betalningarna till en bankfil, när du bokför, om du vill.|[Gör utbetalningar](payables-make-payments.md)|
|Koppla leverantörsbetalningar automatiskt till obetalda inköpsfakturor, genom att importera bankutdragsfil.|[Koppla utbetalningar automatiskt och stämma av bankkonton](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Koppla leverantörsbetalningar till obetalda inköpsfakturor manuellt.|[Så här kopplar du leverantörsbetalningar manuellt](payables-how-apply-purchase-transactions-manually.md)|

## <a name="see-also"></a>Se även
[Hantera inköp](purchasing-manage-purchasing.md)  
[Hantera kundreskontra](receivables-manage-receivables.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)  
[Över affärsområden](ui-across-business-areas.md)

