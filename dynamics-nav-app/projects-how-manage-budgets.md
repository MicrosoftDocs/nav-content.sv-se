---
title: "Så här: hanterar du projektbudget"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c28e23c4ae0082265357a567ea82795b77ac8f1c
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-budgets"></a>Så här: hanterar du projektbudget
Du kan lägga upp en budget för varje projekt. Budgeten används för att planera de resurser du tilldelar ett projekt. Budgeten kan antingen vara allmän med få poster eller innehålla fler poster som är indelade i aktivitetsnivåer. Du kan sedan jämföra budgeterade belopp med den faktiska förbrukningen enligt registreringen i projektjournalen. Genom att övervaka skillnader mellan faktisk förbrukning och budgeterad användning kan du kontrollera pågående projekt och förbättra kvaliteten hos framtida projekt genom att minska risken för att kostnader underskattas.

Efterföljande procedur beskriver hur du beräknar budgeterade kostnader under planering. Mer information om registrering av budgeterade jämfört med faktiskta projektpriser och kostnader finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).  

## <a name="JobBudgetCosts"></a> Att ange budgeterade kostnader för ett projekt  
När en kund vill veta priset på ett projekt som kommer att faktureras baserat på förbrukning, måste du fastställa de budgeterade kostnaderna för projektet. Du använder fönstret **Projektaktivitetsrader** om du vill göra detta.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.  
2. Öppna ett relevant projekt.
3. Markera en projektrad av typen Bokföring och välj sedan åtgärden **Projektplaneringsrader**.
4. Fyll i fälten på en ny rad efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.   

Se följande information för fältet **Radtyp**.  

|Typ av rad |Beskrivning |
|----------|------------|
|**Både Budget och Fakturerbart**|Kostnads- och prisbelopp som har angetts på planeringsraderna är de budgeterade kostnaderna för denna specifika planeringsrad. Prisbeloppet faktureras.|
|**Budget**|Kunden debiteras inte för användning. Förbrukningen överförs inte till en faktura, men den kommer fortfarande att användas i PIA-beräkningen.|
|**Fakturerbart**|Kunden debiteras för användning. Förbrukningen överförs till fakturan baserat på det antal som finns angivet i fältet Antal. att överföra till faktura.|

**Obs**! Fältet **Planeringsdatum** för planeringsraden innehåller datumet då förbrukning som relateras till planeringsraden förväntas slutföras. Det är också datumet då planeringsraden kan överföras till en försäljningsfaktura och bokföras.  

**Obs**! När du fyller i fältet **Antal** kommer all information om totalt pris och total kostnad att beräknas och fyllas i för planeringsraden. De kan redigeras när det passar dig.

I fönstret **Projektkort** kan du nu se en översikt över de totala budgeterade kostnaderna, budgeterat pris, fakturerbar kostnad och fakturerbart pris för varje aktivitet.

Mer information om registrering av budgeterade jämfört med faktiskta projektpriser och kostnader finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).

## <a name="see-also"></a>Se även
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)  

