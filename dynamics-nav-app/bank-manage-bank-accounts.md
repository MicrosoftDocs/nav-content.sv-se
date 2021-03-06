---
title: Hantera bankkonton
description: "Du måste regelbundet stämma av banktransaktioner i Dynamics NAV med relaterade banktransaktioner i dina bankkonton."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: cd33af7062b5a8e75937f8750e09414f734d8c04
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="managing-bank-accounts"></a>Hantera bankkonton
Du måste regelbundet stämma av dina banktransaktionerna i [!INCLUDE[d365fin](includes/d365fin_md.md)] med de relaterade transaktionerna på dina bankkonton i din bank och sedan bokföra saldot till ditt bankkonto. Du kan utföra denna aktivitet antingen som en del av bearbetning av betalningarna som representeras på kontoutdraget i **Betalningsavstämningsjournal**. Eller så kan du utföra aktiviteten separat från betalningsbehandling i fönstret **Bankkontoavstämning** som stöder checktransaktioner. I båda fallen fyller du i fönstren genom att importera kontoutdraget till [!INCLUDE[d365fin](includes/d365fin_md.md)].

Ibland kan du överföra belopp mellan bankkontot i [!INCLUDE[d365fin](includes/d365fin_md.md)] för att visa överföringar på din bank. Du utför denna aktivitet i fönstret **redovisningsjournal** på olika sätt beroende på pengarnas valuta.

Innan du kan hantera bankkonton, måste du registrera varje bankkonto som bankkontokort. Dessutom måste du skapa elektroniska tjänster som du kan använda för kontoutdragsimport-och betalningsfilexport. Mer information finns i [Skapa bankkonton](bank-setup-banking.md).

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.

| Om du vill | Gå till |
| --- | --- |
| Stämma av bankkonton i samband med betalningsbehandling i fönstret **Betalningsavstämningsjournal**. |[Koppla utbetalningar automatiskt och stämma av bankkonton](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Du kan stämma av bankkonton inklusive checktransaktioner som en separat aktivitet i fönstret **Bankkontoavstämning**. |[Så här stämmer du av bankkonton separat](bank-how-reconcile-bank-accounts-separately.md) |
| bokföra överföringar mellan bankkonton i samma valuta eller olika valutor. |[Så här överför du banktillgångar](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a>Se även
[Ställa in bankverksamhet](bank-setup-banking.md)  
[Hantera kundreskontra](receivables-manage-receivables.md)  
[Hantera Leverantörsreskontra](payables-manage-payables.md)    
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Allmänna affärsfunktioner](ui-across-business-areas.md)  

