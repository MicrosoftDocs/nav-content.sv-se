---
title: "Så här fakturerar du projekt"
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
ms.openlocfilehash: c0dcce83dfba30af38f33a6bf814b15862d5fc19
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-jobs"></a>Så här fakturerar du projekt
Under projektet kan projektkostnade från resursförbrukning, material och projektrelaterade inköp uppstå. Dessa transaktioner bokförs i projektjournalen. Det är viktigt att alla kostnader registreras i projektjournalen innan kunden faktureras.

Du kan fakturera hela projektet från fönstret **Projektaktivitetsrader** eller fakturera endast valda fakturerbara rader i fönstret **Planeringsrader**. Faktureringen kan göras när projektet har slutförts eller allt eftersom projektet fortlöper enligt ett faktureringsschema.

**OBS**! Om du väljer **Fakturerbart** i fältet **Projektradtyp** på inköpsdokumentet för projektrelaterade inköp, skapas projektplaneringsrader som är klara att faktureras till kunden. Mer information finns i [Så här hanterar du projektleveranser](projects-how-manage-project-supplies.md).

## <a name="to-create-and-post-a-job-sales-invoice"></a>Så här skapar och bokför du en försäljningsfaktura för ett projekt  
Du kan skapa en faktura för ett projekt för en eller flera projektaktiviteter för en kund, antingen när det arbete som ska faktureras har slutförts eller när datumet för fakturering, som är baserat på ett faktureringsschema, har infallit.

Från fönstret **Projekt** kan du fakturera en kund genom att välja projekt och sedan välja åtgärden **Skapa jobbförsäljningsfaktura**. Efterföljande procedur visar hur du kan använda ett batch-jobb för att fakturera flera projekt.  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt - Skapa förs.faktura** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. Ange filter om du vill begränsa de projekt som ska bearbetas av batch-jobbet.
3. Klicka på **OK** för att skapa fakturorna.  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a>Så här skapar du flera projektförsäljningsfakturor från projektplaneringsrader  
Du kan skapa en faktura från projektplaneringsrader och då ange antal av artikeln, resursen eller redovisningskontot som du vill fakturera.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.
2. Öppna ett relevant projekt.
3. Markera ett projekt där fältet **Typ av projektaktivitet** innehåller **Bokföring** och klicka sedan på åtgärden **Projektplaneringsrader**.  
4. Gå till fältet **Antal att överföra till faktura** på en projektplaneringsrad och ange antal av artikeln, resursen, typen av redovisningskonto som du vill fakturera.  
5. Välj åtgärden **Skapa försäljningsfaktura**.
6. I fönstret **Projekt - Skapa förs.faktura** anger du bokföringsdatum och om du vill skapa en ny faktura eller koppla denna faktura till en befintlig.
7. Välj **OK**.

    På projektplaneringsradens fält **Antal överfört till faktura** kan du se antalet.

8. I fönstret **Projektplaneringsrader** väljer du åtgärden **Försäljningsfakturor/kreditnotor**.

    Fönstret **Försäljningsfaktura** öppnas och visar antalet som du har överfört till fakturan.  
9. Gör ytterligare ändringar och välj sedan åtgärden **Bokför**.

**OBS**! Ovanstående förfarande är liknande för att skapa, granska och publicera en projektrelaterad försäljningskreditnota.

## <a name="to-calculate-and-post-job-completion-entries"></a>Så här kan du beräkna och bokföra slutförda projekt  
När du har slutfört alla aktiviteter i ett projekt, bland annat bokföringen och faktureringen av förbrukning, måste du uppdatera projektet så att projektet får **Statusen** **Slutförd**. Sedan måste du återföra alla PIA som har bokförs i redovisningen.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.  
2. Välj ett öppet projekt och välj sedan åtgärden **Redigera**.
3. Markera **Slutförd** i fältet **Status** .
4. Följ hjälpstegen steg för att beräkna och bokföra PIA. Följ alternativt steg 5 och 6 för att göra det manuellt.  
5. Välj åtgärden **Beräkna PIA**.
6. I fönstret **Projekt - Beräkna PIA** fyller du i fälten efter behov.  

     De PIA-transaktioner för jobbet som skapas när du kör batch-jobbet kommer nu att ha fältet **Slutfört projekt** markerat för att visa att de är slutförda.  

7. Välj åtgärden **Projekt - Bokför PIA i redovisning**.
8. I fönstret **Projekt - Bokför PIA i redovisning** fyller du i fälten efter behov.  

     De PIA-transaktioner för jobbet som skapas när du kör batch-jobbet kommer nu att ha fältet **Slutfört projekt** markerat för att visa att de är slutförda.

## <a name="see-also"></a>Se även
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)  
