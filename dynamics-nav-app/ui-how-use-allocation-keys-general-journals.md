---
title: "Så här använder du fördelningsnycklar i redovisningsjournaler"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d239ab62c4be88ccc4a2ce2669dcc2c20a3c0126
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a>Så här använder du fördelningsnycklar i redovisningsjournaler
Du kan fördela en transaktion i en redovisningsjournal på flera olika konton när du bokför journalen. Fördelningen kan göras efter kvantitet, procentuellt eller med ett belopp.

## <a name="to-set-up-allocation-keys"></a>Så här skapar du fördelningsnycklar 
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Återkommande redov.journal** och välj sedan relaterad länk.
2. Välj fältet **Journalnamn** för att öppna fönstret **redovisningsjournaler**.
3. Du kan antingen ändra fördelningar på en befintlig journal i listan eller skapa en ny journal med fördelningar.
  * För att skapa en y journal väljer du åtgärden **Ny** och går vidare till nästa steg för att skapa en ny journal.
  * Välj journalen och gå till steg 7 för att ändra fördelningar av en befintlig journal.    
4. I fältet **Namn** anger du ett namn för journalens som t.ex. RENSNING. I fältet **beskrivning** anger du en beskrivning som t.ex. Rensning av utläggsjournal.
5. Stäng fönstret när du är klar. En ny, tom återkommande journal öppnas. 
6. Fyll i fälten på raden.
7. Välj åtgärden **Fördelningar**. 
8. Lägg till en rad för varje fördelning. Du måste fylla i fältet **Fördelning %**, **Fördelningskvantitet** eller **Belopp**. Du måste fylla i **Kontonr.** och om du fördelar transaktionen bland globala dimensioner, fälten för globala dimensioner.
9. Om du anger ett värde i procent på en rad beräknas beloppet i fältet **Belopp** automatiskt. Dessa belopp har motsatt tecken mot det totala beloppet i fältet **Belopp** i den återkommande journalen.
10. Välj **OK** för att återgå till fönstret **Återkommande redov.journal** fönstret, när du har angett fördelningsraderna. Fältet **Fördelat belopp (USD)** är ifyllt och matchar fältet **Belopp**.
11. Bokför journalen.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>För att ändra en fördelningsnyckel som redan har angetts.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Återkommande redov.journal** och välj sedan relaterad länk.
2. Välj journalen med fördelningen i fältet **Återkommande redov.journal**.
3. Välj raden med fördelningen och välj sedan åtgärden **fördelningar**.
4. Ändra de relevanta fälten, och stäng fönstret.

## <a name="see-also"></a>Se även
[Arbeta med redovisningsjournaler](ui-work-general-journals.md)  
[Bokför dokument och journaler](ui-post-documents-journals.md)




