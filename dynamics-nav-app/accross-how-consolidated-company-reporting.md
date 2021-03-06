---
title: "Konsolidera data från flera företag"
description: "Få en översikt av den ekonomiska situationen i ditt företag."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: consolidation, subsidiaries, consolidate
ms.date: 07/14/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f1590afe99c5cea9a70e580445014ff4e25dccee
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-work-with-the-consolidated-trial-balance-report"></a>Så här: Arbeta med rapporten Konsoliderad råbalans
Om du har fler än ett företag i [!INCLUDE[d365fin](includes/d365fin_md.md)] kan rapporten Konsoliderad råbalans i rollcentret Revisor ge dig en översikt av hela verksamheten.  

Rapporten kombinerar redovisningstransaktioner från var och ett av företagen i ett nytt företag som du skapar för att innehålla konsoliderade data. Detta företag kallas normalt för "det konsoliderade företaget". Det konsoliderade företaget är bara en behållare för konsoliderade data och saknar levande affärsdata. Företagen som du inkluderar i det konsoliderade företaget blir **Affärsenheter** i rapporten.

Du kan konsolidera:  

* Genom företag med olika kontoplaner.  
* Företag som använder olika räkenskapsår och olika valutor.  
* Antingen hela beloppet eller en procentandel av ett företags finansiella information
* Med hjälp av olika valutakurser på enskilda redovisningskonton 

Det finns två sätt att ställa in rapporten beroende på hur komplicerad ditt företag är:

* Om du inte behöver avancerade inställningar, exempelvis med ett företag som du bara har en del av, kan du använda den assisterade konfigurationen **Företagskonsolidering** för att snabbt skapa en konsolidering. Guiden hjälper dig att följa de grundläggande stegen.
* Om du behöver mer avancerade inställningar kan du ställa in det konsoliderade företaget och koncernföretagen själv.

## <a name="to-do-a-simple-consolidation-setup"></a>Om du vill ställa in en enkel konsolidering 
Om din konsolidering är enkel, till exempel eftersom du äger de koncernföretag som ska konsolideras helt, kommer den assisterade konfigurationen **Företagskonsolidering** att hjälpa dig med följande steg:
  
* Välj om du vill skapa ett nytt konsoliderat företag eller om du vill konsolidera data i ett företag som du har skapat för konsolideringen. Företaget bör inte innehålla transaktioner.
* Förhandsgranska resultatet. [!INCLUDE[d365fin](includes/d365fin_md.md)] verifierar att huvuddata och transaktioner kan överföras till det konsoliderade företaget.

Så här använder du den assisterade konfigurationsguiden:

1. I rollcentret **Revisor** väljer du åtgärden **Assisterad konfiguration**.
2. Välj **Ställ in konsolideringsrapportering** och slutför sedan varje steg i den assisterade konfigurationsguiden.

## <a name="to-do-an-advanced-consolidation-setup"></a>Så här gör du en avancerad konsolideringskonfiguration
Om du behöver mer avancerade inställningar för en konsolidering kan du konfigurera konsolideringen manuellt. Till exempel om du har kunder som du endast delvis äger eller om du har kunder som du inte vill inkludera i konsolideringen. Du kan lägga upp det konsoliderade företaget i en databas på samma sätt som du lägger upp andra företag. Mer information finns i [Komma igång med att göra affärer ](ui-get-ready-business.md).  

[!INCLUDE[d365fin](includes/d365fin_md.md)] låter dig lägga upp en lista över företag som ska konsolideras, verifiera redovisningsinformation innan du konsoliderar den, importera filer och generera konsolideringsrapporter.  

1. Logga in på det konsoliderade företaget.
2. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Affärsenheter** och välj sedan relaterad länk.  
3. Välj **Ny** och fyll sedan i relevanta fält.  

Om en utländsk valuta används för koncernföretaget måste du ange vilken valutakurs som ska användas vid konsolideringen. Dessutom måste du ange konsolideringsinformation på koncernföretagets redovisningskonton. De här processerna beskrivs i följande avsnitt.

