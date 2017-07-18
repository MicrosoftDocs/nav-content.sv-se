---
title: "Ställa in dimensioner"
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
ms.openlocfilehash: 18237c4b755926222a36bc97dec5d6783c11454d
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="set-up-dimensions"></a>Ställa in dimensioner
Du måste ange vilka dimensioner och dimensionsvärden som ska användas i företaget. Du bör också ange vilka dimensioner som ska användas som globala dimensioner respektive genvägsdimensioner. Du bör tänka igenom ordentligt vilka dimensioner som är lämpligast att använda som globala dimensioner respektive genvägsdimensioner på företaget.  
Du ställer in alla olika dimensioner som du vill spåra i fönstret **Dimensioner**. Fönstret Dimensioner innehåller en rad för varje dimension, till exempel *Projekt*, *Avdelning*, *Område* och *Säljare*.  

För varje dimension måste du också ställa in dimensionsvärdena, till exempel alla företagets olika avdelningar. Dimensionsvärden kan anges i en hierarkisk struktur som liknar kontoplanen, så att data kan brytas ned i olika detaljeringsgrader och delmängder av dimensionsvärden kan räknas samman.  

Du kan ange två globala dimensioner som automatiskt blir tillgängliga överallt, till exempel i rapporter och batch-jobb. Du kan även ange sex ytterligare genvägsdimensioner som blir tillgängliga som ett fält på journal- och dokumentrader. De återstående dimensionerna kan du använda genom att öppna ett separat fönster där dimensioner för raden visas.  

Du kan definiera så många dimensioner som behövs i företaget och du kan definiera ett obegränsat antal dimensionsvärden i varje dimension. Alla dimensioner som du definierar kan användas i transaktioner i journaler och dokument samt i dimensionsrelaterade rapporter och batch-jobb.  

## <a name="set-up-default-dimensions-for-customers-vendors-and-other-accounts"></a>Konfigurera standarddimensioner för kunder, leverantörer och andra konton
Om du vill kan du definiera en standarddimension för ett enskilt konto. Den här koden kopieras sedan till journalen eller dokumentet när kontonummerfältet fylls i på raden. Du kan emellertid ta bort eller ändra koden vid behov. Du kan också göra en dimension obligatorisk, så att det inte går att bokföra en transaktion med en viss typ av konto såvida inte kontot har ett tilldelat dimensionsvärde.  

Om du vill kan du definiera en dimension för varje kontotyp. Koden kopieras då till journalen eller dokumentet när kontotypen fylls i på raden. Du kan alltid ändra koden på dokumentet, om det behövs.  

Du kan slutligen göra en dimension obligatorisk, så att det inte går att bokföra en transaktion med en viss typ av konto såvida inte kontot har ett tilldelat dimensionsvärde.

## <a name="see-also"></a>Se även
[Dimensioner](finance-setup-dimensions.md)  
[Konfigurera Centrala finansiella processer](finance-setup-setup-finance-setup.md)

