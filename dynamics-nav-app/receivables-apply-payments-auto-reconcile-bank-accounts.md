---
title: "Koppla utbetalningar automatiskt och stämma av bankkonton"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 11df387c16e19421090531fd03c209103b9989d9
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="apply-payments-automatically-and-reconcile-bank-accounts"></a>Koppla utbetalningar automatiskt och stämma av bankkonton
Du måste regelbundet stämma av din bank, kundfordringar och konto för kundreskontra i Dynamics NAV genom att koppla betalningar registrerade i ditt bankkonto till deras motsvarande obetalda fakturor och kreditnotor eller andra öppna transaktioner i Dynamics NAV.

Du kan utföra denna aktivitet i fönstret **Betalningsavstämningsjournal** genom att importera ett kontoutdrag eller feed för att snabbt registrera utbetalningarna i Dynamics NAV. En automatisk kopplingsfunktion gäller betalningar till deras relaterade öppna kund- eller leverantörsreskontratransaktioner som baseras på datamatchningar mellan utbetalningtext och transaktionsinformation. Du kan granska och ändra automatiska kopplingar, innan du bokför journalen. Du kan välja att avsluta alla öppna bankkontotransaktioner som relateras till kopplade transaktioner, när du bokför journalen. Det betyder att bankkontot avstäms automatiskt, när alla utbetalningar kopplas.

Om du vill aktivera import av bankutdrag som en bankfeed måste du först skapa och aktivera tjänsten Envestnet Yodlee bankfeed och sedan länka dina bankkonton till relaterade onlinebankkonton. Mer information finns i [Så här konfigurerar du tjänsten Envestnet Yodlee bankfeeder](bank-how-setup-bank-statement-service.md).

**Obs!**: Tjänsten Envestnet Yodlee bankfeeder eller någon annan leverantörs tjänst för bankfeed kanske inte är tillgänglig i systemet. Kontakta din Microsoft-partner om du vill använda en tjänst för bankfeed för att importera kontoutdrag.

Du kan alternativt använda funktionen för bankdatakonvertering om du vill få en bankutdragsfil i något format konverterad till en dataström som du kan importera till Dynamics NAV. Mer information finns i [Så här konfigurerar du bankdatakonverteringstjänsten](bank-how-setup-bank-data-conversion-service.md).

I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.

|Om du vill |Gå till |
|---|----|
|Koppla betalningar för att öppna kund- eller leverantörsreskontratransaktioner genom att importera ett kontoutdrag och stämma av bankkonton när alla betalningar är kopplade. | [Så här stämmer du av betalningar genom att använda automatisk koppling](receivables-how-reconcile-payments-auto-application.md) |
|Koppla betalningar manuellt genom att visa detaljerad information om matchade data och förslag om att öppna kandidattransaktioner att koppla betalningar till. | [Så här granskar och kopplar du betalningar efter automatisk koppling](receivables-how-review-apply-payments-auto-application.md)
|Lös betalningar som inte kan användas automatiskt till dess relaterade öppna transaktion, till exempel för att beloppen skiljer sig, eller för att en artikelrelaterad transaktion inte finns. | [Så här stämmer du av betalningar som inte kan kopplas automatiskt](receivables-how-reconcile-payments-cannot-apply-auto.md)
|Koppla text på betalningar till specifika kund-, leverantörs- eller redovisningskonton för att alltid bokföra återkommande inbetalningar eller kostnader på dessa konton när det inte finns dokument att applicera dem på.| [Så här mappar du text på återkommande betalningar till konton för automatisk avstämning](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)|

## <a name="see-also"></a>Se även
[Hantera kundreskontra](receivables-manage-receivables.md)  
[Hantera försäljning](sales-manage-sales.md)

