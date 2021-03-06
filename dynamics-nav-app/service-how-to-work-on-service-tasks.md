---
title: "Så här arbetar du med serviceuppgifter"
description: "När du har skapat en serviceorder eller serviceoffert, registrerat serviceartikelrader och fördelat resurser på orderns eller offertens serviceartiklar kan du börja reparera och underhålla serviceartiklarna."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 3e8fd9d1e56de77c54f5190d97f95faa0702908e
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-work-on-service-tasks"></a>Så här arbetar du med serviceuppgifter
När du har skapat en serviceorder eller serviceoffert, registrerat serviceartikelrader och fördelat resurser på orderns eller offertens serviceartiklar kan du börja reparera och underhålla serviceartiklarna.  

I [!INCLUDE[d365fin](includes/d365fin_md.md)] finns fönstret **Serviceuppgifter** där du får en översikt över alla serviceartiklar som behöver åtgärdas. Du kan se det som en instrumentbräda för service - se vilka order som väntar på att åtgärdas, söka efter och registrera reservdelar och hålla lagret uppdaterat.  
  
Om du vill spåra ändringar och få en grafisk översikt över serviceverksamheten, kan du med statistikverktygen i [!INCLUDE[d365fin](includes/d365fin_md.md)] automatiskt skapa en snabb analys i diagramformat.  
  
## <a name="to-work-on-a-service-task"></a>Så här arbetar du med serviceuppgifter  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceuppifter** och välj sedan relaterad länk. 
2. Om du vill ha en lista över serviceuppgifterna som en viss resurs/resursgrupp är fördelad till, fyller du i fältet **Resursfilter**/ **Resursgruppfilter** och trycker på RETUR.  
3. Om du vill ha en lista över serviceuppgifter med ett visst svarsdatum eller svarsdatum inom en viss tidsperiod, fyller du i fältet **Svarsdatumfilter** och trycker på RETUR.  
4. Om du vill ha en lista över serviceuppgifter med en viss fördelningsstatus/reparationsstatus fyller du i fältet **Fördelningsstatusfilter** eller **Reparationsstatus kodfilter** och trycker på RETUR.  
5. Markera serviceuppgiften som du vill arbeta med. På fliken **Analysera** i gruppen **Serviceuppgifter** väljer du **Artikelförslag**. Fönstret **Serviceartikeldokument** öppnas.  
6. Registrera standardtext, reservdelar, resurstid och kostnader med hjälp av motsvarande alternativ i fältet **Typ**:  <Blank>, **Artikel**, **Resurs**, och **Kostnad**.  
7. I fältet **Reparationsstatus** markerar du lämplig status.  
  
   > [!NOTE]  
   >  Fyll i fältet **Reparationsstatus** med statusvärdet **Avslutad** eller **Delvis servad** om serviceartikeln har avslutats eller om en annan resurs ska fortsätta med servicen. Statusvärdet **Avslutad** eller **Omfördelning nödvändig** väljs automatiskt för den här serviceartikelns fördelningstransaktion.  

## <a name="to-register-service-operations"></a>Så här registrerar du serviceoperationer  
När du utför en service på en serviceorder kan du registrera detaljerad information om de artiklar som använts, uppkomna kostnader och tidsåtgång. Den information som du anger lagras i fönstret **Serviceartikeldokument**. Du kan uppdatera informationen när det behövs. 
   
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceorder** och välj sedan relaterad länk.  
2. Öppna serviceordern som du vill registrera service för och välj artikelrad.  
3. Välj **Åtgärder**, välj **Rad** och välj sedan **Serviceartikeldokument.**  
4. På raderna anger du de artiklar som använts, uppkomna kostnader och tidsåtgång.  
  
   > [!NOTE]  
   >  Du kan också registrera en service direkt på de servicerader som är kopplade till serviceordern.  
  
## <a name="to-register-spare-parts"></a>Så här registrerar du reservdelar  
När du arbetar med serviceartiklar i serviceorder kanske du behöver använda reservdelar till servicen. Nedan beskrivs en procedur för att registrera reservdelarna som du använder i fönstret **Serviceartikeldokument**.  
  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceuppifter** och välj sedan relaterad länk. 
2. Klicka på raden som innehåller relevant serviceartikel och klicka på **Artikelförslag**.  
3. Ange en ny servicerad.  
4. I fältet **Typ** väljer du **Artikel**.  
5. I fältet **Nr.** markera relevant reservdel.  
6. I fältet **Antal** anger du hur många artiklar du vill använda.  
  
 Du kan använda en liknande procedur för att registrera reservdelarna på sidan **Servicerader** som du öppnar från sidan **Serviceorder**.  
  
