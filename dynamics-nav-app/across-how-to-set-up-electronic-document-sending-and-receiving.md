---
title: "Så här konfigurerar du utskick och mottagning av elektroniska dokument"
description: "Som alternativ till att e-posta en filbilaga kan du skicka och ta emot elektroniska affärsdokument."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 3ddac8fe7edaded893d7bf63538e3145dead0602
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-electronic-document-sending-and-receiving"></a>Så här konfigurerar du utskick och mottagning av elektroniska dokument
Som alternativ till att e-posta en filbilaga kan du skicka och ta emot elektroniska affärsdokument. Med elektroniska dokument menas en standarduppfyllande\-fil som representerar ett affärsdokument, till exempel en faktura från en leverantör som kan tas emot och konverteras till en inköpsorder i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Utbytet av elektroniska dokument mellan två handelspartners utförs av en extern leverantör av dokumentväxlingstjänster. Den generiska versionen av [!INCLUDE[d365fin](includes/d365fin_md.md)] stöder utskick och mottagning av elektroniska fakturor och kreditnotor i PEPPOL-format, som stöds av de största leverantörerna av dokumentväxlingstjänster. En större leverantör av dokumentväxlingstjänster är förkonfigurerad och klar att ställa in för ditt företag.  

Från PDF- eller bildfiler som representerar inkommande dokument kan du låta en extern OCR-tjänst (Optical Character Recognition) skapa elektroniska dokument som du kan konvertera till dokumentposter i [!INCLUDE[d365fin](includes/d365fin_md.md)] som du gör för elektroniska PEPPOL-dokument. När du exempelvis tar emot en faktura i PDF-format från leverantören, kan du skicka den till OCR-tjänsten från fönstret **Inkommande dokument**. Efter några sekunder får du tillbaka filen tillbaka som en elektronisk faktura som kan omvandlas till en inköpsfaktura för leverantören. Om du skicka filen till OCR-tjänsten via e-post, skapas en ny inkommande dokumentpost automatiskt när du får tillbaka det elektroniskt dokument.  

Det elektroniskt dokumentformatet **PEPPOL** har förkonfigurerats så att du kan skicka elektroniska fakturor och kreditnotor i PEPPOL-format. Först måste du skapa olika huvuddata, som företagsinformation, kunder, artiklar och enheter. Dessa används för att identifiera dina affärspartners och artiklar vid konvertering av data i fält i [!INCLUDE[d365fin](includes/d365fin_md.md)] till element i den utgående dokumentfilen. Sedan måste du välja formatet i fönstret **Elektroniskt dokumentformat** för varje kund som du ska skicka elektroniska PEPPOL-dokument till. Mer information finns i [Så här skickar du dokument](sales-how-to-send-electronic-documents.md).  

Dataväxlingsdefinitionerna **PEPPOL – Faktura** och **PEPPOL – Kreditfaktura** är förkonfigurerade så att du kan ta emot elektroniska fakturor och kreditfakturor i PEPPOL-format. Först måste du skapa olika huvuddata, som företagsinformation, leverantörer, artiklar och enheter. Dessa används för att identifiera dina affärspartners och artiklar vid konvertering av data i element i den utgående dokumentfilen till fält i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Sedan måste du välja valutakursdefinitionen i fönstret **Inkommande dokument** för varje inkommande elektroniskt dokument som du vill omvandla till ett inköpsdokument i [!INCLUDE[d365fin](includes/d365fin_md.md)].  

Dataväxlingsdefinitionen **OCR - Faktura** är förkonfigurerad så att du kan ta emot elektroniska dokument som genererats av OCR-tjänsten. Om du vill ta emot till exempel en faktura som ett elektroniskt OCR-dokument ställer du in huvuddatum och behandlar dokumentet som när du tar emot ett elektroniskt PEPPOL-dokument. Mer information [Så här använder du OCR för att omvandla PDF- och bildfiler till elektroniska dokument](across-how-use-ocr-pdf-images-files.md).  

