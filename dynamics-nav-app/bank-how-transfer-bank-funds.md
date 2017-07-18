---
title: "Så här överför du banktillgångar"
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
ms.openlocfilehash: f34bef80c64cbad0a0b20d4d021cefbdc5a1cb64
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-transfer-bank-funds"></a>Så här överför du banktillgångar
Ibland kan du behöva överföra ett belopp från ett bankkonto till ett annat. För att göra detta måste du bokföra en transaktion i redovisningsjournalen. Uppgiften varierar beroende på om bankkontona använder samma valuta eller olika valutor.

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a>Så här bokför du en överföring mellan bankkonton med samma valutakod
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournal** och välj sedan relaterad länk.
2. Fyll i fälten **Bokföringsdatum** och **Verifikationsnr** på en . .
3. Ange **Bankkonto** i fältet **Kontotyp**.
4. I fältet **Bankkontonr.** väljer du den bank som du vill överföra pengarna från.
5. Ange det belopp som ska överföras i fältet **Belopp**.
6. I fältet **Motkontotyp** väljer du **Bankkonto**.
7. I fältet **Motkonto** väljer du det bankkonto som du vill överföra pengarna till.
8. Bokför journalen.

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a>Så här bokför du överföringar mellan bankkonton med olika valutakoder
För att överföra pengar mellan bankkonton som använder olika valutor måste du bokföra två redovisningsjournalrader.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournal** och välj sedan relaterad länk.
2. Skapa två journalrader och fyll i fälten **Bokföringsdatum** och **Verifikationsnr**. .
3. På den första journalraden anger du **Bankkonto** i fältet **Typ**.
4. I fältet **Bankkontonr.** väljer du det bankkonto som du vill överföra pengarna från.
5. I fältet **Belopp** anger du beloppet i samma valuta som bankontot. Ange kreditbelopp med ett minustecken. Ange debetbelopp utan ett minustecken.
6. I fältet **Motkontotyp** väljer du **Bankkonto**.
7. I fältet **Motkonto** väljer du det bankkonto som du vill överföra pengarna till.
8. På den andra journalraden anger du **Bankkonto** i fältet **Typ**.
9. I fältet **Bankkontonr.** väljer du det bankkonto som du vill överföra pengarna till.
10. I fältet **Belopp** anger du beloppet i samma valuta som bankontot. Ange kreditbelopp med ett minustecken. Ange debetbelopp utan ett minustecken.
11. I fältet **Motkontotyp** väljer du **Bankkonto**.  
12. I fältet **Motkonto** väljer du det bankkonto som du vill överföra pengarna från.

    **Obs!** Om de valutakurser som används i journalen inte är samma som valutakurserna i fönstret **Valutakurser** skapar du en tredje rad för valutavinsten eller valutaförlusten. Ange **Redovisningskonto** i fältet **Kontotyp**. Ange numret för redovisningskontot för valutavinster och valutaförluster i fältet **Kontonr**. . Ange valutavinsten eller valutaförlusten i fältet **Belopp** med eller utan ett minustecken för respektive kredit och debet.
13. Bokför journalen.

## <a name="see-also"></a>Se även  
[Hantera bankkonton](bank-manage-bank-accounts.md)  
[Konfigurera bank](bank-setup-banking.md)  
[Arbeta med redovisningsjournaler](ui-work-general-journals.md)

