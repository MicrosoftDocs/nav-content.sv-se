---
title: "Använd OCR för att göra PDF-dokument till E-fakturor | Microsoft Docs"
description: "Beskriver hur du kan använda en OCR-tjänst för att omvandla inkommande PDF-filer eller bildfiler till elektroniska dokument i Financials."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 11/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: f002a3975ecb6efe851cc9ac9774626f63bf760b
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-use-ocr-to-turn-pdf-and-image-files-into-electronic-documents"></a>Så här använder du OCR för att omvandla PDF- och bildfiler till elektroniska dokument
Från PDF eller bildfiler som du får från dina handelspartner kan du låta en extern OCR-tjänst (Optical Character Recognition) skapa elektroniska dokument som du kan konvertera till dokumentposter i [!INCLUDE[d365fin](includes/d365fin_md.md)]. När du exempelvis tar emot en faktura i PDF-format från leverantören, kan du skicka den till OCR-tjänsten från fönstret **Inkommande dokument**. Detta beskrivs i den första proceduren.

Ett alternativ till att skicka filen från **Inkommande dokument**-fönstret är att skicka filen till OCR-tjänstn med e-post. När du sedan får tillbaka det elektroniska dokumentet skapas en relaterad inkommande dokumentpost automatiskt. Detta beskrivs i den andra proceduren.

Efter några sekunder får du tillbaka filen från OCR-tjänsten som en elektronisk faktura som kan omvandlas till en inköpsfaktura för leverantören. Detta beskrivs i den tredje proceduren.

Eftersom OCR baseras på optisk läsning är det troligt att OCR-tjänsten tolkar tecknen i dina PDF- eller bildfiler fel första gången dokument från till exempel en viss leverantör behandlas. Det går kanske inte tolka företagslogotypen som leverantörens namn eller summan på ett kvitto kan misstolkas på grund av layouten. Du kan undvika att dessa fel vidarebefordras genom att korrigera felen i en separat version av **Inkommande dokument**-fönstret. Sedan skickar du korrigeringarna tillbaka till OCR-webbtjänsten för att utbilda den till att tolka de specifika tecknen korrekt nästa gång den behandlar ett PDF eller bilddokument för samma leverantör. Mer information finns i avsnittet"Så här utbildar du OCR-tjänsten till att undvika fel".

Trafiken av filer till och från OCR-tjänsten behandlas av en dedikerad jobbköpost, som skapas automatiskt när du aktiverar den relaterade tjänstkopplingen. Mer information finns i [Så här skapar du inkommande dokument](across-how-setup-income-documents.md).

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-from-the-incoming-documents-window"></a>Så här skickar du en PDF- eller bildfil till OCR-tjänsten från fönstret **Inkommande dokument**
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inkommande dokument** och välj sedan relaterad länk.
2. Skapa en ny inkommande dokumentpost och bifoga filen. Mer information finns i [Så här skapar du inkommande dokumentposter](across-how-create-income-document-records.md).  
3. Markera sedan en eller flera rader i fönstret **Inkommande dokument** och välj sedan åtgärden **Skicka till jobbkö**.

    Värdet i fältet **OCR-status** ändras till **Klar**. Bifogad PDF eller bildfil skickas till OCR-servicen av jobbkön enligt schemat, förutsatt att inga fel finns.
4. Markera alternativt en eller flera rader i fönstret **Inkommande dokument** och välj sedan åtgärden **Skicka till OCR-tjänst**.

Värdet i OCR-status fältet ändras till **OCR-status** ändras till **Skickat**, förutsatt att inga fel finns.

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-by-email"></a>Så här skickar du en PDF eller bildfil till OCR-tjänstn via e-post
Skicka e-post till OCR-tjänstleverantören från ditt e-postprogram med PDF- eller bildfilen bifogad. Se OCR-tjänstleverantörens webbplats för information om e-postadress att skicka till.

Eftersom ingen inkommande dokumentpost finns för filen skapas en ny post automatiskt i fönstret **Inkommande dokument** när du får det resulterande elektroniska dokumentet från OCR-tjänsten. Mer information finns i [Så här skapar du inkommande dokumentposter](across-how-create-income-document-records.md).

> [!NOTE]  
>   Om du arbetar med en Tablet PC eller en telefon, kan du skicka filen till OCR-servicen, så snart som du har tagit ett foto av dokumentet, eller så kan du skapa ett inkommande dokument direkt. Mer information finns i avsnittet "Så här skapar du inkommande dokumentposter genom att ta ett foto" i [Så här skapar du inkommande dokumentposter](across-how-create-income-document-records.md).

## <a name="to-receive-the-resulting-electronic-document-from-the-ocr-service"></a>Så här tar du emot det resulterande elektroniska dokumentet från OCR-tjänsten.
Elektroniska dokument, som skapas med OCR-tjänsten från PDF- eller bildfilen tas emot automatiskt i fönstret**Inkommande dokument** jobbkötransaktionen som konfigureras när du aktiverar OCR-tjänsten.

