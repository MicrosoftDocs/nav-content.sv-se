---
title: "Om beräkning av standardkostnad"
description: "I standardkostnadssystemet fastställs styckkostnaden i lagret utifrån en historisk eller förväntad kostnad som är rimlig. På det här sättet skapas ett underlag för standardkostnaderna, eftersom tidigare och förväntade framtida kostnadsdata undersöks."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e87127c63dca7154bee52106f20a3df3dd3b4699
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="about-calculating-standard-cost"></a>Om beräkning av standardkostnad
Många produktionsföretag använder värderingsbasen för standardkostnad. Detta gäller också företag som utför lätt produktion, t.ex. montering och paketering. I standardkostnadssystemet fastställs styckkostnaden i lagret utifrån en historisk eller förväntad kostnad som är rimlig. På det här sättet skapas ett underlag för standardkostnaderna, eftersom tidigare och förväntade framtida kostnadsdata undersöks. Innan ett beslut fattas om att ändra de här kostnaderna förblir de frysta. Den faktiska kostnaden för att tillverka en produkt kan skilja sig från den beräknade standardkostnaden. Den faktiska kostnaden jämförs sedan med standardkostnaden för en särskild artikel och skillnaderna eller *avvikelserna* identifieras och analyseras för den ekonomiska styrningen.  

Standardkostnader kan bibehållas för artiklar som fylls i via inköp, montering och produktion. För varje återanskaffning kan standardkostnader bestå av följande delar.  

|Återanskaffningssystem|Standardkostnadselement|  
|--------------------------|----------------------------|  
|**Inköp**|Inköpskostnad för varor och material och materialkostnad, om det behövs.|  
|**Montering**|Inköpskostnad för material, direkt eller fast arbetskostnad och omkostnad.|  
|**Prod.order**|Inköpskostnad för material, arbetskostnad, underleverantörskostnad och omkostnad.|  

## <a name="setting-up-standard-costs"></a>Ställa in standardkostnader  
Eftersom standardkostnaden för en producerad eller monterad artikel kan innehålla flera kostnadsslag måste en standardkostnad utarbetas för alla följande kostnadsslag: materialkostnader, kapacitetskostnader (arbete) och leveratörskostnader (inköpskostnader och overheadkostnader).  

Redovisningen i ett produktionsföretag som använder standardkostnadskalkylering består av:  

-   Att uppskatta en standardkostnad för en färdig artikel samt att ställa in den på artikelkortet.  
-   Att registrera och fördela den faktiska kostnaden för de viktigaste kostnadsslagen samt att redovisa avvikelser.  

Alla komponentkostnader måste räknas samman när den direkta kostnaden för en färdig artikel ska bestämmas. En monterad eller en tillverkad artikel kan bestå av halvfabrikat, som också består av flera komponenter.  

Följande viktiga kostnadselement utgör den totala inköpskostnaden för en färdig och bearbetad artikel:  

-   Materialkostnader.  
-   Kapacitetskostnad.  
-   Underleverantörskostnader endast för den producerade artikeln.  

### <a name="material-costs"></a>materialkostnader  
 Materialkostnaderna är kostnader som är kopplade till detaljmontage och inköpt råmaterial. Materialkostnaden kan bestå av kostnadsslag för både inköpskostnad och indirekt kostnad.  

-   Inköpskostnaden för materialet utgörs av ett fakturerat belopp för inköpt råmaterial eller av produktionskostnaden för ett detaljmontage.  
-   Den indirekta kostnaden för materialet eller *overheadkostnaden* kan t.ex. utgöras av lagerhållningskostnaden för den färdiga artikeln när den har tillverkats.  

Inställningen av materialkostnaden för inköpta artiklar, som påverkar inköpskostnad och indirekt kostnad, beror på den värderingsprincip du har valt för den aktuella artikeln. Du kan skapa kostnadsinformation för varje värderingsprincip på artikelkortet. Mer information finns i [Så här registrerar du nya artiklar](inventory-how-register-new-items.md).

Kassationskostnaden (endast produktion) är ytterligare en faktor att beakta när du beräknar den totala materialkostnaden. När en viss mängd med råmaterial kasseras när du monterar eller tillverkar en artikel brukar komponentkvantiteten som krävs för att tillverka denna artikel öka. Detta ökar materialkostnaden för komponenterna som förbrukas vid tillverkningen av en struktur. Du ställer in kassationskostnad för material i produktionsstrukturen eller produktionsoperationsföljden.  

Materialkostnaden för en tillverkad artikel kan visas på två sätt som motsvarar följande standardsätt för kostnadsberäkning.  

|Kostnadsberäkningsbas|Materialkostnadsberäkning|  
|----------------------------|-------------------------------|  
|En nivå|Den producerade artikeln är lika med totalkostnaden för alla inköpta eller detaljmonterade artiklar i artikelns produktionsstruktur.|  
|En nivå eller flera nivåer|Producerad artikel är summan av materialkostnaden för alla delmontage i den artikelns struktur och kostnaden för alla inköpta artiklar i den artikelns produktionsstruktur.|  

