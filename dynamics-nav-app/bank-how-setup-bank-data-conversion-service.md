---
title: "Så här ställer du in tjänsten bankdatakonvertering"
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
ms.openlocfilehash: 801e2abee52ec9804028a797e4f330b5e080549a
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-bank-data-conversion-service"></a>Så här ställer du in tjänsten bankdatakonvertering
Du kan exportera betalningsrader från fönstret **Utbetalningsjournal** till en dataström som du sedan överför till din bank för automatisk behandling, så att du inte behöver göra electroniska betalningar individuellt. Mer information finns i [Så här exporterar du betalningar till en bankfil](payables-how-export-payments-bank-file.md).

En global tjänstleverantör för att konvertera betalningsinformation till alla dataformat som din bank kräver är ansluten och redo att aktiveras i Dynamics NAV.

Som ett alternativ till tjänsten Envestnet bankdatafeeder kan du även använda bankdatakonverteringstjänsten till att omvandla en kontoutdragsfil som du får från din bank till en dataström som du kan importera till Dynamics NAV. Mer information finns i [Så här kopplar du betalningar automatiskt och stämmer av bankkonton](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Obs!** Bankdatakonverteringstjänsten kan ha en gräns för antal rader som kan exporteras i en fil. Du får ett felmeddelande om gränsen överskrids. Vi rekommenderar att kontoutdragsfiler inte innehåller fler än 1 000 rader eftersom behandlingstiden i bankdatakonverteringstjänsten annars kan öka markant.

## <a name="to-sign-your-company-up-for-the-bank-data-conversion-service"></a>Så här registrerar du ditt företag för tjänsten bankdatakonvertering.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Serviceinställningar för bankdatakonv.** och välj sedan relaterad länk.  
2. Fönstret **Serviceinställningar för bankdatakonv.** öppnas med tre fält förifyllda med relevanta URL-adresser till leverantören av tjänsten för bankdatakonvertering.

    **Obs!** I demodatabasen CRONUS International Ltd. har fälten Användarnamn och Lösenord fyllts i förväg med information om demonstrationsinloggningen, som du ska ersätta med företaget faktiska information när du registrerar dig för bankdatakonverteringen.
3. I fältet **URL för registrering** väljer du webbläsarknappen för att öppna tjänstleverantörens inloggningssida.  
4. På bankdatatjänstleverantörens registreringssida anger du användarnamnet och lösenord för ditt företags prenumeration på tjänsten, och slutför sedan inloggningen enligt tjänstleverantörens anvisningar.

    Ditt företag är nu registrerat för tjänsten bankdatakonvertering. Fortsätt med att ange användarnamnet och lösenordet som du har angett för tjänsten i de relaterade inställningsfälten i Dynamics NAV.
5. I fönstret **Serviceinställningar för bankdatakonv.** i fältet **Användarnamn** anger du samma värde som du har angett som inloggningsnamn på tjänstleverantörens sida i steg 4.
6. I fältet **Lösenord** anger du samma värde som du angav i fältet **Lösenord** på tjänstleverantörens sida i steg 4.

## <a name="to-encrypt-your-login-information"></a>Så här kan du kryptera dina inloggningsuppgifter
Du rekommenderas att skydda de inloggningsuppgifter som du anger i fönstret **Serviceinställningar för bankdatakonv.**. Du kan kryptera data på servern för Dynamics NAV genom att skapa nya eller importera befintliga krypteringsnycklar som aktiverar på serverinstansen för Dynamics NAV som ansluter till databasen.

1. I fönstret **Serviceinställningar för bankdatakonv.** väljer du åtgärden **Krypteringshantering**.
2. Aktivera krypteringen av dina data i fönstret **Datakrypteringshantering**.

##<a name="to-view-or-update-the-list-of-currently-supported-bank-data-formats"></a>Så här visar eller uppdaterar du listan över bankdataformat som stöds för närvarande
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Serviceinställningar för bankdatakonv.** och välj sedan relaterad länk.
2. I fönstret **Serviceinställningar för bankdatakonv.** väljer du åtgärden **Banknamn – datakonverteringslista** för att öppna listan med banknamn som representerar bankdataformat som stöds av konverteringstjänsten.
3. På sidan **Banknamn – datakonverteringslista** väljer du åtgärden **Uppdatera lista med banknamn**.

Listan över bankdataformat som stöds av tjänsten för bankdatakonvertering uppdateras nu. Det här är listan över banknamn, filtrerade efter landet/regionen, som du kan välja mellan i fältet **Banknamn – Datakonvertering** i fönstret **Bankkontokort**.

**Obs!** Uppdatering av bankdataformat som stöds inträffar också när du väljer eller anger ett värde i fältet **Banknamn – Datakonvertering** på bankkontot.

Du har nu registrerat dig för tjänsten bankdatakonvertering. Fortsätt för att visa inloggningsinformationen på varje bankkonto som ska användas tjänsten.

## <a name="to-set-up-bank-accounts-to-use-the-bank-data-conversion-service"></a>Så här skapar du bankkonton som ska användas för tjänsten bankdatakonvertering
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.
2. Öppna kortet för ett bankkonto som du ska exportera eller importera bankfiler för med hjälp av tjänsten för bankdatakonvertering.
3. På snabbfliken **Överföring** i fältet **Format för betalningsexport** väljer du **Service för bankdatakonvertering - krediteringsöverföring** för att ställa in för betalningsexport.
4. I fältet **Banknamn – Datakonvertering** på bankens dataformat som du registrerade dig för i steg 4 i avsnittet “Registrera dig för tjänsten bankdatakonvertering”.
5. Upprepa steg 1 till och med 4 för andra bankkonton som ska använda bankdatakonverteringstjänsten.

## <a name="see-also"></a>Se även  
[Konfigurera bank](bank-setup-banking.md)  
[Hantera bankkonton](bank-manage-bank-accounts.md)

