---
title: "Så här hanterar du budgetar för anläggningstillgångar"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 47b5e0abcae4fab92da5dd9c1bda350a37ec0358
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-budgets-for-fixed-assets"></a>Så här hanterar du budgetar för anläggningstillgångar
Du kan skapa budgeterade anläggningstillgångar. På så sätt kan du inkludera eventuella förutsedda anskaffningar och försäljningar i rapporter.  

 Om du vill förbereda den budgeterade resultaträkningen, balansräkningen och likviditetsbudgeten måste du ha tillgång till information om framtida investeringar, avyttringar och avskrivning av anläggningstillgångar. Den här informationen får du i rapporten **Anl.tillg. - planerat värde**. Innan du skriver ut rapporten måste du förbereda budgeten.  

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a>För att budgetera anskaffningskostnaden för en anläggningstillgång
När du förbereder en budget måste du skapa anläggningstillgångskort för de anläggningstillgångar som du avser att införskaffa i framtiden. De budgeterade anläggningstillgångarna ställs in som vanliga anläggningstillgångar, men de måste ställas in för att inte bokföras i redovisningen.

När du bokför anskaffningskostnaden, anger du numret på den budgeterade fasta anläggningstillgången i **Budgeterat anl.nr.** . På så sätt bokförs en anskaffningskostnad med ett motsatt tecken för den budgeterade tillgången. Detta innebär att den totala anskaffningskostnaden för den budgeterade tillgången är mellanskillnaden mellan den budgeterade och den verkliga anskaffningskostnaden.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.
2. Välj åtgärden **Ny** för att skapa ett nytt anläggningstillgångskort för den budgeterade anläggningstillgången.
3. Markera kryssrutan **Budgeterad anläggningstillgång** så förhindras bokföring i redovisningen.
4. Fyll i de återstående fälten, tilldela en avskrivningsregel och bokför sedan den första anskaffningskostnaden med budgeterade anläggningstillgången som anges i fältet **Budgeterat anl.nr.** på journalraden. Mer information finns i [Så här skaffar du anläggningstillgångar](fa-how-acquire.md).

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a>För att budgetera avyttringen av en anläggningstillgång:
Om du planerar att sälja tillgångar under budgetperioden kan du föra in uppgifter om försäljningspris och försäljningsdatum.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.
2. Markera den anläggningstillgång som du vill avyttra och välj sedan åtgärden **Avskrivningsregler**.
3. Lägg till **Planerat avyttringsdatum** och **Planerad avyttringsintäkt** i fönstret **Anl. avskrivningsregler**. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

## <a name="to-view-projected-disposal-values"></a>Så här visar du planerade avyttringsvärden
Om du vill se de planerade avyttringsvärdena och beräkna vinsten och förlusten kan du använda rapporten **Anl. - planerat värde**.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. - planerat värde** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs.
3. Välj knappen **Skriv ut** eller **Förhandsgranska**.

## <a name="to-budget-depreciation"></a>Så här budgeterar du avskrivning
Du kan använda rapporten **Anl.tillg. - planerat värde** för att beräkna framtida avskrivning. I rapporten visas bokföringsvärdet och den ackumulerade avskrivningen vid inledningen av den angivna perioden, ändringar under perioden och bokföringsvärde och ackumulerad avskrivning vid slutet av den angivna perioden.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. - planerat värde** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs.
3. Om du vill se det totala värdena föra alla tillgångar avmarkerar du kryssrutan **Skriv ut per anl.tillg.**.
4. Fyll inte i fälten på snabbfliken **Anläggningstillgång** så inkluderas alla tillgångar. I fältet **Budgeterad tillgång** kan du fylla i **Nej** om du vill utesluta budgeterade tillgångar eller **Ja** om du endast vill visa de budgeterade tillgångarna.
5. Välj knappen **Skriv ut** eller **Förhandsgranska**.

## <a name="see-also"></a>Se även
[Hantera anläggningstillgångar](fa-manage.md)  
[Skapa anläggningstillgångar](fa-setup.md)  
[Finans](finance-setup.md)  
[Välkommen till Dynamics NAV](across-get-started.md)
