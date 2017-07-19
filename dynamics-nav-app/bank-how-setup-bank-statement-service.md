---
title: "Så här konfigurerar du tjänsten Envestnet Yodlee bankfeeder"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 270568214afd2ca8af15f0fa7640337c77ec2f1e
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-envestnet-yodlee-bank-feeds-service"></a>Så här konfigurerar du tjänsten Envestnet Yodlee bankfeeder
Du kan importera elektroniska bankutdrag från banken så att du snabbt kan fylla i fönstret **Betalningsavstämningsjournal** och koppla betalningar och stämma av bankkontot. Mer information finns i [Koppla betalningar automatiskt och stäm av bankkonton](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Obs!**: Tjänsten Envestnet Yodlee bankfeeder eller någon annan leverantörs tjänst för bankfeed kanske inte är tillgänglig i systemet. Kontakta din Microsoft-partner om du vill använda en tjänst för bankfeed för att importera kontoutdrag.

När du har aktiverat bankfeedtjänsten måste du länka det involverade bankkontot till det onlinebankkonto som feeden ska komma från. Du länkar bankkonton till onlinebankkonton i följande olika scenarier:

- Det finns inget bankkonto i Dynamics NAV för ditt onlinebankkonto. Därför skapar du bankkontot genom att länka från onlinebankkontot.
- Det finns ett bankkonto i Dynamics NAV som du vill länka till ett onlinebankkonto.
- Ett länkat bankkonto måste länkas av eftersom du vill sluta använda bankfeedtjänsten för kontot.
- Onlinebankkonton har ändrat och du vill uppdatera informationen om bankkonton i Dynamics NAV.

När bankfeedtjänsten är aktiverad, kan du konfigurera ett bankkonto att automatiskt importera nya kontoutdrag till fönstret **Betalningsavstämningsjournal** varannan timme. Transaktioner för utbetalningar som redan har bokförts som kopplade och/eller avstämda i fönstret **Betalningsavstämningsjournal** kommer inte att importeras. Mer information finns i avsnittet “Att aktivera automatisk import av kontoutdrag”.

**Obs!** Om du använder den assisterade inställningen Konfigurera företag kommer några av stegen i följande procedurer att utföras automatiskt när du kommer till inställningen av företagets bankkonto. Mer information finns i [Välkommen till Dynamics NAV](across-get-started.md).

## <a name="to-enable-the-bank-feed-service"></a>Så här aktiverar du bankfeedtjänsten
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.
2. Öppna det bankkonto som du ska använda för bankfeedtjänsten.
3. I fönstret **Bankkonto** i fältet **Format för bankutdragsimport** väljer du YODLEEBANKFEED.  

Bankfeedtjänsten aktiveras när du länkar ett bankkonto till dess relaterade onlinebankkonto. Visa nästa procedur.  

## <a name="to-create-a-new-linked-bank-account"></a>Så här skapar du ett nytt länkat bankkonto
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.
2. Välj det relevanta bankkontot och välj sedan **Skapa nytt länkat bakkonto**. Fönstret **Länkning av bankkonto** öppnas efter några ögonblick.

    **Obs!** Det här fönstret visar den verkliga webbsidan för tjänsten Envestnet Yodlee bankfeeder. Terminologi och funktionalitet i fönstret kanske inte matchar instruktionerna som tillhandahålls i det här avsnittet.  
3. I fönstret **Länka till onlinebankkonto** i rutan **Länka konto** använd Sökfunktionen för att hitta banken där du har ett eller flera onlinebankkonton.
4. Välj bankens namn. Rutan **Inloggning** öppnas.
5. Ange användarnamnet och lösenordet som du använder för att logga in på onlinebanken och tryck sedan på knappen **Nästa**.  
6. Bankfeedtjänsten förbereder dig på att länka det första onlinebankkontot på den angivna banken till ett nytt bankkonto i Dynamics NAV.

    **Obs!** Om du har fler än ett onlinebankkonto på banken, måste du skapa ytterligare bankkonton i Dynamics NAV för ytterligare onlinebankkonton. Se steg 8 till 10.

    När processen är korrekt slutförd kommer bankens namn att visas i rutan **Mina konton** på fliken **Länkad**. Numret i hakparenteser anger hur många onlinebankkonton som länkades.
7. Välj **OK**.

    Om endast ett onlinebankkonto länkades kommer fönstret **Bankkontokort** för ett nytt bankkonto att öppnas som är ifyllt med namnet på den detta bankkonto. I det här fallet är bankkontolänkninguppgiften slutförd. Allt som återstår är att skapa bankkontot. Mer information finns i [Så här skapar du bankkonton](bank-how-setup-bank-accounts.md).

    Om fler än ett bankkonto länkades kommer fönstret **Länkning av bankkonto** att öppnas med det ytterligare onlinebankkonton som inte ännu är länkade till bankkonton i Dynamics NAV. I detta fall, följ nästa steg.  
8. I fönstret **Länkning av bankkonto** väljer du raden för ett onlinebankkonto och väljer sedan åtgärden **Länka till nytt bankkonto**.

    Fönstret **Bankkontokort** för ett nytt bankkonto kommer att öppnas som är ifyllt med namnet på den detta bankkonto.

    Om ett bankkonto redan finns i Dynamics NAV som du vill länka det ytterligare onlinebankkontot till, följer du nästa steg.  
9. I fönstret **Länkning av bankkonto** väljer du raden för ett onlinebankkonto och väljer sedan åtgärden **Länka till befintligt bankkonto**.
10. I fönstret **Bankkontolista** väljer du det bankkonto som du vill länka till och väljer sedan knappen **OK**.

## <a name="to-link-a-bank-account-to-an-online-bank-account"></a>Så här länkar du ett bankkonto till ett onlinebankkonto
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.
2. Välj raden för ett bankkonto som inte är kopplad till ett onlinebankkonto och välj sedan åtgärden **Länka till onlinebankkonto**. Fönstret **Länka till onlinebankkonto** öppnas med bankens namn ifyllt i rutan **Länka konto**.
3. Välj bankens namn. Rutan **Inloggning** öppnas.
4. Ange användarnamnet och lösenordet som du använder för att logga in på onlinebanken och tryck sedan på knappen **Nästa**.

    Bankfeedtjänsten förbereder dig på att länka ditt bankkontot bankkonto i Dynamics NAV till det relaterade onlinebankkontot.

    När processen är korrekt slutförd kommer bankens namn att visas i rutan **Mina konton** på fliken **Länkad**. Om banken har fler än ett bankkonto, länkas endast det bankkonto som du valde i steg 2.
5. Välj **OK**.

I fönstret **Bankkontolista** markeras kryssrutan **Länkad**.

## <a name="to-unlink-a-bank-account"></a>Så här tar du bort länk till bankkonto
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.  
2. Välj raden för ett länkat bankkonto som du vill ta bort länken till dess relaterade onlinebankkonto för och välj sedan åtgärden **Ta bort länk till onlinebankkonto**.

**Obs!**: Om du väljer **Ja** i bekräftelsedialogrutan, tas länken till onlinebankkontot bort och inloggningsdetaljerna avmarkeras. Om du vill länka bankkontot till onlinebankkonto igen måste du logga in i banken igen. Mer information finns i avsnittet “Så här länkar du ett bankkonto till ett onlinebankkonto“.

## <a name="to-update-bank-account-linking"></a>Så här uppdaterar du länkning till bankkonto
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.
2. Välj det relevanta bankkontot och välj sedan åtgärden **Uppdatera länkning av bankkonto**.

Om problem finns för någon av de länkade bankkontona i fönstret **Bankkontolista** kommer fönstret **Länkning av bankkonto** med information om vilka bankkonton som har problem. Problemen kan bäst lösas genom att ta bort länken till onlinebankkontot och sedan återskapa länken. Mer information finns i avsnittet “Så här länkar du ett bankkonto till ett onlinebankkonto“.

## <a name="to-enable-automatic-import-of-bank-statements"></a>Om du vill aktivera automatisk import av bankutdrag
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bankkonton** och välj sedan relaterad länk.
2. Markera raden för ett länkat bankkonto och välj sedan åtgärden **Inställningar för automatisk import av bankutdrag**.
3. I fönstret **Inställningar för automatisk import av bankutdrag** i fältet **Antal dagar som ingår** anger du hur långt tillbaka i tiden som du får nya banktransaktioner för.

    **Obs!** Det rekommenderas att du ställer in detta värde till 7 dagar eller fler.
4. Markera kryssrutan **Aktiverad**.  
Varje timme kommer fönstret **Betalningsavstämningsjournal** att fyllas i med alla nya utbetalningar som har gjorts på detta onlinebankkonto.

**Obs!** Transaktioner för utbetalningar som redan har bokförts som kopplade och/eller avstämda i fönstret **Betalningsavstämningsjournal** kommer inte att importeras.

## <a name="see-also"></a>Se även  
[Konfigurera bank](bank-setup-banking.md)  
[Hantera bankkonton](bank-manage-bank-accounts.md)  
[Koppla utbetalningar automatiskt och stämma av bankkonton](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Anpassa Dynamics NAV med hjälp av tillägg](ui-extensions.md)

