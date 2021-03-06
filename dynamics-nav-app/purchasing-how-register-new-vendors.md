---
title: "Skapa ett leverantörskort för att registrera en ny leverantör"
description: "Lär dig skapa ett leverantörskort för att registrera en ny leverantör."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c7fee8b43940fc5e5fb020b4ca1ac9b27b90decd
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-new-vendors"></a>Så här registrerar du nya leverantörer
Leverantörer erbjuder produkter som du säljer. Varje leverantör som du har köpt av måste registreras som ett leverantörskort.

Innan du kan registrera nya leverantörer, måste du lägga upp olika inköpskoder som du kan välja mellan, när du fyller i leverantörskort. När alla obligatoriska huvuddata skapats kan du konfigurera leverantören ytterligare, till exempel genom att prioritera leverantören i betalningssyfte och upprätta en lista över artiklar som leverantören och andra leverantörer kan tillhandahålla. En annan grupp av inställningsuppgifter för leverantörer är att lägga in dina avtal om inköpspris, rabatter och betalning. Mer information finns i [Konfigurera inköp](purchasing-setup-purchasing.md).

Leverantörskort innehåller den information som behövs för att köpa produkter från leverantören. Mer information finns i [Så här bokför du inköp](purchasing-how-record-purchases.md), [Så här registrerar du nya artiklar](inventory-how-register-new-items.md).

> [!NOTE]  
>   Om leverantörsmallar finns för olika leverantörstyper, visas ett fönster när du skapar ett nytt leverantörskort där du kan välja en lämplig mall. Om endast en leverantörsmall finns, då använder nya leverantörskort alltid den mallen.

## <a name="to-create-a-new-vendor-card"></a>Skapa ett nytt leverantörskort.
1. Välj **Leverantörer** på startsidan för att öppna listan över befintliga leverantörer.  
2. I fönstret **Leverantörer** väljer du **Ny**.

    Om fler än en leverantörsmall finns, öppnas ett fönster där du kan välja leverantörsmall. I detta fall, följ nästa två steg.
3. Välj den mall som du vill använda för den nya leverantörskortet i fönstret **Välj en mall för en ny leverantör**.
4. Välj **OK**. Ett nytt leverantörskort öppnas med några ifyllda fält med information från mallen.
5. Fortsätt att fylla i eller ändra fält på leverantörskortet vid behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Om du inte känner till den faktureringsadress som kommer att användas för alla fakturor från en leverantör fyller du inte i fältet **Betalningsleverantörsnr**. Välj i stället betalningsleverantörens nummer när du har skapat en inköpsoffert, order eller ett inköpshuvud.

Leverantören är nu registrerad, och leverantörskortet är klart att användas i inköpsdokument.

Om du vill använda detta leverantörskort som en mall när du skapar nya leverantörskort, så fortsätt med att spara den som en leverantörsmall. Mer information finns i följande avsnitt:

## <a name="to-save-the-vendor-card-as-a-template"></a>Om du vill spara leverantörskortet som en mall
1. I fönstret **leverantörskort** väljer du åtgärden **Spara som mall**. Det **leverantörsmall** fönstret öppnas uppvisar leverantörskortet som mall.
2. Fyll i fälten om det behövs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Om du vill återanvända dimensioner i mallar väljer du fönstret **Dimensioner**. Fönstret **Dimensionsmallar** öppnas och visar de dimensionskoder som ställts in för leverantören.
4. Ändra eller ange dimensionskoder som ska kopplas till nya leverantörskort som skapas med hjälp av mallen.
5. Välj **OK** när du har slutfört den nya leverantörsmallen.  
   Leverantörsmallen läggs till listan över leverantörsmallar, så att du kan använda det för att skapa nya leverantörskort.

## <a name="see-also"></a>Se även
[Inköp](purchasing-manage-purchasing.md)  
[Så här registrerar du inköp](purchasing-how-record-purchases.md)   
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

