---
title: "Skapa försäkring för anläggningstillgångar"
description: "Om du vill hantera täckning av försäkring för anläggningstillgångar måste du ange ett försäkringskort och allmän försäkringsinformation."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: policy, coverage
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0c0b553adee7df5979352999c60549b280501926
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-fixed-asset-insurance"></a>Så här skapar du försäkring för anläggningstillgångar
Om du vill hantera täckning av försäkring för anläggningstillgångar måste du först ange en viss allmän försäkringsinformation och ett försäkringskort per brev.

## <a name="to-set-up-general-insurance-information"></a>Så här anger du allmän försäkringsinformation
Om du vill använda den här funktionen i [!INCLUDE[d365fin](includes/d365fin_md.md)], måste du ange viss allmän information.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inställningar i anl.** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-set-up-insurance-types"></a>Så här skapar du försäkringstyper
Du kan gruppera dina försäkringsbrev i kategorier, t.ex. stöldförsäkring och brandförsäkring. Försäkringstyperna används på försäkringskortet.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäkringstyp** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs.

## <a name="to-set-up-insurance-cards"></a>Så här skapar du försäkringskort
Du kan lagra information om varje försäkringsbrev på försäkringskortet.  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäkring** och välj sedan relaterad länk.  
2. I fönstret **Försäkring** väljer du åtgärden **Ny** åtgärder för att skapa ett nytt försäkringskort.  
3. Fyll i fälten om det behövs.

## <a name="to-set-up-insurance-journal-templates"></a>Så här skapar du journalmallar för försäkringar
[!INCLUDE[d365fin](includes/d365fin_md.md)] skapar automatiskt en försäkringsjournalmall första gången du öppnar fönstret **Försäkringsjournal**. Du kan dessutom skapa ytterligare mallar. Mer information finns i [Arbeta med Redovisningsjournaler](ui-work-general-journals.md).  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäkringsjournalmallar** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs.

## <a name="to-set-up-insurance-journal-batches"></a>Så här skapar du försäkringsjournaler
Du kan skapa journaler i en försäkringsjournalmall. Värdena i journalen används som standardvärden om du inte fyller i fälten på journalraderna. Mer information finns i [Arbeta medSkapa redovisningsjournaler](ui-work-general-journals.md)  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäkringsjournalmallar** och välj sedan relaterad länk.  
2. Välj en försäkringsjournalmall och välj sedan åtgärden **Journaler**.
3. I fönstret **Försäkringsjournaler** fyller du i fälten efter behov.

> [!NOTE]  
>   Siffror fyller en särskild funktion i journalnamnen. Om ett journalmallsnamn eller ett journalnamn innehåller ett nummer, får namnet efterföljande nummer automatiskt när journalen bokförs. Om till exempel HH1 anges i fältet **Namn** ändras journalnamnet till HH2 när journalen som heter HH1 har bokförts.

## <a name="see-also"></a>Se även
[Ställa in anläggningstillgångar](fa-setup.md)  
[Anläggningstillgångar](fa-manage.md)  
[Ekonomi](finance.md)  
[Välkommen till [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

