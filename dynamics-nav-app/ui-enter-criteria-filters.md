---
title: Ange villkor i filter
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
ms.openlocfilehash: 8eab393a0a77f9f1595ca1247c7549e68b491cb2
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="entering-criteria-in-filters"></a>Ange villkor i filter
När du vill söka efter data, till exempel kundnamn, adresser eller produktgrupper, anger du kriterier. I sökkriterier kan du använda alla siffror och bokstäver som du normalt kan använda i det specifika fältet. Dessutom kan du använda specialtecken som du vill filtrera resultatet ytterligare.

## <a name="searching-using-the-quick-filter"></a>Sök genom att använda snabbfiltret
Du kan lägga till filter för alla sidor genom att använda snabbfiltret. Snabbfiltret aktiveras genom att välja ikonen med förstoringsglas i det övre högra hörnet av en sida. Filtrering av den här typen används för att snabbt ange kriterier.

**Viktigt!** Snabbfiltret ger enkelt tillgång till filterdata genom att ange vanlig text, men ger även många alternativet för sökningkriterier. Beroende på om du anger vanlig text, eller text inklusive symboler, uppför sig snabbfiltret på olika sätt.  
- Om du anger vanlig text i sökkriterierna tolkas sökkriterierna som en skiftlägesokänslig sökning som innehåller viss text.  
- Om du anger en text inklusive symboler i sökkriterierna tolkas sökkriterierna exakt som du har angett den, och sökningen är skiftlägeskänslig.

### <a name="quick-filter-criteria"></a>Snabbfilterkriterium
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH>Sökkriterier</TH>
    <TH>Tolkat som…</TH>
    <TH>Returer...</TH>
  </TR>
  <TR>
    <TD>>tillverk</TD>
    <TD>@*tillverk*</TD>
    <TD>Alla transaktioner som innehåller texten man och är skiftlägesokänsliga.</TD>
  </TR>
  <TR>
    <TD>>sö</TD>
    <TD>@*se*</TD>
    <TD>Alla transaktioner som innehåller texten se och är skiftlägesokänsliga.</TD>
  </TR>
  <TR>
    <TD>>Tillverk*</TD>
    <TD>Börjar med Man och är skiftlägeskänsligt.</TD>
    <TD>Alla poster som börjar med texten Man.</TD>
  </TR>
  <TR>
    <TD>'tillverk'</TD>
    <TD>En exakt text och är skiftlägeskänsligt.</TD>
    <TD>Alla poster som matchar man exakt.</TD>
  </TR>
  <TR>
    <TD>@*tillverk</TD>
    <TD>Slutar på och är skiftlägesokänsligt.</TD>
    <TD>Alla poster som slutar på man.</TD>
  </TR>
  <TR>
    <TD>@man*</TD>
    <TD>Börjar med och skiftlägesokänsligt.</TD>
    <TD>Alla poster som börjar med man.</TD>
  </TR>
</TABLE>

**Obs!** Du kan inte använda ett jokertecken när du filtrerar på uppräkningsfält, t.ex fältet **Status** på försäljningsorder. För att ange ett filter för den här typen av fält kan du ange det numeriska värdet som en filtreringsparameter. Använd till exempel värdena **0**, **1**, **2** och **3** för att filtrera för dessa alternativ i fältet **Status** på en försäljningsorder, som har värdena **Öppna**, **Släppt**, **Väntar på godkännande** och **Väntar på förskottsbetalning**.  

## <a name="see-also"></a>Se även
[Arbeta med Dynamics NAV](ui-work-product.md)

