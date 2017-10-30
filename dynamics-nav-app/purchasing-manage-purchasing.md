---
title: "Översikt över uppgifter för hantering av inköp"
description: "Beskriver uppgifter för hantering av inköp eller inköpsprocesser, inklusive hur inköpsfakturor och inköpsorder fungerar."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement, supply, vendor order
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a265cd9e34bd379a6ffc4e7b8f5bcbdfd25702cd
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="purchasing"></a>Inköp
Du skapar en inköpsfaktura eller inköpsorder för att registrera kostnaden för inköp och för att spåra leverantörsskulder. Om du vill kontrollera ett lager används inköpsfakturor också för att uppdatera lagernivåer dynamiskt, så att du kan minimera lagerkostnader och ge bättre service. Inköpskostnaderna, inklusive serviceutgifter och lagervärden som kommer från bokföring av inköpsfakturor bidrar till vinstsiffror och övriga ekonomiska nyckeltal på din startsida.

Du måste använda inköpsorder om din inköpsprocess kräver att du t.ex. kan registrera delleveranser av en orderkvantitet eftersom hela kvantiteten inte var tillgänglig hos leverantören. Om du säljer artiklar genom att leverera direkt från din leverantör till kunden, som en direktleverans, måste du även använda inköpsorder. För mer information finns i [Så här gör du Direktleveranser](sales-how-drop-shipment.md). I alla andra aspekter fungerar inköpsorder på samma sätt som inköpsfakturor.

Du kan låta inköpsfakturor skapas automatiskt, genom att använda OCR-tjänsten (optisk teckenigenkänning) för att konvertera PDF-fakturor från leverantörer till elektroniska dokument, som sedan omvandlas till inköpsfakturor av ett arbetsflöde. För att kunna använda den här funktionen måste du först utföra registrera dig för OCR-tjänsten och därefter utföra olika inställningar. Mer information finns i [Så här bearbetar du inkommande dokument](across-process-income-documents.md).      

Produkter kan vara både lagerartiklar och tjänster. Mer information finns i [Så här registrerar du nya artiklar](inventory-how-register-new-items.md).

För alla inköpsprocesser kan du t.ex. inkludera ett arbetsflöde för godkännande för att kräva att stora inköp godkänns av redovisningschefen. Mer information finns i [Använda arbetsflöden för godkännande](across-how-use-approval-workflows.md).

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.

| Till | Gå till |
| --- | --- |
| Skapa en inköpsfaktura för att registrera en överenskommelse med en leverantör om att köpa produkter till vissa leverans- och betalningsvillkor. |[Så här registrerar du inköp](purchasing-how-record-purchases.md) |
|Skapa en inköpsoffert för att återspegla en anbudsförfrågan från leverantören, som du senare kan konvertera till en inköpsorder.|[Så här begär du offerter](purchasing-how-request-quotes.md)|
| Skapa en inköpsfaktura för alla eller valda rader på en försäljningsfaktura. |[Så här köper du artiklar för en försäljning](purchasing-how-purchase-products-sale.md) |
| Utför en åtgärd på en obetald bokförd inköpsfaktura som automatiskt skapar en kreditnota och antingen annullerar inköpsfakturan eller skapar den på nytt, så att du kan göra korrigeringar. |[Så här rättar eller makulerar du obetalda försäljningsfakturor](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Skapa en inköpskreditnota för att återföra en särskild bokförd inköpsfaktura för att visa produkter som du returnerar till leverantören, och vilka belopp som du ska inkassera. |[Så här behandlar du inköpsreturer eller annulleringar](purchasing-how-register-new-vendors.md) |
|Förbered för att fakturera flera inleveranser från samma leverantör en gång genom att kombinera inleveranser på en faktura.|[Så här kombinerar du inleveranser på en enda faktura](purchasing-how-to-combine-receipts.md)|
| Lär dig hur [!INCLUDE[d365fin](includes/d365fin_md.md)] beräknas när du måste beställa en artikel för ett visst datum.|[Datumberäkning för inköp](purchasing-date-calculation-for-purchases.md)|

## <a name="see-also"></a>Se även
[Ställa in inköp](purchasing-setup-purchasing.md)  
[Så här registrerar du nya leverantörer](purchasing-how-register-new-vendors.md)  
[Hantera Leverantörsreskontra](payables-manage-payables.md)  
[Hantera projekt](projects-manage-projects.md)    
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Allmänna affärsfunktioner](ui-across-business-areas.md)

## 

