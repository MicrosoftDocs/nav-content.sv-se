---
title: "Så här hanterar du projektleveranser"
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
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a>Så här hanterar du projektleveranser
Att hantera projektleveranser av artiklar, tjänster och utgifter är en viktig del och aspekt av allt projektgenomförande. Du kan använda lagerantal eller göra projektspecifika inköp med hjälp av inköpsorder eller inköpsfakturor. Ett servicejobb för en dator kan till exempel kräva en ny hårddisk. Du skapar då en inköpsfaktura för att köpa en ny hårddisk och registrerar det i projektet.

Om inköpsprocessen inte kräver att den fysiska transaktionen registreras separat kan ett inköp registreras endast i en inköpsfaktura eller i fönstret **Projektredovisningsjournal**. Mer information finns i [Så här registrerar du förbrukning för projekt](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>Köpa artiklar eller tjänster till ett projekt
Efterföljande procedur visar hur du använder en inköpsfaktura för att köpa produkter till ett projekt. Samma steg gäller när du använder en inköpsorder.  

1. Välj ikonen **söka efter sida eller rapport** i det övre högra hörnet, gå till **Inköpsfakturor** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny** och fyll i fälten efter behov. Mer information finns i [Så här registrerar du inköp](purchasing-how-record-purchases.md).
3. I fälten **Projektnr**. och **Projektaktivitetsnr** väljer du informationen för det projekt som du vill köpa artiklar eller tjänster för.  

    Värdet som du väljer i fältet **Projektradtyp** definierar om en planeringsrad skapas när du bokför artikelförbrukningen. Om fältet innehåller **Fakturerbart** skapas projektplaneringsrader som är klara att faktureras till kunden. Mer information finns i [Så här skapar du fakturaprojekt](projects-how-invoice-jobs.md).

4. Välj åtgärden **Bokföra**.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>Visa värdet på inköp till ett projekt  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.
2. Öppna ett relevant projektkort.

    På snabbfliken **Uppgifter** visar fältet **Utestående order** det totala utestående beloppet, i lokal valuta, för lagerartiklar och tjänster för inköpsdokument för projektaktivitetsraden.  

    Fältet **Inlevererat bel. ej faktrd** visar värdet för artiklarna som har levererats på inköpsdokument, men ännu inte har fakturerats.  

3. Välj något av fälten för att öppna fönstret **Inköpsrader** där du kan granska information om relaterade inköpsdokumentrader, bland annat vilka artiklar eller tjänster som har inlevererats.

## <a name="to-post-a-job-related-expense"></a>Så här bokför du en projektrelaterad utgift  
Om du ådrar dig extraordinära eller engångsutgifter för projekt kan du använda fönstret **Projektredovisningsjournal** för att bokföra dem direkt till det relevanta projektkontot.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projektredovisningsjournaler** och välj sedan relaterad länk.  
2. Skapa en ny rad och registrera information om utgiften, bland annat information i fälten **Projektnr**. och **Projektaktivitetsnr**.  
3. När journalen är slutförd väljer du åtgärden **Bokföra**.


## <a name="see-also"></a>Se även
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)  

