---
title: "Bokföra inköp"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c03d031e951bc185b18bedaf428d414c1fe2e7d1
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="posting-purchases"></a>Bokföra inköp
I **Bokföringsgrupp** i ett inköpsdokument kan du välja mellan följande bokföringsfunktioner:

- **Bokföra**
- **Förhandsgranska bokföring**
- **Bokför och skriv ut**
- **Testa rapport**
- **Bokför batch-jobb**

När du har fyllt i alla raderna och skrivit in all information på inköpsordern kan du bokföra den, d.v.s. skapa en inleverans och en faktura.

När en inköpsorder bokförs, uppdateras leverantörens konto, redovisningen och artikeltransaktionerna.

För varje inköpsorder skapas en inköpstransaktion i tabellen **Redovisningstransaktion**. Dessutom skapas en transaktion på leverantörens konto i tabellen **Lev.reskontratransaktion** och en redovisningstransaktion på det relevanta kontot för leverantörsskulder. Dessutom kan bokföring av inköpsordern resultera i en momstransaktion och en redovisningstransaktion för rabattbeloppet. Om rabattransaktionen är bokförd eller ej beror på innehållet i fältet **Rabattbokföring** i fönstret **Inköpsinställning**.

För varje inköpsorderrad skapas en artikeltransaktion i tabellen **Artikeltransaktion** (om inköpsraden innehåller artikelnummer) eller en redovisningstransaktion i tabellen **Redovisningstransaktion** (om inköpsraden innehåller ett redovisningskonto). Dessutom registreras inköpsorder alltid i tabellerna **Inleveranshuvud** och **Inköpsfakturahuvud**.

Innan du börjar bokföra kan du välja att skriva ut en testrapport som visar all information på inköpsordern tillsammans med eventuella fel. Om du vill skriva ut rapporten väljer du **Bokföring** och sedan **Testrapport**.

**Viktigt!** När du bokför en order kan du skapa både en inleverans och en faktura. Detta kan göras samtidigt eller oberoende av varandra. Du kan också skapa en delinleverans och en delfaktura genom att fylla i fältet **Ant. att inlevereras** och **Ant. att fakturera** på de enskilda inköpsorderraderna innan du bokför. Observera att du inte kan skapa en faktura för något som inte har inlevererats. Innan du kan fakturera måste du således ha registrerat en inleverans alternativt välja att inleverera och fakturera samtidigt.

Du kan bokföra eller bokföra och skriva ut. Om du väljer Bokför och Skriv ut, skrivs en rapport ut när ordern bokförs. Du kan även välja funktionen **Bokför batch-jobb** som ger dig möjlighet att bokföra fler fakturor samtidigt.

När bokföringen är slutförd tas de bokförda inköpsraderna bort från ordern. Du får ett meddelande när bokföringen är slutförd. Sedan kan du se de bokförda transaktionerna i de olika fönster som innehåller bokförda transaktioner, t.ex. fönsterna **Leverantörsreskontratransaktion**, **Redovisningstransaktion**, **Artikeltransaktioner**, **Inleverans** och **Bokförda inköpsfakturor**.

## <a name="see-also"></a>Se även
[Bokför dokument och journaler](ui-post-documents-journals.md)