### <a name="to-prepare-general-ledger-accounts-for-consolidation"></a>Så här förbereder du redovisningskonton för konsolidering 
Om kontoplanen i affärsenheten skiljer sig från det konsoliderade företaget måste du förbereda redovisningskonton för konsolidering. Du kan ange vilka konton som ska bokföra debet- och kreditbelopp och metoden du använder för att översätta valutor i det konsoliderade företaget. Detta är till exempel användbart om du kör rapporten ofta.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Kontoplan** och välj sedan relaterad länk.  
2. Öppna kortet för kontot och fyll sedan i fälten på snabbfliken **konsolidering**.

### <a name="to-specify-exchange-rates-for-consolidations"></a>Så här anger du valutakurs för konsolidering
Om en affärsenhet har en annan valuta än det konsoliderade företaget, måste du ange valutakurser för metoder för varje konto innan du konsoliderar. För varje konto bestämmer innehållet i **Konsoliderad omräkningsmetod** valutakursen. På varje affärsenhetskort, i fältet **Valutakurstabell** anger du om konsolideringen ska använda valutakurser från affärsenhetsföretaget eller det konsoliderade företaget. Om du använder valutakurser från det konsoliderade företaget kan du ändra valutakurserna för en affärsenhet. För affärsenheter, om fältet **Valutakurstabell** innehåller **Lokal** kan du ändra valutakursen från affärsenhetskortet. Valutakurserna kopieras från tabellen **Valutakurs**, men du kan ändra dem före konsolideringen. 

Följande tabell beskriver valutakursmetoderna som du kan använda för konton.

|Växlingskurs | Normal användning |
|---|---|
|Genomsnittskurs (manuell) | Du kan beräkna genomsnittskurs manuellt för den period som ska konsolideras. Beräkna genomsnittet antingen som ett aritmetiskt genomsnitt eller som en bästa uppskattning och ange resultatet för varje affärsenhet. Används för resultaträkningskonton.| 
|Slutkurs | Används för balansräkningskonton.|
|Senaste slutkurs | Kursen som var giltig på den utländska valutamarknaden vid den tidpunkt då balansräkningen eller resultaträkningen förbereds för. Du registrerar denna kurs för varje affärsenhet. Används för balansräkningskonton.|
|Historisk kurs | Valutakursen som användes när transaktionen genomfördes.|
|Sammansatt kurs | Den aktuella perioden omräknas med den genomsnittliga kursen och läggs till det tidigare registrerade saldot i det konsoliderade företaget. Den här metoden används vanligtvis för konton för balanserade vinstmedel eftersom de innehåller belopp från olika perioder och är därför en summa av belopp som omräknats med olika växelkurser.|
|Aktiekurs | Detta liknar **Sammansatt**. Differenser bokförs på olika redovisningskonton.|   

Om du vill ange valutakurs för affärsenheter gör du följande:

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Affärsenheter** och välj sedan relaterad länk.  
2. På sidan **Affärsenhetslista** väljer du affärsenhet och sedan åtgärden **Genomsnittskurs (manuell)**.   
3. På sidan **Ändra valutakurser** har innehållet i fältet **Relationsvalutakurs** kopierats från tabellen **Valutakurs**, men det går att ändra värdet. Stäng sidan.  
4. Välj **Slutkurs** på fliken **Analysera** i gruppen **Valutakurs**.  
5. På fältet **Relations- valutakurs belopp** anger du valutakursen. 

<!-- ### To include or exclude dimensions

COMMENTING THIS OUT BECAUSE i CANNOT REPRODUCE THE SETTINGS. tHERE IS NO CONSOLIDATION CODE FIELD ON DIMENSIONS OR DIMENSIOIN VALUES.

You can consolidate dimension information and general ledger accounts, as follows:

* To exclude dimension information in the consolidation, leave the **Consolidation Code** field blank, and do not choose dimensions in the **Copy Dimensions** fields in any consolidation functions or reports described later in this topic.
* To include dimension information in the consolidation, leave the **Consolidation Code** field blank. However, the consolidation will only work if the dimension values in the business unit are the same as the consolidated company.
* To consolidate the dimension value code in the business unit with a different dimension value code in the consolidated company, fill in the **Consolidation Code**. -->

### <a name="to-exclude-a-company-from-consolidation"></a>Om du vill exkludera ett företag från konsolidering
Om du inte vill inkludera en affärsenhet i konsolideringen kan du exkludera den. Om du vill göra det, öppnar du affärsenhetskortet och avmarkerar kryssrutan **konsolidera**.

