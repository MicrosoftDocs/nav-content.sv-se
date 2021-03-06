---
title: Konfigurera datautbyte
description: "Ställa in ramverket för datautbyte i Dynamics NAV."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bd45b6a3d0a611154828a0c9b6a8e39fe1c14635
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-data-exchange"></a>Konfigurera datautbyte
Innan du kan skicka och ta emot elektroniska dokument eller importera och exportera bankfiler måste du konfigurera ramverket för datautbyte för att bearbeta relevanta filerna. Dessutom kanske du måste skapa relaterade feltyper, till exempel huvuddata för kunder som du skickar elektroniska fakturor till eller bankdatakonverteringstjänsten om du vill använda den externa tjänsteleverantören för konvertering av dina bankfiler. Mer information finns i [Utbyta data elektroniskt](across-data-exchange.md).  

 När [!INCLUDE[d365fin](includes/d365fin_md.md)] har konfiguerats för utbyte av data med externa filer kan användare använda konfigurationen i gemensamma affärsuppgifter, till exempel för att skicka och ta emot elektroniska dokument och importera och exportera bankfiler.  

 I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.  

|**För att**|**Gå till**|  
|------------|-------------|  
|Ställ in den förkonfigurerade dokumentväxlingstjänsten för att aktivera att skicka och ta emot elektroniska dokumentet från och till [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Så här konfigurerar du en dokumentväxlingstjänst](across-how-to-set-up-a-document-exchange-service.md)|  
|Ställ in den förkonfigurerade OCR-tjänsten för att omvandla PDF- eller bildfiler till elektroniska dokument som därefter kan konverteras till dokumentposter i [!INCLUDE[d365fin](includes/d365fin_md.md)]|[Så här konfigurerar du Inkommande dokument](across-how-setup-income-documents.md)|  
|Ställ in en av två förkonfigurerade tjänster för att uppdaterade valutakurser ska få de senaste växelkurserna i fönstret **Valutor**.|[Så här uppdaterar du valutakurser](finance-how-update-currencies.md)|  
|Dtäll in olika huvuddata, som företagsinformation, kunder, leverantörer, artiklar och enheter relaterade till mappning av data i [!INCLUDE[d365fin](includes/d365fin_md.md)]|[Så här konfigurerar du utskick och mottagning av elektroniska dokument](across-how-to-set-up-electronic-document-sending-and-receiving.md)|  
|Skapa ett bankkonto, en leverantör och en utbetalningsjournal för SEPA-kreditöverföring.|[Så här: Skapar SEPA-kreditöverföring](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Förbered bankkontoformat, betalningssätt och kundavtal för SEPA-autogiro.|[Så här: Konfigurera SEPA Autogiro](finance-how-to-set-up-sepa-direct-debit.md)|  
|Skapa användarautentisering och URL-adressen för serviceleverantören för bankdatakonvertering som krävs för att få bankfiler konverterade till din banks format.|[Så här ställer du in tjänsten bankdatakonvertering](bank-how-setup-bank-data-conversion-service.md)|  
|Konfigurera och aktivera en extern tjänst som låter dig importera kontoutdrag direkt som bankfeed.|[Så här ställer du in tjänsten bankdatakonvertering](bank-how-setup-bank-data-conversion-service.md)|  
|När bankdatakonverteringstjänsten har aktiverats, länkar du bankkonton i [!INCLUDE[d365fin](includes/d365fin_md.md)]|[Så här skapar du bankkonton](bank-how-setup-bank-accounts.md)|  
|Förbered för att konfigurera en ny datautbytesdefinition för en datafil eller strömma med hjälp av filens XML-schema för att autofylla snabbfliken **Kolumndefinitioner** i fönstret **Definitioner för bokföringsbyte**.|[Så här använder du XML-scheman för att förbereda datautbytesdefinitioner](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)|  
|Konfigurera ramverket för datautbyte så att användare kan ta emot ett nytt inköpsdokumentformat, skicka ett nytt försäljningsdokumentformat, importera en ny bankfil eller göra andra datautbyten.|[Så här konfigurerar du datautbytesdefinitioner](across-how-to-set-up-data-exchange-definitions.md)|  

## <a name="see-also"></a>Se även  
[Utbyta data elektroniskt](across-data-exchange.md).  
[Utbyta data](across-exchange-data.md)   
[Inkommande dokument](across-income-documents.md)  
[Allmänna affärsfunktioner](ui-across-business-areas.md)  