De förkonfigurerade tjänsterna för dokumentutbyte och OCR måste vara aktiverad innan du skickar och tar emot. Mer information finns i [Så här konfigurerar du en dokumentväxlingstjänst](across-how-to-set-up-a-document-exchange-service.md).  

Avsnittet innehåller följande procedurer:  

* Så här ställer du in företaget för utskick och mottagning av elektroniska dokument  
* Så här ställer du in momsbokföring för utskick och mottagning av elektroniska dokument  
* Så här ställer du in länder/regioner för utskick och mottagning av elektroniska dokument  
* Så här ställer du in artiklar för utskick och mottagning av elektroniska dokument  
* Så här ställer du in måttenheter för utskick och mottagning av elektroniska dokument  
* Så här ställer du in kunder för utskick av elektroniska dokument  
* Så här väljer du det elektroniska dokumentformatet **PEPPOL** för utskick och mottagning av elektroniska dokument  
* Så här ställer du in leverantörer för mottagning av elektroniska dokument  
* Så här väljer du datautbytesdefinitionen **PEPPOL - Faktura** för mottagning av elektroniska dokument  
* Så här ställer du in det redovisningskonto som ska användas på nya inköpsfakturarader för icke\-identifierbara artiklar och icke\-objekt  

### <a name="to-set-up-the-company-for-electronic-document-sending-and-receiving"></a>Så här ställer du in företaget för utskick och mottagning av elektroniska dokument  
1. I rutan **Sök**, ange **Företagsinformation** och välj sedan relaterad länk.  
2. Fyll i fälten enligt beskrivningen i följande tabell på snabbfliken **Allmänt**.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**GLN**|Identifiera företaget.<br /><br /> När du till exempel skickar elektroniska fakturor i PEPPOL-format används värdet i detta fält för att fylla i **EndPointID**-element under noden **AccountingSupplierParty** i filen. Numret baseras på standarden GS1, som är kompatibel med ISO 6523.|  
    |**Momsregistreringsnr**|Ange företagets momsregistreringsnummer.|  
    |**Ansvarsenhet**|Om ditt företag ställs in med en ansvarsenhet så se till att fältet **Lands-/regionskod** är ifyllt.|  

### <a name="to-set-up-vat-posting-for-electronic-document-sending-and-receiving"></a>Så här ställer du in momsbokföring för utskick och mottagning av elektroniska dokument  
1. I rutan **Sök**, ange **Bokföringsinställningar för moms** och välj sedan relaterad länk.  
2. Fyll i fältet enligt beskrivningen i följande tabell för varje rad med momsbokföringsinställning som du kommer att använda för elektroniskt dokument.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Momskategori**|Ange momskategorin.<br /><br /> När du till exempel skickar elektroniska fakturor i PEPPOL-format används värdet i detta fält för att fylla i **TaxApplied**-element under noden **AccountingSupplierParty** i filen. Numret baseras på standarden UNCL5305.|  

### <a name="to-set-up-countriesregions-for-electronic-document-sending-and-receiving"></a>Så här ställer du in länder/regioner för utskick och mottagning av elektroniska dokument  
1. I rutan **Sök** anger du **Länder/regioner** och väljer sedan relaterad länk.  
2. Fyll i fältet enligt beskrivningen i följande tabell för varje land/region som du ska utbyta elektroniska dokument med.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Momssystem**|Identifiera den nationella myndighet som utfärdar momsregistreringsnummer för landet\/regionen i samband med utskick av elektroniska dokument.<br /><br /> När du till exempel skickar elektroniska fakturor i PEPPOL-format används värdet i detta fält för att fylla i **SchemeID**-attributet för **EndPointID**-elementet under både noden **AccountingSupplierParty** och **AccountingCustomerParty** i filen.<br /><br /> Fältet **Momssystem** används endast om fältet **GLN** i fönstret **Företagsinformation** inte är ifyllt. **Obsa:**  Värdet i fältet **Kod** i fönstret **Länder\/Regioner** måste uppfylla ISO 3166\-1:Alpha2.|  

