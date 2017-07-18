---
title: "Så här registrerar du nya produkter"
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
ms.openlocfilehash: df84a4d3e15035cd956c7612a12069844f5601d2
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-products"></a>Så här registrerar du nya produkter

Produkter utgör basen för ditt arbete, varorna eller tjänster som du handlar med. Varje produkt måste registreras som ett artikelkort.

**Obs!** I Dynamics NAV  refereras en produkt till termen “item”.

Artikelkort innehåller den information som behövs för att köpa, lagra, sälja, leverera och informera om produkter.

Artikelkortet kan vara av typen Lager eller Service för att ange om produkten är en fysisk enhet eller en arbetstidsenhet. Förutom vissa fält som är knutna till de fysiska aspekterna av en artikel, fungerar alla fält på ett artikelkort på samma sätt för lagerartiklar och tjänster. Mer information om att sälja en artikel finns i [Så här säljer du produkter](sales-how-sell-products.md) eller [Så här fakturerar du försäljning](sales-how-invoice-sales.md).

**Obs!** Om artikelmallar finns för olika artikeltyper, visas ett fönster när du skapar ett nytt artikelkort där du kan välja en lämplig mall. Om endast en artikelmall finns, då använder nya artikelkort alltid den mallen.

## <a name="to-create-a-new-item-card"></a>Skapa ett nytt artikelkort
1. På startsidan väljer du åtgärden **Artiklar** för att öppna listan över befintliga artiklar.  
2. I fönstret **Artiklar** väljer du åtgärden **Ny**.

    Om endast en artikelmall finns, då öppnas ett nytt artikelkort med fält ifyllda med information från mallen.
3. Välj den mall som du vill använda för den nya artikelkortet i fönstret **Välj en mall för en ny artikel**.
4. Välj **OK**. Ett nytt artikelkort öppnas med ifyllda fält med information från mallen.
5. Fortsätt att fylla i eller ändra fält på artikelkortet vid behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

På snabbfliken **Försäljningspriser** ser du specialpriser eller rabatter som du beviljar för artikeln om vissa kriterier uppfylls, till exempel kund, lägsta partistorlek eller slutdatum Varje rad representerar ett speciellt pris eller radrabatt. Varje kolumn representerar ett kriterium som måste gälla för att garantera specialpriset som du anger i fältet **Enhetspris** eller radrabatten som du anger i fältet **Radrabatt %**. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).

Artikeln är nu registrerad, och artikelkortet är klart att användas i försäljningsdokument.

Om du vill använda detta artikelkort som en mall när du skapar nya artikelkort, så fortsätt med att spara den som en mall. Mer information finns i följande avsnitt:

## <a name="to-save-the-item-card-as-a-template"></a>Om du vill spara artikelkortet som en mall
1. I fönstret **artikelkort** väljer du åtgärden **Spara som mall**. Det **artikelmall** fönstret öppnas uppvisar artikelkortet som mall.
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. Om du vill återanvända dimensioner i mallar väljer du fönstret **Dimensioner**. Fönstret **Dimensionsmallar** öppnas och visar de dimensionskoder som ställts in för artikeln.
4. Ändra eller ange dimensionskoder som ska kopplas till nya artikelkort som skapas med hjälp av mallen.
5. Välj **OK** när du har slutfört den nya artikelmallen.

Artikelmallen läggs till listan över artikelmallar, så att du kan använda det för att skapa nya artikelkort.

## <a name="see-also"></a>Se även
  [Hantera lager](inventory-manage-inventory.md)  
  [Hantera inköp](purchasing-manage-purchasing.md)  
  [Hantera försäljning](sales-manage-sales.md)

