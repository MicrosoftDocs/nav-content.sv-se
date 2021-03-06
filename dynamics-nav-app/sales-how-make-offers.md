---
title: "Skapa ett försäljningserbjudande till en kund"
description: "Beskriver hur du skapar ett försäljningserbjudande eller begäran om förslag (Offertförfrågan) för att registrera ditt erbjudande till kunden att sälja produkter under vissa villkor."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 08/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 21611abbb658ddcd4e422269db9677bca3ea4f35
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-make-offers"></a>Så här gör du erbjudanden
Du kan skapa en försäljningsoffert för att erbjuda en kund att sälja vissa produkter till vissa leverans- och betalningsvillkor. Du kan skicka försäljningsofferten till kunden för att meddela erbjudandet. Du kan e-posta dokument som en PDF-bilaga. Du kan också välja e-postbrödtexten förifylld med en sammanfattning av offerten. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).

Medan du förhandlar med kunden kan du ändra och skicka försäljningsofferten så mycket som behövs. När kunden accepterar offerten omvandlar du försäljningsofferten till en försäljningsfaktura eller försäljningsorder som du bearbetar försäljningen. Mer information finns i [Så här fakturerar du försäljning](sales-how-invoice-sales.md), [Så här säljer du produkter](sales-how-sell-products.md).

Du kan fylla i kundfälten på försäljningsofferten på två sätt, beroende på om kunden redan har registrerats. Se steg 2 och 3 i följande procedur.

## <a name="to-create-a-sales-quote"></a>Så här skapar du en försäljningsoffert
Välj åtgärden **Försäljningsoffert** på startsidan.  
2. Ange namnet på en befintlig kund i fältet **Kund**.

   Andra fält i fönstret **Försäljningsoffert** innehåller standardinformation om den valda kunden. Om kunden inte är registrerad, gör så här:
3. Ange namnet på en ny kund i fältet **Kund**.
4. Välj knappen **ja** i dialogrutan om registrering av den nya kunden.
5. Välj en mall det nya kundkortet ska baseras på i fönstret **Välj en mall för en ny kund** och välj sedan knappen **OK**.
6. Ett nytt kundkort visar information från den markerade kundmallen. Fyll i resterande fält. Mer information finns i [Så här registrerar du nya kunder](sales-how-register-new-customers.md).  
7. Välj **OK** för att gå tillbaka till fönstret **Försäljningsoffert**, när du har slutfört kundkortet.

   Flera fält i Försäljningsofferten är nu ifyllda med information som du har angett på det nya kundkortet.  
8. I fönstret **Försäljningsoffert** fyller du i de återstående fälten efter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

Du är nu klar att fylla i försäljningsorderraderna för produkter som du säljer till kunden eller för en transaktion med den kund som du vill registrera en post i ett redovisningskonto.   

Om du har ställt in återkommande försäljningsrader för kunden, till exempel en månatlig återanskaffningsorder, kan du infoga de här raderna på ordern, genom att välja åtgärden **Hämta återkommande försäljningsrader**.  
9. På snabbfliken **rader** i fältet **typ** väljer du vilken typ av produkt, kostnad eller transaktion som du vill bokföra för kunden med försäljningsraden.
10. I fältet **Nr.** väljer du en post som ska bokföras enligt värdet i fältet **typ**.

 Du lämnar fältet **Nr.** tomt i följande fall: om raden gäller en kommentar. Skriv kommentaren fältet **beskrivning**.
 -Om raden är för en ej lagerförd artikel. Välj åtgärd **markera ej lagerförda artiklar**. Mer information finns i [Så här arbetar du med ej lagerförd artikel](inventory-how-work-nonstock-items.md).

11. I fältet **antal** anger du hur många enheter av produkt, kostnad eller transaktion som registreras på raden för kunden.

    Värdet i fältet **Radbelopp** beräknas som *enhetspris* x *antal*.  

    Pris- och radbeloppen visas med eller utan omsättningsskatt beroende på vad du valde i fältet **Priser inkl. moms** på kundkortet.  
12. Om du vill ge en rabatt kan du ange ett procenttal i fältet **radrabatt %**. Värdet i fältet **Radbelopp** uppdateras i enlighet därmed.  

    Om du har ställt in särskild artikelpriser på snabbfliken **Försäljningspriser och försäljningsradrabatter** på kund- eller artikelkortet uppdateras priset och beloppet på försäljningsraden automatiskt om de överenskomna priskriterierna uppfylls. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).  
13. Upprepa moment 9 till 12 för varje produkt som du vill att erbjuda kunden.  

    Summorna under raderna beräknas automatiskt när du skapar eller ändrar rader.  
14. I fältet **Fakturarabatt** anger du ett belopp som ska dras från värdet som visas i fältet **Totalt inkl. moms**.

    Om du har ställt in fakturarabatter för kunden, då infogas det angivna procentsatsvärdet automatiskt i fältet **Fakturarabatt %** om kriteriet uppfylls, och det relaterade beloppet infogas i fältet **Inv. Rabattbelopp exkl. moms**. Mer information finns i [Registrera försäljningspris, rabatt och betalningsavtal](sales-how-record-sales-price-discount-payment-agreements.md).
15. När försäljningsoffertraderna slutförda väljer du åtgärden **Skicka med e-post**.
16. I fönstret **Skicka e-post** fyller du i återstående fält och granskar den inbäddade försäljningsofferten. Mer information finns i [Så här skickar du dokument via e-post](ui-how-send-documents-email.md).
17. Om kunden accepterar offerten väljer du åtgärden **Gör faktura** eller **Gör order**.

Försäljningsofferten tas bort från databasen. En försäljningsfaktura eller försäljningsorder har skapats baserat på informationen i försäljningsofferten där du kan bearbeta försäljningen. I fältet **Offertnr** på försäljningsfakturan eller försäljningsordern kan du ange numret på försäljningsofferten som den har skapats från. Mer information finns i [Så här fakturerar du försäljning](sales-how-invoice-sales.md), [Så här säljer du produkter](sales-how-sell-products.md).

## <a name="see-also"></a>Se även
[Försäljning](sales-manage-sales.md)  
[Konfigurera försäljning](sales-setup-sales.md)  
[Så här skickar du dokument som e-post](ui-how-send-documents-email.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

