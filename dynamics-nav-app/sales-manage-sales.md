---
title: "Översikt över uppgifter för hantering av försäljning"
description: "Beskriver hur du hanterar försäljningsaktiviteter."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 030739b491ba5c914d10811cfbac994917f9eb9d
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="sales"></a>FÖRS
Du kan skapa en försäljningsfaktura eller försäljningsorder för att registrera en överenskommelse med en kund om att sälja vissa produkter till vissa leverans- och betalningsvillkor.

Du måste använda försäljningsorder om din försäljningsprocess kräver att du t.ex. kan leverera delar av en orderkvantitet eftersom hela kvantiteten inte är tillgängliga på en gång. Om du säljer artiklar genom att leverera direkt från din leverantör till kunden, som en direktleverans, måste du även använda försäljningsorder. I alla andra aspekter fungerar försäljningsorder på samma sätt som försäljningsfakturor. Med försäljningsorder kan du också använda funktionen orderlöfte för att kommunicera vissa leveransdatum till dina kunder.  

Du kan förhandla med kunden genom att först skapa förs.offerter, som du kan omvandla till en försäljningsfaktura eller försäljningsorder när du instämmer om försäljningen. När kunden har bekräftat avtalet skickar du en orderbekräftelse för att registrera dina åtagande att leverera produkterna enligt överenskomment.

Det är enkelt att korrigera eller annullera en bokförd försäljningsfaktura, innan den betalas. Det är användbart om du vill rätta till ett skrivfel eller om du kunden göra en ändring tidigt i orderprocessen. Om den bokförda försäljningsfakturan betalas, måste du skapa en försäljningskreditnota och försäljningsreturorder för att återföra försäljningen.

Effektiva metoder för försäljning och marknadsföring handlar om hur du fattar rätt beslut vid rätt tidpunkt. Marknadsföringsfunktionen i [!INCLUDE[d365fin](includes/d365fin_md.md)] ger en exakt överblick över din kontaktinformation när du behöver den, så att du kan arbeta effektivt med potentiella kunder och öka kundtillfredsställelsen. Mer information finns i [Kundhantering](marketing-relationship-management.md).

I affärsmiljöer där kunden måste betala för produkter i förväg måste du vänta på kvittot på betalning innan du levererar produkterna. I de flesta fall behandlar du inkommande betalningar några veckor efter leverans, genom att koppla betalningarna till dess relaterade obetalda bokförda försäljningsfakturor. Mer information finns i [Så här stämmer du av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md).

Försäljningsdokument kan skickas som PDF-filer kopplade till e-postmeddelande. Brödtexten för e-post ska innehålla ett utdrag av försäljningsdokumentet, till exempel produkter, totalt belopp och en länk till webbplatsen för PayPal. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).

För alla försäljningsprocesser kan du t.ex. inkludera ett arbetsflöde för godkännande för att kräva att stora försäljningar till vissa kunder godkänns av redovisningschefen. Mer information finns i [Använda arbetsflöden](across-use-workflows.md).

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.

| Om du vill | Gå till |
| --- | --- |
| Skapa en försäljningsoffert där du erbjuder produkter med förhandlingsbara villkor, innan du omvandlar offerten till en försäljningsfaktura. |[Så här gör du erbjudanden](sales-how-make-offers.md) |
| Skapa en försäljningsfaktura för att registrera en överenskommelse med en kund om att sälja produkter till vissa leverans- och betalningsvillkor. |[Så här fakturerar du försäljning](sales-how-invoice-sales.md) |
| Behandla en försäljningsorder som rör delvis leverans eller direktleverans. |[Så här säljer du produkter](sales-how-sell-products.md) |
|Lägga upp standardförsäljnings- eller inköpsrader som du kan snabbt infoga i dokument, till exempel för återkommande påfyllningsorder.|[Så här: Skapa återkommande försäljnings- och inköpsrader](sales-how-work-standard-lines.md)|  
| Länka en försäljningsorder till en inköpsorder för att sälja ett direktutleveransobjekt som ska levereras direkt från din leverantör till kunden. |[Så här utför du direktleveranser](sales-how-drop-shipment.md) |
|Har en ej lagerförd artikel levererad från en leverantör till distributionslagret så att du kan leverera den till kunden.|[Så här skapar du specialorder](sales-how-to-create-special-orders.md)|
| Utför en åtgärd på en obetald bokförd försäljningsfaktura som automatiskt skapar en kreditnota och antingen annullerar försäljningsfakturan eller skapar den på nytt, så att du kan göra korrigeringar. |[Så här rättar eller makulera du obetalda försäljningsfakturor](sales-how-correct-cancel-sales-invoice.md) |
| Skapa en försäljningskreditnota för att återföra en särskild bokförd försäljningsfaktura för att visa produkter som kunden returnerar och vilka belopp som du ska återbetala. |[Så här behandlar du försäljningreturer eller annulleringar](sales-how-process-sales-returns-cancellations.md) |
|Hantera kundens engagemang att köpa stora kvantiteter som levereras i flera leveranser med tiden.|[Så här: Arbeta med försäljningsavropsorder](sales-how-to-create-blanket-sales-orders.md)|
|Sälj monteringsartiklar som inte är tillgängliga genom att skapa en länkad monteringsorder för att tillhandahålla hela eller delvisa försäljningsorderantal.|[Så här säljer du en artikel som monterats mot kundorder](assembly-how-to-sell-items-assembled-to-order.md)|
|Fakturera kunder en gång för flera utleveranser genom att kombinera leveranser på en faktura.|[Så här kombinerar du leveranser på en enda faktura](sales-how-to-combine-shipments-on-a-single-invoice.md)|
|Informera dina kunder om orderleveransdatum genom att beräkna antingen kapabel att lova-datum eller dispositionsdatum.|[Så här beräknar du ett orderlöftesdatum](sales-how-to-calculate-order-promising-dates.md)|

## <a name="see-also"></a>Se även
[Konfigurera försäljning](sales-setup-sales.md)  
[Så här registrerar du nya kunder](sales-how-register-new-customers.md)  
[Hantera kundreskontra](receivables-manage-receivables.md)  
[Hantera Leverantörsreskontra](payables-manage-payables.md)  
[Projekthantering](projects-manage-projects.md)    
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Allmänna affärsfunktioner](ui-across-business-areas.md)

## 

