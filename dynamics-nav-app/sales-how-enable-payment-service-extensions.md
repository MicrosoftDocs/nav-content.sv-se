---
title: "Aktivera kundbetalningar via betalningstjänster"
description: "Gör det enklare för kunderna att betala sina fakturor genom att aktivera betalningstjänster."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 71ff4af2fa3c0d1020a24de4325aafe17978f715
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-customer-payments-through-payment-services"></a>Så här aktiverar du kundbetalningar via betalningstjänster
Som alternativ till att samla utbetalningar via banköverföring eller kreditkort, kan dina kunder betala via sina konton med betalningstjänster som t.ex. Microsoft Pay, PayPal, or WorldPay.  

När du har aktiverat en betalningstjänst i [!INCLUDE[d365fin](includes/d365fin_md.md)], är en länk till den här tjänsten tillgänglig på försäljningsdokument som du skickar med e-post till kunder. Kunder kan använda länken för att gå till betalningstjänsten och betala fakturan direkt från försäljningsdokumentet. Om du inte vill inkludera länken, exempelvis om en kund vill betala kontant, kan du ta bort betalningstjänsten från fakturan innan du bokför.  

Tilläggen Microsoft Pay, PayPal Payments Standard och WorldPay Payments Standard är installerade i [!INCLUDE[d365fin](includes/d365fin_md.md)], och klara att aktiveras.  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a>Så här aktiverar du en betalningstjänst i [!INCLUDE[d365fin](includes/d365fin_md.md)]
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Betalningstjänster** och välj sedan relaterad länk.  
2. I fönstret **Betalningstjänst** väljer du åtgärden **Ny**.  
3. Välj betalningstjänsten och stäng sedan fönstret.  
4. I fönstret **Betalningstjänst** väljer du åtgärden **Konfiguration**.  
5. Fyll i fälten om det behövs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. Stäng fönstret.  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a>Välj en betalningstjänst för en försäljningsfaktura
1. Välj åtgärden **Försäljningsfakturor** på startsidan.  
2. Öppna den försäljningsorder som du vill betala med hjälp av betalningstjänsten.  
3. I fältet **Betalningtjänst** väljer du betalningtjänsten.  

    > [!NOTE]  
>   Fältet **betalningstjänst** är bara tillgängligt om du har aktiverat betalningstjänsten.  

## <a name="see-also"></a>Se även  
[Konfigurera försäljning](sales-setup-sales.md)  
[Försäljning](sales-manage-sales.md)  
[Anpassa [!INCLUDE[d365fin](includes/d365fin_md.md)] med tillägg](ui-extensions.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

