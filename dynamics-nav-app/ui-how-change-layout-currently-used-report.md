---
title: "Så här ändrar du vilken layout som används i en rapport för närvarande"
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
ms.openlocfilehash: f1411704a7b2a0565d4b23d91e04e271af07659e
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-change-which-layout-is-currently-used-on-a-report"></a>Så här ändrar du vilken layout som används i en rapport för närvarande
En rapport kan ställas in med fler än en rapportlayout som du kan växla mellan.

Beroende på layouterna som finns tillgängliga för en rapport kan du välja att använda en inbyggd RDLC-rapportlayout, en inbyggd Word-rapportlayout eller en anpassad layout. Mer information om RDLC- och Word-rapportlayouter, inbyggda och anpassade layouter och mer finns i [Hantera rapportlayouter](ui-manage-report-layouts.md).

## <a name="to-change-the-layout-that-is-used-on-a-report"></a>Så här ändrar du layout som används i en rapport
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Val av rapportlayout** och välj sedan relaterad länk.  
I fönstret **Val av rapportlayout** visas alla rapporter som är tillgängliga i företaget som har angetts i fältet Företag högst upp i fönstret. Fältet Vald layout anger den layout som används i rapporten för närvarande.
2. Ange fältet **Företag** fältet högst upp i fönstret till företaget som inkluderar rapporten.
3. I raden för rapporten i listan och anger du fältet **Vald layout** till ett av följande alternativ för att ändra layouten som används för en rapport:
    - RDLC (inbyggd), använder den inbyggda RDLC-rapportlayouten i rapporten.
    - Word (inbyggd), använder den inbyggda Word-rapportlayouten i rapporten.
    - Anpassad använder en anpassad layout i rapporten.  
    Du kan se vilka anpassade layouter som är tillgängliga för rapporten i faktaboxen Rapportlayoutdelar. Om det inte finns några anpassade layouter för rapporten, måste du skapa en först. Om du väljer det här alternativet, gå vidare till nästa procedur för att ange den anpassade layout som du vill använda.
**Obs!** Om du väljer **RDLC (inbyggt)** eller **Word (inbyggt)** och du får ett felmeddelande att rapporten inte har en layout för den angivna typen, måste du välja ett annat layoutalternativ eller skapa en anpassad rapportlayout av den typ som du vill använda.

Om du har valt en inbyggd RDLC- eller Word-rapportlayout krävs ingen mer åtgärd och layouten används i när rapporten körs nästa gång.

## <a name="to-specify-a-custom-layout-on-a-report"></a>Så här anger du en anpassad layout på en rapport
1. Du anger vilken anpassad layout som ska användas i rapporten i fönstret **Anpassad rapportlayout**. Om fönstret **Anpassad rapportlayout** inte är öppet väljer du sökknappen i fältet **Rapportlayoutbeskrivning**.
2. I fönstret **Rapportlayoutbeskrivning** markera raden för anpassad layout som du vill använda, och välj sedan knappen **OK**.

Du återgår till fönstret **Val av rapportlayout**. Namnet på den valda anpassade layouten visas i fältet **Anpassad layoutbeskrivning**. Den anpassade layouten används nästa gången som du kör rapporten.

## <a name="see-also"></a>Se även
[Hantera rapportlayouter](ui-manage-report-layouts.md)

