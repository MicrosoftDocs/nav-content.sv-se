---
title: "Så här skapar du inkommande dokumentposter"
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
ms.openlocfilehash: 10ba191b197be8b98b2d5d5ab9ac4bc3baf0d82b
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-incoming-document-records"></a>Så här skapar du inkommande dokumentposter
I fönstret **Inkommande dokument** använder du olika funktioner för att förhandsgranska utgiftskvitton, hantera OCR-uppgifter och konvertera inkommande dokumentfiler, manuellt eller automatiskt, till relevanta dokument eller journalrader i . De externa filerna kan kopplas till något processteg, inklusive till bokförda dokument och till resulterande leverantörs-, kund- och redovisningstransaktioner.

Om du vill registrera ett externt dokument i | Dynamics NAV måste du först skapa eller slutföra en inkommande dokumentpost. Du kan göra detta manuellt eller så kan du ta ett foto på det externa dokumentet och sedan skapa en inkommande dokumentpost med bildfilen bifogad.

Innan du kan använda funktionen för inkommande dokument måste du utföra de nödvändiga inställningarna. Mer information finns i [Så här skapar du inkommande dokument](across-how-setup-income-documents.md).

## <a name="to-approve-or-reject-an-incoming-document"></a>Så här Godkänn eller avvisa ett inkommande dokument.
Om du inte vill att användare ska skapa fakturor eller redovisningsjournalrader från inkommande dokumentposter om inte dokumenten har godkänts först kan du konfigurera godkännare som måste godkänna transaktionerna innan de kan behandlas.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inkommande dokument** och välj sedan relaterad länk.
2. Markera raden med dokumentet som du vill godkänna eller avvisa, och välj sedan åtgärden **godkänna** eller **avvisa**.

Om du godkänner den inkommande dokumentposten markeras kryssrutan **Släppt** på den inkommande dokumentraden. Användaren som ansvarar för att skapa t.ex inköpsfakturor kan fortsätta med att bearbeta transaktionen.

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a>Så här skapar du en inkommande dokumentpost genom att ta ett foto
**Obs!**: Följande proceduren gäller endast Dynamics NAV för surfplatte- och telefonklienter.

1. Välj panelen **Skapa inkommande dokument från kamera** i appfältet och gå sedan till steg 4.
2. Välj annars alternativknappen på appfältet, välj **Inkommande dokument** och välj sedan **Alla**.
3. I fönstret **Inkommande dokument** väljer du ellipsknappen och sedan **Skapa från kamera**. Kameran på Tablet PC:n eller telefonen aktiveras.
4. Ta ett foto av ett dokument, t.ex. ett inköpskvitto, som du vill bearbeta som ett inkommande dokument, och välj sedan knappen **OK** .

En ny inkommande dokumentpost skapas med bilden bifogad.

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a>Så här bifogar du en bild till en inkommande dokumentpost genom att ta ett foto
**Obs!**: Följande proceduren gäller endast Dynamics NAV för surfplatte- och telefonklienter.

1. Välj alternativknappen på appfältet, välj **Inkommande dokument** och välj sedan **Alla**.
2. Öppna kortet för en befintlig inkommande dokumentpost.
3. I fönstret **Inkommande dokument** väljer du ellipsknappen och sedan **Bifoga fil från kamera**. Kameran på Tablet PC:n eller telefonen aktiveras.
4. Ta ett foto av ett dokument, t.ex. ett inköpskvitto, som du vill bearbeta som ett inkommande dokument, och välj sedan knappen **OK** .

Bilden har bifogats till den inkommande dokumentposten.

## <a name="to-create-an-incoming-document-record-manually"></a>Så här skapar du en inkommande dokumentpost manuellt
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inkommande dokument** och välj sedan relaterad länk.
2. Välj åtgärden **Skapa från fil**.  
3. Välj en fil och välj sedan **Öppna** i fönstret **Infoga fil**.

    Filen kopplas automatiskt.
4. Välj alternativt åtgärden **Ny**.
5. För att bifoga en fil väljer du åtgärden **Bifoga fil**.
6. Markera filen som representerar det inkommande dokumentet i fråga och välj sedan knappen **Öppna** i fönstret **Infoga fil**.
7. I fönstret **Inkommande dokument** fyller du i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

##<a name="see-also"></a>Se även  
[Bearbeta inkommande dokument](across-process-income-documents.md)  
[Inkommande dokument](across-income-documents.md)  
[Hantera inköp](purchasing-manage-purchasing.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

