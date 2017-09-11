---
title: "Prognos för försäljning och lager"
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 765527ed4f4800acec20f0abbd4374e95c9c36dc
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="sales-and-inventory-forecast-for-dynamics-nav"></a>Prognos för försäljning och lager för Dynamics NAV 
Lagerhantering är en kompromiss mellan kundservice och hantering av din kostnad. Å ena sidan kräver ett lågt lager mindre rörelsekapital, men å andra sidan leder eventuellt slut i lager till missade försäljningar. Tilläggen för Försäljning och Lagerprognos förutsäger potentiella försäljningar med hjälp av historiska data och ger en tydlig översikt av förväntade slut i lager. Baserat på prognosen hjälper tilläggen till att skapa påfyllningförfrågningar till dina leverantörer, vilket sparar tid.  

## <a name="setting-up-forecasting"></a>Konfigurera prognoser
I Dynamics NAV måste du konfigurera anslutningen till Azure Machine Learning (Azure ML). För mer information, se [Så här registrerar du Dynamics NAV i ledningportalen för Azure](ui-how-register-dynamics-nav-azure.md). När du har upprättat anslutningen kan du konfigurera prognosen till att använda en annan typ av period att rapportera efter, t.ex ändra från prognos per månad till prognos per kvartal. Du kan även välja antal perioder att beräkna prognosen efter, beroende på hur många detaljnivåer du vill att prognosen ska vara. Vi föreslår att du gör prognoser per månad och med en 12 månaders horisont för prognosen.  

## <a name="using-the-forecasts"></a>Att använda prognoserna
Detta tillägg använder funktionerna i Azure ML för att förutsäga framtida försäljningar som baseras på din försäljninghistorik för att undvika lagerbrist. När du till exempel väljer en artikel i fönstret **Artiklar** visar diagrammet i fönstret **Prognostiserad artikel** de beräknade försäljningarna av artikeln i den kommande perioden. På så sätt kan du se om du förmodligen kommer att få slut på lagret av artikeln snart.  

Du kan också använda tillägget för att föreslå när du ska fylla på lagret. Om du till exempel skapar en inköpsorder för Fabrikam eftersom du vill köpa deras nya skrivbordstol, kommer tillägget Prognos för försäljning och lager att föreslå att du fyller i distributionslagret även på den LONDON snurrstol som du brukar köpa från leverantören. Detta beror på att tilläggprognoserna att du kommer att få slut i lager av LONDON snurrstol de kommande två månaderna, vilket innebär att det kan hända att du vill beställa fler stolar redan nu.  

## <a name="see-also"></a>Se även
[Hantera försäljning](sales-manage-sales.md)  
[Hantera lager](inventory-manage-inventory.md)  
[Anpassa Dynamics NAV med hjälp av tillägg](ui-extensions.md)  
[Så här registrerar du Dynamics NAV i ledningportalen för Azure](ui-how-register-dynamics-nav-azure.md)  

