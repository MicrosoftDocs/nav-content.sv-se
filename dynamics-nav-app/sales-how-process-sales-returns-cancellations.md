---
title: "Så här behandlar du försäljningreturer eller annulleringar"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 92b65379f2ec633712a2b2c0f06615c6de61cc6e
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-sales-returns-or-cancellations"></a>Så här behandlar du försäljningreturer eller annulleringar
Om din kund vill returnera artiklar eller få återbetalning för artiklar eller tjänster du har sålt och få betalning för detta, måste du skapa och bokföra en försäljningskreditnota som anger begärd ändring. För att inkludera rätt uppgifter om försäljningsfakturan kan du skapa försäljningkreditnotan från den bokförda försäljningsfakturan eller använda en kopieringsfunktion.

Förutom den ursprungliga bokförda försäljningsfakturan kan du koppla försäljningskreditnotan till andra försäljningsdokument, t.ex en annan bokförd försäljningfaktura, eftersom kunden också returnerar artiklarna som har levererats med den fakturan.

En retur eller en återbetalning kan relatera till endast några av artiklarna eller tjänsterna på den ursprungliga försäljningsfakturan. I så fall måste du redigera information på raderna i försäljningskreditnotan. När du bokför försäljningskreditnotan, kan försäljningsdokumenten, som påverkas av ändringen återföras, och en återbetalning skapas för kunden.

Du kan skicka den bokförda försäljningskreditnotan till kunden för att bekräfta returen eller avbryt och att meddela att det relaterade värdet ska ersättas, till exempel när artiklar returneras.

## <a name="to-create-a-sales-credit-memo-from-a-posted-sales-invoice"></a>Skapa en ny försäljningskreditnota från en bokförd försäljningsfaktura.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bokförda försäljningsfakturor** och välj sedan relaterad länk.  
2. I fältet **Bokförda försäljningsfakturor** väljer du den bokförda försäljningsfakturan som du vill återföra och väljer sedan åtgärden **Skapa korrigerande kreditnota**.

    De flesta fält på försäljningskreditnotans huvud fylls i med informationen från den bokförda försäljningsfakturan. Du kan redigera alla fält, till exempel med ny information som behövs för returavtalet.
3. Redigera information på raderna enligt avtalet, till exempel antal artiklar som har returnerats, eller beloppet som ska ersättas.
4. Välj åtgärden **Koppla transaktioner**.
5. I fönstret **Koppla kundtrans.** markerar du raden med det bokförda försäljningsdokumentet som du vill koppla försäljningskreditnota till, och väljer sedan åtgärden **Koppla till ID**.

    Numret på försäljningskreditnotan infogas i fältet **Koppla till ID**.  
6. I fältet **Belopp att koppla** anger du det belopp som du vill koppla om det är mindre än det ursprungliga beloppet.

    Längst ned i fönstret **Koppla kundtrans.** kan du se det totala beloppet för att koppla för att återföra alla berörda transaktioner, nämligen när värdet i fältet **Saldo** är noll.  
7. Välj **OK**. När du bokför försäljningskreditnotan kopplas den till de angivna bokförda säljdokumenten.

    När du har skapat eller redigerat de försäljningskreditnotarader som krävs och ett eller flera program anges, kan du fortsätta att bokföra försäljningskreditnotan.
8. Välj åtgärden **Bokför och skicka.**.

Dialogrutan **Bekräftelse för bokför och utskick** öppnas och visar kundens önskad utskicksmetod. Du kan ändra utskicksmetoden genom att välja sökknappen för fältet **Skicka dokument till**. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).

De bokförda försäljningsdokumenten som du vill koppla kreditnotan till återförs nu, och en betalningsåterbetalning kan skapas för kunden. Försäljningskreditnotan tas bort och ersätts med ett nytt dokument i listan över bokförda försäljningskreditnotor.

## <a name="to-create-a-sales-credit-memo-from-scratch"></a>Så här skapar du försäljningskreditnoto från början:
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bokförda försäljningsfakturor** och välj sedan relaterad länk.
2. Välj åtgärden **Ny** för att öppna en ny tom försäljningskreditnota.
3. Ange namnet på en befintlig kund i fältet **Kund**.
4. Välj åtgärden **kopiera dokument**.
5. I fönstret **Kopiera försäljningsdokument** i fältet **Dokumenttyp** väljer du **Bokförd faktura**.
6. Välj **Dokumentnr.** för att öppna fönstret **Bokförda försäljningsfakturor** och välj den bokförda försäljningsfakturan som har rader som du vill återföra.
7. Markera kryssrutan **Beräkna om rader** om du vill att de kopierade bokförda försäljningsfakturaraderna ska uppdateras med ändringar av artikelpris och styckkostnad sedan fakturan bokfördes.
8. Välj **OK**. De kopierade fakturaraderna infogas i säljkreditnotan.
9. Slutför försäljningskreditnotan enligt vad som förklaras i avsnittet "Att skapa en försäljningskreditnota från en bokförd försäljningsfaktura" i det här ämnet.

## <a name="see-also"></a>Se även  
[Hantera försäljning](sales-manage-sales.md)  
[Ställa in försäljning](sales-setup-sales.md)  
[Så här skickar du dokument som e-post](ui-how-send-documents-email.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

