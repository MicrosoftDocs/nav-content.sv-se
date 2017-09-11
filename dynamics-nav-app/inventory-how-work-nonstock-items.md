---
title: "Så här arbetar du med Ej lagerförda artiklar"
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 6d99e06c167d3b86db97883c02c8bf5cd746ae10
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---

# Så här arbetar du med Ej lagerförda artiklar
Du kan erbjuda vissa artiklar till dina kunder för deras bekvämlighet, som du inte vill hålla i lager, tills du börjar sälja dem. När du vill börja hålla sådana artiklar i lager, kan du konvertera dem till vanliga artikelkort på två sätt.

- Från en ej lagerförd artikel skapar du ett nytt lagerkort baserat på en mall.
- Från en försäljningsorderrad med ett tomt fält **Artikel** väljer du en ej lagerförd artikel. När du bokför försäljningen, skapas ett artikelkort automatiskt för den ej lagerförda artikeln.

**Obs**: Du kan inte välja en ej lagerförd artikel från fönstret **Försäljningsfaktura**. Du kan välja en ej lagerförd artikel från fönstret **Försäljningsoffert** men den ej lagerförda artikeln kommer inte att omvandlas till en vanlig artikel när du använder funktionen **Gör beställning**.

En ej lagerförd artikel har vanligtvis artikelnumret från den leverantör som levererar den. Om du vill aktivera konvertering av ett kort för en ej lagerförd artikel till ett vanligt artikelkort måste du först ställa in hur leverantörens artikelnumrering konverteras till din egen artikelnumrering.   

## Så här skapar du en ej lagerförd artikel
Kort för ej lagerförd artikel har mycket mindre information än normala artikelkort, eftersom du bara använder dem för att erbjuda på offerter och på andra sätt. Därför måste de konverteras till normala artikelkort, innan du kan bokföra försäljningstransaktioner för dem.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Ej lagerförda artiklar** och välj sedan relaterad länk.
2. Välj åtgärden **Ny**.
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

## Så här ställer du in hur ej lagerförda artikelnummer konverteras till ditt eget nummer  
Om du vill aktivera konvertering av ett kort för en ej lagerförd artikel till ett vanligt artikelkort måste du först ställa in hur leverantörens artikelnumrering konverteras till dit eget nummerformat.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inställning av ej lagerförda artiklar** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs.

## Om du vill omvandla en ej lagerförd artikel till en normal artikel
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Ej lagerförda artiklar** och välj sedan relaterad länk.
2. Öppna kortet för den ej lagerförda artikeln som du vill konvertera till en normalt artikel.
3. I fönstret **Ej lagerförd artikelkort** väljer du åtgärden **Skapa artikel**.

Ett nytt artikelkort förifyllt med information från den ej lagerförda artikeln och en relevant artikelmall skapas. Du kan sedan ange eller redigera fält på det nya artikelkortet vid behov. Mer information finns i [Så här registrerar du nya produkter](inventory-how-register-new-products.md).

## Om du vill sälja en ej lagerförd artikel och konvertera den till en normal artikel
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Försäljningsorder** och välj sedan relaterad länk.
2. Välj åtgärden **Ny**. Fyll i övriga fält på snabbfliken **Allmänt** som för alla andra försäljningsorder.
3. På en ny försäljningsrad lämnar du fältet **Artikel** tomt, väljer **Rad**, **Funktioner** och väljer sedan **Ej lagerförd artikel**.

    Den ej lagerförda artikeln omvandlas till en normal artikel Ett nytt artikelkort förifyllt med information från den ej lagerförda artikeln och en relevant artikelmall skapas.
4. Markera den ej lagerförda artikel som du vill visa i fönstret **Ej lagerförda artiklar** och klicka på **OK**.
5. När försäljningsordern är slutförd väljer du åtgärden **Bokföra**.

Du kan sedan ange eller redigera fält på det nya artikelkortet vid behov. Mer information finns i [Så här registrerar du nya produkter](inventory-how-register-new-products.md).

**Obs!**: En korsreferenspost för artikel skapas automatiskt för den leverantör som levererar artikeln mellan leverantörens artikelnummer och det nya artikelnumret.

## Se även
[Så här registrerar du nya produkter](inventory-how-register-new-products.md)  
[Hantera lager](inventory-manage-inventory.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

