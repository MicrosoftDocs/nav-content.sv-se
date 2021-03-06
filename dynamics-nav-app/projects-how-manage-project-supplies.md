---
title: "Köpa artiklar eller tjänster för ett projekt och hantera leveranser"
description: "Beskriver hur du hanterar försörjning och inköp av material och tjänster för projekt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3405af0c06df0fb04c528cf114d4ef6326f7c0a9
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-job-supplies"></a>Så här hanterar du projektleveranser
Att hantera projektleveranser av artiklar, tjänster och utgifter är en viktig del och aspekt av allt projektgenomförande. Du kan använda lagerantal eller göra projektspecifika inköp med hjälp av inköpsorder eller inköpsfakturor. Ett servicejobb för en dator kan till exempel kräva en ny hårddisk. Du skapar då en inköpsfaktura för att köpa en ny hårddisk och registrerar det i projektet.

Om inköpsprocessen inte kräver att den fysiska transaktionen registreras separat kan ett inköp registreras endast i en inköpsfaktura eller i fönstret **Projektredovisningsjournal**. Mer information finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>Köpa artiklar eller tjänster till ett projekt
Efterföljande procedur visar hur du använder en inköpsfaktura för att köpa produkter till ett projekt. Samma steg gäller när du använder en inköpsorder.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inköpsfakturor** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny** och fyll i fälten efter behov. Mer information finns i [Så här registrerar du inköp](purchasing-how-record-purchases.md).
3. I fälten **Projektnr.** och **Projektaktivitetsnr.** väljer du informationen för det projekt som du vill köpa artiklar eller tjänster för. Använd funktionen **Välj kolumner** om fältet inte visas. Mer information finns i [Användaranpassning](ui-user-personalization.md).

    Värdet som du väljer i fältet **Projektradtyp** definierar om en planeringsrad skapas när du bokför artikelförbrukningen. Om fältet innehåller **Fakturerbart** skapas projektplaneringsrader som är klara att faktureras till kunden. Mer information finns i [Så här skapar du fakturaprojekt](projects-how-invoice-jobs.md).
4. Välj åtgärden **Bokföra**.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>Visa värdet på inköp till ett projekt
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projekt** och välj sedan relaterad länk.
2. Öppna ett relevant projektkort.

    På snabbfliken **Uppgifter** visar fältet **Utestående order** det totala utestående beloppet, i lokal valuta, för lagerartiklar och tjänster för inköpsdokument för projektaktivitetsraden.  

    Fältet **Inlevererat bel. ej faktrd** visar värdet för artiklarna som har levererats på inköpsdokument, men ännu inte har fakturerats.  
3. Välj något av fälten för att öppna fönstret **Inköpsrader** där du kan granska information om relaterade inköpsdokumentrader, bland annat vilka artiklar eller tjänster som har inlevererats.

## <a name="to-post-a-job-related-expense"></a>Så här bokför du en projektrelaterad utgift
Om du ådrar dig extraordinära eller engångsutgifter för projekt kan du använda fönstret **Projektredovisningsjournal** för att bokföra dem direkt till det relevanta projektkontot.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Projektredovisningsjournaler** och välj sedan relaterad länk.  
2. Skapa en ny rad och registrera information om utgiften, bland annat information i fälten **Projektnr** och **Projektaktivitetsnr**.  
3. När journalen är slutförd väljer du åtgärden **Bokföra**.

## <a name="see-also"></a>Se även
[Projekthantering](projects-manage-projects.md)  
[Ekonomi](finance.md)  
[Inköp](purchasing-manage-purchasing.md)         
[Försäljning](sales-manage-sales.md)      
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

