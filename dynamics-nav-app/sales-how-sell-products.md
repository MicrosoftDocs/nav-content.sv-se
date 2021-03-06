---
title: "Skapa en försäljningsreturorder och sälja produkter"
description: "Beskriver hur du skapar en försäljningsorder för att registrera ditt avtal med en kund om att sälja eller handla med produkter som omfattas av särskilda villkor."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1371f7a1d1e5b5c9bd0add845d37e194db86218d
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-sell-products"></a>Så här säljer du produkter
Du kan skapa en försäljningsorder eller försäljningsfaktura för att registrera en överenskommelse med en kund om att sälja vissa produkter till vissa leverans- och betalningsvillkor.

> [!NOTE]  
>   Du måste använda försäljningsorder om din försäljningsprocess kräver att du t.ex. kan leverera delar av en orderkvantitet eftersom hela kvantiteten inte är tillgängliga på en gång. Om du säljer artiklar genom att leverera direkt från din leverantör till kunden, som en direktleverans, måste du även använda försäljningsorder. För mer information finns i [Så här gör du Direktleveranser](sales-how-drop-shipment.md). I alla andra aspekter fungerar försäljningsorder på samma sätt som försäljningsfakturor. Mer information finns i [Så här fakturerar du försäljning](sales-how-invoice-sales.md).

Du kan förhandla med kunden genom att först skapa förs.offerter, som du kan omvandla till en försäljningsorder när du instämmer om försäljningen. För mer information finns i [Så här gör du erbjudanden](sales-how-make-offers.md).

När kunden har bekräftat avtalet, till exempel efter en offertprocess, skickar du en orderbekräftelse för att registrera dina åtagande att leverera produkterna enligt överenskomment.

När du har levererat produkterna, antingen helt eller delvis, bokför du försäljningsordern som levererade eller som levererade och fakturerade för att skapa kundreskontratransaktioner i systemet. När du bokför försäljningsorder, kan du också e-posta dokument som en PDF-bilaga. Du kan använda ifylld e-postbrödtext med en sammanfattning av ordern och betalningsinformationen, till exempel en länk till PayPal. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).

I affärsmiljöer där kunden måste betala för produkter i förväg måste du vänta på kvittot på betalning innan du levererar produkterna. I de flesta fall behandlar du inkommande betalningar några veckor efter leverans, genom att koppla betalningarna till dess relaterade obetalda bokförda försäljningsfakturor. Mer information finns i [Så här stämmer du av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md).

Det är enkelt att rätta eller avbryta en bokförd försäljningsfaktura som härrör från en försäljningsorder, innan den har betalas. Det är användbart om du vill rätta till ett skrivfel eller om du kunden göra en ändring tidigt i orderprocessen. Mer information finns i [Så här rättar eller annullerar du obetalda försäljningsfakturor](sales-how-correct-cancel-sales-invoice.md). Om den bokförda försäljningsfakturan betalas, måste du skapa en försäljningskreditnota för att återföra försäljningen. Mer information finns i [Så här behandlar du försäljningsreturer eller annulleringar](sales-how-process-sales-returns-cancellations.md).

Du kan fylla i kundfälten på försäljningsorder på två sätt, beroende på om kunden redan har registrerats. Se steg 2 och 3 i följande procedur.

## <a name="to-create-a-sales-order"></a>Så här skapar du försäljningsorder
1. På startsidan väljer du åtgärden **Försäljningsorder**.  
2. Ange namnet på en befintlig kund i fältet **Kund**.

    Andra fält i fönstret **Försäljningsorder** fylls nu i med standardinformation om den valda kunden. Om kunden inte är registrerad, gör så här:
3. Ange namnet på en ny kund i fältet **Kund**.
4. Välj knappen **ja** i dialogrutan om registrering av den nya kunden.
5. Välj en mall det nya kundkortet ska baseras på i fönstret **Välj en mall för en ny kund** och välj sedan knappen **OK**.

    Ett nytt kundkort öppnas med förifylld information från den markerade kundmallen. Fältet **Namn** förifylls med nya kundens namn som du har angett på Försäljningsordern.
6. Fortsätt att fylla de återstående fälten på kundkortet. Mer information finns i [Så här registrerar du nya kunder](sales-how-register-new-customers.md).  
7. Välj **OK** för att gå tillbaka till fönstret **Försäljningsorder**, när du har slutfört kundkortet.

    Flera fält i Försäljningsorder är nu ifyllda med information som du har angett på det nya kundkortet.
8. I fönstret **Försäljningsorder** fyller du i de återstående fälten efter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    Du är nu redo att fylla i Försäljningsorderraderna med lagerförda artiklar eller tjänster som du vill sälja till kunden.

    Om du har ställt in återkommande försäljningsrader för kunden, till exempel en månatlig återanskaffningsorder, kan du infoga de här raderna på ordern, genom att välja åtgärden **Hämta återkommande försäljningsrader**.
9. Ange numret på en lagerförd artikel eller service på snabbfliken **Rader** Snabbfliken, i **Artikel** fältet.  
10. Skriv det antal artiklar som ska säljas i fältet **Kvantitet**.

    Fältet **Radbelopp** uppdateras och visar värdet i fältet **Enhetspris** multiplicerat med värdet i fältet **Kvantitet**.

    Pris- och radbeloppen visas med eller utan omsättningsskatt beroende på vad du valde i fältet **Priser inkl. moms** på kundkortet.
