---
title: "Så här stämmer du av betalningar som inte kan kopplas automatiskt"
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
ms.openlocfilehash: f9fd7c2958aaa359d2f6af5dde2e8be81349e900
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-that-cannot-be-applied-automatically"></a>Så här stämmer du av betalningar som inte kan kopplas automatiskt
Du måste ibland hantera betalningar till ditt bankkonto som inte kan kopplas till en relaterad öppen kund, leverantör eller bankkontotransaktion. Anledningar kan vara att det inte finns något dokument i Dynamics NAV som betalningen kan kopplas till, eller det relaterade dokumentet i Dynamics NAV har ett annat belopp än transaktionbeloppet, tex på grund av valutakursen. I fönstret **Betalningavstämningjournal** visas inte alla transaktionsbelopp för betalningar som inte kopplats ännu i fältet **Skillnad** inklusive belopp, som inte kan användas på grund av anledningarna ovan.

Betalningar som inte kan kopplas kan visas på betalningavstämningjournalrader på följande sätt:

- Värdet i fältet **skillnad** är lika med värdet i fältet **transaktionbelopp** vilket betyder att ingen del av betalningen kan kopplas till en relaterad öppen kund, leverantör eller bankkontotransaktion.

- Värdet i fältet **skillnad** är lägre än värdet i fältet **transaktionbelopp** vilket betyder att ingen del av betalningen kan kopplas till en relaterad öppen kund, leverantör eller bankkontotransaktion. Återstående del av betalningen kan inte kopplas och måste avstämmas manuellt eller genom att bokföra den direkt till ett konto.

Om du vill avstämma sådana betalningar kan du välja knappen Överföringsskillnad till konto och sedan skriva in vilket konto som beloppet i fältet Skillnad ska bokföras på när du bokför betalningavstämningjournalen.

**Obs!** Liknande funktioner finns för att definiera automatisk avstämning återkommande betalningar som inte kan användas till relaterade öppna kund-, leverantörs- eller bankkontotransaktioner. Mer information finns i [Så här mappar du text på återkommande betalningar till konton för automatisk avstämning](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

## <a name="to-reconcile-payments-that-cannot-be-applied"></a>Så här stämmer du av betalningar som inte kan kopplas
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningsavstämningsjournaler** och välj sedan relaterad länk.
2. Öppna en betalningsavstämningsjournal. Mer information finns i [Så här stämmer du av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md).
3. Välj **Överför differens till konto**. Fönstret **Överför differens till konto** 3. öppnas.
4. I fältet **Kontotyp** anger du typen av konto som betalningsbeloppet bokförs på.
5. I fältet **Bankkontonr.** anger du typen av bankkonto som betalningsbeloppet bokförs på.
6. I fältet **Beskrivning** anger du den text som beskriver denna direktbetalningsbokföring.  Som standard infogas texten i fältet **transaktionstext** på betalningavstämningjournalraden.
7. Välj **OK**.

Om värdet i fältet **skillnad** var lika med värdet i fältet **transaktionbelopp** när du bokförde betalningavstämningjournalen, kommer hela betalningen på journalraden bokföras direkt på angivet motkonto.

Om värdet i fältet **skillnad**var mindre än värdet i fältet **transaktionsbelopp** kommer en ytterligare journalrad skapas med samma text och datum och med skillnaden som infogas i fältet **transaktionbelopp**. På den ursprungliga journalraden kommer skillnaden dras av från värdet i fältet **transaktionbelopp** och betalningen kommer att fortsätta vara kopplad till kund-, leverantörs- eller bankkontotransaktionen. När du bokför betalningsavstämningsjournalen kommer en del av betalningen att bokföras som en kopplad betalning. Den andra delen av betalningen ska bokföras direkt till det angivna kontot.

## <a name="see-also"></a>Se även
[Hantera kundreskontra](receivables-manage-receivables.md)  
[Hantera försäljning](sales-manage-sales.md)

