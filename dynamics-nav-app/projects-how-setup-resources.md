---
title: "Så här skapar du resurser"
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 72f5304e6a69a736c9df2cbb9ca64c5f3c5261a2
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-resources"></a>Så här skapar du resurser
Du måste lägga upp resurser och relaterade kostnader och priser för att hantera resursaktiviteter på rätt sätt. Projektrelaterade priser, rabatter och kostnadsfaktorregler är definierade på projektkortet. Du kan specificera kostnader och priser för enskilda resurser, resursgrupper eller alla tillgängliga resurser i företaget.

När resurser är förbrukade eller sålda i ett projekt hämtas associerade priser och kostnader från informationen som du anger.

Du kan ange standardbeloppet per timme när resursen skapas. Om du till exempel använder en viss maskin för ett projekt i 5 timmar beräknas projektet baserat på beloppet per timme.

## <a name="to-set-up-a-resource"></a>Så här skapar du resurser
Skapa ett kort för varje resurs som du vill använda i projekt.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resurser** och välj sedan relaterad länk.
2. Välj åtgärden **Ny**.
3. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.  

## <a name="to-set-up-a-resource-group"></a>Så här skapar du en resursgrupp
Du kan kombinera flera resurser i en resursgrupp. All kapacitet och budget i resursgrupperna samlas från de individuella resurserna. Det är också möjligt att skriva in resursgruppskapacitet, antingen oberoende av de samlade värdena eller som tillägg till dem.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resursgrupper** och välj sedan relaterad länk.
2. Välj åtgärden **Ny**.
3. Fyll i fälten om det behövs.

## <a name="to-set-capacity-for-a-resource"></a>Ställa in kapaciteten för en resurs 
För att beräkna hur lång tid en resurs kan läggas på projekt, måste deras kapacitet först ställas in som tillgänglig tid per period i arbetskalendern. Denna inställning används när du fyller i projektplaneringsrader som innehåller resursen. Mer information finns i [Så här skapar du Projekt](projects-how-create-jobs.md).

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resurser** och välj sedan relaterad länk.
2. Öppna det relevanta resurskortet och välj sedan åtgärden **Resurskapacitet**.
3. I fönstret **Resurskapacitet** ställer du i fältet **Visa per** in periodlängden, exempelvis **Dag**, som visas i kolumnerna på **Matris för resurskapacitet** på snabbfliken.
4. För varje resurs på en rad anger du för respektive period i kolumnerna hur många timmar som resursen är tillgänglig.
5. Du kan också välja att ställa in resurskapaciteten veckovis med start- och slutdatum genom att välja åtgärden **Ställ in kapacitet**.
6. I fönstret **Inställningar för resurskapacitet** fyller du i fälten efter behov.
7. Välj åtgärden **Uppdatera kapacitet**. Fönstret **Resurskapacitet** uppdateras med den angivna kapaciteten.
8. Stäng fönstret.

## <a name="to-set-up-alternate-resource-costs"></a>Så här skapar du alternativa resurskostnader
Förutom kostnaden som anges på resurskortet, kan du registrera alternativa kostnader för varje resurs. Om t.ex. en anställd har en annan timpenning för övertidsarbete kan du registrera en resurskostnad för denna övertidskostnad. Den alternativa kostnad som du skapar för resursen har företräde framför kostnaden på resurskortet när du använder resursen i resursjournalen.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resurser** och välj sedan relaterad länk.  
2. Välj den resurs för det som du vill skapa en eller flera alternativa kostnader för och välj sedan åtgärden **Kostnader**.  
3. I fönstret **Resurskostnader** fyller du i fälten på en rad efter behov.  
4. Upprepa steg 3 för varje alternativ kostadsresurs som du vill skapa.

**Obs**. Om du vill skapa resurskostnader som gäller alla resurser och resursgrupper öppnar du fönstret **Resurskostnader** och fyller i alla fält.

## <a name="to-set-up-alternate-resource-prices"></a>Så här skapar du alternativa resurspriser  
Förutom priset som anges på resurskortet, kan du registrera alternativa priser för varje resurs. Dessa alternativa priser kan vara villkorliga. De kan bero på om resursen används med ett särskilt projekt eller en särskild arbetstyp.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resurser** och välj sedan relaterad länk.
2. Välj den resurs för det som du vill skapa en eller flera alternativa priser för och välj sedan åtgärden **Priser**.
3. I fönstret **Resurspriser** fyller du i fälten på en rad efter behov.
4. Upprepa steg 3 för varje alternativt resurspris som du vill skapa.

## <a name="see-also"></a>Se även
[Ange projekthantering](projects-setup-projects.md)  
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)  