11. Ange ett värde i procent, om du vill bevilja kunden en rabatt på produkten i fältet **Radrabatt %**. Värdet i fältet **Radbelopp** uppdateras i enlighet därmed.

    Om du har ställt in särskild artikelpriser på snabbfliken **Försäljningspriser och försäljningsradrabatter** på kund- eller artikelkortet uppdateras priset och beloppet på offertraden automatiskt om de överenskomna priskriterierna uppfylls. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).
12. Ange en text i fältet **Beskrivning** på en tom rad för att lägga till en kommentar om offertraden som kunden kan se på den utskrivna offerten.  
13. Upprepa moment 10 till 13 för varje artikel som du vill att erbjuda kunden.

    Summorna under raderna beräknas automatiskt när du skapar eller ändrar rader.
6. Ett nytt kundkort visar information från den markerade kundmallen. Fyll i resterande fält. Mer information finns i [Så här registrerar du nya kunder](sales-how-register-new-customers.md).  
7. Välj **OK** för att gå tillbaka till fönstret **Försäljningsorder**, när du har slutfört kundkortet.

   Flera fält i Försäljningsorder är nu ifyllda med information som du har angett på det nya kundkortet.  
8. I fönstret **Försäljningsorder** fyller du i de återstående fälten efter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

   Du är nu klar att fylla i försäljningsorderraderna för produkter som du säljer till kunden eller för en transaktion med den kund som du vill registrera en post i ett redovisningskonto.   

   Om du har ställt in återkommande försäljningsrader för kunden, till exempel en månatlig återanskaffningsorder, kan du infoga de här raderna på ordern, genom att välja åtgärden **Hämta återkommande försäljningsrader**.  
9. På snabbfliken **rader** i fältet **typ** väljer du vilken typ av produkt, kostnad eller transaktion som du vill bokföra för kunden med försäljningsraden.
10. I fältet **Nr.** väljer du en post som ska bokföras enligt värdet i fältet **typ**.

    Du lämnar fältet **Nr.** tomt i följande fall: om raden gäller en kommentar. Skriv kommentaren fältet **beskrivning**.
    -Om raden är för en ej lagerförd artikel. Välj åtgärd **markera ej lagerförda artiklar**. Mer information finns i [Så här arbetar du med ej lagerförd artikel](inventory-how-work-nonstock-items.md).

11. I fältet **antal** anger du hur många enheter av produkt, kostnad eller transaktion som registreras på raden för kunden.  

    > [!NOTE]  
>   Om artikeln är av typen **Artikel - tjänst** eller **Resurs** är kvantiteten en tidsenhet, till exempel timmar, enligt fältet **Enhetskod** på raden.  

    Värdet i fältet **Radbelopp** beräknas som *enhetspris* x *antal*.  

    Pris- och radbeloppen visas med eller utan omsättningsskatt beroende på vad du valde i fältet **Priser inkl. moms** på kundkortet.  
12. Om du vill ge en rabatt kan du ange ett procenttal i fältet **radrabatt %**. Värdet i fältet **Radbelopp** uppdateras i enlighet därmed.  

    Om du har ställt in särskild artikelpriser på snabbfliken **Försäljningspriser och försäljningsradrabatter** på kund- eller artikelkortet uppdateras priset och beloppet på försäljningsraden automatiskt om de överenskomna priskriterierna uppfylls. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).  
13. Upprepa moment 9 till 12 för varje produkt som du vill att sälja till kunden.  

    Summorna under raderna beräknas automatiskt när du skapar eller ändrar rader.  
14. I fältet **Fakturarabatt** anger du ett belopp som ska dras från värdet som visas i fältet **Totalt inkl. moms**.

    Om du har ställt in fakturarabatter för kunden, då infogas det angivna procentsatsvärdet automatiskt i fältet **Fakturarabatt %** om kriteriet uppfylls, och det relaterade beloppet infogas i fältet **Inv. Rabattbelopp exkl. moms**. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).
15. Att enbart leverera en del av orderkvantiteten , anger denna kvantitet i **Ant. att utleverera**. Värdet kopieras till **Ant. att fakturera**.
16. För att enbart fakturera en del av den levererade kvantiteten , anger du denna kvantitet i **Ant. att fakturera**. Antalet kan inte vara högre än värdet i fältet **Ant. att utleverera**.   
17. När försäljningsorderraderna slutförda väljer du åtgärden **Bokföra och skicka**.

Dialogrutan **Bokför och skicka bekräftelse** visar kundens standardmetod för mottagning av dokument. Du kan ändra utskicksmetoden genom att välja sökknappen för fältet **Skicka dokument till**. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).

Relaterade artiklar och kundtransaktionerna skapas nu i systemet, och försäljningsorder matas ut som ett PDF-dokument. När försäljningsordern bokförs helt tas den bort från listan över försäljningsorder och ersätts med nya dokument i listan över bokförda försäljningsfakturor och listan över bokförda försäljningsleveranser.

## <a name="see-also"></a>Se även
[Försäljning](sales-manage-sales.md)  
[Konfigurera försäljning](sales-setup-sales.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Så här skickar du dokument som e-post](ui-how-send-documents-email.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

