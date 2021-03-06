---
title: "Genomgång: Plockning och leverans i grundläggande lagerkonfiguration"
description: "I [!INCLUDE[d365fin](includes/d365fin_md.md)], kan de utgående processerna för plockning och utleverans utföras på fyra sätt med hjälp av olika funktionaliteter beroende på lagerkomplexitetsnivån."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ce9d58f93edeebd4933a532deb7c4672ced6f76a
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a>Genomgång: Plockning och leverans i grundläggande lagerkonfiguration
I [!INCLUDE[d365fin](includes/d365fin_md.md)] kan de utgående processerna för plockning och utleverans utföras på fyra sätt med hjälp av olika funktionaliteter beroende på lagerkomplexitetsnivån.  

|Metod|Ankommande behandling|Lagerplatser|Plockningar|Utleveranser|Nivå av komplexitet (Se [Designdetaljer: Lagerstyrningsinställning](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Bokföra plockning och utleverans från orderraden|INTER|||2|  
|B|Bokföra plockning och utleverans från ett lagerplockningdokument||X||3|  
|L|Bokföra plockning och utleverans från ett distributionslagerutleveransdokument|||X|6-4-5|  
|D|Bokföra plockning från ett distributionslagerplockningdokument och bokföra leveransen från ett distributionslagerutleveransdokument||INTER|INTER|6-4-5|  

Mer information finns i [Designdetaljer: Avgående distributionslagerflöde](design-details-outbound-warehouse-flow.md).  

Efterföljande genomgången visar metod B i föregående tabellen.  

## <a name="about-this-walkthrough"></a>Om den här genomgången  
För grundläggande lagerkonfigurationer där lagerstället har konfigurerats att kräva plockningsbearbetning men inte leveransbearbetning, använder du fönstret **Lagerplockning** för att registrera och bokföra plocknings- och leveransinformation för dina avgående källdokument. Det utgående källdokumentet kan vara en försäljningsorder, inköpsreturorder, utgående överföringsorder eller produktionsorder med komponentbehov.  

I den här genomgången tas följande aktiviteter upp:  

-   Lägger upp lagerstället SILVER för lagerplockning.  
-   Skapa en försäljningsorder för kund 10000 på 30 högtalare.  
-   Släppa försäljningsordern för lagerhantering.  
-   Skapa en lagerplockning som baseras på ett släppt källdokument.  
-   Registrering av lagerrörelsen från lagret och samtidigt bokföra försäljningsutleveransen för källförsäljningsorder.  

## <a name="roles"></a>Roller  
Den här genomgången innehåller arbetsuppgifter som utförs av följande användarroller:  

-   Dist.lagerchef  
-   Orderhandläggare  
-   Lagerarbetare  

## <a name="prerequisites"></a>Förutsättningar  
För att kunna utföra den här genomgången behöver du:  

-   CRONUS Sverige AB installerad  
-   Gör dig själv till distributionslageranvändare på lagerstället SILVER med följande steg:  

    1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Dist.lager personal** och välj sedan relaterad länk.  
    2.  Välj fältet **Användar-ID** och välj ditt eget användarkonto i fönstret **Användare**.  
    3.  Ange SILVER i fältet **Lagerställekod**.  
    4.  Välj fältet **Standard**.  

-   Gör artikeln LS-81 tillgänglig på platsen SILVER, genom att följa nedanstående steg:  

    1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Artikeljournaler** och välj sedan relaterad länk.  
    2.  Öppna standardjournalen och skapa sedan två artikeljournalrader med följande information om arbetsdatumet (23 januari).  

        |Transaktionstyp|Artikelnummer|Platskod|Lagerplatskod|Antal|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |Positiv antalsjust.|LS-81|SILVER|S-01-0001 **Obs!**  Artikelns standardlagerplats i CRONUS|2.0|  
        |Positiv antalsjust.|LS-81|SILVER|S-01-0002|2.0|  

    3.  Välj åtgärden **Bokföra** och sedan knappen **Ja**.  

## <a name="story"></a>Situation  
Ellen, lagerchefen i CRONUS ställer in lagret SILVER för grundläggande plockning där lagerarbetare behandlar utgående beställningar var för sig. Susan, orderhandläggaren, skapar en försäljningsorder för 30 enheter av artikeln LS-81 att levereras till kund 10000 från SILVERLAGRET. Anders, lagerarbetaren, måste kontrollera att leveransen förbereds och levereras till kunden. Anders hanterar alla uppgifter som är involverade i fönstret **Lagerplockning** som automatiskt pekar på lagerplatserna där LS-81 lagras.  

## <a name="setting-up-the-location"></a>Lägger upp lagerstället  
Inställningen av fönstret **Lagerställekort** definierar företagets lagerflöden.  

### <a name="to-set-up-the-location"></a>Så här lägger du upp lagerställen  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.  
2.  Öppna lagerställekortet SILVER.  
3.  Markera kryssrutan **Begär plockning**.  

## <a name="creating-the-sales-order"></a>Skapar försäljningsreturordern  
Försäljningsorder är den vanligaste typen för utgående källdokumentet.  

### <a name="to-create-the-sales-order"></a>Så här skapar du försäljningsreturordern  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Försäljningsorder** och välj sedan relaterad länk.  
2.  Välj åtgärden **Ny**.  
3.  Skapa en försäljningsorder för kund 10000 på arbetsdatumet (23 januari) med följande försäljningsorderrad.  

    |Artikel|Lagerställekod|Antal|  
    |----------|-------------------|--------------|  
    |LS_81|SILVER|30|  

     Fortsätt med att meddela lagret att försäljningsordern är klar för lagerhantering.  

4.  Välj åtgärden **Släppa**.  

    Anders fortsätter att plocka och leverera de sålda artiklarna.  

## <a name="picking-and-shipping-items"></a>Plocka och leverera artiklar  
I fönstret **Lagerplockning** kan du hantera alla utgående distributionslageraktiviteter för ett särskilt källdokument, t.ex en försäljningsorder.  

### <a name="to-pick-and-ship-items"></a>Plocka och utleverera artiklar så här  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerplockningar** och välj sedan relaterad länk.  
2.  Välj åtgärden **Ny**.  
3.  Välj fältet **Källdokument** och sedan **Försäljningsorder**.  
4.  Välj fältet **Ursprungsnr.**, markera raden för försäljningen till kund 10000 och välj sedan knappen **OK**.  

    Välj alternativt åtgärden **Hämta källdokument** och välj sedan försäljningsordern.  
5.  Välj åtgärden **Fyll i auto. ant. att hantera**.  

    Alternativt, ange 10 respektive 30 i fältet **Ant. att hantera** på de två lagerplockningsraderna.  
6.  Välj åtgärden **bokför**, välj **leverera**, och välj sedan **OK**-knappen.  

    De 30 högtalarna har nu registrerats som plockade från lagerplatser S-01-0001 och S-01-0002, och en negativ artikeltransaktion skapas som återspeglar den bokförda leveransen.  

## <a name="see-also"></a>Se även  
 [Så här plockar du artiklar med Lagerplockning](warehouse-how-to-pick-items-with-inventory-picks.md)   
 [Så här: plocka artiklar för Dist.lager utleverans](warehouse-how-to-pick-items-for-warehouse-shipment.md)   
 [Så här: Ställa in grundläggande dist.lager med operationsområden](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)   
 [Så här: Flytta komponenter till ett operationsområde i grundläggande lagerkonfiguration](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)   
 [Så här: Plocka för produktion eller montering](warehouse-how-to-pick-for-production.md)   
 [Så här flyttar du artiklar ad hoc i grundläggande lagerkonfiguration](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)   
 [Designdetaljer: Avgående distributionslagerflöde](design-details-outbound-warehouse-flow.md)   
 [Genomgång av affärsprocesser](walkthrough-business-process-walkthroughs.md)  
 [Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

