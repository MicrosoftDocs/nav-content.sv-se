---
title: "Så här gör du erbjudanden"
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
ms.openlocfilehash: e126c755a9121c3a91f3af72f3f1ae14702a4701
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-offers"></a>Så här gör du erbjudanden
Du kan skapa en försäljningsoffert för att erbjuda en kund att sälja vissa produkter till vissa leverans- och betalningsvillkor. Du kan skicka försäljningsofferten till kunden för att meddela erbjudandet. Du kan e-posta dokument som en PDF-bilaga. Du kan också välja e-postbrödtexten förifylld med en sammanfattning av offerten. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).

Medan du förhandlar med kunden kan du ändra och skicka försäljningsofferten så mycket som behövs. När kunden accepterar offerten omvandlar du försäljningsofferten till en försäljningsfaktura eller försäljningsorder som du bearbetar försäljningen. Mer information finns i [Så här fakturerar du försäljning](sales-how-invoice-sales.md), [Så här säljer du produkter](sales-how-sell-products.md).

Produkter kan vara både lagerartiklar och tjänster. Mer information finns i [Så här registrerar du nya produkter](inventory-how-register-new-products.md). Försäljningsoffertprocessen är samma för båda produkttyper.

**Obs!** I Dynamics NAV refereras en produkt med termen “item”.

Du kan fylla i kundfälten på försäljningsofferten på två sätt, beroende på om kunden redan har registrerats.

## <a name="to-create-a-sales-quote"></a>Så här skapar du en försäljningsoffert
1. Välj åtgärden **Försäljningsoffert** på startsidan.  
2. Ange namnet på en befintlig kund i fältet **Kund**.

    Andra fält i fönstret **Försäljningsoffert** fylls nu i med standardinformation om den valda kunden. Om kunden inte är registrerad, gör så här:

3. Ange namnet på en ny kund i fältet **Kund**.
4. Välj knappen **ja** i dialogrutan om registrering av den nya kunden.
5. Välj en mall det nya kundkortet ska baseras på i fönstret **Välj en mall för en ny kund** och välj sedan knappen **OK**.
6. Ett nytt kundkort öppnas med förifylld information från den markerade kundmallen. Fältet **Namn** förifylls med nya kundens namn som du har angett på försäljningsfakturan.
7. Fortsätt att fylla de återstående fälten på kundkortet. Mer information finns i [Så här registrerar du nya kunder](sales-how-register-new-customers.md).  
8. Välj **OK** för att gå tillbaka till fönstret **Försäljningsoffert**, när du har slutfört kundkortet.

    Flera fält i Försäljningsofferten är nu ifyllda med information som du har angett på det nya kundkortet.
9. I fönstret **Försäljningsoffert** fyller du i de återstående fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

    Du är nu redo att fylla i Försäljningsoffertraderna med lagerförda artiklar eller tjänster som du vill erbjuda till kunden.

    **Obs!** Om du har ställt in återkommande försäljningsrader för kunden, till exempel en månatlig återanskaffningsorder, kan du infoga de här raderna på offerten, genom att välja åtgärden **Hämta återkommande försäljningsrader**.
10. På snabbfliken **rader** i fältet **Artikelnr.** anger du ett nummer för en lagerartikel eller tjänst.
11. Skriv det antal artiklar som ska erbjudas i fältet **Antal**.

    **Obs!** För artiklar av typen Tjänst är kvantiteten en tidsenhet, till exempel timmar, enligt fältet **Enhetskod** på raden.

    Fältet **Radbelopp** uppdateras och visar värdet i fältet **Enhetspris** multiplicerat med värdet i fältet **Kvantitet**.

    Pris- och radbeloppen visas med eller utan omsättningsskatt beroende på vad du valde i fältet **Priser inkl. omsättningsskatt** på kundkortet.
12. Ange ett värde i procent, om du vill bevilja kunden en rabatt på produkten i fältet **Radrabatt %**. Värdet i fältet **Radbelopp** uppdateras i enlighet därmed.

    **Obs!** Om du har ställt in särskild artikelpriser på snabbfliken **Försäljningspriser och försäljningsradrabatter** på kund- eller artikelkortet uppdateras priset och beloppet på offertraden automatiskt om de överenskomna priskriterierna uppfylls. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).
13. Ange en text i fältet **Beskrivning** på en tom rad för att lägga till en kommentar om offertraden som kunden kan se på den utskrivna offerten.  
14. Upprepa moment 10 till 13 för varje artikel som du vill att erbjuda kunden.

    Summorna under raderna beräknas automatiskt när du skapar eller ändrar rader.
15. I fältet **Fakturarabatt** anger du ett belopp som ska dras från värdet som visas i fältet **Totalt inkl. moms**.

    **Obs!** Om du har ställt in fakturarabatter för kunden, då infogas det angivna procentsatsvärdet automatiskt i fältet **Fakturarabatt %** om kriteriet uppfylls, och det relaterade beloppet infogas i fältet **Rabattbelopp exkl. moms**. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).
16. När försäljningsoffertraderna slutförda väljer du åtgärden **E-posta** eller **Skriva ut**.

    Om du markerade **E-post** bifogas en PDF-fil automatiskt till ett e-postmeddelande till kunden. Du kan ställa in e-postmeddelandet till att innehålla en sammanfattning av offerten. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).
17. Om kunden accepterar offerten väljer du åtgärden **Gör faktura** eller **Gör order**.

Försäljningsofferten tas bort från databasen. En försäljningsfaktura eller försäljningsorder har skapats baserat på informationen i försäljningsofferten där du kan bearbeta försäljningen. I fältet **Offertnr.** på försäljningsfakturan eller försäljningsordern kan du ange numret på försäljningsofferten som den har skapats från. Mer information finns i [Så här fakturerar du försäljning](sales-how-invoice-sales.md), [Så här säljer du produkter](sales-how-sell-products.md).

## <a name="see-also"></a>Se även  
[Hantera försäljning](sales-manage-sales.md)  
[Ställa in försäljning](sales-setup-sales.md)  
[Så här skickar du dokument som e-post](ui-how-send-documents-email.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

