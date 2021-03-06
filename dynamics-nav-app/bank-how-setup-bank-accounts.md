---
title: Skapa bankkonton
description: "Du kan stämma av bankkonton i Dynamics NAV med utdrag från banken."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: feed, stream
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3581615fe94006aa9245f5e66fe6cf475b22acfb
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bank-accounts"></a>Så här skapar du bankkonton
Du använder bankkonton i [!INCLUDE[d365fin](includes/d365fin_md.md)] för att hålla reda på dina banktransaktioner. Konton kan definieras i den lokala valutan eller i en utländsk valuta. När du har skapat bankkonton kan du också använda funktionen för utskrift av checkar.

## <a name="to-set-up-bank-accounts"></a>Så här skapar du bankkonton
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Bankkonton** och välj sedan relaterad länk.
2. I fönstret **Bankkonton** väljer du åtgärden **Ny**.
3. Fyll i fälten om det behövs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> Så här fyller du i fältet **Saldo** med en ingående balans, du måste bokföra en bankkontotransaktion med beloppet i fråga. Du kan göra detta genom att utföra en bankkontoavstämning. Mer information finns i [Så här stämmer du av bankkonton separat](bank-how-reconcile-bank-accounts-separately.md). Alternativt kan du implementera den ingående balansen som en del av skapande av allmänna data i nya företag med hjälp av den assisterade konfigurationen **Migrera affärsdata**. Mer information finns i [Välkommern till [!INCLUDE[d365fin](includes/d365fin_md.md)](index.md).

## <a name="to-set-up-your-bank-account-for-import-or-export-of-bank-files"></a>Så här skapar du ett bankkonto för import eller export av bankfilerna
Fälten på snabbfliken **Överför** i fönstret **Bankkontokort** är relaterade till import och export av bankfeeds och filer. Mer information finns i [Så här konfigurerar du bankdatakonverteringstjänsten](bank-how-setup-bank-data-conversion-service.md).

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Bankkonton** och välj sedan relaterad länk.
2. Öppna kortet för ett bankkonto som du ska exportera eller importera bankfiler.
3. I snabbfliken **Överför** fyller du i nödvändiga fält. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Andra filexporttjänster och deras format kräver olika inställningsvärden i fönstret **bankkontokort**. Du får information om vilka inställningsvärden som är fel eller saknas när du försöker exportera filen. Så läs de korta beskrivningarna av fälten eller se relaterad procedur i närliggande ämnen. Till exempel exportera en betalningsfil för nordamerikansk elektronisk överföring kräver att både fältet **Sista kundremissnr.** och fältet **Transitnr.** fylls i. Mer information finns i [Så här exporterar du betalningar till en bankfil](payables-how-export-payments-bank-file.md).

## <a name="to-set-up-vendor-bank-accounts-for-export-of-bank-files"></a>Så här skapar du leverantörsbankkonto för export av bankfiler
Fälten på snabbfliken **Överför** i fönstret **Leveraqntörsbankkontokort** är relaterade till export av bankfeeds och filer. Mer information finns i [Så här skapar du tjänsten för Bankdatakonvertering](bank-how-setup-bank-data-conversion-service.md) och [Så här exporterar du betalningar till en bankfil](payables-how-export-payments-bank-file.md).

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Leverantör** och välj sedan relaterad länk.
2. Öppna kortet för en leverantör vars bankkonto som du ska exportera betalningsbankfiler till.
3. Välj åtgärden **bankkonton**.
3. I fönstret**Leverantörsbankkontokort** på snabbfliken **Överför** fyller du sedan de fält som behövs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-the-opening-balance-on-new-bank-accounts"></a>Ange den ingående balansen för nya bankkonton


## <a name="see-also"></a>Se även
[Ställa in bankverksamhet](bank-setup-banking.md)  
[Hantera bankkonton](bank-manage-bank-accounts.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

