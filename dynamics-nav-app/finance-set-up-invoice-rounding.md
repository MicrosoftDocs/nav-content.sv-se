---
title: "Ställa in överavrundning"
description: "Du kan avrunda fakturabelopp när du skapar fakturor. Dessutom kan lokala regler eller lokal praxis kräva att fakturan rundas av på ett visst sätt, till exempel till ett belopp som är delbart med 0,05."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d52f27fc7733a485a329884d15c58921caf4719f
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="set-up-invoice-rounding"></a>Ställa in överavrundning
Om du måste avrunda fakturabelopp när du skapar fakturor, kan du använda funktionen för automatisk avrundning. När en faktura rundas av infogas en extra rad med avrundningsbeloppet och bokförs tillsammans med övriga fakturarader.

> [!NOTE]  
>  Lokala regler eller lokal praxis kanske kräver att fakturan rundas av på ett visst sätt, till exempel till ett belopp som är delbart med 0,05.  
  
För att kunna använda den automatiska fakturaavrundningen måste du:  
  
* ange vilka redovisningskonton som differenserna ska bokföras på.  
* ange regler för fakturaavrundning i lokal valuta och i utländsk valuta.  
* aktivera funktionen.  
  
> [!NOTE]  
>  Förutom fakturaavrundningsfunktionen kan belopp på fakturor rundas av med funktionerna A-pris avrundning och Belopp avrundning.  
 
## <a name="how-to-set-up-general-ledger-accounts-for-invoice-rounding-differences"></a>Så här: Skapa redovisningskonton för avrundningsdifferenser av fakturor
Om du vill använda programmets funktion för automatisk avrundning av fakturabelopp måste du först upprätta redovisningskonton eller konton där avrundningsskillnaderna bokförs. Innan du kan göra detta måste du definiera produktbokföringsmallar för moms. Mer information finns i [Ange moms](finance-setup-vat.md).  
  
### <a name="to-set-up-general-ledger-accounts-for-invoice-rounding-differences"></a>Så här skapar du redovisningskonton för avrundningsdifferenser av fakturor  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kontoplan** och välj sedan relaterad länk.  
2. På sidan **Kontoplan** ställer du in kontot och kallar det för **Faktura avrundning** eller något liknande. [!INCLUDE[d365fin](includes/d365fin_md.md)] använder kontonamnet som text för de fakturor som avrundas.  
3. Beroende på om du använder moms eller omsättningsskatt väljer du i fälten **Omsättn. skatt produktbokföringsmall** eller **Moms produktbokföringsmal** och väljer en bokföringsmall för avrundade belopp. Du vill kanske skapa en ny gruppkod som kan användas för fakturaavrundning.
4. Lämna fälten **Typ av bokföring**, och antingen **Omsättn. skatt rörelsebokföringsmall** eller **Moms rörelsebokföringsmall** tomma. <!-- Why do we say to leave these blank, when there are a lot of other fields we also leave blank but don't mention? -->  
  
Nu kan du koppla fakturaavrundningskontot till bokföringsmallar på sidan **Leverantörsbokföringsmallar**.  <!-- Why only the vendor posting groups? -->

## <a name="how-to-set-up-rounding-for-foreign-and-local-currencies"></a>Så här: Ange avrundningsregler för utländska valutor
Innan du kan använda den automatiska fakturaavrundningsfunktionenmåste du ställa in avrundningsregler för utländsk och lokal valuta.

### <a name="to-set-up-rounding-for-foreign-currencies"></a>Så här anger du avrundningsregler för utländska valutor:  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Valutor** och välj sedan relaterad länk.  
2. På sidan **valutor** väljer du valutan för att öppna **valutakort**, och fyller sedan i fälten **Belopp avrundning**, **A-pris avrundning**, **Faktura avrundning** och **Avrundningstyp**.
  
### <a name="to-set-up-rounding-for-your-local-currency"></a>Så här anger du avrundningsregler för den lokala valutan:
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Redovisningsinställningar** och välj sedan relaterad länk.  
2. På sidan **Redovisningsinställningar** på snabbfliken **Allmänt** fyller du i fälten **Faktura avrundning** och **Avrundningstyp**.  

## <a name="how-to-activate-the-invoice-rounding-function"></a>Så här aktiverar du funktionen Avrunda fakturabelopp:  
För att se till att försäljnings- och inköpsfakturor avrundas automatiskt aktiverar du funktionen Avrunda fakturabelopp. Du kan aktivera fakturaavrundningen separat för försäljnings- och inköpsfakturor.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningsinställningar** eller **Inköpsinställningar** och väljer sedan relaterad länk.  
2. På snabbfliken **Allmänt**, välj kryssrutan **Öresutjämning**.  
  
## <a name="see-also"></a>Se även  
[Så här fakturerar du försäljning](sales-how-invoice-sales.md)  
[Så här registrerar du inköp](purchasing-how-record-purchases.md)
