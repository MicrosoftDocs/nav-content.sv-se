---
title: "Så här aktiverar du kundutbetalning via PayPal"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a>Så här aktiverar du kundutbetalning via PayPal#
Som alternativ till att samla utbetalningar via banköverföring eller kreditkort, kan du erbjuda dina kunder att betala via sina PayPal-konton.

När kunden väljer PayPal-länken på en försäljningsfaktura eller försäljningsorderdokument visar servicesidan för deras PayPal-konto försäljningens betalningsdetaljer. Då kan kunden betala fakturan som en PayPal-betalning.

För att aktivera kundutbetalningar via PayPal måste du göra följande:

1. Skapa PayPal Payments Standard som betalningsservice i fönstret **Betalningstjänst**.
2. Välj PayPal Payments Standard i fältet **Betalningstjänst** försäljningsdokumentet i fråga.

Tjänsten för PayPal-standardbetalning har installerats som ett tillägg till Dynamics NAV och är klar att aktiveras. Mer information finns i [Anpassa Dynamics NAV med tillägg](ui-extensions.md).

## <a name="to-enable-the-paypal-payments-standard-service"></a>Så här aktiverar du Tjänsten för PayPal Payments Standard
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Betalningstjänst** och välj sedan relaterad länk.  
2. I fönstret **Betalningstjänst** väljer du åtgärden **Ny**.
3. Markera **PayPal-standard** och stäng sedan fönstret.
4. I fönstret **Betalningstjänst** väljer du åtgärden **Konfiguration**.
5. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

    **Obs!** Markera kryssrutan **Inkludera alltid på dokument** om hyperlänken för PayPal-betalningstjänsten alltid ska visas på försäljningsdokument där utbetalning via PayPal är aktiverat.

6. Stäng fönstret.

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a>Om du vill välja PayPal Payments Standard på en försäljningsfaktura
1. Välj åtgärden **Försäljningsfakturor** på startsidan.
2. Öppna försäljningsfakturan som du vill aktivera PayPal-betalningar för.
3. I fältet **Betalningtjänst** väljer du PayPal Payments Standard

**Obs!** Fältet **Betalningtjänst** visas endast för om Tjänsten för PayPal Payments Standard är aktiverat.   

## <a name="see-also"></a>Se även  
[Ställa in försäljning](sales-setup-sales.md)  
[Hantera försäljning](sales-manage-sales.md)  
[Anpassa Dynamics NAV med tillägg](ui-extensions.md)

