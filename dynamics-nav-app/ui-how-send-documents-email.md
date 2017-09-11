---
title: "Så här skickar du dokument som e-post."
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: e4476c2ab903001017dcd6c8bdaa84892ba79c9e
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-send-documents-by-email"></a>Så här skickar du dokument som e-post.
För att meddela innehållet i affärsdokument snabbt till dina affärspartners, till exempel betalningsinformationen på försäljningsdokument till kunder, kan du använda funktionen Rapportlayout för att definiera dokumentspecifikt innehåll som infogas i e-postbrödtexter automatiskt.

Om du vill aktivera e-post i Dynamics NAV, startar du assisterad installation för **Konfigurera e-post** på startsidan.

Du kan e-posta praktiskt taget alla dokumenttyper som bilagor till e-postmeddelanden direkt från fönstret om du vill visa dokument. Förutom bilagan kan du skapa dokumentspecifika e-postbrödtexter med viktig information från dokumentet föregås av standardtext som hälsar e-postmottagaren och introducerar själva dokumentet. Om du vill erbjuda dina kunder att betala elektroniskt för försäljningar med en utbetalningtjänst, till exempel PayPal, kan du också ha PayPal-information och hyperlänk infogade i e-postbrödtexten.

Från alla dokument som stöds börjar du att e-posta genom att välja åtgärden **Skicka** på bokförda dokument, eller åtgärden **Bokför och skicka** på ej bokförda dokument.

Om fältet **E-posta** i fönstret **Skicka dokument till** anges till **Ja (fråga efter inställningar)** och sedan öppnas fönstret **Skicka e-post** med kontaktperson ifylld i fältet **Till:** och dokument som är bifogat som en PDF-fil. I fältet **brödtext** kan du antingen skriva in en text manuellt, eller också kan du fylla i fältet med en dokumentspecifik e-postbrödtext som du har ställt in.

Efterföljande procedur beskriver hur du ställer in rapporten **Försäljning - faktura** att användas för dokumentspecifika e-postbrödtexter, när du e-postar bokförda försäljningsfakturor.

## <a name="to-set-up-a-document-specific-email-body-for-sales-invoices"></a>Så här skapar du en dokumentspecifik e-postbrödtext för försäljningsfakturor
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Rapportval, försäljning** och välj sedan relaterad länk.
2. I fönstret **Rapportval, försäljning** i fältet **Användning** väljer du **Faktura**.
3. På en ny rad i fältet **Rappport-ID** väljer du t.ex. standardrapport 1306.
4. Markera kryssrutan **Använd för e-postbrödtex**.
5. Välj fältet **Layout-ID för brödtext i e-post** och välj en tillgängliga layouter från fönstret **Anpassade rapportlayouter**.
6. Rapportlayouter definierar både formatet och innehållet i e-postbrödtexten, inklusive standardtexten som föregår den centrala dokumentinformationen i e-postbrödtexten.
7. Om du vill visa eller redigera den layout som e-postbrödtexten baseras på väljer du åtgärden **Redigera layouter** i fönstret **Anpassade rapportlayouter**.
8. Om du vill erbjuda dina kunder att betala elektroniskt för försäljningar kan du konfigurera relaterad utbetalningtjänst, till exempel PayPal, och sedan ha PayPal-information och hyperlänk infogade i e-postbrödtexten. Mer information finns i [Så här aktiverar du kundbetalningar via PayPal](sales-how-enable-customer-payments-paypal.md).
9. Välj **OK**.

Nu när du till exempel väljer åtgärden Skicka i fönstret **Bokförd försäljningsfaktura** kommer e-postbrödtexten att innehålla information om dokumentet i rapport 1306 som föregås av utformad standardtext enligt den rapportlayout du valde i steg 5.

Efterföljande procedur beskriver hur du skickar en bokförd försäljningsfaktura som ett e-postmeddelande med dokumentet bifogat som en PDF-fil och med dokumentspecifik e-postbrödtext.
## <a name="to-send-documents-by-email"></a>Så här skickar du dokument som e-post
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bokförda försäljningsfakturor** och välj sedan relaterad länk.
2. Markera den relevanta försäljningsfakturan, välj åtgärden **Skicka**. Fönstret **Skicka dokument till** öppnas.
3. I fältet **E-post** väljer du **Ja (fråga efter inställningar)**. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).
4. Välj **OK**. Fönstret **Skicka e-post** öppnas.
5. I fältet **Till:** anger du en giltig e-postadress. Standardvärdet är kundens e-postadress.
6. Ange en e-postadress i fältet **Kopia** för att skicka en kopia av e-postmeddelandet till en annan mottagare.
7. Ange en e-postadress i fältet **Dold kopia** för att skicka en kopia av e-postmeddelandet till en annan mottagare utan att e-postadressen och namnet visas för andra mottagare.
8. Ange ett beskrivande ämnestext i fältet **Ämne**. Standardvärdet är kundnamnet och fakturanumret.
9. I fältet **Bilaga** är den genererade fakturan bifogad som standard som en PDF-fil. Välj uppslagningknappen för att öppna filen eller bifoga en annan.
10. Ange ett kort meddelande till mottagaren i fältet **Text**.

    Om en dokumentspecifik e-postbrödtext anges i fönstret **Rapportval - försäljning** kommer fältet **Brödtext** att fyllas i automatiskt. Mer information finns i avsnittet “Så här skapar du en dokumentspecifik e-postbrödtext för försäljningsfakturor” i detta ämne.
11. Markera kryssrutan **Redigera i Outlook Web App** för att öppna e-postmeddelande i e-postprogrammet för Office 365.
12. Välj knappen **OK** för att skicka e-postmeddelandet.

**Obs!** Om du behöver inte ange e-postinställningar varje gång du e-postar ett dokument, kan du välja alternativet **Ja (använd standardinställningar)** i fältet E-post i fönstret **Skicka dokument till**. I så fall kommer inte fönstret **Skicka e-post** att öppnas. Se steg 4. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).

## <a name="see-also"></a>Se även  
[Arbeta med Dynamics NAV](ui-work-product.md)  
[Så här fakturerar du försäljning](sales-how-invoice-sales.md)

