---
title: "Så här fakturerar du försäljning"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: cba338ec6469ea0ac22f024571664a718988e827
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-sales"></a>Så här fakturerar du försäljning

Du kan skapa en försäljningsfaktura eller försäljningsorder för att registrera en överenskommelse med en kund om att sälja vissa produkter till vissa leverans- och betalningsvillkor.

**Obs!** Du måste använda försäljningsorder om din försäljningsprocess kräver att du t.ex. kan leverera delar av en orderkvantitet eftersom hela kvantiteten inte är tillgängliga på en gång. Om du säljer artiklar genom att leverera direkt från din leverantör till kunden, som en direktleverans, måste du även använda försäljningsorder. För mer information finns i [Så här gör du Direktleveranser](sales-how-drop-shipment.md). I alla andra aspekter fungerar försäljningsorder på samma sätt som försäljningsfakturor. Mer information finns i [Så här säljer du produkter](sales-how-sell-products.md).

Du kan förhandla med kunden genom att först skapa förs.offerter, som du kan omvandla till en försäljningsfaktura när du instämmer om försäljningen. För mer information finns i [Så här gör du erbjudanden](sales-how-make-offers.md).

När kunden har bekräftat avtalet, till exempel efter en offertprocess, bokför du försäljningsfakturan för att skapa den relaterade kvantiteten och värdetransaktioner i ditt system. När du bokför försäljningsfakturan, kan du också e-posta dokument som en PDF-bilaga. Du kan använda ifylld e-postbrödtext med en sammanfattning av fakturan och betalningsinformationen, till exempel en länk till PayPal. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).

I affärsmiljöer där kunden måste betala för produkter i förväg måste du vänta på kvittot på betalning innan du levererar produkterna. I de flesta fall behandlar du inkommande betalningar några veckor efter leverans, genom att koppla betalningarna till dess relaterade obetalda bokförda försäljningsfakturor. Mer information finns i [Så här stämmer du av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md).

Om den bokförda försäljningsfakturan betalas, måste du skapa en försäljningskreditnota för att återföra försäljningen. Mer information finns i [Så här behandlar du försäljningsreturer eller annulleringar](sales-how-process-sales-returns-cancellations.md).

Produkter kan vara både lagerartiklar och tjänster. Mer information finns i [Så här registrerar du nya produkter](inventory-how-register-new-products.md). Försäljningsfakturaprocessen är samma för båda produkttyper.

**Obs!** I Dynamics NAV refereras en produkt med termen “item”.

Du kan fylla i kundfälten på försäljningsfakturan på två sätt, beroende på om kunden redan har registrerats.

## <a name="to-create-a-sales-invoice"></a>Så här skapar du en försäljningsfaktura
1. Välj åtgärden **Försäljningsfaktura** på startsidan.  
3. Ange namnet på en befintlig kund i fältet **Kund**.

    Andra fält i fönstret **Försäljningsfaktura** fylls nu i med standardinformation om den valda kunden. Om kunden inte är registrerad, gör så här:
4. Ange namnet på en ny kund i fältet **Kund**.
5. Välj knappen **ja** i dialogrutan om registrering av den nya kunden.
6. Välj en mall det nya kundkortet ska baseras på i fönstret **Välj en mall för en ny kund** och välj sedan knappen **OK**.
7. Ett nytt kundkort öppnas med förifylld information från den markerade kundmallen. Fältet **Namn** förifylls med nya kundens namn som du har angett på försäljningsfakturan.
8. Fortsätt att fylla de återstående fälten på kundkortet. Mer information finns i [Så här registrerar du nya kunder](sales-how-register-new-customers.md).  
9. Välj **OK** för att gå tillbaka till fönstret **Förs.faktura**, när du har slutfört kundkortet.

    Flera fält i försäljningsfakturahuvudet är nu ifyllda med information som du har angett på det nya kundkortet.
10. I fönstret **Inkommande dokument** fyller du i de återstående fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

    Du är nu redo att fylla i försäljningsfakturaraderna med lagerförda artiklar eller tjänster som du vill sälja till kunden.

    Om du har ställt in återkommande försäljningsrader för kunden, till exempel en månatlig återanskaffningsorder, kan du infoga de här raderna på fakturan, genom att välja åtgärden **Hämta återkommande försäljningsrader**.
11. Ange numret på en lagerförd artikel eller service på snabbfliken **Rader** Snabbfliken, i **Artikel** fältet.  
12. Skriv det antal artiklar som ska säljas i fältet **Kvantitet**.

    **Obs!** För artiklar av typen Tjänst är kvantiteten en tidsenhet, till exempel timmar, enligt fältet **Enhetskod** på raden.

    Fältet **Radbelopp** uppdateras och visar värdet i fältet **Enhetspris** multiplicerat med värdet i fältet **Kvantitet**.

    Pris- och radbeloppen visas med eller utan omsättningsskatt beroende på vad du valde i fältet **Priser inkl. moms** på kundkortet.
13. Ange ett värde i procent, om du vill bevilja kunden en rabatt på produkten i fältet **Radrabatt %**. Värdet i fältet **Radbelopp** uppdateras i enlighet därmed.

    Om du har ställt in särskild artikelpriser på snabbfliken **Försäljningspriser och försäljningsradrabatter** på kund- eller artikelkortet uppdateras priset och beloppet på offertraden automatiskt om de överenskomna priskriterierna uppfylls. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).
14. Ange en text i fältet **Beskrivning** på en tom rad för att lägga till en kommentar om offertraden som kunden kan se på den utskrivna offerten.  
15. Upprepa moment 10 till 13 för varje artikel som du vill att erbjuda kunden.

    Summorna under raderna beräknas automatiskt när du skapar eller ändrar rader.
16. I fältet **Fakturarabatt** anger du ett belopp som ska dras från värdet som visas i fältet **Totalt inkl. moms**.

    Om du har ställt in fakturarabatter för kunden, då infogas det angivna procentsatsvärdet automatiskt i fältet **Fakturarabatt %** om kriteriet uppfylls, och det relaterade beloppet infogas i fältet **Inv. Rabattbelopp exkl. moms**. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).
17. När försäljningsfakturaraderna slutförda väljer du åtgärden **Bokföra och skicka**.

Dialogrutan **Bekräftelse för bokför och utskick** öppnas och visar kundens önskad utskicksmetod. Du kan ändra utskicksmetoden genom att välja sökknappen för fältet **Skicka dokument till**. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).

Relaterade artiklar och kundtransaktionerna skapas nu i systemet, och försäljningsfakturan matas ut som ett PDF-dokument. Försäljningsfakturan tas bort från listan över försäljningsfakturor och ersätts med ett nytt dokument i listan över bokförda försäljningsfakturor.

## <a name="see-also"></a>Se även  
[Hantera försäljning](sales-manage-sales.md)  
[Ställa in försäljning](sales-setup-sales.md)  
[Lager](inventory-manage-inventory.md)    
[Så här skickar du dokument som e-post](ui-how-send-documents-email.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

