---
title: "Flera räntesatser – översikt"
description: "För varje räntevillkorskod kan du ange flera räntesatser så att du kan beräkna dröjsmålsränta med flera räntesatser för en särskild period."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: e2c207abbd53aa0e05a84ad44be2baea5d1eb4f0
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="multiple-interest-rates-overview"></a>Flera räntesatser – översikt
För varje räntevillkorskod kan du ange flera räntesatser så att du kan beräkna dröjsmålsränta med flera räntesatser för en särskild period. Detta är praktiskt om du debiterar olika räntor på försenade betalningar. Ränteberäkningen görs på samma sätt för alla dröjsmålsräntor, men räntan kan variera under en viss period.  

## <a name="creating-finance-charges"></a>Skapa dröjsmålsräntor  
När du skapar en räntefaktura innehåller raderna dröjsmålsräntor med olika räntesatser för varje tidsperiod. För varje räntevillkor kan du ange en beskrivning och du kan definiera en beskrivning som används när flera räntesatser används.  

För att kunna använda flera räntesatser måste du först definiera en räntevillkorskod, och du måste sedan lägga till flera räntesatsrader i villkoren. Mer information finns i [Så här ställer du in flera räntesatser](how-to-set-up-multiple-interest-rates.md).  

Om det inte finns flera räntesatser använder [!INCLUDE[navnow](../../includes/navnow_md.md)] den räntesats och den period som definieras i fönstret **Räntevillkor** för hela beräkningsperioden.  

## <a name="delayed-payments"></a>Försenade betalningar  
Flera räntesatser används för olika perioder för försenade betalningar i handelstransaktioner. En myndighet anger till exempel den högsta räntan som kan tas ut för en kund. Den räntan kan ändras två gånger per år, den 1 januari och den 1 juli. Räntesatsen mellan företag avtalas av parterna och det finns ingen gräns för den kundgruppen. Den räntesatsen ligger vanligtvis 4 procent över den normala bankräntan.  

## <a name="see-also"></a>Se även  
 [Så här ställer du in flera räntesatser](how-to-set-up-multiple-interest-rates.md)   
 [Så här kräver du in utestående saldon](../../receivables-collect-outstanding-balances.md)

