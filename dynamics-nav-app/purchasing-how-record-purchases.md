---
title: "Så här registrerar du inköp"
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
ms.openlocfilehash: 6d1933bf1e1c9236d34d429a4da84c907df13708
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-purchases"></a>Så här registrerar du inköp
Du skapar en inköpsfaktura eller inköpsorder för att registrera kostnaden för inköp och för att spåra leverantörsskulder. Om du vill kontrollera ett lager används inköpsfakturor eller inköpsorder också för att uppdatera lagernivåer dynamiskt, så att du kan minimera lagerkostnader och ge bättre service. Inköpskostnaderna, inklusive serviceutgifter och lagervärden som kommer från bokföring av inköpsfakturor eller order bidrar till vinstsiffror och övriga ekonomiska nyckeltal på din startsida.

**Obs!**: Du måste använda inköpsorder om din inköpsprocess kräver att du t.ex. kan registrera delleveranser av en orderkvantitet eftersom hela kvantiteten inte var tillgänglig hos leverantören. Om du säljer artiklar genom att leverera direkt från din leverantör till kunden, som en direktleverans, måste du även använda inköpsorder. För mer information finns i [Så här gör du Direktleveranser](sales-how-drop-shipment.md). I alla andra aspekter fungerar inköpsorder på samma sätt som inköpsfakturor. Följande procedur är baserad på en inköpsfaktura. Momenten är liknande för en inköpsorder.

När du tar emot lagerartiklarna, eller när den inköpta tjänsten avslutas, bokför du inköpsfaktura eller order för att uppdatera lager och finansiella transaktioner och för att aktivera betalning till leverantören utifrån betalningsvillkoren. Mer information finns i [Gör betalningar](payables-make-payments.md).

**Obs!** Bokför inte en inköpsfaktura förrän du tar emot produkterna och vet slutkostnaden för inköpet, inklusive eventuella extrakostnader. Annars kan lagervärdet och vinstsiffrorna ha oriktiga resultat.

Om du redan har betalt för produkter på den bokförda inköpsfakturan, måste du skapa en inköpskreditnota för att återföra köpet. Mer information finns i [Så här behandlar du inköpsreturer eller annulleringar](purchasing-how-process-purchase-returns-cancellations.md).

Produkter kan vara både lagerartiklar och tjänster. Mer information finns i [Så här registrerar du nya produkter](inventory-how-register-new-products.md). Inköpsfakturaprocessen är samma för båda produkttyper.



Du kan fylla i leverantörsfälten på inköpsfakturan på två sätt, beroende på om leverantören redan har registrerats.

## <a name="to-create-a-purchase-invoice"></a>Skapa en inköpsfaktura
1. Välj åtgärden **Inköpsfaktura** på startsidan.  
2. Ange namnet på en befintlig kund i fältet **leverantör**.

    Andra fält i fönstret **Inköpsfaktura** fylls nu i med standardinformation om den valda leverantören. Om leverantören inte är registrerad, gör så här:
3. Ange namnet på en ny leverantör i fältet **leverantör**.
4. Välj knappen **ja** i dialogrutan om registrering av den nya leverantören.
5. Välj en mall det nya leverantörskortet ska baseras på i fönstret **Välj en mall för en ny leverantör** och välj sedan knappen **OK**.
6. Ett nytt leverantörskort öppnas med förifylld information från den markerade leverantörsmallen. Fältet **Namn** förifylls med nya leverantörens namn som du har angett på inköpsfakturan.
7. Fortsätt att fylla de återstående fälten på leverantörskortet. Mer information finns i [Så här registrerar du nya leverantörer](purchasing-how-register-new-vendors.md).  
8. Välj **OK** för att gå tillbaka till fönstret **Inköpsfaktura**, när du har slutfört leverantörskortet.

    Flera fält i fönstret **Inköpsfaktura** är ifyllda med information som du har angett på det nya leverantörskortet.
9. I fönstret **Inköpsfaktura** fyller du i de återstående fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

    Fortsätt med att fylla inköpsfakturaraderna med lagerförda artiklar eller tjänster som du har köpt från leverantören.

    **Obs!** Om du har ställt in återkommande inköpsrader för leverantöre, till exempel en månatlig återanskaffningsorder, kan du infoga dessa rader på fakturan, genom att välja knappen **Hämta återkommande inköpsrader**.
10. På snabbfliken **rader** i fältet **Artikelnr.** anger du ett nummer för en lagerartikel eller tjänst.
11. Ange hur många artiklar som ska införskaffas i fältet **Antal**.

    **Obs!** För artiklar av typen **Tjänst** är kvantiteten en tidsenhet, till exempel timmar, enligt fältet **Enhetskod** på raden.

    Fältet **Radbelopp** uppdateras och visar värdet i fältet **Inköpspris** multiplicerat med värdet i fältet **Kvantitet**.

    Pris- och radbeloppen visas med eller utan omsättningsskatt beroende på vad du valde i fältet **Priser inkl. moms** på leverantörskortet.
12. I fältet **Fakturarabatt** anger du ett belopp som ska dras från värdet som visas i fältet **Totalt inkl. moms** längst ned på fakturan.

    **Obs!** Om du har ställt in fakturarabatter för leverantören, då infogas det angivna procentsatsvärdet automatiskt i fältet **Leverantörsfakturarabatt %** om kriteriet uppfylls, och det relaterade beloppet infogas i fältet **Fakturarabattbelopp**.
13. Välj **Bokför** när du tar emot de beställda artiklarna eller tjänster.

Inköpet visas nu i lager och ekonomiska transaktioner, och leverantörsbetalning aktiveras. Inköpsfakturan tas bort från listan över inköpsfakturor och ersätts med ett nytt dokument i listan över bokförda inköpsfakturor.

## <a name="see-also"></a>Se även  
[Hantera inköp](purchasing-manage-purchasing.md)  
[Konfigurera inköp](purchasing-setup-purchasing.md)  
[Så här köper du produkter för en försäljning](purchasing-how-purchase-products-sale.md)  
[Så här registrerar du nya leverantörer](purchasing-how-register-new-vendors.md)  
[Så här förbereder du direktutleveranser](sales-how-drop-shipment.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

