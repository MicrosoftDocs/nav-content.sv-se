---
title: "Så här avyttrar och ställer av anläggningstillgångar."
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
ms.openlocfilehash: 795bb23e7c0b46be095b2bbdfe7705b3d7b1e4ee
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-dispose-of-or-retire-fixed-assets"></a>Så här avyttrar och ställer av anläggningstillgångar.
När du säljer eller på annat sätt avyttrar en anläggningstillgång, måste avyttringsvärdet bokföras för att beräkna och registrera vinst eller förlust. En avyttringstransaktion måste vara den sista bokförda transaktionen för en anläggningstillgång. För delvis avyttrade anläggningstillgångar kan du bokföra fler än en avyttringstransaktion. Summan av alla bokförda avyttringsbelopp måste vara ett kreditbelopp.

 **OBS**: Om du byter en anläggningstillgång mot en annan måste du registrera både försäljningen av den gamla tillgången (avyttring) och inköpet av den nya (anskaffning). Mer information finns i [Så här skaffar du anläggningstillgångar](fa-how-acquire.md).

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a>Bokföra en avyttringstransaktion i redovisningsjournalen för anläggningstillgångar.  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournaler för anl.tillg.** och välj sedan relaterad länk.  
2. Skapa en första journalrad och fyll i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. Välj **Anskaffningskostnad** i fältet **Avyttring**.
4. Välj åtgärden **Infoga anl. motkonto**. En andra journalrad skapas för motkontot som ställs in för bokföring av avyttring.

    **Obs**: Steg 4 fungerar bara om du har ställt in följande: I fönstret **Anl. bokföringsmallkort** för den fasta anläggningstillgångens bokföringsmall, innehåller fältet **Avyttringskonto** redovisningsdebitkontot och fältet **Avuttringskontosaldo** innehåller det redovisningskonto där du vill bokföra mottransaktioner för uppskrivning. För mer information, se avsnittet "Att ställa in bokföringsmallar för anläggningstillgångar" i [Så här ställer du in allmän information för anläggningstillgångar](fa-how-setup-general.md).
5. Välj åtgärden **Bokföra**.

Om du säljer eller på annat sätt avyttrar en del av en anläggningstillgång måste du dela upp tillgången innan du kan registrera avyttringstransaktionen. För mer information, se [Så här överför, delar eller kombinerar du Anläggningstillgångar](fa-how-trans-split-combine.md).

## <a name="to-view-disposal-ledger-entries"></a>Så här visar du avyttringstransaktioner  
När du säljer eller avyttrar en anläggningstillgång måste avyttringsvärdet bokföras på redovisningskonton där du kan se resultatet.   

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.  
2. Markera den fasta anläggningstillgång som du vill visa poster för välj sedan åtgärden **Avskrivningsregler**.
3. Markera den avskrivningsregel som du vill visa poster för välj sedan åtgärden **Transaktionsposter**.
4. Markera en rad med **Avyttring** i fältet **Anl. bokföringskategori** och klicka sedan på åtgärden **Analysera**, .  
5. I fönstret **Analysera** väljer du redovisningstransaktionen och väljer sedan åtgärden **Visa**.
Fönstret **Redovisningstransaktioner** öppnas där du kan visa de transaktioner som förfogandeinlägget ledde till.

## <a name="see-also"></a>Se även
[Hantera anläggningstillgångar](fa-manage.md)  
[Skapa anläggningstillgångar](fa-setup.md)  
[Finans](finance-setup.md)  
[Välkommen till Dynamics NAV](across-get-started.md)

