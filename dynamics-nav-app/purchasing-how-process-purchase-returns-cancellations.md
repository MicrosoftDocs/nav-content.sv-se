---
title: "Så här behandlar du inköpsreturer eller annulleringar"
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
ms.openlocfilehash: 94067fb3d10975c1db29d2e3f1d5d6373fcbf9f2
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-purchase-returns-or-cancellations"></a>Så här behandlar du inköpsreturer eller annulleringar
Om du vill returnera artiklar till leverantören eller annullera tjänster som du har köpt, kan du skapa och bokföra en inköpskreditnota som anger begärd ändring med hänsyn till den ursprungliga inköpfakturan. För att inkludera rätt uppgifter om inköpsfakturan kan du skapa inköpskreditnotan från den bokförda inköpsfakturan eller använda en kopieringsfunktion.

Vanligtvis skapar du en inköpskreditnota som reaktion på en kreditnota som skickas till dig av en leverantör. Inköpskreditnotan fungerar som din interna dokumentation över kreditnotabearbetningen i redovisningssyfte.

Ändring kan vara kopplad till alla produkter på den ursprungliga inköpfakturan eller bara till vissa av produkterna. Därmed kan du delvis returnera mottagna artiklar eller begära delvis återbetalning av mottagna tjänster. I så fall måste du redigera den kopierade informationen om inköpsfakturan.

Förutom den ursprungliga bokförda inköpsfakturan kan du koppla inköpskreditnotan till andra inköpsdokument, t.ex en annan bokförd inköpsfaktura, eftersom du också returnerar artiklarna som har levererats med den fakturan.

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Skapa en ny inköpskreditnota från en bokförd inköpsfaktura.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inköpskreditnota** och välj sedan relaterad länk.  
2. I fältet **Bokförda inköpsfakturor** väljer du den bokförda inköpsfakturan som du vill återföra och väljer sedan åtgärden **Skapa korrigerande kreditnota**.

    De flesta fält på inköpskreditnotans huvud fylls i med informationen från den bokförda inköpsfakturan. Du kan redigera alla fält, till exempel med ny information som behövs för returavtalet.
3. Redigera information på raderna enligt avtalet, till exempel antal artiklar som har returnerats, eller beloppet som ska ersättas.
4. Välj åtgärden **Koppla transaktioner**.
5. I fönstret **Koppla leverantörstrans.** markerar du raden med det bokförda inköpsdokumentet som du vill koppla inköpskreditnota till, och väljer sedan åtgärden **Koppla till ID**. Numret på inköpskreditnotan infogas i fältet **Koppla till ID**.
6. I fältet **Belopp att koppla** anger du det belopp som du vill koppla om det är mindre än det ursprungliga beloppet.

    Längst ned i fönstret **Koppla leverantörstrans.** kan du se det totala beloppet för att koppla för att återföra alla berörda transaktioner, nämligen när värdet i fältet **Saldo** är noll.
7. Välj **OK**. När du bokför inköpskreditnotan kopplas den till de angivna bokförda inköpsdokumenten.

    När du har skapat eller redigerat de inköpskreditnotarader som krävs och ett eller flera program anges, kan du fortsätta att bokföra inköpskreditnotan.
8. Välj åtgärden **Bokföra**.

De bokförda inköpsfakturorna som du koppla kreditnotan till återförs nu. Om du redan har betalt den ursprungliga fakturan ska leverantören nu återbetala betalningen till dig. Om kreditnotan endast är för en del av produkten på den ursprungliga fakturan, kan du endast betala återstående belopp på den ursprungliga inköpsfakturan för att stänga den.

Inköpskreditnotan tas bort och ersätts med ett nytt dokument i listan över bokförda inköpskreditnotor.

## <a name="to-create-a-purchase-credit-memo-from-scratch"></a>Så här skapar du inköpskreditnoto från börjanr:
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bokförda inköpsfakturor** och välj sedan relaterad länk.
2. Välj åtgärden **Ny** för att öppna en ny tom inköpskreditnota.
3. Ange namnet på en befintlig leverantör i fältet **Leverantör**.
4. Välj åtgärden **kopiera dokument**.
5. I fönstret **Kopiera inköpsdokument** i fältet **Dokumenttyp** väljer du **Bokförd faktura**.
6. Välj **Dokumentnr.** för att öppna fönstret **Bokförda inköpsfakturor** och välj den bokförda inköpsfakturan som har rader som du vill återföra.
7. Markera kryssrutan **Beräkna om rader** om du vill att de kopierade bokförda inköpsfakturaraderna ska uppdateras med ändringar av artikelpris och styckkostnad sedan fakturan bokfördes.
8. Välj **OK**. De kopierade fakturaraderna infogas i inköpskreditnotan.
9. Slutför inköpskreditnotan enligt vad som förklaras i avsnittet "Att skapa en inköpskreditnota från en bokförd inköpsfaktura" i det här ämnet.

## <a name="see-also"></a>Se även
[Hantera inköp](purchasing-manage-purchasing.md)  
[Så här registrerar du inköp](purchasing-how-record-purchases.md)  

