---
title: "Så här skapar du en färglagd indikator på stack-ikoner"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 04272431b01c0ab398618d9878b90d73e6324abe
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

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

|Alternativ|Färg|
|------|-----|
|**Ingen**|Ingen färg (samma färg som stack-ikonen|
|**Positiv**|Grön|
|**Negativ**|Röd|
|**Tvetydigt**|Gul|
|**Underordnad**|Grått|

## <a name="see-also"></a>Se även
[Arbeta med Dynamics NAV](ui-work-product.md)


