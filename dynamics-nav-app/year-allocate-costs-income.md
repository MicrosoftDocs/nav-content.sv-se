---
title: "Översikt över arbetsuppgifter för att fördela kostnader och intäkter"
description: "Beskriver uppgiften att fördela en transaktion i en redovisningsjournal på flera olika konton när du bokför journalen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fdb03090dc9ba024d84a175e313f7d530bd0feae
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-allocate-costs-and-income"></a>Förklarar hur du fördelar kostnader och intäkter.
Du kan fördela en transaktion i en redovisningsjournal på flera olika konton när du bokför journalen. Fördelningen kan göras enligt tre olika metoder:

* Antal
* Procent (%)
* Belopp

Fördelningsfunktionerna kan användas med återkommande redovisningsjournaler och i anläggningstillgångsjournaler.
<!--You can also distribute the cost or revenue of a line to an intercompany partner when you post a sales or purchase document. When you post the document, a line will be posted in your general journal, and a corresponding line will be created in the intercompany outbox.-->

I följande procedurer beskrivs hur du förbereder att fördela kostnader i en återkommande redovisningsjournal genom att definiera fördelningsnycklar. När fördelningsnycklar definieras slutför du och bokför journalen som alla andra återkommande redovisningsjournaler. Mer information finns i [Arbeta med Redovisningsjournaler](ui-work-general-journals.md).

## <a name="to-set-up-allocation-keys"></a>Så här skapar du fördelningsnycklar
Du kan fördela en transaktion i en återkommande redovisningsjournal på flera olika konton när du bokför journalen. Fördelningen kan göras efter kvantitet, procentuellt eller med ett belopp.
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Återkommande redov.journal** och välj sedan relaterad länk.
2. Välj fältet **Journalnamn** för att öppna fönstret **redovisningsjournaler**.
3. Du kan antingen ändra fördelningar på en befintlig journal i listan eller skapa en ny journal med fördelningar.
   * För att skapa en y journal väljer du åtgärden **Ny** och går vidare till nästa steg för att skapa en ny journal.
   * Välj journalen och gå till steg 7 för att ändra fördelningar av en befintlig journal.    
4. I fältet **Namn** anger du ett namn för journalens som t.ex. RENSNING. I fältet **beskrivning** anger du en beskrivning som t.ex. Rensning av utläggsjournal.
5. Stäng fönstret när du är klar. En ny, tom återkommande journal öppnas.
6. Fyll i fälten på raden.
7. Välj åtgärden **Fördelningar**.
8. Lägg till en rad för varje fördelning. Du måste fylla i fältet **Fördelning %**, **Fördelningskvantitet** eller **Belopp**. Du måste också fylla i fältet **Nr** och, om du fördelar transaktionen bland globala dimensioner, fälten för globala dimensioner.
9. Om du anger ett värde i procent på en rad beräknas beloppet i fältet **Belopp** automatiskt. Dessa belopp har motsatt tecken mot det totala beloppet i fältet **Belopp** i den återkommande journalen.
10. Välj **OK** för att återgå till fönstret **Återkommande redov.journal** fönstret, när du har angett fördelningsraderna. Fältet **Fördelat belopp (USD)** är ifyllt och matchar fältet **Belopp**.
11. Bokför journalen.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>För att ändra en fördelningsnyckel som redan har angetts.
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Återkommande redov.journal** och välj sedan relaterad länk.
2. Välj journalen med fördelningen i fältet **Återkommande redov.journal**.
3. Välj raden med fördelningen och välj sedan åtgärden **fördelningar**.
4. Fyll i de relevanta fälten och välj sedan knappen **OK**.

## <a name="see-also"></a>Se även
[Avsluta år och perioder](year-close-years-periods.md)  
[Arbeta med redovisningsjournaler](ui-work-general-journals.md)    
[Bokför dokument och journaler](ui-post-documents-journals.md)    
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

