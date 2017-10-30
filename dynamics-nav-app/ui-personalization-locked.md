---
title: "Varför är sidan är låst för anpassning?"
description: "Förklarar varför du inte kan anpassa en sida och vad du kan göra om du vill låsa upp den så att du kan anpassa den."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalization locked, cannot personalize page
ms.date: 09/07/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b365d14c199d36abebcae0b3ac86340fd59cf8ef
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="why-is-the-page-is-locked-from-personalizing"></a>Varför är sidan är låst för anpassning?
Om det finns en låsikon i banderollen **anpassa** när du öppnar en sida (enligt bilden), betyder det att du för tillfället inte kan göra några fler anpassningsändringar på sidan i [!INCLUDE[nav_web](includes/nav_web_md.md)].

![Anpassa låsning](media/personalization-locked.png "Anpassa låsning")

Det finnas två orsaker till detta:
1.  Hittills har du bara använt [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] för att anpassa sidan.

2. Du har använt [!INCLUDE[nav_web](includes/nav_web_md.md)] för att anpassa sidan, men det har gjorts med hjälp av [!INCLUDE[nav2017](includes/nav2017.md)] eller tidigare version.   

Om du vill fortsätta anpassa sidan med hjälp av [!INCLUDE[nav_web](includes/nav_web_md.md)] väljer du Lås-ikonen och sedan **Lås upp**.

## <a name="what-happens-when-you-unlock-the-page"></a>Vad händer om du låser upp sidan
Om du vill låsa upp sidan kommer den aktuella anpassningen på sidan i [!INCLUDE[nav_web](includes/nav_web_md.md)] att rensas, vilket innebär att sidan går tillbaka till dess ursprungliga layout och du måste börja om från början.

I [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] kommer sidan att behållas så som den var innan och kommer inte att påverkas av de nya ändringarna i [!INCLUDE[nav_web](includes/nav_web_md.md)]. Anpassningen i [!INCLUDE[nav_web](includes/nav_web_md.md)]och [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] blir uppdelade, så att du nu har en anpassad version i varje klient. 

I framtiden kan du anpassa sidan i två klienter separat. Därför kan sidan se annorlunda ut mellan två.

## <a name="see-also"></a>Se även
[Anpassning, översikt](ui-personalization-overview.md)  
[Arbeta med anpassning mellan Dynamics NAV Windows- och webbklienten](ui-personalization-overview.md#PersonalizationWinWeb)  
[Anpassa din arbetsyta med webbklienten](ui-personalization-user.md)  
[Anpassa din arbetsyta med Windows-klienten](ui-personalization-windows-client.md)  
[Hantera anpassning](ui-personalization-manage.md)  
[Arbeta med [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Så här ändrar du rollcentret](change-role.md)  

