---
title: "Ställa in eller ändra kontoplanen"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 48cd91958545b40b2ab0c5e48442fc874845af5b
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a>Ställa in eller ändra kontoplanen
Kontoplanen visar huvudbokskontona som lagrar dina ekonomiska data. Dynamics NAV inkluderar en standardkontoplan som är klar att stödja din verksamhet.
Du kan dock ändra standardkontona och du kan lägga till nya konton.  

## <a name="adding-or-changing-accounts"></a>Lägga till eller ändra konton
Från Kontoplan kan du öppna varje Redovisningskonto och lägga till eller ändra inställningar.

**Obs!** Du kan ta bort ett redovisningskonto. Men om du tar bort det, måste följande förutsättningar gälla:  
- Saldot på kontot måste vara noll.  
- Fältet **Tillåt borttag. av redov.konto** måste anges i fönstret **Redovisningsinställningar** och kontot får inte ha några redovisningstransaktioner på eller efter det datumet.  
- Om fältet **Kontr. redov.kontoanv.** i fönstret **Redovisningsinställningar** markeras får kontot inte användas i någon av följande bokföringsgrupper eller bokföringsinställningar.  

Dynamics NAV kommer att förhindra att du tar bort ett redovisningskonto som lagrar data som behövs i kontoplanen.  

##<a name="see-also"></a>Se även  
[Redovisningen och kontoplanen](finance-setup-general-ledger.md)  
[Hantera bankkonton](bank-manage-bank-accounts.md)  
[Dimensioner](finance-setup-dimensions.md)  
[Så här arbetar du med GIFI-koder i Kanada](ca-finance-setup-work-GiFI-codes.md)