### <a name="to-set-up-items-for-electronic-document-sending-and-receiving"></a>Så här ställer du in artiklar för utskick och mottagning av elektroniska dokument  
1. I rutan **Sök**, ange **Artiklar** och välj sedan relaterad länk.  
2. Fyll i fälltet enligt beskrivningen i följande tabell för varje artikel som du köper eller säljer.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**GTIN**|Identifierar artikeln i samband med utskick och mottagning av elektroniska dokument. För PEPPOL-format används fältet enligt följande:<br /><br /> Om **StandardItemIdentification\/ID**-element har **SchemeID**-attribut inställt på **GTIN**, mappas elementet till fältet **GTIN** på artikelkortet.|  

### <a name="to-set-up-units-of-measure-for-electronic-document-sending-and-receiving"></a>Så här ställer du in måttenheter för utskick och mottagning av elektroniska dokument  
1. I rutan **Sök**, ange **Måttenhet** och välj sedan relaterad länk.  
2. Fyll i fältet enligt beskrivningen i följande tabell för varje måttenhet som du kommer att använda för artiklar i elektroniska dokument.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Internationell standardkod**|Ange den använda måttenheten i enlighet med standarden UNECERec20 i samband med utskick av elektroniska dokument.<br /><br /> När du till exempel skickar elektroniska fakturor i PEPPOL-format används värdet i detta fält för att fylla i **unitCode**-attributet för elementet **InvoicedQuantity** under noden **InvoiceLine**. **Obs:**  Om fältet **Måttenhet** på försäljningsraden är tomt, infogas standardvärdet i UNECERe20 för “Piece” \(H87\) som standard. Mer information och en lista över giltiga enhetskoder finns i [Recommendation No. 20 \- Units of Measure used in International Trade](http://www.unece.org/fileadmin/DAM/cefact/recommendations/rec20/rec20_rev3_Annex2e.pdf).|  

### <a name="to-set-up-customers-for-electronic-document-sending"></a>Så här ställer du in kunder för utskick av elektroniska dokument  
1. I rutan **Sök**, ange **Kunder** och välj sedan relaterad länk.  
2. Fyll i fältet enligt beskrivningen i följande tabell för varje kund som du vill skicka elektroniska dokument till.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**GLN**|Identifiera kunden.<br /><br /> När du till exempel skickar elektroniska fakturor i PEPPOL-format används värdet i detta fält för att fylla i **EndPointID**-element under noden **AccountingCustomerParty** i filen. Numret baseras på standarden GS1, som är kompatibel med ISO 6523.<br /><br /> Om **GLN** är tomt används värdet i fältet **Momsregistreringsnr.**.|  
    |**Momsregistreringsnr**|Ange kundens momsregistreringsnummer. **Tips:**  Välj knappen Specificera om du vill använda webbtjänsten som verifierar om numret finns i landets företagsregister.|  
    |**Ansvarsenhet**|Om kunden ställs in med en ansvarsenhet så se till att fältet **Lands-/regionskod** är ifyllt.|  

    Du kan skapa varje kund med en önskad metod för att skicka affärsdokument så att du inte behöver välja utskicksalternativ varje gång som du skickar ett dokument till kunden. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).  

### <a name="to-select-the-peppol-electronic-document-format-for-electronic-document-sending"></a>Så här väljer du det elektroniska dokumentformatet PEPPOL för utskick och mottagning av elektroniska dokument  
1. I rutan **Sök** anger du **Dokumentutskicksprofiler** och väljer sedan relaterad länk.  
2. Öppna en befintlig dokumentutskicksprofil eller skapa en ny. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).  
3. I fönstret **skicka dokumentprofil** väljer du **elektroniskt Format**markerar raden för PEPPOL och välj **OK**.  
4. I fältet **Elektroniskt dokument** väljer du **Ja (Genom dokumentväxlingstjänst)**.  

    > [!NOTE]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)]  identifierar automatiskt om dokumentet är en faktura eller kreditnota och tillämpar PEPPOL-formatet därefter.  

