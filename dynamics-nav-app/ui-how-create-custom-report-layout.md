---
title: "Så här skapar du en anpassad rapportlayout"
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
ms.openlocfilehash: 90136439e09deb00a9aed9344fc5f89812caef3a
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-a-custom-report-layout"></a>Så här skapar du en anpassad rapportlayout
Som standard kommer en rapport ha inbyggd rapportlayout, antingen RDLC- eller Word-rapportlayout eller båda typerna. Du kan inte ändra inbyggda layouter. Du kan skapa egna anpassade layouter som du kan använda för att ändra utseendet på rapporten när den visas, skrivs ut eller sparas. Du kan skapa flera anpassade rapportlayouter för samma rapport, och sedan byta layout som används av en rapport efter behov.

Om du vill skapa en anpassad layout kan du antingen skapa en kopia av en befintlig anpassad layout eller lägga till en ny anpassad layout, som baseras i de flesta fall på en inbyggd layout. När du lägger till en ny anpassad layout kan du välja att lägga till en RDLC-rapportlayout, Word-rapportlayout eller både och. Den nya anpassade layouten baseras automatiskt på den inbyggda layouten för rapporten, om en är tillgänglig. Om det inte finns någon inbyggd layout för typen, skapas en ny tom layout som du måste ändra och utforma från noll. Mer information om RDLC- och Word-rapportlayouter, inbyggda och anpassade layouter och mer finns i [Hantera rapportlayouter](ui-manage-report-layouts.md).  

## <a name="to-create-a-custom-layout"></a>Så här skapar du en anpassad layout
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Val av rapportlayout** och välj sedan relaterad länk.  
I fönstret ** Report Layout Selection** visas alla rapporter som är tillgängliga i företaget som har angetts i fältet Företag högst upp i fönstret.
2. Ange fältet **Företag** till företaget som du vill skapa rapportlayouten i.
3. Markera raden för rapporten som du skapa layouten för och välj sedan **Anpassade layouter**.  
i fönstret **Anpassade rapportlayouter** visas alla anpassade layouter som är tillgängliga för den valda rapporten.
4. Om du vill skapa en kopia av en befintlig anpassad layout, markera den befintliga anpassade layouten i listan och välj sedan **Kopiera**.  
Kopian av den anpassade layouten visas i fönstret **Anpassade rapportlayouter** och har orden Kopia av i fältet Beskrivning.
5. Om du vill lägga till en ny anpassad layout som baseras på en inbyggd layout gör du följande:  
    1. Välj **Ny**. Fönstret **Infoga inbyggd layout för en rapport** visas. Fälten **ID** och **Namn** fylls i automatiskt.
    2. Om du vill lägga till en anpassad Word-rapportlayouttyp markerar du kryssrutan **Infoga Word-layout**.
    3. Om du vill lägga till en anpassad RDLC-rapportlayouttyp markerar du kryssrutan **Infoga RDLC-layout**.
    4. Välj **OK**.  
    De nya anpassade layouterna visas i fönstret **Anpassade rapportlayouter**. Om en ny layout baseras på en inbyggd layout får den orden **Kopia av en inbyggd layout** i fältet **Beskrivning**. Om det inte fanns en inbyggd layout för rapporten, får den nya layouten orden **Ny layout** i fältet **Beskrivning**, vilket anger att den anpassade layouten är tom.
6. Som standard är fältet **Företagsnamn** tomt, vilket betyder att den anpassade layouten är tillgänglig för rapporten i alla företag. För att du ska kunna göra den anpassade layouten tillgänglig väljer du **Redigera** och ställer sedan in fältet **Företagsnamn** till företaget som du vill ha.

## <a name="see-also"></a>Se även
[Hantera rapportlayouter](ui-manage-report-layouts.md)  
[Så här ändrar du vilken layout som används i en rapport för närvarande](ui-how-change-layout-currently-used-report.md)