Om du inte använder en jobbkö, eller om du vill ta emot ett färdigt OCR-dokument snabbare än per jobbköschemat, kan du välja knappen**Ta emot från OCR-tjänst**. Det kommer att få alla dokument som slutförs av OCR-tjänsten.

> [!NOTE]  
>   Om OCR-tjänsten är inställd på att kräva manuell verifiering av bearbetade dokument, när fältet **OCR-status** innehåller **Avvaktar verifiering**. I så fall utför du följande steg för att logga in på OCR-tjänstwebbplatsen manuellt för att kontrollera ett OCR-dokument.

1. I fälter**OCR-status** väljer du hyperlinken**Avvaktar verifiering**. Välj alternativt panelen**Avvaktar verifiering** på startsidan.
2. På OCR-servicewebbplatsen loggar du in med hjälp av autentiseringsuppgifter på OCR-servicekontot. Dessa är autentiseringsuppgifter som du också använde när du konfigurerade servicen. För mer information, se avsnittet"Att konfigurera en OCR-service" i [Så här ställer du in inkommande dokument](across-how-setup-income-documents.md).

    Om du öppnar webbplatsen från fältet**OCR-status**  visas dokument omedelbart när du loggar in. Om du öppnar en webbplats, genom att välja panelen på startsidan, på den första OCR-servicesidan som öppnas, måste du välja knappen**Start** på fliken**Bekräfta**eller dubbelklickar på det dokument som du vill bekräfta.

    Information för OCR-dokumentet visas med både källinnehållet av PDF- eller bildfilen och de resulterande OCR-fältvärdena.
3. Granska de olika fältvärdena och redigera dem manuellt eller ange värden i fält som OCR-servicen har taggat som osäkra.
4. Välj **OK**. OCR-processen är klar och det resulterande elektroniska dokumentet skickas tillinkommande dokument i **inkommande dokument** i [!INCLUDE[d365fin](includes/d365fin_md.md)], enligt jobbkönschemat.

    Om du öppnar en webbplats, genom att välja panelen på startsidan visas alla andra OCR-dokument som ska valideras, automatiskt på webbplatsen.
5. Upprepa steg 4 för alla andra OCR-dokument som ska valideras.

Du kan nu fortsätta med att skapa dokumentposter för de inlevererade elektroniska dokumenten i [!INCLUDE[d365fin](includes/d365fin_md.md)], manuellt eller automatiskt. Mer information finns i nästa procedur: Du kan också koppla den nya inkommande dokumentposten till det bokförda eller icke bokförda befintliga dokumentet så att källfilen är lättillgänglig i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Mer information finns i [Bearbeta inkommande dokument](across-process-income-documents.md).

## <a name="to-create-a-purchase-invoice-from-an-electronic-document-received-from-the-ocr-service"></a>Så här skapar du en inköpsfaktura från ett elektroniskt dokument som har tagits emot från OCR-servicen
Efterföljande procedur beskriver hur du skapar en inköpsfakturatransaktion från en leverantörsfaktura som tas emot som ett elektroniskt dokument från OCR-servicen. Proceduren är samma när du skapar, till exempel, en redovisningsjournalrad från ett kostnadskvitto eller från en försäljningsreturorder.

> [!NOTE]  
>   Fälten **Beskrivning** och **Nr.** på de nya dokumentraderna kommer endast att fyllas i om du först har mappat text som finns på OCR-dokumentet till de två fälten i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Du kan göra den här mappningen som korsreferenser till artikel, för dokumentrader av typartikel. Du kan också använda mappningsfunktionen Text-till-konto. Mer information finns i avsnittet ”Mappa ett inkommande dokument till en viss leverantör, redovisning eller adress”.

För att mappa artikelnumren på dokumentet till dina beskrivningar av leverantörens artiklar, öppna kortet för varje artikel och välj sedan åtgärden**Krossreferens**för att ställa in korsreferenser mellan dina artikelbeskrivningar och leverantörens. Mer information finns i beskrivningen för åtgärden **Tvärreferenser** på artikelkort.

1. Markera raden för inkommande dokument och välj sedan åtgärden **skapa dokument**.

En inköpsfaktura kommer att skapas av [!INCLUDE[d365fin](includes/d365fin_md.md)] utifrån informationen i det elektroniska leverantördokumentet som du fick av OCR-servicen. Informationen infogas i den nya inköpsfakturan, baserat på mappningen som du har definierat som en tvärreferens eller mappningen text-till-konto.

Eventuella valideringsfel som vanligtvis beror på fel eller saknade huvuddata [!INCLUDE[d365fin](includes/d365fin_md.md)], visas på snabbfliken **Fel och varningar**. För mer information, se avsnittet "Hantera fel när du tar emot ett elektroniskt dokument".

### <a name="to-map-text-on-an-incoming-document-to-a-specific-vendor-account"></a>Du mappar ett inkommande dokument till ett särskilt leverantörskonto
För inkommande dokument använder du vanligtvis åtgärden**Mappa text till konto** för att definiera att en viss text på en leverantörsfaktura som har tagits emot från OCR-servicen mappas till en viss leverantörskonto. Framöver kommer alla delar av det inkommande dokumentets beskrivning som existerar som en mappningstext innebära att fältet**Nr.** på resulterande dokument- eller journalrader av typen redovisningskonto fylls i med leverantören i fråga.

