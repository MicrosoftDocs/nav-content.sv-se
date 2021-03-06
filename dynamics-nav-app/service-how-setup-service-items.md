---
title: "Översikt över inställningar för serviceartiklar och serviceartikelkomponenter"
description: "Mer information om saker som du måste ställa in innan du kan använda serviceartiklar, inklusive standardvärden, till exempel svarstid, kontraktrabatt i procent och serviceprisgrupp."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0632bdc3b12e60c9b49893df748e8ca165c5b9d4
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-service-items-and-service-item-components"></a>Så här ställer du in serviceartiklar och serviceartikelkomponenter
Om du vill arbeta med serviceartiklar måste du ställa in följande

* Serviceartikelgrupper 
* Valfritt

## <a name="to-set-up-service-item-groups"></a>Så här skapar du serviceartikelgrupper:
Du anger grupper med artiklar som hör ihop med avseende på reparation och underhåll. Du kan ange standardvärden för serviceartiklar i serviceartikelgruppen, t.ex. svarstid, kontraktrabatt i procent och serviceprisgrupp. För artiklar i en serviceartikelgrupp kan du välja om du vill att de ska registreras automatiskt som serviceartiklar då de säljs..  
  
Du tilldelar serviceartikelgrupper till artiklar på **Artikelkortet** och till serviceartiklar på **serviceartikelkortet**.  
  
1. Välj ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceartikelgrupper** och välj sedan relaterad länk.  
2. Skapa en ny serviceartikelgrupp.  
3. Fyll i fälten **Kod** och **Beskrivning**.  
4. I fältet **Standard kontraktsrabatt %** anger du standardrabatten i procent för kontrakt som du vill att serviceartiklarna i gruppen ska ha.  
5. I fältet **Standard serviceprisgruppskod** anger du den förvalda serviceprisgruppskoden som du vill att serviceartiklarna i gruppen ska ha.  
6. I fältet **Standard svarstid (timmar)** anger du standardsvarstiden som du vill att serviceartiklarna i gruppen ska ha, i timmar.  
7. Om du vill att artiklarna i gruppen ska registreras som serviceartiklar då de säljs, väljer du fältet **Skapa serviceartikel**.  

## <a name="to-set-up-service-item-components"></a>Så här ställer du in serviceartikelkomponenter
En serviceartikel kan bestå av flera komponenter, som kan ersättas med reservdelar då artikeln är servad. Komponenterna läggs upp på sidan **Serviceartikelkomponent lista**. Om du vill skapa komponenter för serviceartiklar som är strukturer kan du låta kopiera strukturartiklarna automatiskt och skapa dem som serviceartikelkomponenter. 
  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceartiklar**, och välj sedan relaterad länk. 
2. Öppna serviceartikeln som du vill skapa komponenter för.  
3. Välj åtgärden **Komponenter**. Fönstret **Serviceartikelkomponent lista** öppnas.  
4. Lägg till en ny komponent.  
5. I fältet **Typ** väljer du **Serviceartikel** om själva komponenten är en registrerad serviceartikel. Välj annars **Artikel**.  
6. I fältet **Nr.** väljer du den artikel eller serviceartikel som utgör en serviceartikelkomponent.  

## <a name="to-set-up-service-item-components-from-a-bom"></a>Så här ställer du in serviceartikelkomponenter från en struktur
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceartiklar**, och välj sedan relaterad länk.  
2. Öppna den serviceartikel som du vill skapa komponenter från en struktur för.  
3. Välj åtgärden **Komponenter**. Fönstret **Serviceartikelkomponent lista** öppnas.  
4. Välj fältet **Kopiera från struktur**  
  
    Om artikeln som serviceartikeln är kopplad till är en struktur skapas automatiskt komponenter för alla artiklarna i strukturen.  

## <a name="to-set-up-a-service-shelf"></a>Så här skapar du en servicehylla
Du kan lägga upp servicehyllor som hjälper till att identifiera där du lagrar dina serviceartiklar. Du tilldelar servicehyllor till serviceartiklar på sidan **Serviceorder** och i fönstret **Serviceartikel arbetsblad**.  
  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Servicehyllor** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs.

## <a name="see-also"></a>Se även
[Så här skapar du koder för standardservice](service-how-setup-service-coding.md)   
[Så här skapar du felsökning:](service-how-setup-troubleshooting.md)
