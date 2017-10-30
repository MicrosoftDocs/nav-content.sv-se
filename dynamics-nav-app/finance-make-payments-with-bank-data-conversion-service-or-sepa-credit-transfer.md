---
title: "Välj metoden för elektroniska betalningar"
description: "Behandla betalningar till dina leverantörer genom att exportera en fil tillsammans med betalningsinformation från på journalraderna."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: baafa833fb170fb05f866aac91a05085545aaf97
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Gör betalningar med tjänsten för bankdatakonvertering eller SEPA Kreditöverföring
I fönstret **Betalningsjournal** kan du behandla betalningar till dina leverantörer genom att exportera en fil tillsammans med betalningsinformation från på journalraderna. Du kan sedan överföra filen till den elektroniska banken där relaterade pengaöverföringar bearbetas. [!INCLUDE[d365fin](includes/d365fin_md.md)] stödjer SEPA kreditöverföringar-format, men andra format för elektroniska betalningar i ditt land/din region kan finnas.   

 Om du vill aktivera SEPA-kreditöverföringar måste du först lägga upp ett bankkonto, en leverantör och redovisningsjournalen som utbetalningsjournalen baseras på. Sedan förbereder du betalningar till leverantörer genom att automatiskt fylla i fönstret **Betalningsjournal** med förfallna betalningar med angivna bokföringsdatum.  

> [!NOTE]  
>  När du har verifierat att betalningarna har behandlats korrekt av banken kan du fortsätta att bokföra utbetalningsjournalraderna.  

 I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.   

|**Om du vill**|**Gå till**|  
|------------|-------------|  
|Aktivera funktionen för bankdatakonvertering om du vill få en eventuell bankutdragsfil konverterad till ett format som du kan importera eller få dina exporterad betalningfiler konverterade till det format som din bank kräver.|[Så här ställer du in tjänsten bankdatakonvertering](bank-how-setup-bank-data-conversion-service.md)|  
|Skapa ett bankkonto, en leverantör och en utbetalningsjournal för SEPA-kreditöverföring.|[Så här: Skapar SEPA-kreditöverföring](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Fyll i betalningsjournalen med rader för förfallna betalningar till leverantörer, med alternativet att infoga bokföringsdatum som baseras på förfallodatumet för de relaterade inköpsdokumenten.|[Hantera likviditet](payables-manage-payables.md)|  
|Exportera utbetalningsjournalraderna till en fil i formatet SEPA Krediteringsöverföring.|[Så här exporterar du betalningar till en bankfil](payables-how-export-payments-bank-file.md)|  
|Granska vilka betalningar som har exporterats och till vilka filer.|Kreditöverföringsregister|  
|Bokför betalningarna när den elektroniska betalningen har behandlats utan problem av banken.|[Arbeta med redovisningsjournaler](ui-work-general-journals.md)|  

## <a name="see-also"></a>Se även  
[Så här ställer du in tjänsten bankdatakonvertering](bank-how-setup-bank-data-conversion-service.md)  
[Så här: Skapar SEPA-kreditöverföring](finance-how-to-set-up-sepa-credit-transfer.md)  
[Hantera likviditet](payables-manage-payables.md)   
[Arbeta med redovisningsjournaler](ui-work-general-journals.md)  
[Samla in betalningar med SEPA-autogiro](finance-collect-payments-with-sepa-direct-debit.md)   

