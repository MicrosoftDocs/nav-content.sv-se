---
title: "Ange färgindikatorer för att anpassa visuella signaler om en stack-ikons aktivitet"
description: "Skapa en färgindikator på en stack-ikon för att ge en anpassad visuell signal på stack-ikonens aktivitet."
documentationcenter: 
author: SusanneWindfeldPedersen
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalize, customize
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6a2b7deb2f256e3b6bf52f1b0a66fe47d049c452
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a>Så här skapar du en färglagd indikator på stack-ikoner
Du kan skapa stack-ikoner som visas på **Startsidan** för att inkludera en indikator som ändrar färg baserat på datavärdena i stack-ikonerna.

Indikatorn visas som en kulört stapel längs den övre kanten på stack-ikon-panelen. Den ger en visuell signal över statusen för stack-ikonaktivitet, som kan ange gynnsamma eller ofördelaktiga förhållanden för att meddela användaren att vidta åtgärd. Om t.ex. en stack-ikon visar pågående försäljningsfakturor kan du ställa in indikatorn för att visa grönt (positivt) när totala antalet pågående försäljningsfakturor är under 10, och röd (negativt) när antalet är större än 20.

Från fönstret **Inställning av stack-ikon** ställer du in indikatorer för alla stack-ikoner som är tillgängliga i företagsdatabasen.

För att ställa in indikatorn, anger du upp till två tröskelvärden som definierar tre intervall av datavärden (låg, medel och hög) som du kan koppla en annan färg (eller stil).

## <a name="to-set-up-colored-indicators-on-cues"></a>Så här ställer du in kulörta indikatorer på stack-ikoner
1. Under **Aktiviteter** på din **Startsida** väljer du **Inställning av stack-ikon**.  
   Fönstret **Inställning av stack-ikon** visas. I fönstret anges indikatorerna som för närvarande är inställda på stack-ikoner.
2. För att ändra en indikator redigerar du fälten och för att ändra till exempel,värdena för de olika trösklarna.  

Efterföljande tabeller listar de bakgrundsfärger som motsvarar alternativen för fälten **Lågt intervallformat**, **Medelintervallformat** och **Högt intervallformat**.

| Alternativ | Färg |
| --- | --- |
| **Ingen** |Ingen färg (samma färg som stack-ikonen)|
| **Positiv** |Grön |
| **Negativ** |Röd |
| **Tvetydigt** |Gul |
| **Underordnad** |Grått |

## <a name="see-also"></a>Se även
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

