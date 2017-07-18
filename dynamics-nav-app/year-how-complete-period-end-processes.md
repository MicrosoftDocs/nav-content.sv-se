---
title: Avsluta perioder
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a>Avsluta perioder
Programmet tvingar dig inte att avsluta perioder, men det finns många periodslutsaktiviteter (månadsslut) som du kan utföra om du vill. Det här avsnittet innehåller en översikt över dessa processer och aktiviteter, som kan vara obligatoriska eller inte i ditt företag.

## <a name="general-ledger"></a>Redovisning
* Specificera intervall för bokföringsdatum som gäller hela systemet och är användarspecifik.

    Detta anger datumen som bokföring kan göras i. Beroende på vilka behov som finns i ditt företag kanske du vill begränsa användares intervall för bokföringsdatum i början av periodslutsprocessen eller vid senare tillfälle mot slutet av perioden. Mer information finns [Så här anger du bokföringsperioder](finance-setup-how-specify-posting-periods.md).
* Gör alla nödvändiga redovisningsjusteringar.
* Uppdatera och bokför återkommande journaler.
<!--* Process Consolidations-->
* Kör kontouppställningar enligt följande:
  1. Öppna fönstret **Kontouppställning** och klicka på **Skriv ut**.
  2. Fyll i förfrågan om **Kontouppställning** och klicka på **Skriv ut**.

## <a name="sales--receivables"></a>Försäljning & kundreskontra
* Bokför alla försäljningsorder, fakturor, kreditnotor och returorder
* Bokför alla inbetalningsjournaler.
* Uppdatera och bokför återkommande journaler som hör till försäljning- och kundreskontra
* Stäm av kundreskontra i redovisningen
* Kör batch-jobbet **Ta bort fakturerade förs.order**

## <a name="purchases--payables"></a>Inköp & Leverantörsreskontra
* Bokför alla inköps order, fakturor, kreditnotor och returorder
* Bokför alla betalningsjournaler.
* Uppdatera och bokför återkommande journaler som relaterar till inköps- och leverantörsreskontra.
* Kör rapporten **Lev.skulder - ålder** och stäm av leverantörsskulder i redovisningen.
* Kör batch-jobbet **Ta bort fakturerade inköpsorder**

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a>Beräkna och bearbeta Omsättningsskatt
*  Fyll i skattmeddelanden.

## <a name="see-also"></a>Se även
[Avsluta år och perioder](year-close-years-periods.md)  
[Avsluta böcker](year-close-books.md)

