---
title: "Sparade inställningar i rapporter"
author: jswymer
ms.custom: na
ms.date: 09/26/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 0f11d862315c8ecd160cd18afb0a72a2d684b9b2
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---
# <a name="saved-settings-on-reports"></a>Sparade inställningar i rapporter
Beroende på rapporten som körs, kan du presenteras med en sida som gör att du kan ange vissa alternativ och filter för att ändra data som ingår i den skapade rapporten. Den här sidan är känd som sidan för rapportbegäran. En rapport kan innehålla en eller flera *sparade inställningar* som du kan tillämpa till rapporten från sidan för begäran. *Sparade inställningar* är i grunden fördefinierade alternativ och filter. Att använda sparade inställningar är ett snabbt och pålitligt sätt att konsekvent skapa rapporter som innehåller korrekta data.

Du kan se de sparade inställningar som är tillgängliga för dig för en rapport i avsnittet **Sparade inställningar** på sidan för rapportbegäran.

## <a name="to-apply-saved-settings-to-a-report"></a>Om du vill ange sparade inställningar till en rapport
1.  Öppna rapporten.

    Sidan för rapportbegäran visas.    
2.  I avsnittet **Sparade inställningar** på sidan anger du fältet **Namn** till de sparade inställningar som du vill använda.

    Avsnittet **Sparade inställningar** visas bara om rapporten har körts tidigare eller om det finns befintliga poster med sparade inställningar. Posten vid namn **Senast använda alternativ och filter** med sparade inställningar är alltid tillgänglig. Dessa inställningar är de alternativ- och filtervärden som användes förra gången som du körde rapporten.

## <a name="administer-saved-report-settings-for-users"></a>Administrera sparade rapportinställningar för användare
Om du har rätt behörigheter kan du visa, ändra och skapa sparade inställningarna för alla rapporter för alla användare i företaget. Du kan tilldela sparade inställningar för en rapport till individuella användare eller alla användare i företaget.

Du hanterar sparade inställningar från sidan 1506 **rapportinställningar**. För att öppna denna sida väljer du ikonen **Söka efter sida eller rapport** i det övre högra hörnet, går till **Rapporinställningar** och väljer sedan relaterad länk. 

Från sidan **Rapporinställningar** kan du skapa nya inställningar från noll, eller så kan du göra en kopia och ändra befintliga inställningar. För att ändra alternativ och filter för inställningar väljer du åtgärden **Redigera**.

**Anteckningar**:
-    Funktionen för sparade inställningar i rapporter är bara relevant när egenskapen SaveValues på sidan för begäran är inställd på Ja. Egenskapen SaveValues anges i utvecklingsmiljön.
-    Om du skapar en artikel med sparade inställningar för alla användare och denna artikel har samma namn som befintliga sparade inställningar för en viss användare, kan den användaren inte använda de sparade inställningar som har tilldelats alla.  I fältet Sparade inställningar på sidan för rapportbegäran visas två alternativ för sparade inställningar med samma namn. Oavsett vilket alternativ användaren väljer kommer de användarspecifika sparade inställningarna att tillämpas.

## <a name="see-also"></a>Se även
[Så här schemalägger du en rapportkörning](ui-schedule-report.md)

