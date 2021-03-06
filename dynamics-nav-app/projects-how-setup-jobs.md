---
title: "Ställ in projektpris projektbokföringsmallar"
description: "Beskriver hur du ställer in jobb för allmän information och ställer in priser för projektartiklar, resurser och redovisningskonton och projektbokföringsmallar."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6a1c4c6f6b90d3e721d545f86841472ba3a71388
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-jobs"></a>Så här skapar du projekt
I fönstret **Projektinställningar** måste du ange hur du vill använda vissa projektfunktioner.

På de individuella de projektkorten måste du lägga upp priser för projektartiklar, projektresurser och projektredovisningskonton och du måste skapa projektbokföringsmallar.

## <a name="to-set-general-information-for-jobs"></a>Så här anger du allmän information för projekt
1. Välj ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projektinställningar** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Kryssrutan **Använd förbrukningslänk** är ganska komplex och förklaras därför i följande avsnitt.

## <a name="to-set-up-job-usage-tracking"></a>Så här anger du projektförbrukningsspårning
När du vill köra ett jobb, kan det hända att du vill veta hur förbrukningen spåras mot ditt plan. Det gör du enkelt genom att skapa en koppling mellan dina projektplaneringsrader och den faktiska förbrukningen. Detta gör att du kan spåra dina kostnader och enkelt visa hur mycket som återstår att göra. Som standard är projektplaneringsradtypen **Budget**, men radtypen **Både Budget och Fakturerbart** har liknande effekter.

Om du väljer kryssrutan **Använd förbrukningslänken** kan du granska informationen på projektplaneringsraden. Du kan ange antal av resursen, artikeln eller redovisningskontot och sedan ange vilket antal som du vill överföra i projektjournalen. Fältet **Återstående antal** på projektplaneringsraden talar om vad som återstår att överföra och bokföra till projektjournalen.

Om kryssrutan **Använd förbrukningslänk** är markerad och projektplaneringsraden är av typen **Fakturerbart** skapar Finansiell en projektplaneringsrad av typen **Budget** när du har bokfört journalraden.

> [!NOTE]  
>   Om kryssrutan **Använd förbrukningslänk** på arbetskortet är markerad och fältet **Radtyp** på projektjournalraden är tomt, skapas nya projektplaneringsrader av radtypen **Budget** när du bokför projektjournalrader. Om kryssrutan **Använd förbrukningslänk** på arbetskortet inte är markerad och fältet **Radtyp** på projektjournalraden är tomt, skapas inga projektplaneringsrader när du bokför projektjournalrader. Mer information finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).

1. Välj ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projektinställningar** och välj sedan relaterad länk.
2. Markera eller avmarkera kryssrutan **Använd förbrukningslänk**.

> [!NOTE]  
>   Du kan skapa en annan inställning av **Använd förbrukningslänken** på de individuella arbetskorten. I så fall åsidosätter inställningen för det projektet den allmänna standardinställningen som beskrivs ovan.

## <a name="to-set-up-prices-for-job-resources"></a>Så här anger du priser för projektresurser
Du kan lägga upp särskilda resurspriser för ett projekt. Du använder fönstret **Resurspriser för projekt** om du vill göra detta.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projekt** och välj sedan relaterad länk.  
2. Välj relevant projekt och välj sedan åtgärden **Resurs**.
3. I fönstret **Resurspriser för projekt** fyller du i fälten efter behov.

Den valfria informationen i fälten **Projektaktivitetsnr**, **Arbetstyp**, **Valutakod**, **Radrabatt %** och **Styckkostnadsfaktor** kommer att användas i projektplaneringsrader och förbrukningsjournaler när den här resursen anges och läggs till i projektet.  

Värdet i fältet **Enhetspris** för resursen kommer att användas i projektjournalerna och projektets planeringsrader när den här resursen, en resurs tilldelad till resursgruppen eller valfri resurs anges.  

> [!NOTE]  
>   Det här priset kommer alltid att åsidosätta eventuella priser som har angetts i det befintliga fönstret **Resurspris/Resursgruppriser**.

## <a name="to-set-up-prices-for-job-items"></a>Så här anger du priser för projektartiklar
Du kan lägga upp särskilda artikelpriser för ett projekt. Använd fönstret **Artikelpriser** för projekt om du vill göra detta.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projekt** och välj sedan relaterad länk.  
2. Välj relevant projekt och välj sedan åtgärden **Artikel**.
3. I fönstret **Artikelpriser för projekt** fyller du i fälten efter behov.

Den valfria informationen i fälten **Projektaktivitetsnr**, **Valutakod** och **Radrabatt %** kommer att användas i projektjournalraderna och projektjournalerna när den här artikeln anges eller läggs till i projektet.  

Värdet i fältet **Enhetspris** för artikeln kommer att användas i projektplaneringsraderna och projektjournalerna när den här artikeln anges.  

> [!NOTE]  
>   Det här priset kommer alltid att åsidosätta det vanliga kundpriset (bästa pris-mekanismen) för artiklar. Du bör inte skapa några artikelpriser för projektet om du vill använda mekanismerna för vanliga kundpriser.

