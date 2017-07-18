---
title: "Hantera försäljning"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 20e380abb2f8f598391a66e50a7ec7a1c8b15fa1
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="manage-sales"></a>Hantera försäljning
Du kan skapa en försäljningsfaktura eller försäljningsorder för att registrera en överenskommelse med en kund om att sälja vissa produkter till vissa leverans- och betalningsvillkor.

Du måste använda försäljningsorder om din försäljningsprocess kräver att du t.ex. kan leverera delar av en orderkvantitet eftersom hela kvantiteten inte är tillgängliga på en gång. Om du säljer artiklar genom att leverera direkt från din leverantör till kunden, som en direktleverans, måste du även använda försäljningsorder. I alla andra aspekter fungerar försäljningsorder på samma sätt som försäljningsfakturor.  

Effektiva metoder för försäljning och marknadsföring handlar om hur du fattar rätt beslut vid rätt tidpunkt. Marknadsföringsfunktionen i Dynamics NAV ger en exakt överblick över din kontaktinformation när du behöver den, så att du kan arbeta effektivt med potentiella kunder och öka kundtillfredsställelsen. Mer information finns i [Kundhantering](marketing-relationship-management.md).

Du kan förhandla med kunden genom att först skapa förs.offerter, som du kan omvandla till en försäljningsfaktura när du instämmer om försäljningen. När kunden har bekräftat avtalet, till exempel efter en offertprocess, skickar du en orderbekräftelse för att registrera dina åtagande att leverera produkterna enligt överenskomment.

När du har levererat produkterna, antingen helt eller delvis, bokför du försäljningsfakturan eller försäljningsordern som levererade eller som levererade och fakturerade för att skapa kundreskontratransaktioner i systemet.

I affärsmiljöer där kunden måste betala för produkter i förväg måste du vänta på kvittot på betalning innan du levererar produkterna. I de flesta fall behandlar du inkommande betalningar några veckor efter leverans, genom att koppla betalningarna till dess relaterade obetalda bokförda försäljningsfakturor. Mer information finns i [Så här stämmer du av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md).

Försäljningsdokument kan skickas som PDF-filer kopplade till e-postmeddelande. Brödtexten för e-post ska innehålla ett utdrag av försäljningsdokumentet, till exempel produkter, totalt belopp och en länk till webbplatsen för PayPal. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).

För alla försäljningsprocesser kan du t.ex. inkludera ett arbetsflöde för godkännande för att kräva att stora försäljningar till vissa kunder godkänns av redovisningschefen. Mer information finns i [Använda arbetsflöden för godkännande](across-how-use-approval-workflows.md).

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.

|Om du vill |Gå till |
|---|----|
|Skapa en försäljningsoffert där du erbjuder produkter med förhandlingsbara villkor, innan du omvandlar offerten till en försäljningsfaktura.|[Så här gör du erbjudanden](sales-how-make-offers.md)|
|Skapa en försäljningsfaktura för att registrera en överenskommelse med en kund om att sälja produkter till vissa leverans- och betalningsvillkor.|[Så här fakturerar du försäljning](sales-how-invoice-sales.md)|
|Behandla en försäljningsorder som rör delvis leverans eller direktleverans.|[Så här säljer du produkter](sales-how-sell-products.md)|
|Länka en försäljningsorder till en inköpsorder för att sälja ett direktutleveransobjekt som ska levereras direkt från din leverantör till kunden.|[Så här utför du direktleveranser](sales-how-drop-shipment.md)|
|Skapa en försäljningskreditnota för att återföra en särskild bokförd försäljningsfaktura för att visa produkter som kunden returnerar och vilka belopp som du ska återbetala.|[Så här behandlar du försäljningreturer eller annulleringar](sales-how-process-sales-returns-cancellations.md)|
|Skapa ett kundkort för varje kund som du säljer till.|[Så här registrerar du nya kunder](sales-how-register-new-customers.md)|

## <a name="see-also"></a>Se även  
[Ställa in försäljning](sales-setup-sales.md)  
[Hantera kundreskontra](receivables-manage-receivables.md)  
[Hantera likviditet](payables-manage-payables.MD)      
[Arbeta med Dynamics NAV](ui-work-product.md)  
[Över affärsområden](ui-across-business-areas.md)

