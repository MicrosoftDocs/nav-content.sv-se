---
title: "Låta Dynamics NAV föreslå värden"
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
ms.openlocfilehash: 889d0aa5da36d7a4b7e2be1d796ac95e74aaaaf6
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="letting-dynamics-nav-suggest-values"></a>Låta Dynamics NAV föreslå värden
Dynamics NAV kan hjälpa dig att avsluta uppgifter som är snabbare och korrektare genom att fylla i fält eller färdigställa rader med data som du annars måste annars beräkna och ange själv. Även om sådana automatiska datainmatningar inte alltid är korrekta kan du ändra den efteråt om du vill.

Funktionen som matar in fältvärden åt dig, erbjuds vanligtvis för uppgifter där du anger stora volymer av transaktionsdata och vill undvika fel och spara tid. Det här avsnittet innehåller ett urval av sådana funktioner. Mer avsnitt ska läggas till i framtida uppdateringar av Dynamics NAV.

## <a name="the-suggest-balancing-amount-check-box-in-the-general-journal-batches-window"></a>Kryssrutan **Föreslå saldobelopp** i fönstret **Redovisningsjournaler**
Om du till exempel vill ange redovisningsjournalrader för åtskilliga kostnader som alla måste bokföras till samma bankkontot, kan du när du varje gång anger en ny journalrad för en kostnad, låta fältet **Belopp** på bankkontoraden uppdateras automatiskt till beloppet som balanserar kostnaderna. Mer information om att arbeta med redovisningsjournaler finns i [arbeta med redovisningsjournaler](ui-work-general-journals.md).

### <a name="to-have-the-amount-field-on-balancing-general-journal-lines-filled-automatically"></a>Om du vill ha fältet **Belopp** på balanserande redovisningsjournalrader fyllas i automatiskt
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournaler** och välj sedan relaterad länk.
2. På raden för din föredragna redovisningsjournal väljer kryssrutan **Föreslå saldobelopp**.
3. Öppna redovisningsjournalen och fortsätt att registrera och bokföra transaktioner med den beskrivna funktionen för automatisk bokföring av ett fältvärde.       

Mer information om hur du konfigurerar en personlig redovisningsjournal för t.ex. kostnadsbearbetning finns i [Arbeta med redovisningsjournaler](ui-work-general-journals.md).

## <a name="the-automatically-fill-date-received-field-in-the-payment-registration-window"></a>Fältet **Fyll i Tillbaka datum automatiskt** i fönstret **Betalningregistrering**
Fönstret **Betalningsregistrering** visar utestående inkommande betalningar som rader som representerar de försäljningsdokument, där ett belopp har förfallit till betalning. Mer information om att koppla kundbetalningar finns i [Så här stämmer du av kundutbetalningar manuellt från en lista med obetalda försäljningsdokument](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)

Dina huvudåtgärder i fönstret är att fylla i kryssrutan **Utförd betalning** och fältet **Tillbaka datum**. Du kan konfigurera Dynamics NAV att automatiskt ange arbetsdatum i fältet **Tillbaka datum** när du markerar kryssrutan **Utförd betalning**.

### <a name="to-have-the-date-received-field-in-the-payment-registration-window-filled-automatically"></a>Att ha fältet **Fyll i Tillbaka datum automatiskt** i fönstret **Betalningregistrering** ifyllt automatiskt.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inställning av betalningsregistrering** och välj sedan relaterad länk.
2. Markera kryssrutan **Fyll i Tillbaka datum automatiskt**.
3. Öppna fönstret **Betalningsregistrering** och fortsätt behandla inkommande kundbetalningar med hjälp av den beskrivna funktionen för automatisk bokföring av ett fältvärde.

## <a name="see-also"></a>Se även
[Arbeta med Dynamics NAV](ui-work-product.md)  
[Finans](Finance.md)