### <a name="capacity-costs"></a>Kapacitetskostnader  
Kapacitetskostnaderna är kostnader som är kopplade till interna kostnader för arbetskraft och maskiner. Du måste lägga upp dessa kostnader för varje resurs (i monteringshanteringen) och arbete eller maskingrupp i operationsföljden (i produktion). På samma sätt som med materialkostnaderna kan du identifiera kostnadsslag för kapacitetskostnaden, vad beträffar både inköpskostnaden och den indirekta kostnaden. Inköpskostnaden för en produktionsgrupp kan t.ex. vara "verkstadskostnaden" som har skapats för en särskild uppgift. Den indirekta kostnaden för en produktionsgrupp kan utgöras av allmänna kostnader för fabriken, t.ex. belysning, uppvärmning o.s.v. På liknande sätt som med materialkostnaderna kan kapacitetsoverhead uttryckas i form av en procentsats för den indirekta kostnaden eller en fast overheadkostnad.  

Inställningen av kapacitetskostnaderna för monterade artiklar består av följande delar:  

-   Inköpskostnad och indirekt styckkostnad för resursen.  
-   Fast eller direkt resursförbrukningstyp.  

Inställningen av kapacitetskostnaderna för producerade artiklar består av följande delar:  

-   Inköpskostnad och indirekt styckkostnad för maskin- eller produktionsgruppen.  
-   Inställning av tid och partistorlek.  

Om en standardinställd kapacitetskostnad ska kunna beräknas måste du fastställa standardinställda tidskostnader som behövs till operationerna i maskin- och produktionsgrupperna. Den totala tiden för att slutföra en operation består vanligtvis av omställningstiden, bearbetningstiden och av väntetiden och transporttiden.  

Du ställer in kostnaderna för varje tidstyp för varje maskin-/produktionsgrupp i enskilda operationsföljder.  

> [!NOTE]  
    >  Kostnaderna för bearbetningstiden gäller för varje enskild tillverkad artikelenhet och att kostnaderna för omställningstiden gäller för varje enskilt parti. Därför måste omställningstiden i operationsföljden fördelas proportionellt över partistorleken för varje operation. Partistorleken anges i motsvarande fält på snabbfliken **Beställning** för artikelkortet.  

För att ange omställningstid i operationsföljden i planeringssyfte, men inte inkludera den här kostnaden i den standardinställda kostnadsberäkningen avmarkerar du fältet **Kostnad inkl. omst.tid** i fönstret **Produktionsinställningar**.  

På En-nivå-basis är detta den arbetskostnad som krävs för att producera den färdiga produktionsartikeln och anges på produktionsartikelns operationsföljd. På en fler-nivå-basis är den kapacitet som har angetts för varje enskild tillverkad artikel som ingår i den överordnade artikelns struktur.  

### <a name="subcontractor-costs"></a>Underleverantörskostnader  
Underleverantörskostnaderna är kostnader som är kopplade till tjänster från företagets fristående leverantörer eller underleverantörer. På liknande sätt som med material- och kapacitetskostnaderna kan underleverantörskostnaderna bestå av både inköpskostnad och overheadkostnad. Inköpskostnaden för legotillverkningen utgörs av den faktiska avgiften per enhet för de erhållna tjänsterna. Overheadkostnaden för legotillverkningen kan t.ex. vara frakt- och hanteringskostnader som företaget ådrog sig vid en legotillverkningsorder.  

Eftersom legotillverkning är en utlagd kapacitet ställs kostnaden för legotillverkningstjänsterna (inköpskostnad och indirekt kostnad) in för produktionsgruppkortet som motsvarar legotillverkningsoperationen.  

## <a name="updating-standard-costs"></a>Uppdatera standardkostnader  
Använd funktionen från artikelkortet för att uppdatera eller beräkna standardkostnaden för monteringsartiklar.  

Processen för att uppdatera eller att beräkna standardkostnader består vanligtvis av följande uppgifter:  

1.  Uppdatera kostnader på komponent- och kapacitetsnivå. Mer information finns i batch-jobben **Föreslå artikelstandardkostnad** och **föreslå kapacitet standardkostnad**.  
2.  Konsolidera och summera komponent- och kapacitetskostnader för att beräkna den totala monterings- eller produktionskostnaden för artiklarna. Mer information finns i avsnittet ”Att beräkna standardkostnaden för en monteringsartikel” i [Så här arbetar du med strukturer](inventory-how-work-BOMs.md).  
3.  Använda standardkostnaderna som anges när du kör de föregående batch-jobben. Standardkostnaderna börjar inte gälla förrän de implementeras. Mer information finns i batch-jobbet **Implementera standardkostnadsändringar**.  
4.  Implementera ändringarna för att uppdatera fältet **Styckkostnad** för artikelkortet och utföra lagerutvärderingen. Mer information finns i [Så här omvärderar du lager](inventory-how-revalue-inventory.md).

## <a name="see-also"></a>Se även  
 [Designdetaljer: Värderingsprinciper](design-details-costing-methods.md)   
 [Så här arbetar du med strukturer](inventory-how-work-BOMs.md)   
 [Så här kan du uppdatera standardkostnader](finance-how-to-update-standard-costs.md)   
 [Designdetaljer: Lagerkalkylering](design-details-inventory-costing.md)

