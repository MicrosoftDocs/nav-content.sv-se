---
title: Anpassa din arbetsyta med Dynamics NAV webbklient
description: "Lär dig mer om att anpassa användargränssnittet så att det passar ditt sätt att arbeta."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalize page, personalization, hide columns, remove fields, move fields
ms.date: 07/26/2017
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c266842d4a64b62c90dab8db26f5206f9a10e4cc
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace-using-the-dynamics-nav-web-client"></a>Anpassa din arbetsyta med Dynamics NAV webbklient
<!--NAV in the Web client-->
Du kan *anpassa* arbetsytan för att passa ditt arbete och dina inställningar genom att ändra sidor så att de endast visar den information som du behöver när du behöver den. De anpassningar som du gör kommer bara att påverka bara vad som visas, inte vad andra användare ser.

Beroende på vilken typ av sida och vad den innehåller kan göra du följande:

-   Lägga till, flytta och ta bort fält.
-   Lägga till, flytta och ta bort kolumner i en lista.
-   Ändra låsning av kolumner i listan. Låsningen låser en eller flera kolumner till vänster i en lista så att de alltid visas även om du bläddrar vågrätt.
-   Flytta och ta bort stack-ikoner (paneler).
-   Flytta och ta bort delar. Delar är underavdelningar eller områden på en sida som innehåller flera fält, en annan sida, ett diagram eller paneler.  

## <a name="to-personalize-a-page"></a>Så här anpassar du en sida

1. I det övre högra hörnet väljer du ikonen ![inställningar](media/ui-experience/settings_icon_small.png "ikonen inställningar för rollcenter") och sedan **anpassa**.

    Banderollen **anpassa** visas längst upp, vilket innebär att du kan börja göra ändringar.

    ![Anpassningsläget](media/ui_personalize_mode_small.png "Anpassningsläget")

2.  Gå till sidan du vill anpassa.

    Om du ser en låsikon i informationstexten, se [Varför sidan är låst](ui-personalization-locked.md) för mer information.

3.  Peka på ett område som du vill anpassa, t.ex. fält eller en kolumnrubrik i en lista. Allt som du kan anpassa markeras omedelbart med en pil eller en ram.
<!--
    -  If a component can be personalized, an arrow head (![Personalization indicator arrow left](media/ui_personalize_arrow_left.png "Personalization indicator arrow left") or ![Personalization indicator arrow down](media/ui_personalize_arrow_down.png "Personalization indicator arrow down")) appears.
    -   If the component is a part, the extent of the part is indicated by a border.
    -   The freeze pane in a list is indicated by a vertical line along the entire right-side of the last column of the freeze pane.
    -->

4.  Använd den här tabellen för att göra ändringar:     <table>
        <tr><th>Vad vill du göra</td><th>Hur du gör det.</th></tr>
        <tr><td>Flytta någonting, precis som fält, kolumn i listan, panel eller del</td><td> Peka var som helst på vad du vill flytta och dra den till dess nya plats. Platsen anges med antingen en tjock vågrät eller lodrät linje.</td></tr>
        <tr><td>Ta bort någonting</td><td>Markera pilen och välj <b>Ta bort</b>. </td></tr>
        <tr><td>Lägga till ett fält eller kolumn</td><td>I banderollen <b>anpassa</b> välj <b>mer</b> och sedan <b>fält</b>.<br /></br>Rutan <b>lägga till fält på sidan</b> öppnas till höger. Den visar de fält som du kan lägga till på sidan. Fält som är markerade som <b>Placerad</b> finns redan finns på sidan. Fält som är markerade som <b>Klar</b> finns redan finns på sidan.<br /></br>Om du vill lägga till ett fält, drar du det från fönstret till den plats där du vill ha den. Platsen anges med antingen en tjock vågrät eller lodrät linje.</td></tr>
        <tr><td>Ändra låsning i en lista till en annan kolumn</td><td>Markera pilen i kolumnen som du vill ska vara den sista kolumnen på låsningen och välj <b>Ange låsning</b>.<br /><br/>Om du vill ange låsningen tillbaka till den ursprungliga angivna platsen, markera pilen för den aktuella kolumnen i låsningen och välj <b>ta bort låsning</b>. Obs! Du kan ta bort den ursprungliga låsningen. Det kommer alltid att finnas en låsning som innehåller minst en kolumn.</td></tr>
      </table>

    > [!IMPORTANT]  
    >   Du kan inte ändra en lista om listan visas som paneler. Måste du först ändra sidan till listvyn genom att välja ikonen ![visa som lista](media/ui_show_as_list_icon.png "Visa som listpil vänster").

5.  Du kan fortsätta att göra ändringar på samma sida eller flytta till en annan sida. Dina ändringar sparas automatiskt medan du gör dem. När du är klar väljer du i **anpassa** banderoll **Klar**.

## <a name="clear-personalization-to-change-a-page-back-to-its-original-layout"></a>Ta bort anpassningar för att ändra en sida till dess ursprungliga layout
Vid något tillfälle kanske du vill ångra alla anpassningsändringar som du har gjort på sidan så att sidan ser ut som den gjorde från början För att göra detta väljer du i banderollen **anpassa** **mer**, och sedan **Avmarkera anpassning**.

## <a name="personalization-in-detail"></a>Anpassning i detalj
Här följer några tips som hjälper dig att bättre förstå anpassning.  
-   När du ändrar en kortsida som du öppnar från en lista påverkar ändringarna alla poster som du öppnar från listan. Anta till exempel att du öppnar en specifik kund från listsidan kunder och sedan anpassar sidan genom att lägga till ett fält. När du öppnar andra kunder från listan visas också det fält som du har lagt till.
-   Ändringarna börjar gälla i alla dina rollcenter. Till exempel om du gör en ändring i kundlistan när rollcentret har angetts till Chef visas dessutom ändringen i kundlistan när rollcentret anges till Försäljningsorderhandläggare.
-   Ändringar av en sida i rutan börjar gälla på sidan var den än visas.  
-   Du kan bara lägga till fält och kolumner från en fördefinierad lista som baseras på sidan. Du kan inte skapa nya.

## <a name="see-also"></a>Se även
[Anpassning, översikt](ui-personalization-overview.md)  
[Hantera anpassning](ui-personalization-manage.md)  
[Arbeta med [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Så här ändrar du rollcentret](change-role.md)  

