---
title: "Anpassa din arbetsyta - översikt"
description: "Lär dig mer om att anpassa användargränssnittet så att det passar ditt sätt att arbeta."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 04334d3bb50b37b9643b848ca4f59b015f03ad04
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace---overview"></a>Anpassa din arbetsyta - översikt
Du kan *anpassa* arbetsytan för att passa ditt arbete och dina inställningar genom att ändra layouten på sidor så att de endast visar den information som du behöver när du behöver den. De anpassningar som du gör kommer bara att påverka bara vad som visas, inte vad andra användare ser.

Du kan anpassa arbetsytan med hjälp av [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] och [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Anpassningsändringar som du gör visas också i [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] och [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].
  
> [!NOTE]  
> Administratören inom företaget kanske redan har anpassat ditt användargränssnitt till en rollspecifik layout för alla användare som har samma profil som du och använder samma Rollcenter. Anpassningar som du gör i arbetsytan sparas under ditt användarkonto så att de bevaras även om en administratör rullar ut en ny uppsättning rollspecifika layouter i företaget. Mer information finns i [Konfigurera användargränssnittet](admin-configure-user-interface.md).

## <a name="comparing-personalization-in-the-dynamics-nav-windows-and-web-clients"></a>Jämföra anpassning i Dynamics NAV Windows- och webbklienter
Du kan anpassa många delar av användargränssnittet, exempelvis vilka fält eller kolumner som ska visas och deras placering, vilka åtgärder som ingår i menyfliken, etc. Många av dessa saker kan du göra på i både Windows-klienten och webbklienten. I tabellen nedan finns en översikt över anpassningsfunktionerna i varje klient.

|  Anpassa  ||  Windows-klient  |  Webbklient  |
|---------------|-|------------------|--------------|
|Fält på snabbflikar||||
||Lägg till, flytta, ta bort |x|x|
||Visa i komprimerat huvud|x||
||Dölj under åtgärden **visa fler fält**|x||
|Listor och dokumentrader ||||
||Lägg till, flytta, ta bort kolumner  |x|x|
||Lägg till, flytta, ta bort låsning  |x|x|
|Faktaboxar|||
||Flytta, ta bort|x|x|
||Lägg till|x||
||Lägga till, flytta och ta bort fält.|x|x|
|Stack-ikon||||
||Flytta, ta bort|x|x|
||Lägg till |x||
|Diagram||||
||Flytta, ta bort|x|x|
||Lägg till|x| |
|Menyfliksområdet och åtgärder||x||
|Navigeringsruta||x||

En annan skillnad är att du kan ha olika anpassade versioner av samma sida, utifrån olika åtkomstpunkter till sidan när du anpassar med hjälp av Windows-klienten. Till exempel kan fönstret **Försäljningsorder** anpassas för att se olika ut när det öppnas från sidan **Kundkort** än när det öppnas från sidan **Försäljningsorderhandläggare**. När du anpassar en sida med hjälp av webbklienten, finns det bara en anpassad version per sida så att ändringarna syns på sidan, oavsett varifrån du öppnar den.

##  <a name="PersonalizationWinWeb"></a>Arbeta med anpassning mellan Dynamics NAV Windows- och webbklienten
Innan du börjar anpassa sidor är det viktigt att förstå hur anpassningen mellan Windows-klienten och webbklienten fungerar. Om du endast använder antingen Windows-klienten eller webbklienten, är denna information inte så relevant. Det är viktigt om du börjar anpassa sidor med båda klienter eller vid övergång från Windows-klienten till att använda webbklienten permanent.  

-   Om du använder Windows-klienten för att anpassa en viss sida från början, visas också anpassningsändringarna till sidan i [!INCLUDE[nav_web_md](includes/nav_web_md.md)] också.

-   Så länge du fortsätter att använda Windows-klienten för att anpassa sidan, kommer alla anpassningar som du gör även påverka sidan i webbklienten.

-   När du börjar att anpassa sidan med hjälp av webbklienten blir anpassningen för sidan separat mellan två klienter och du har en anpassad version för varje klient. I webbklienten har tidigare anpassningar på sidan rensats, vilket innebär att sidan återställs till dess ursprungliga layout och startar anpassningen av sidan från början. Tidigare anpassningar i Windows-klienten har inte ändrats.

- Från och med nu ska du anpassa sidan i Windows- och webbklienten oberoende av varandra, vilket innebär att sidan kan eventuellt se annorlunda ut i varje klient. Telefon- och surfplatte-klienter visar samma sidanpassningar som webbklienten.  

> [!Tip]  
>Om du öppnar sidan **ta bort användaranpassning** visas alla sidor som har anpassats för varje användare. Kolumnen **äldre anpassning** innehåller uppgift om anpassningen har gjorts i Windows-klienten eller webbklienten. Om det är markerat en kryssruta i kolumnen har anpassningen utförts i Windows-klienten (eller i webbklienten före [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## <a name="see-also"></a>Se även
[Anpassa din arbetsyta i Dynamics NAV Windows-klienten](ui-personalization-windows-client.md)  
[Anpassa din arbetsyta i Dynamics NAV webbklienten](ui-personalization-user.md)  
[Hantera anpassning](ui-personalization-manage.md)  
[Anpassa Dynamics NAV](ui-customizing-overview.md)  

