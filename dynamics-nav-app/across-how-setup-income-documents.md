---
title: "Så här konfigurerar du Inkommande dokument"
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
ms.openlocfilehash: 2bce97c76876c86a576ec6a281a306a46881027c
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-incoming-documents"></a>Så här konfigurerar du Inkommande dokument
Om du skapar redovisningsjournalrader från inkommande dokumentposter måste du ange vilken journalmall och batch som ska användas i fönstret **Inställning av inkommande dokument**.

Om du inte vill att användare ska skapa fakturor eller redovisningsjournalrader från inkommande dokumentposter om inte dokumenten har godkänts först, måste du konfigurera godkännare i fönstret **Godkännare för inkommande dokument**.

För att omvandla PDF- och bildfiler till elektroniska dokument som du kan konverteras till, till exempel,inköpsfakturor inne i Dynamics NAV måste du först konfigurera OCR-funktionen och aktivera tjänsten.

När funktionen för Inkommande dokument är inställd, kan du använda olika funktioner för att förhandsgranska utgiftskvitton, hantera OCR-uppgifter och konvertera inkommande dokumentfiler, manuellt eller automatiskt, till relevanta dokument eller journalrader i . De externa filerna kan kopplas till något processteg, inklusive till bokförda dokument och till resulterande leverantörs-, kund- och redovisningstransaktioner. Mer information finns i [Så här bearbetar du inkommande dokument](across-process-income-documents.md).

## <a name="to-set-up-the-incoming-documents-feature"></a>Så här konfigurerar du funktionen för inkommande dokument
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inställning av inkommande dokument** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

## <a name="to-set-up-approvers-of-incoming-document-records"></a>Så här konfigurerar du godkännare för inkommande dokument
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inställning av inkommande dokument** och välj sedan relaterad länk.  
2. I fönstret **Inställning av inkommande dokument** väljer du åtgärden **Godkännare**.

    Fönstret **Godkännare för inkommande dokument** visar alla användare som är inställda i Dynamics NAV.  
3. Markera en eller flera användare som kan godkänna ett inkommande dokument, innan en relaterat dokumentet eller journalrad kan skapas.

När godkännare har konfigurerats i fönstret **Godkännare för inkommande dokument** kan endast dessa användare godkänna ett inkommande dokument om kryssrutan **Kräv godkännande för att skapa** i fönstret **Inställning av inkommande dokument** är markerad.

**Obs!** Denna inställning av godkännande är inte relaterad till arbetsflöden för godkännande. Mer information finns i [Så här använder du arbetsflöden för godkännande](across-how-use-approval-workflows.md).

## <a name="to-set-up-an-ocr-service"></a>Så här konfigurerar du en OCR-tjänst
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **OCR-serviceinställningar** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.


## <a name="to-encrypt-your-login-information"></a>Så här kan du kryptera dina inloggningsuppgifter
Du rekommenderas att skydda de inloggningsuppgifter som du anger i fönstret **OCR-serviceinställningar**. Du kan kryptera data på servern genom att skapa nya eller importera befintliga krypteringsnycklar som aktiverar på serverinstansen med anslutningen till databasen.

1. I fönstret **OCR-serviceinställningar** väljer du åtgärden **Krypteringshantering**.
2. Aktivera krypteringen av dina data i fönstret **Datakrypteringshantering**.

## <a name="see-also"></a>Se även  
[Bearbeta inkommande dokument](across-process-income-documents.md)  
[Inkommande dokument](across-income-documents.md)  
[Hantera inköp](purchasing-manage-purchasing.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

