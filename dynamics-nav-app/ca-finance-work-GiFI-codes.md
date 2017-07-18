---
title: "Så här arbetar du med GIFI-koder i Kanada"
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 695bca0a6836c47610210b759ae48af27484761f
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-work-with-gifi-codes-in-canada"></a>Så här arbetar du med GIFI-koder i Kanada
Skatteinformation kan inkludera redovisningskonton, rapporter, resultaträkningar, balansräkningar och rapporter över balanserad vinst och förlust. Skatteinformation grupperas med hjälp av koder. Hanteringen av koder hjälper regeringen att bearbeta information, förbereda sig för elektronisk arkivering och validera skatteinformation elektroniskt. Hanteringen av koder hjälper också statistiska organisationer att arbeta mer effektivt, eftersom den ekonomiska informationen är mer lättillgänglig. Mer information finns i [Webbplatsen för Canada Revenue Agency](http://www.cra-arc.gc.ca/).

Canada Revenue Agency använder det allmänna indexet av koder för ekonomisk information (GIFI) för att elektroniskt samla, verifiera och bearbeta ekonomisk information och skatteinformation. Det är bäst att endast tilldela GIFI-koder för bokföringskonton så att all summering görs av ditt skattförberedelseprogram.

När ett konto är kopplat till en GIFI-kod, rapporteras den till Revenue Agency med den koden. Flera konton kan använda samma GIFI-kod, men varje konto kan endast ha en GIFI-kod.

Du kan exportera information om saldo per GIFI-kod och spara den exporterade filen i Excel, vilket är användbart för att överföra information till ditt skattförberedelseprogram.

## <a name="to-set-up-gifi-codes"></a>Så här skapar du GIFI-koder:
I Dynamics NAV måste du lägga upp GIFI-koder för redovisningskonton, rapporter, balansräkningar, inkomstark och rapporter över balanserad vinst och förlust.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **GIFI-koder** och välj sedan relaterad länk.
2. I fönstret **GIFI-koder** väljer du åtgärden **Ny**.
3. Skapa GIFI-koder, genom att fylla i fälten. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

## <a name="to-associate-gifi-codes-with-gl-accounts"></a>Om du vill koppla GIFI-koder med redovisningskonton
Om du vill rapportera ekonomiska information med GIFI-kod, måste varje GIFI-kod vara kopplad till korrekta konton i kontoplanen.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Kontoplan** och välj sedan relaterad länk.
2. Välj ett relevant redovisningskonto och välj sedan åtgärden **Redigera**.
3. På snabbfliken **Kostnadsredovisning** i fältet **GIFI-kod** väljer du lämplig GIFI-kod.

## <a name="to-view-account-balances-using-the-gifi-code-report"></a>Om du vill visa kontosaldon som använder GIFI-kodrapport
Du kan granska kontosaldon per GIFI-kod, genom att använda rapporten **kontosaldon per GIFI-kod**.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **kontosaldon per GIFI-kod** och välj sedan relaterad länk.
2. Ange vad som ska ingå i rapporten genom att fylla i fälten. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. Välj knappen **Skriv ut** eller **Förhandsgranska**.

## <a name="to-export-balance-information-using-gifi-codes"></a>Så här exporterar du saldoinformation med hjälp av GIFI-koder
Du kan exportera saldoinformation med hjälp av GIFI-koder och spara den exporterade filen i Excel. Du kan ändra, spara eller ta bort filen. Du kan använda den för att överföra information till ditt skattförberedelseprogram.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Exportera information om GIFI till Excel** och välj sedan relaterad länk.
2. Ange vad du vill exportera till Excel, genom att fylla i fälten. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. Välj **OK**.

**Obs!** Excel-filen har följande egenskaper:

* Saldot avrundas till den närmaste procentsatsen, men cellvärdet behåller samma procentsats som i redovisningen.

* Negativa nummer representeras av positiva nummer i hakparenteser. -123 anges därför som (123).

## <a name="see-also"></a>Se även
[Finans](finance-setup.md)   
[Konfigurera Centrala finansiella processer](finance-setup-setup-finance-setup.md)

