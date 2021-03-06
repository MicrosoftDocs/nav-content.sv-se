---
title: "Automatisk bryta ned volym med dirigerad artikelinförsel och plockning"
description: "För lagerställen, som använder artikelinförsel och plockning, kan du dela upp en större enhet till mindre enheter, när du skapar lagerinstruktioner som uppfyller behoven hos källdokument, produktionsorder eller intern plockning och artikelinförsel."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 67b292438c0b262e7baecd622909ce3fc0f7f233
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-automatic-breaking-bulk-with-directed-put-away-and-pick"></a>Så här: Aktivera Automatisk bryta ned volym med dirigerad artikelinförsel och plockning
För lagerställen, som använder artikelinförsel och plockning, kan [!INCLUDE[d365fin](includes/d365fin_md.md)] i olika situationer, automatiskt använda brytenhet, d.v.s. dela upp en större enhet till mindre enheter, när du skapar lagerinstruktioner som uppfyller behoven hos källdokument, produktionsorder eller intern plockning och artikelinförsel. Med brytenhet menas ibland också samling av mindre måttenheter, om det behövs, för att uppfylla utgående förfrågningar, genom att analysera den större måttenheten i ursprungsdokumentet eller produktionsorder till de mindre enheter som är tillgängliga i distributionslagret.   

## <a name="breakbulking-in-picks"></a>Enhetsbrytning vid plockning  
Om du vill lagra artiklar i flera olika måttenheter och tillåta dem att kombineras automatiskt efter behov vid plockning väljer du fältet **Tillåt brytenhet** på lagerställekortet.  

När en aktivitet ska utföras söker programmet automatiskt efter en artikel i den begärda måttenheten. Om artikeln inte finns i denna enhet och du har valt fältet, föreslår programmet att du bryter ned en större måttenhet till den mindre måttenhet som behövs.  

Om systemet bara hittar mindre måttenheter, föreslår programmet att du samlar ihop flera artiklar för att komma upp i den kvantitet som begärs på utleverans- eller produktionsordern. Det som sedan sker är att den större måttenheten i ursprungsdokumentet bryts ned i mindre enheter för plockning.  

## <a name="breakbulking-in-put-aways"></a>Enhetsbrytning vid artikelinförsel  
Vid en artikelinförsel i distributionslagret föreslås automatiskt åtgärdsrader för Placera i den måttenhet som används i artikelinförseln, till exempel enheter, även om artiklarna inlevereras i en annan måttenhet.  

## <a name="breakbulking-in-movements"></a>Enhetsbrytning vid transport  
Enhetsbrytning sker också automatiskt vid påfyllningstransporter om fältet **Tillåt brytenhet** är valt på snabbfliken **Alternativ** i fönstret **Beräkna lagerplatsåteranskaffning**.  

Du kan granska resultaten av enhetskonverteringsprocessen som övergångsrader för enhetsbrytning i instruktionerna för artikelinförsel, plockning eller transport.  

> [!NOTE]  
>  Om du väljer fältet **Sätt brytenhetsfilter** i huvudet för instruktionerna för distributionslagret, döljs enhetsbrytningsraderna om det uteslutande är den större måttenheten som ska användas. Exempel: Om en lastpall består av 12 enheter och samtliga enheter kommer att användas, dirigeras du under plockningen att ta en lastpall och placera 12 enheter. Om du bara ska plocka nio enheter döljs inte enhetsbrytningsraderna, även om du markerar fältet **Brytenhetsfilter**, eftersom du måste placera de återstående tre enheterna någonstans i distributionslagret.  

> [!NOTE]  
>  Om du vill att måttenheterna ska fungera så bra som möjligt i distributionslagret, också när du använder enhetsbrytning, ska du alltid försöka göra följande:  
>   
> - Ange den minsta måttenhet som du tror kommer att användas i distributionslagret som basmåttenhet för artiklar.  
> - Ange alternativa måttenheter för artiklar som multiplar av basmåttenheten.  

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