## <a name="to-set-up-prices-for-job-general-ledger-accounts"></a>Så här lägger du upp priser för redovisningskonton för projekt
Du kan lägga upp specifika priser för redovisningskostnader för ett projekt. Du använder fönstret **Redov.kontopriser för projekt** för att göra detta.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projekt** och välj sedan relaterad länk.  
2. Välj relevant projekt och välj sedan åtgärden **Redovisningskonto**.  
3. I fönstret **Redov.kontopriser för projekt** fyller du i fälten efter behov.

Den valfria informationen i fälten **Projektaktivitetsnr**, **Valutakod**, **Radrabatt %**, **Styckkostnadsfaktor** och **Enhetskostnad** kommer att användas i projektplaneringsrader och projektjournaler när det här redovisningskontot anges och läggs till ett projekt.  

Värdet i fältet **Enhetspris** för projektkostnaden för redovisningskontot kommer att användas i projekplaneringstjournalerna och projektjournalerna när detta redovisningskonto anges.

## <a name="to-set-up-job-posting-groups"></a>Så här lägger du upp projektbokföringsmallar
En aspekt av att planera projektet är att bestämma vilka bokföringskonton som ska användas för projektvärdering. Om du vill kunna bokföra projekt måste du lägga upp bokföringskonton för varje projektbokföringsmall. En bokföringsmall representerar en länk mellan projektet och hur det ska hanteras i redovisningen. När du skapar ett projekt anger du en bokföringsmall och, som standard, kopplar du varje aktivitet som du skapar för projektet till den här bokföringsmallen. Men medan du skapar aktiviteter kan du välja att åsidosätta standarden och välja en annan, mer lämplig, bokföringsmall.  

> [!NOTE]  
>   Nödvändiga konton i kontoplanen måste registreras innan du registrerar bokföringsmallar. Mer information finns i [Ställa in eller ändra kontoplanen](finance-setup-chart-accounts.md).  

1. Välj ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projektinställningar** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny** och fyll sedan i kontofälten enligt instruktionerna i följande tabell.  

| Kontofält | Beskrivning |
| --- | --- |
| **Kod** |En kod för bokföringsmallen. Du kan ange upp till 10 tecken inklusive blanksteg. |
| **Konto för PIA-kostnader** |PIA-kontot för den beräknade kostnaden för projektets PIA, vilket är ett konto för anläggningstillgångar i balansräkningen. |
| **Konto för upplupna PIA-kostnader** |Ett konto för kostnadsvärde eller kostnadsförsäljningsmetod för beräkningen av PIA, vilket är ett skuldkonto för upplupna kostnader i balansräkningen. Bokföring kommer att ske på detta konto när det krävs att förbrukningskostnader som har bokförts på resultatkontot ökas i PIA-justeringsprocessen. |
| **Konto för kopplade projektkostnader** |Ett balanskonto för PIA-kostnadskontot, som är ett motkonto för ett negativt kostnadskonto. |
| **Konto för kopplade artikelkostnader** |Ett balanskonto för PIA-kostnadskontot, som är ett motkonto för ett negativt kostnadskonto. |
| **Konto för kopplade resurskostnader** |Ett balanskonto för PIA-kostnadskontot, som är ett motkonto för ett negativt kostnadskonto. |
| **Konto för kopplade kostnader** |Ett balanskonto för PIA-kostnadskontot, som är ett motkonto för ett negativt kostnadskonto. |
| **Konto för projektkostnadsjustering** |Balanskontot för kontot för upplupna PIA-kostnader, som är ett kostnadskonto. |
| **Konto för redovisningskostnader (budget)** |Försäljningskontot som ska användas för redovisningskostnader i projektaktiviteter med den här bokföringsmallen. Om fältet lämnas tomt kommer det redovisningskonto som har angetts på projektplaneringsraden att användas. |
| **Konto för upplupen PIA-försäljning** |PIA-kontot för det beräknade försäljningsvärdet för PIA, vilket är ett konto för upplupen intäkt i balansräkningen. Bokföring kommer att ske på detta konto när den bokförda intäkten måste ökas i PIA-justeringsprocessen. |
| **Konto för fakturerad PIA-försäljning** |Kontot för värdet för fakturerad PIA-försäljning som inte kan bokföras. Det är ett konto för förutbetald intäkt i balansräkningen. |
| **Konto för kopplad projektförsäljning** |Balanskontot för kontot för fakturerad PIA-försäljning, vilket är ett motkonto för inkomst. |
| **Konto för projektförsäljningsjustering** |Balanskontot för PIA-projektförsäljningskontot, som är ett inkomstkonto. |
| **Konto för bokförda kostnader** |Det kostnadskonto som innehåller bokförda kostnader för projektet. Kontot är vanligtvis ett debetkonto för kostnader. |
| **Konto för bokförd försäljning** |Inkomstkontot som innehåller den bokförda inkomsten för projektet. Kontot är vanligtvis ett kreditkonto för inkomst. |

## <a name="see-also"></a>Se även
[Ange projekthantering](projects-setup-projects.md)  
[Hantera projekt](projects-manage-projects.md)  
[Ekonomi](finance.md)  
[Inköp](purchasing-manage-purchasing.md)         
[Försäljning](sales-manage-sales.md)      
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

