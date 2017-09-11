---
title: "Så här ansluter du och kopplar från inkommande dokumentposter från dokument och transaktioner"
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
ms.openlocfilehash: fece4e6e38075db6d394c71418fda82a7aa082e1
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-connect-and-disconnect-incoming-document-records-from-documents-and-entries"></a>Så här ansluter du och kopplar från inkommande dokumentposter från dokument och transaktioner
Du kan lagra externa affärsdokument i  Dynamics NAV genom att koppla dokumentfilerna till de relaterade inkommande dokumentposterna. Om dokumentet, t.ex. en inköpsfaktura, inte ursprungligen skapades som en inkommande dokumentpost kan du fortfarande skapa och koppla en inkommande dokumentpost till den senare. Du kan även bifoga inkommande dokumentfiler till bokförda inköps- och försäljningsdokument och till leverantörs-, kund - och redovisningsposter genom att använda till exempel faktaboxen **Inkommande dokumentfiler** t.ex. i fönstren **Bokförda inköpsfakturor** och **Lev.reskontratransaktioner**.

Från fönstren **Kontoplan** och **Redovisningstransaktioner** kan du använda en sökfunktion för att hitta redovisningsposter för bokförda inköps- och försäljningsdokument som inte har inkommande dokumentposter och sedan länka dem till befintliga poster eller skapa nya centralt med bifogade dokumentfiler. Mer information finns i [Så här söker du efter bokförda dokument utan inkommande dokumentposter](across-how-find-posted-documents-without-income-document-records.md).

Följande tillvägagångssätt visar hur du bifoga en fil till en befintlig inköpsfaktura som inte har skapats från en inkommande dokumentpost och hur du bifogar en fil till en leverantörsreskontrapost. Att bifoga en fil till bokförda inköps- eller försäljningsdokument fungerar på liknande sätt.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Så här skapar du och kopplar en inköpsfaktura från en inköpsfaktura
1. Välj ikonen **söka efter sida eller rapport** i det övre högra hörnet, gå till **Inköpsfakturor** och välj sedan relaterad länk.
2. Markera raden för en inköpsfaktura som du vill bifoga en fil till och välj sedan åtgärden **Skapa inkommande dokument från fil**.
3. Eller markera raden för en inköpsfaktura som du vill bifoga en fil till och välj sedan åtgärden **Bifoga fil**.
4. Markera filen som representerar det inkommande dokumentet i fråga och välj sedan knappen **Öppna** i fönstret **Infoga fil**.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Så här skapar du och kopplar en inköpsfaktura från en leverantörsreskontrapost
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Lev.reskontratransaktioner** och välj sedan relaterad länk.
2. Markera raden för en leverantörsreskontratransaktion som du vill bifoga en fil till och välj sedan åtgärden **Skapa inkommande dokument från fil**.
3. Eller markera raden för en leverantörsreskontratransaktion som du vill bifoga en fil till och välj sedan åtgärden **Bifoga fil**.
4. Markera filen som representerar det inkommande dokumentet i fråga och välj sedan knappen **Öppna** i fönstret **Infoga fil**.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>Så här tar du bort kopplingen från en inkommande dokumentpost till ett bokfört dokument
Du kan ta bort bifogade filer från ej bokförda dokument när som helst genom att radera posten för det inkommande dokumentet. Om dokumentet är bokfört måste du först ta bort kopplingen från den inkommande dokumentposten.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inkommande dokument** och välj sedan relaterad länk.
2. Markera raden för en inkommande dokumentpost som kopplas till ett bokfört dokument som du vill ta bort, och välj sedan åtgärden **Ta bort referens till post**.

Kopplingen till det bokförda dokumentet tas bort. Du kan nu fortsätta med att koppla en annan inkommande dokumentpost till det bokförda dokumentet enligt vad som beskrivs i det här avsnittet..

## <a name="see-also"></a>Se även  
[Bearbeta inkommande dokument](across-process-income-documents.md)  
[Inkommande dokument](across-income-documents.md)  
[Hantera inköp](purchasing-manage-purchasing.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