## <a name="to-register-spare-parts-from-a-service-order"></a>Så här kan du registrera reservdelar från en serviceorder  
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceorder** och välj sedan relaterad länk.  
2. Öppna serviceordern som du vill registrera reservdelar för.  
3. Välj den rad som innehåller aktuell serviceartikel. Välj **Åtgärder**, välj **Order**, och sedan **Servicerader**.  
4. Ange en ny servicerad.  
  
## <a name="to-replace-a-service-item-or-a-service-item-component"></a>Så här ersätter du en serviceartikel eller en Serviceartikelkomponent  
När du servar en serviceartikel som innehåller komponenter kanske du måste byta ut trasiga komponenter mot nya. När du anger en reservdel för en serviceartikel med komponenter kan du välja mellan att ersätta komponenten eller skapa en ny. Den nya artikeln registreras inte som komponent i serviceartikeln förrän du bokför serviceraden eller serviceordern. 
    
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceuppifter** och välj sedan relaterad länk. 
2. Klicka på raden som innehåller relevant serviceartikel och klicka på **Artikelförslag**.  
3. Ange en ny servicerad.  
4. I fältet **Typ** väljer du **Artikel**.  
5. I fältet **Nr.** Välj komponenten som ska ersättas.  
6. Tryck på **Retur**. En dialogruta visas med tre alternativ: **Ersätt komponent**, **Ny komponent** och **Ignorera**. Alternativen beskrivs i tabellen nedan.  
  
    |Alternativ | Description|  
    |----------------------------------|---------------------------------------|  
    |**Ersätt komponent**|Status för den komponent som ska ersättas ändras till ej aktiv och den visas på listan över ersatta komponenter för serviceartikeln.|  
    |**Ny komponent**|Den nya komponenten infogas på komponentlistan för serviceartikeln.|  
    |**Ignorera**|Ingenting händer med serviceartikelns komponentlista.|  
  
7. Välj **Ersätt komponent**.  
8. Välj komponenten som ska ersättas och välj sedan **OK**.  

## <a name="to-change-the-response-time-for-a-service-item-line"></a>Så här ändrar du svarstid för en serviceartikelrad  
När du registrerar en serviceartikelrad i en serviceorder eller offert om serviceartikeln finns i ett servicekontrakt anges automatiskt standardsvarstiden i timmar. Svarsdatum och svarstid beräknas därefter. Du kan ändra svarstiden i timmar och svarsdatum och svarstid om du vill.  

1. Välj ikonen ![Sök efter sida eller rapport](media/ui-search/search_small.png "Söka efter sida eller rapport") ange **Serviceorder** eller **Serviceofferter** och välj sedan relaterad länk.  
2. Välj den serviceorder eller serviceoffert som du vill öppna kortet.  
3. På den serviceartikelrad som du vill ändra svarstid för i fältet **Svarstid (timmar)** eller i fälten **Svarsdatum** och **Svarstid** anger du nya svarstimmar eller svarsdatum och svarstid.  

## <a name="to-register-faultresolution-codes"></a>Så här registrerar du fel/åtgärdskoder  
När en serviceartikel har reparerats kan du ange både felkoden och åtgärdskoden för artikeln genom att välja en kombination från de befintliga fel- och åtgärdskodssambanden. De fel- och åtgärdskoder som valts visas nu i motsvarande fält i fönstret **Serviceartikeldokument**. Du kan också registrera koderna direkt i det här fönstret.  
    
1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Serviceuppifter** och välj sedan relaterad länk. 
2. Klicka på raden som innehåller relevant serviceartikel och klicka på **Artikelförslag**.  
3. På sidan **Serviceartikeldokument** väljer du **Fel- och åtgärdssamband koder**. Fönstret **Fel-/åtgärdssambandskoder** öppnas.  
  
  >  [!Note]
  >  Filter sätts på de samband som visas i fönstret via kopiering av serviceartikelgruppen och felkoderna från fönstret **Serviceartikeldokument**.  
  
4. Fyll i raden. Välj rätt kombination av fel- och åtgärdskoder och klicka sedan på **OK** för att kopiera den till serviceartikeln. Om någon lämplig kombination inte finns kan du skapa en ny kombination i fönstret.  

## <a name="see-also"></a>Se även  
[Så här: ställa in felrapporteringsnivån](service-how-setup-fault-reporting.md)
[fördelningsstatus och reparationsstatus](service-allocation-status-and-repair-status.md)  
[Servicebokföring](service-service-posting.md)  


