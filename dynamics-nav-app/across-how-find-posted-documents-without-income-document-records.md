---
title: "Sök efter dokument utan bilagor"
Description: "Du kan söka efter redovisningstransaktioner för bokförda inköps- och försäljningsdokument som inte har inkommande elektroniska dokument, till exempel importerade fakturor."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 515026b4da842afeda1759f50313dc26bcfd3350
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>Så här söker du efter bokförda dokument utan inkommande dokumentposter
Från fönstren **Kontoplan** och **Redovisningstransaktioner** kan du använda en sökfunktion för att hitta redovisningsposter för bokförda inköps- och försäljningsdokument som inte har inkommande dokumentposter och sedan länka dem till befintliga poster eller skapa nya centralt med bifogade dokumentfiler.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>Söka efter bokförda dokument utan inkommande dokumentposter
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kontoplan** och välj sedan relaterad länk.
2. Välj en rad för ett redovisningskonto för vilka redovisningstransaktioner du vill se bokförda inköps- och försäljningsdokument utan inkommande dokumentpost och välj sedan **Bokförda dokument utan inkommande dokument**.
3. Välj alternativt åtgärden **Transaktioner**.
4. I fönstret **Redovisningstransaktioner** väljer du åtgärden **Bokförda dokument utan inkommande dokument**.

Fönstret **Dokförda dokument utan inkommande dokument** öppnas med visning av bokförda inköps- och försäljningsdokument utan inkommande dokumentposter som representeras av redovisningstransaktioner på det redovisningskonto som du öppnade fönstret för. Fönstret kan innehålla högst 1000 rader. Som standard innehåller fältet **Datumfilter** därför ett filter som begränsar raderna till poster med bokföringsdatum från början av bokföringsperioden till arbetsdatumet.

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a>Koppla hittade dokument till befintliga inkommande dokumentposter
1. I fönstret **Bokförda dokument utan inkommande dokument** väljer du raden för ett bokfört dokument som du vill koppla till en befintlig inkommande dokumentpost och väljer sedan åtgärden **Välj inkommande dokument**.
2. I fönstret **Inkommande dokument** väljer du den inkommande dokumentpost som du vill koppla till det hittade bokförda dokumentet och klickar sedan på knappen **OK**.
3. Nu är den valda inkommande dokumentposten kopplad till det bokförda dokumentet i fönstret **Bokförda dokument utan inkommande dokument**, som du kan se i faktaboxen **Inkommande dokumentfiler**.

Om en relevant inkommande dokumentpost inte finns i fönstret **Inkommande dokument** kan du skapa den. Mer information finns i [Så här skapar du inkommande dokumentposter](across-how-create-income-document-records.md).

## <a name="see-also"></a>Se även
[Bearbeta inkommande dokument](across-process-income-documents.md)  
[Inkommande dokument](across-income-documents.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

