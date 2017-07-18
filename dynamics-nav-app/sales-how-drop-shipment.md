---
title: "Så här utför du direktleveranser"
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
ms.openlocfilehash: f636de789dc6b006a449ec59c390fab85e62b443
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-drop-shipments"></a>Så här utför du direktleveranser
Direktleverans innebär leverans av artiklar från någon av företagets leverantörer direkt till någon av företagets kunder.

När en försäljningsorder är markerad för direktleverans, och du skapar en inköpsorder där du anger kunden i fältet **Förs.kundnr.** kan du länka de två dokumenten och därmed instruera leverantören att leverera direkt till kunden.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Så här skapar du försäljningsorder för direktleveranser
För att förbereda en direktleverans skapar du en försäljningsorder för en artikel som vanligt, förutom att du måste ange på försäljningsraden att försäljningen kräver direktleverans.

1. Skapa en försäljningsorder för en artikel. Mer information finns i [Så här säljer du produkter](sales-how-sell-products.md).
2. På försäljningsorderraden för direktleveransartikeln markerar du kryssrutan **Direktleverans**.

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>Så här skapar du inköpsorder för direktleverans
Om du vill förbereda en direktleverans för den artikel som ska säljas kan du skapa en inköpsorder som vanligt förutom att du måste ange på inköpsordern att den ska levereras till din kund och inte till dig själv.

1. Skapa en inköpsorder. Fyll inte i några fält på raderna. Mer information finns i [Så här registrerar du inköp](purchasing-how-record-purchases.md).
2. I fältet **Förs.kundnr.** markerar du kunden som du säljer till.
3. Välj åtgärden **Direktleverans** och välj sedan åtgärden **Hämta förs.order**.
4. I fönstret **Försäljningslista** väljer du den försäljningsorder som du förberedde i avsnittet "Så här skapar du försäljningsorder för direktleveranser".
5. Välj **OK**.

Radinformationen från försäljningsordern infogas på inköpsorderraden.

Du kan nu instruera leverantören att leverera artiklarna till kunden, till exempel genom att e-posta inköpsordern som en PDF.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>Om du vill se den länkade inköpsordern från försäljningsordern
1. Markera försäljningsordern direktleverans, välj åtgärden **Order**, välj åtgärden **Direktleverans** och välj sedan åtgärden **Inköpsorder**.

Den länkade inköpsordern öppnas.

## <a name="to-post-a-drop-shipment"></a>Så här bokför du en direktutleverans
När leverantören har levererat artiklarna kan du bokföra försäljningsordern som levererad. Du kan också bokföra inköpsordern, men endast med alternativet **Ta emot** tills försäljningsordern har fakturerats.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Försäljningsorder** och välj sedan relaterad länk.
2. Öppna den försäljningsorder som du skapade i avsnittet "Att skapa en försäljningsorder för en direktleverans" .
3. I fältet **Levereras antal** anger du hur många av orderkvantiteten som ska levereras, hela eller delvis orderkvantitet.
3. Välj åtgärden **Bokför** eller **Bokför och skicka**.
4. Markera antingen alternativet **Leverera** för att fakturera senare eller alternativet **Leverera och fakturera** för att fakturera omedelbart.

## <a name="see-also"></a>Se även
[Så här säljer du produkter](sales-how-sell-products.md)    
[Så här registrerar du inköp](purchasing-how-record-purchases.md)  
[Hantera försäljning](sales-manage-sales.md)  
[Hantera lager](inventory-manage-inventory.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)

