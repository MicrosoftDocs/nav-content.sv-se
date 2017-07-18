---
title: "Hantera inköp"
author: SorenGP
ms.custom: na
ms.date: 11/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df94e447d7d4542f75f3c34105099016b0abbf32
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="manage-purchasing"></a>Hantera inköp
Du skapar en inköpsfaktura eller inköpsorder för att registrera kostnaden för inköp och för att spåra leverantörsskulder. Om du vill kontrollera ett lager används inköpsfakturor också för att uppdatera lagernivåer dynamiskt, så att du kan minimera lagerkostnader och ge bättre service. Inköpskostnaderna, inklusive serviceutgifter och lagervärden som kommer från bokföring av inköpsfakturor bidrar till vinstsiffror och övriga ekonomiska nyckeltal på din startsida.

Du måste använda inköpsorder om din inköpsprocess kräver att du t.ex. kan registrera delleveranser av en orderkvantitet eftersom hela kvantiteten inte var tillgänglig hos leverantören. Om du säljer artiklar genom att leverera direkt från din leverantör till kunden, som en direktleverans, måste du även använda inköpsorder. För mer information finns i [Så här gör du Direktleveranser](sales-how-drop-shipment.md). I alla andra aspekter fungerar inköpsorder på samma sätt som inköpsfakturor.

Du kan låta inköpsfakturor skapas automatiskt, genom att använda OCR-tjänsten (optisk teckenigenkänning) för att konvertera PDF-fakturor från leverantörer till elektroniska dokument, som sedan omvandlas till inköpsfakturor av ett arbetsflöde. För att kunna använda den här funktionen måste du först utföra registrera dig för OCR-tjänsten och därefter utföra olika inställningar. Mer information finns i [Så här bearbetar du inkommande dokument](across-process-income-documents.md).      

**Obs!** I Dynamics NAV refereras en produkt till termen “item”.

Produkter kan vara både lagerartiklar och tjänster. Mer information finns i [Så här registrerar du nya produkter](inventory-how-register-new-products.md).

För alla inköpsprocesser kan du t.ex. inkludera ett arbetsflöde för godkännande för att kräva att stora inköp godkänns av redovisningschefen. Mer information finns i [Använda arbetsflöden för godkännande](across-how-use-approval-workflows.md).

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs. Uppgifterna anges i den ordning de vanligen utförs.


|Om du vill |Gå till |
|---|----|
|Skapa en inköpsfaktura för att registrera en överenskommelse med en leverantör om att köpa produkter till vissa leverans- och betalningsvillkor. |[Så här registrerar du inköp](purchasing-how-record-purchases.md)|
|Skapa en inköpsfaktura för alla eller valda rader på en försäljningsfaktura.|[Så här köper du produkter för en försäljning](purchasing-how-purchase-products-sale.md)|
|Skapa en inköpskreditnota för att återföra en särskild bokförd inköpsfaktura för att visa produkter som du returnerar till leverantören, och vilka belopp som du ska inkassera.|[Så här behandlar du inköpsreturer eller annulleringar](purchasing-how-process-purchase-returns-cancellations.md)|
|Skapa ett leverantörskort för varje leverantör som du har köpt av.|[Så här registrerar du nya leverantörer](purchasing-how-register-new-vendors.md)|

## <a name="see-also"></a>Se även
[Konfigurera inköp](purchasing-setup-purchasing.md)  
[Hantera likviditet](payables-manage-payables.md)    
[Arbeta med Dynamics NAV](ui-work-product.md)  
[Över affärsområden](ui-across-business-areas.md)