Förutom tilldelning eller mappning till ett leverantörskonto eller redovisningskonton kan du också mappa till ett bankkonto. Det är praktiskt, till exempel, för elektroniska dokument för kostnader som redan har betalts, där du vill skapa en redovisningsjournalrad som är klar för bokföring på ett bankkonto.

1. Välj relevant dokumentrad för inkommande och välj åtgärden **Mappa Text till kontot**. Fönstret **Mappa text till konto** öppnas.
3. I fältet **Mappa text** anger du en text som förekommer på leverantörsfakturor som du vill skapa inköpsdokument eller journalrader för. Du kan ange upp till 50 tecken.
4. I fältet **Leverantörsnr** anger du den leverantör som det resulterande inköpsdokumentet eller journalraden skapas för.
5. I fältet **debetkontonr** anger du den typ av debetkonto som ska skrivas in på färdiga dokument- eller journalrader av typen Redovisningskonto.
6. I fältet **kreditkontonr** anger du den typ av kreditkonto som ska skrivas in på färdiga dokument- eller journalrader av typen Redovisningskonto.

    > [!NOTE]
    > Använd inte fälten **Ursprungstyp för motkonto** och **Ursprungsnr för motkonto** fält i samband med inkommande dokument. De används endast för automatisk betalningsavstämning. Mer information finns i [Så här mappar du text på återkommande betalningar till konton för automatisk avstämning](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

7. Upprepa steg 2 till 5 för all text på inkommande dokument som du vill automatiskt vill skapa dokument för.

## <a name="to-handle-errors-when-receiving-electronic-documents"></a>Så här hanterar du fel vid mottagning av elektroniska dokument
1. I fönstret**inkommande dokument** markerar du raden för ett elektroniskt dokument som har tagits emot från OCR-service med fel. Detta indikeras av felvärdet i fältet**OCR-status**.
2. I fönstret **Inkommande dokument** väljer du åtgärden **Redigera**.
3. På snabbfliken**Fel och varningar** väljer du meddelandet och väljer sedanåtgärden**Öppna relaterade poster**.
4. Fönstret som visar om det finns fel eller saknade data, till exempel ett leverantörskort med ett saknat fältvärde, öppnas.
5. Rätta felet eller felen som beskrivs i varje felmeddelande.
6. Fortsätt med att bearbeta det inkommande dokumentet elektroniskt genom att välja åtgärden**Skapa manuellt** igen.
7. Upprepa steg 5 och 6 för alla återstående fel, tills det elektroniska dokumentet kan tas emot korrekt.

## <a name="to-train-the-ocr-service-to-avoid-errors"></a>Så här utbildar du OCR-tjänsten till att undvika fel
Eftersom OCR baseras på optisk läsning är det troligt att OCR-tjänsten tolkar tecknen i dina PDF- eller bildfiler fel första gången dokument från till exempel en viss leverantör behandlas. Det går kanske inte tolka företaglogotypen som leverantörens namn eller summan på ett utläggskvitto kan misstolkas på grund av layouten. Du kan undvika sådana fel genom att korrigera uppgifterna som du får av OCR-tjänsten och skicka återkopplingen till tjänsten.

Fönstret **OCR-datakorrigering** som öppnas från fönstret **Inkommande dokument** visar fälten från snabbfliken **Ekonomisk information** i två kolumner, en med ändringsbara OCR-uppgifter och en med skrivskyddade OCR-uppgifter. När du väljer knappen **Skicka OCR-feedback** skickas innehållet i fönstret **OCR-datakorrigering** till OCR-tjänsten. Nästa gång tjänsten behandlar PDF- eller bildfiler som innehåller samma uppgifter tas dina korrigeringar med för att samma fel ska kunna undvikas.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Inkommande dokument** och välj sedan relaterad länk.
2. Öppna en inkommande dokumentpost som innehåller data som har tagits emot från OCR-servicen och som du vill rätta till.
3. I fönstret **Inkommande dokument** väljer du åtgärden **Korrigera OCR-data**.
4. Skriv över data i den redigerbara kolumnen för varje fält som har ett inkorrekt värde i fönstret **OCR-datakorrigering**.
5. För att ångra korrigeringar som du har gjort sedan du öppnade fönstret **OCR-datakorrigering** väljer du åtgärden **Återställ OCR-data**.
6. För att skicka korrigeringar till OCR-tjänsten väljer du åtgärden **Skicka OCR-feedback**.
7. Om du vill spara korrigeringarna stänger du fönstret **OCR-datakorrigering**.

Fälten på snabbfliken **Ekonomisk information** i fönstret **Inkommande dokument** uppdateras med alla nya värden som du har angett i steg 4.

## <a name="see-also"></a>Se även
[Bearbeta inkommande dokument](across-process-income-documents.md)  
[Inkommande dokument](across-income-documents.md)  
[Inköp](purchasing-manage-purchasing.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