5. Markera kryssrutan **Standard** på snabbfliken **Allmänt**. Fyll i fältet **Dokumentutskicksprofil** på kundkorten i fråga om du vill ange att det ska tillämpas för vissa kunder endast. Mer information finns i [Så här skapar du Dokumentutskicksprofiler](sales-how-setup-document-send-profiles.md).  

    Du kan nu skicka det elektroniska dokumentet med konverterade data. Mer information finns i [Så här skickar du dokument](sales-how-to-send-electronic-documents.md).  

### <a name="to-set-up-vendors-for-electronic-document-receiving"></a>Så här ställer du in leverantörer för mottagning av elektroniska dokument  
1. I rutan **Sök**, ange **Leverantörer** och välj sedan relaterad länk.  
2. Fyll i fälltet enligt beskrivningen i följande tabell för varje leverantör som du vill ta emot elektroniska dokument från.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**GLN**|Identifiera leverantören.<br /><br /> När du till exempel tar emot elektroniska fakturor i PEPPOL-format används värdet i detta fält för att fylla i **EndPointID**-element under noden **AccountingSupplierParty** i filen. Numret baseras på standarden GS1, som är kompatibel med ISO 6523.<br /><br /> Om **GLN** är tomt används värdet i fältet **Momsregistreringsnr.**.|  
    |**Momsregistreringsnr**|Ange leverantörens momsregistreringsnummer. **Tips:**  Välj knappen Specificera om du vill använda webbtjänsten som verifierar om numret finns i landets företagsregister.|  
    |**Ansvarsenhet**|Om leverantören ställs in med en ansvarsenhet så se till att fältet **Lands-/regionskod** är ifyllt.|  

### <a name="to-select-the-peppol---invoice-data-exchange-definition-for-electronic-document-receiving"></a>Så här väljer du datautbytesdefinitionen PEPPOL - Faktura för mottagning av elektroniska dokument  
1. I rutan **Sök**, ange **Inkommande dokument** och välj sedan relaterad länk.  
2. Välj fältet **Typ av dataintegration** och sedan **PEPPOLINVOICE** på raden för elektroniskt dokument som du vill ta emot och konvertera.  

     Om dokument som ska tas emot är en kreditnota väljer du **PEPPOLCREDITMEMO**.  

    Nu kan du ta emot elektroniska dokument genom att starta datakonverteringprocessen i fönstret **Inkommande dokument**. Mer information finns i [Så här tar du emot och omvandlar elektroniska dokument](purchasing-how-to-receive-and-convert-electronic-documents.md).  

### <a name="to-set-up-the-gl-account-to-use-on-new-purchase-invoice-lines-for-non-identifiable-items-and-non-items"></a>Så här ställer du in det redovisningskonto som ska användas på nya inköpsfakturarader för icke-identifierbara artiklar och icke-objekt  
1. I rutan **Sök** anger du **Inköp & Leverantörsreskontra** och sedan väljer du relaterad länk.  
2. Fyll i fältet enligt beskrivningen i följande tabell på snabbfliken **Datautbyte**.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Redovisningskonto för rader utan artikel**|Anger det redovisningskonto som infogas automatiskt på inköpsrader, som skapas från elektroniska dokument när den inkommande dokumentraden inte innehåller en identifierbar artikel. Inkommande dokumentrader som inte har ett EAN- eller leverantörens artikelnummer konverteras till en inköpsorder av typen **redovisningskonto**, och **nr.** på inköpsraden innehåller det konto som du väljer i den **Redovisningskonto för rader utan artikel**.<br /><br /> Om du lämnar fältet **Redovisningskonto för rader utan artikel** tomt, och det inkommande dokumentet har rader utan identifierbara artiklar, kommer inköpsdokumentet inte att skapas. Ett felmeddelande visas med instruktion om att du måste fylla i fältet **Redovisningskonto för rader utan artikel** innan du kan slutföra uppgiften.|  

## <a name="see-also"></a>Se även  
[Utbyta data elektroniskt.](across-data-exchange.md)   
[Så här fakturerar du försäljning](sales-how-invoice-sales.md)   
[Så här registrerar du inköp](purchasing-how-record-purchases.md)