### <a name="to-include-a-partially-owned-company-in-consolidation"></a>Om du vill inkludera ett delvis ägt företag i konsolidering
Om du bara äger en del av ett företag kan inkludera en procentandel av varje transaktion som motsvarar procentandelen av det företag som du äger. Om du äger 70 % av företaget kommer konsolideringen att innehålla 70 SEK av en faktura på 100 SEK. Om du vill ange hur stor procentandel av företaget du äger går du till affärsenhetskortet och anger procentsatsen i fältet **konsolideringsgrad %**.  

### <a name="to-test-the-data-before-you-consolidate"></a>Så här testar du data före konsolidering
Du kan testa data innan du överför den till det konsoliderade företaget. [!INCLUDE[d365fin](includes/d365fin_md.md)] tittar efter skillnader i information som finns i affärsenheterna och det konsoliderade företaget. Till exempel om kontonummer eller dimensionskoder är olika. Du måste åtgärda felen innan du kan köra rapporten. Du kan testa en databas, eller om du importerar data från en XML-fil kan du testa filen.   
  
1. Öppna det konsoliderade företaget.  
2. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Affärsenheter** och välj sedan relaterad länk.  
3. Gör något av följande:  
  
    * Testa en fil genom att välja åtgärden **testa fil**, ange namnet på filen och välj sedan **Skriv ut**.  
    * Om du vill testa en databas väljer du **Testa databas**.  

## <a name="to-run-the-consolidation"></a>Så här kör du konsolideringen
När du har testat data kan du starta konsolideringen överför den till det konsoliderade företaget.  
  
1. Logga in på det konsoliderade företaget.  
2. I rollcentret **Revisor** väljer du åtgärden **Kör konfiguration**.  
3. Fyll i relevanta fält.  
4. I fältet **Var** väljer du **företagsnamn** och väljer sedan det konsoliderade företaget i fältet **Är**.  

## <a name="to-export-data-from-dynamics-nav-and-import-it-in-included365finincludesd365finmdmd"></a>Så här exporterar du data från Dynamics NAVoch importera den i [!INCLUDE[d365fin](includes/d365fin_md.md)]
Om data för en affärsenhete är i en annan databas måste du exportera konsolideringsdata till en fil innan du kan inkludera den i konsolideringen. Varje företag måste exporteras var för sig. I detta avseende används batch-jobbet **Exportera konsolidering**.  
  
När du kör batch-jobbet körs bearbetas alla poster i redovisningskonton. För varje kombination av valda dimensioner och datum summeras och exporteras innehållet i fälten **Belopp** för posterna. Nästa kombination av valda dimensioner och datum med samma kontonummer bearbetas, sedan bearbetas kombinationerna med nästa kontonummer och så vidare.  

De exporterade posterna innehåller följande fält: **Kontonr**, **Bokföringsdatum** och **Belopp**. Om även dimensionsinformation har exporterats inkluderas dimensionskoder och dimensionsvärden.  

1. För varje exporterad rad, om summan av fälten **Belopp** är ett debetbelopp, kommer kontonumret som har angetts i affärsenhetens fält **Debetkonto konsolidering** att exporteras till raden. Om summan är ett kreditbelopp, kommer motsvarande nummer i fältet **Kreditkonto konsolid.** att exporteras till raden.  
2. Det datum som används för varje exporterad rad är antingen periodens slutdatum eller, om överföringen utförs varje dag, det exakta datumet för beräkningen.  
3. Det dimensionsvärde som exporteras för transaktionen är det konsoliderade företagets dimensionsvärde som har lagts upp i fältet **Konsolideringskod** för det dimensionsvärdet. Om inget dimensionsvärde har angetts för det konsoliderade företaget i fältet **Konsolideringskod** för det dimensionsvärdet, exporteras själva dimensionsvärdet till raden.   
4. XML-filerna innehåller dessutom valutakurserna i konsolideringsperioden. Dessa kurser placeras i ett separat avsnitt i början av filen.

## <a name="see-also"></a>Se även
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Exportera affärsdata till Excel](about-export-data.md)

