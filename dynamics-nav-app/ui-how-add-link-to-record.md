---
title: "Så här: Länka från poster till extern information eller program"
description: "Koppla en hyperlänk till ett dokument eller en webbplats till en viss post, till exempel en kund eller ett dokument."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 903d8710a8c77348e1366d9a9a29b75395887198
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="adding-links-to-websites-documents-or-programs-on-records"></a>Lägga till länkar till webbplatser, dokument och program på poster
För en viss post, till exempel kund, dokument eller försäljningsorder, kan du lägga till en länk till ett externt dokument, webbplatser eller program. Eller så kanske du vill ha en länk som öppnar ett nytt, tomt e-postmeddelande till en viss mottagare när du klickar på den. Kortsidan för vissa kort, till exempel kund- och leverantörskorten, innehåller fältet **Hemsida** där en Internettadress (URL) kan anges. Om du vill infoga andra länkar kan du använda den metod som beskrivs i den här artikeln.

Ett annat exempel är när du får utskrivna fakturor från leverantörer. Du kan skanna in dem och spara dem som PDF-filer på en SharePoint-webbplats. Därefter kan du skapa en länk från en inköpsfaktura i [!INCLUDE[d365fin_md](includes/d365fin_md.md)] till motsvarande faktura på SharePoint. Du kan också skapa en länk från ett artikelkort till motsvarande sida i leverantörens onlinekatalog.
  
## <a name="to-add-a-link-on-a-record"></a>Så här lägger du till en länk på en post:   
  
1.  Öppna posten som du vill bifoga länken till, till exempel ett kundkort eller en försäljningsorder. Om du vill bifoga länken till en specifik rad, till exempel till en journalrad, markerar du raden.  
  
2.  Välj åtgärden **länkar** för att öppna fönstret **länkar** som visar de aktuella länkarna som du lägger till posten.

3. För att lägga till en ny länk väljer du **+ny**. 
  
4.  I fältet **länkar** anger du

    -   Om du vill länka till en fil på datorn eller i nätverket, anger du den fullständiga sökvägen och filnamnet som **C:My Documentsinvoice1.doc**.
    -   Länka till en webbplats genom att ange Internet-adressen (URL) som **www.microsoft.com**. 
    -   Länka till en webbplats genom att ange Internet-adressen (URL) som **www.microsoft.com**. 
    -   Länka till ett program genom att ange en sträng för att öppna programmet. Om du vill starta OneNote med en viss sida skriver du **onenote:///C:My Documentstest.one**. Eller om du vill öppna Outlook med ett nytt, tomt e-postmeddelande till ett visst alias skriver du **mailto:testalias**.  
  
5.  Ange information om länken i fältet **Beskrivning**.  
  
6.  Klicka på **Spara**.  
  
## <a name="to-delete-a-link-from-a-record"></a>Så här tar du bort en länk från en post:  
  
För att ta bort en länk kan du i fönstret **länkar** du ange **...** och **Ta bort**.

Om du tar bort en enstaka post (till exempel en försäljningsorderrad, en försäljningsorder eller ett kundkort) tas postens alla bifogade länkar bort. Om användaren däremot tar bort poster med hjälp av ett batch-jobb **Ta bort fakturerade förs.order** sparas länkarna i databasen. Kör kodmodulen **Ta bort tomma postlänkar** för att ta bort länkarna från databasen. För att öppna denna sida väljer du ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rappor"), ange **Ta bort tomma postlänkar**, och väljer sedan relaterad länk.   
  
<!-- ### To run delete orphaned record links  
  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Deletion**, and then choose the related link.  
  
2.  On the **Data Deletion** page, choose **Tasks**, and then choose **Delete Orphaned Record Links**.  -->
  
## <a name="see-also"></a>Se även  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
