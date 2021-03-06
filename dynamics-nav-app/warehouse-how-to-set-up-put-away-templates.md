---
title: "Så här skapar du artikelinförselmallar"
description: "Med dirigerad artikelinförsel och plockning går det alltid att hitta den lämpligaste lagerplatsen för artiklarna enligt den artikelinförselmall som du har skapat för distributionslagret, de lagerplatsordningar som du har angett för lagerplatserna samt de lägsta och högsta antal som du har definierat för de fasta lagerplatserna."
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
ms.openlocfilehash: be51b4d1cfc4d2a54e5f44f6419ed4539c01e9df
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-put-away-templates"></a>Så här skapar du artikelinförselmallar:
Med dirigerad artikelinförsel och plockning går det alltid att hitta den lämpligaste lagerplatsen för artiklarna enligt den artikelinförselmall som du har skapat för distributionslagret, de lagerplatsordningar som du har angett för lagerplatserna samt de lägsta och högsta antal som du har definierat för de fasta lagerplatserna.  

Du kan skapa flera artikelinförselmallar och välja en av dem för att styra allmänna artikelinförslar i distributionslagret. Du kan även välja en artikelinförselmall för valfri artikel eller lagerställeenhet som kan ha specialkrav beträffande artikelinförsel.  

## <a name="to-set-up-put-away-templates"></a>Så här skapar du artikelinförselmallar:  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Artikelinförselmallar** och välj sedan relaterad länk.  
2.  Välj åtgärden **Ny**.  
3.  Ange en kod som är unik för den mall som du ska skapa.  
4.  Ange vid behov en kort beskrivning.  
5.  Fyll i den första raden med de lagerplatskrav som du vill ska uppfyllas först och främst när en artikelinförsel föreslås.  
6.  Fyll i den andra raden med de lagerplatskrav som ska gälla i andra hand vid artikelinförsel till en lagerplats. Den andra raden används endast om det inte går att hitta en lagerplats som uppfyller kraven på den första raden.  
7.  Fortsätt att fylla i raderna tills du har beskrivit alla godtagbara lagerplatsplaceringar som du vill använda vid artikelinförsel.  
8.  På den sista raden i artikelinförselmallen markerar du kryssrutan **Sök flytande lagerplats**.  

Du kan skapa olika artikelinförselmallar och sedan använda dem som du vill. Den artikelinförselmall som du har valt för artikeln eller lagerställeenheten om det finns någon. Om de här fälten inte fylls i används den artikelinförselmall som du har valt för distributionslagret på snabbfliken **Lagerplatsprinciper** på lagerställekortet.  

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

