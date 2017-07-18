---
title: Dimensioner
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a1b38e74717e87bea6efb46f8f4e5236b6ec4e64
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

#<a name="dimensions"></a>Dimensioner
Dimensioner är data som du lägger till i transaktioner för att kategorisera dem för analys. Du kan till exempel ha dimensioner som anger vilket projekt eller vilken avdelning en transaktion ursprungligen kommer ifrån.
Då kan du använda dimensioner i stället för att skapa separata redovisningskonton för varje avdelning och projekt. På så sätt kan du få omfattande analysinformation i dina data utan att behöva använda en komplicerad kontoplan.
Du kan definiera ett valfritt antal dimensioner med ett obegränsat antal dimensionsvärden.  

Om du till exempel angav en dimension kallad *Avdelning* och använder denna dimension och ett dimensionsvärde när du bokför försäljningsdokument. Du kan sedan hämta business intelligence-data senare som artiklar som har sålts på, efter t.ex. avdelningar.
Ju fler dimensioner du ställer in och använder, desto mer detaljerade rapporter kan du baseras dina affärsbeslut på. En enda försäljningstransaktion kan till exempel innehålla information om flera dimensioner, t.ex. på vilket konto som försäljningen av artikeln har bokförts, var artikeln har sålts, vem som har sålt den och vilken typ av kund som har köpt den.  

## <a name="using-dimensions"></a>Använda dimensioner
I ett dokument som t.ex. en försäljningsorder kan du lägga till dimensionsinformation för både en individuell dokumentrad och själva dokument. T.ex. i fönstret **Försäljningsorder** kan du ange dimensionsvärden för de två första genvägsdimensionerna direkt i dokumenthuvudet och lägga till ytterligare dimensionsinformation om du väljer knappen **Dimensioner**.  
Om du istället arbetar med en journal kan du lägga till dimensionsinformation i en transaktion om du har lagt upp genvägsdimensioner som fält direkt på journalraderna.  
Du kan ställa in standarddimensioner för konton eller kontotyper, så att dimensioner och dimensionsvärden fylls i automatiskt.  

## <a name="dimension-sets"></a>Dimensionsuppsättningar
En dimensionsuppsättning en är en unik kombination av dimensionsvärden. Den lagras som dimensionsuppsättningstransaktioner i databasen. Varje dimensionsuppsättningstransaktion representerar ett enstaka dimensionsvärde. Dimensionsuppsättningen identifieras av ett gemensamt dimensionsuppsättnings-ID som tilldelats varje dimensionsuppsättningstransaktion som tillhör dimensionsuppsättningen.  

När du skapar en ny journalrad, dokumenthuvud eller dokumentrad kan du ange en kombination av dimensionsvärden. I stället för att uttryckligen lagra varje dimensionsvärde i databasen tilldelas ett dimensionsuppsättnings-ID till journalraden, dokumenthuvudet eller dokumentraden för att specificera dimensionsuppsättningen.  

## <a name="see-also"></a>Se även
[Finans](finance-setup.md)  
[Ställa in dimensioner](finance-setup-setup-dimensions.md)  

