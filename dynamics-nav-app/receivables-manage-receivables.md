---
title: Hantera kundreskontra
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
ms.openlocfilehash: 3f2be627dfda9720e9f31fd227164d1c27116d2c
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="manage-receivables"></a>Hantera kundreskontra#
En central aktivitet i hanteringen av kundfordringar är att koppla inkommande betalningar till deras relaterade på kund- eller leverantörsreskontratransaktioner och därmed avsluta de relaterade försäljningsfakturorna eller inköpskreditnotorna som betalda. När alla betalningar har använts kan du stämma av bankkontot.  

Du kan utföra denna aktivitet i fönstret **Betalningsavstämningsjournal** genom att importera ett kontoutdrag eller feed för att snabbt registrera utbetalningarna i Dynamics NAV. En automatisk kopplingsfunktion gäller betalningar till deras relaterade öppna kund- eller leverantörsreskontratransaktioner som baseras på datamatchningar mellan utbetalningtext och transaktionsinformation. Du kan granska och ändra automatiska kopplingar, innan du bokför journalen. Du kan välja att avsluta alla öppna bankkontotransaktioner som relateras till kopplade transaktioner, när du bokför journalen. Det betyder att bankkontot avstäms automatiskt, när alla utbetalningar kopplas.

**Obs!** Du kan stämma av bankkonton som en separat aktivitet i fönstret **Bankkontoavstämning** som också stöder checktransaktioner. Mer information finns i [Så här stämmer du av bankkonton separat](bank-how-reconcile-bank-accounts-separately.md).

Du kan också koppla betalningar i fönstret **Betalningsregistrering** genom att manuellt kontrollera betalningar som tas emot som kontanter, check eller banktransaktion mot en skapad lista över obetalda försäljningsdokument. Observera att den här funktionen endast är tillgänglig för försäljningsdokument.

Som en annan manuell avstämning för utbetalningar kan du bokföra varje kvitto till relevant redovisning, kund eller annat konto, genom att ange en betalningsrad i fönstret **Inbetalningsjournal**. I så fall kan du antingen använda kvittot eller återbetalningen till en eller flera öppna transaktioner, innan du bokför inbetalningsjournalen, eller så kan du koppla de skapade kundtransaktionerna.

En annan aktivitet i hanteringen av kundfordringar är att kräva in utestående saldon inklusive att hantera finansinställningsränta och skicka betalningspåminnelser.

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.

|Om du vill |Gå till |
|---|----|
|Koppla betalningar för att öppna kund- eller leverantörsreskontratransaktioner baserade på en importerat kontoutdragsfil eller feed och stämma av bankkonton när alla betalningar är kopplade.|[Koppla utbetalningar automatiskt och stämma av bankkonton](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Koppla utbetalningar till öppna kundreskontratransaktioner som baseras på manuell inmatning i en lista över obetalda försäljningsdokument. | [Så här stämmer du av kundutbetalningar manuellt från en lista med obetalda försäljningsdokument](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)|
|Bokföring av inbetalningar eller återbetalningar för kunder i inbetalningsjournalen och koppla till kundreskontratransaktioner, antingen från journalen eller från bokförda transaktioner. | [Så här stämmer du av kundbetalningar rabatter manuellt](receivables-how-apply-sales-transactions-manually.md) |
|påminna kunder om förfallna belopp, beräkna finansinställningsränta och hantera kundreskontra. | [Så här kräver du in utestående saldon](receivables-collect-outstanding-balances.md) |

## <a name="see-also"></a>Se även
[Hantera försäljning](sales-manage-sales.md)  
[Hantera likviditet](payables-manage-payables.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)  
[Över affärsområden](ui-across-business-areas.md)

