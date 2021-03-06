---
title: "Hantera kunder som använder Dynamics 365 for Sales"
description: "Du kan använda Dynamics 365 for Sales inne i Dynamics NAV for Financials för att mappa data och ha sömlös integration och synkronisering i processen från kundämne till betalning."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: integration, synchronize, map
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 3f26a80427a2a1c38949ca94848751527383d7f9
ms.contentlocale: sv-se
ms.lasthandoff: 10/26/2017

---
# <a name="managing-customers-and-sales-created-in-dynamics-365-for-sales"></a>Hantera kunder och försäljningsorder som har skapats i Dynamics 365 for Sales
Om du använder Dynamics 365 for Sales för kundengagemang kan du använda [!INCLUDE[d365fin](includes/d365fin_md.md)] för orderbehandling och ekonomi och har sömlös integrering i processen från kundämne till betalning.

Om programmet har konfigurerats för integration med Dynamics 365 for Sales, har du åtkomst tillförsäljningsdata från [!INCLUDE[d365fin](includes/d365fin_md.md)]och tvärtom i vissa fall. Integrationen låter dig arbeta med och synkronisera datatyper som är gemensamma för båda tjänsterna, till exempel kunder, kontakter och försäljningsinformation och hålla informationen uppdaterad på båda platserna.  

Säljare i Dynamics 365 for Sales kan till exempel använda prislistor från [!INCLUDE[d365fin](includes/d365fin_md.md)] när de skapar en försäljningsorder. När de lägger till artikeln till försäljningsorderraden i Dynamics 365 for Sales kan de också visa lagernivån (tillgänglighet) av artikeln från [!INCLUDE[d365fin](includes/d365fin_md.md)].

På samma sätt kan orderprocessorer i [!INCLUDE[d365fin](includes/d365fin_md.md)] hantera speciella särdrag hos försäljningsorder som överförs automatiskt eller manuellt från Dynamics 365 for Sales, som t.ex. att automatiskt skapa och bokföra giltiga försäljningorderrader för artiklar eller resurser som har angetts i Sales som produkter ej i register. Mer information finns i avsnittet ”Hantera speciella försäljningsorderdata”.  

> [!NOTE]
> Innan du kan integrera med Dynamics 365 for Sales måste du göra olika tekniska förberedelser. Mer information finns i [så här: lägga upp en Dynamics CRM-anslutning](https://msdn.microsoft.com/en-us/dynamics-nav/how-to-set-up-a-dynamics-crm-connection) och [så här: förbereda för integrering i Dynamics CRM](https://msdn.microsoft.com/en-us/dynamics-nav/how-to-prepare-dynamics-crm-for-integration) på MSDN.

## <a name="setting-up-the-connection"></a>Ställer in anslutningen
Hemifrån kan du öppna den assisterade konfigurationsguiden **anslutningsinställningar för Dynamics 365 for Sales** som hjälper dig att konfigurera anslutningen. När detta är klart får du en sömlös koppling av Dynamics 365 for Sales-poster med [!INCLUDE[d365fin](includes/d365fin_md.md)]-poster.  

> [!NOTE]  
> Förklarar de assisterade inställningarna, men du kan utföra samma aktiviteter manuellt i fönstret **installation av Dynamics 365 for Sales-anslutning**.

I assisterade konfigurationsguiden, kan du välja vilka data som ska synkroniseras mellan två tjänster. Du kan också ange att du vill importera dina befintliga Dynamics 365 for Sales-lösning. I detta fall måste du ange behörigheter för ett användarkonto.

### <a name="setting-up-the-user-account-for-importing-the-solution"></a>Konfigurera användarkontot för att importera lösningen
Om du vill importera en befintlig Dynamics 365 for Sales-lösning, använder guiden ett administratörskonto. Kontot måste vara en giltig användare i Dynamics 365 for Sales med följande säkerhetsrollerna:

* Systemadministratör  
* Lösningsanpassare  

Mer information finns i [skapa användare och tilldela säkerhetsroller i Microsoft Dynamics NAV (online) säkerhetsroller](https://technet.microsoft.com/library/jj191623.aspx) på techNet och [så här hanterar du användare och behörigheter](ui-how-users-permissions.md).  

Det här kontot används bara vid installationen. När lösningen har importerats till [!INCLUDE[d365fin](includes/d365fin_md.md)], behövs inte längre kontot.

### <a name="setting-up-the-user-account-for-synchronization"></a>Konfigurera användarkontot för synkronisering
Integrering med hjälp av ett delat användarkonto används. Därför måste du i din Office 365-prenumeration skapa en särskild användare som ska användas för synkroniseringen mellan två tjänster. Kontot måste redan vara en giltig användare i Dynamics 365 for Sales, men du behöver inte tilldela säkerhetsroller till kontot eftersom guiden gör detta åt dig. Du måste ange det här kontot en eller flera gånger i inställningsguiden, beroende på hur mycket synkronisering du vill aktivera. Mer information finns i [Skapa användare och tilldela Microsoft Dynamics NAV (online) säkerhetsroller](https://technet.microsoft.com/library/jj191623.aspx) på techNet.

Om du vill aktivera *artikeldisposition*, måste integreringsanvändarkontot ha en snabbtangent för webbplatstjänster. Detta är eni två stegssak på sidan [!INCLUDE[d365fin](includes/d365fin_md.md)]för det användarkontot och du måste du välja knappen **ändra webbtjänstnyckeln** och i konfigurationsguiden för Dynamics 365 for Sales-anslutning måste du ange användaren som OData webbtjänstanvändare.

Om du vill aktivera *integrering av försäljningsorder*, måste du ange en användare som kan hantera synkroniseringen - Integrationsanvändare eller ett annat konto.

### <a name="coupling-records"></a>Kopplingsposter
I assisterade konfigurationsguiden, kan du välja vilka data som ska synkroniseras mellan två tjänster. Men du kan också ange inställningar för synkronisering av vissa typer av data. Detta kallas *koppling*, och det här avsnittet innehåller rekommendationer som du måste ta hänsyn till.

Till exempel om du vill visa Dynamics 365 for Sales-konton som kunder i [!INCLUDE[d365fin](includes/d365fin_md.md)], måste du koppla de två typerna av poster. Det är inte mycket komplicerat, öppna fönstret **Kundlista** i [!INCLUDE[d365fin](includes/d365fin_md.md)], och det finns en åtgärd i menyfliksområdet för att koppla dessa data med Dynamics 365 for Sales. Därefter anger du vilka [!INCLUDE[d365fin](includes/d365fin_md.md)]-kunder som matchar vilka konton i Dynamics 365 for Sales.

I vissa områden måste funktionen koppla vissa uppsättningar data innan andra uppsättningar data visas i följande lista:

* Kunder och konton.  
  * Koppla säljare först med Dynamics 365 for Sales-användare  
* Artiklar och resurser  
  * Koppla först måttenheter med Dynamics 365 for Sales enhetsgrupper  
* Artiklar och resurspriser  
  * Koppla kundprisgrupper med Dynamics 365 for Sales priser först  

> [!NOTE]  
>   Obs! Om du använder priser i utländska valutor, se till att du kopplar valutor till Dynamics 365 for Sales transaktionsvalutor.

Försäljningsorder för Dynamics 365 for Sales beror på ytterligare information, till exempel kunder, enheter, valutor, kundprisgrupper, artiklar och/eller resurser. För att Dynamics 365 for Sales försäljningsorder ska fungera utan problem, måste du koppla kunder, enheter, valutor, kundprisgrupper, artiklar och/eller resurser först.

### <a name="synchronizing-records-fully"></a>Synkronisera poster helt
I slutet av den assisterade konfigurationsguiden kan du välja åtgärden **kör fullständig synkronisering** för att starta synkronisering av alla [!INCLUDE[d365fin](includes/d365fin_md.md)]-poster med alla relaterade poster i den kopplade Dynamics 365 for Sales-lösningen. I fönstret **CRM fullständig synk.granskning** kan du välja åtgärden **starta**. Sedan börjar synkroniseringen köra projekt efter beroenden. Exempelvis synkroniseras valutaposter innan kundposter. Fullständig synkronisering kan ta lång tid och kommer att köras i bakgrunden så att du kan fortsätta att arbeta i [!INCLUDE[d365fin](includes/d365fin_md.md)].

Om du vill kontrollera förloppet för enskilda projekt i en fullständig synkronisering, öka detaljnivån i fältet **Transaktionsstatus för jobbkö**, eller **Från projektstatus för int. tabell**, eller **CRM fullständig synk.granskning** i fönstret **CRM fullständig synk.granskning**.

Från fönstret **Konfigurera anslutning till Dynamics 365** kan du få information om fullständig synkronisering när som helst. Här kan du också öppna fönstret **Tabellmappningar för integrering** för att visa detaljerad information om tabeller i Dynamics NAV och i Dynamics 365 for Sales-lösningen som måste synkroniseras.

## <a name="handling-special-sales-order-data"></a>Hantering av speciella försäljningsorderdata
Försäljningsorder i Dynamics 365 for Sales kommer att överföras till [!INCLUDE[d365fin](includes/d365fin_md.md)] automatiskt om du markerar kryssrutan **Automatiskt skapa försäljningsorder** i fönstret **Konfigurera anslutning till Microsoft Dynamics 365 for Sales**. På sådana försäljningsorder överförs fältet **Namn** på den ursprungliga ordern och mappas till fältet **Externa verifikationsnummer** på försäljningsordern i [!INCLUDE[d365fin](includes/d365fin_md.md)].

Detta fungerar även om den ursprungliga försäljningsordern innehåller produkter som ej är i register vilket avser artiklar eller resurser som inte är registrerade hos någon produkt. I så fall måste du fylla i fälten **Produkttyp ej i register** och **Produktnr ej i register** i fönstret **Försäljningsinställningar** så att denna oregistrerade produktförsäljning mappas till ett angivet artikel-/resursnummer för ekonomisk analys.

Om artikelbeskrivningen på den ursprungliga försäljningsordern är mycket omfattande, skapas en ytterligare försäljningsorderrad av typen Kommentar för att hålla hela texten på försäljningsordern i [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="see-also"></a>Se även
[Kundhantering](marketing-relationship-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Anpassa [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)  
[Så här hanterar du användare och behörigheter](ui-how-users-permissions.md)    
[Integrera organisationen och användare till Dynamics NAV (online)](https://www.microsoft.com/en-US/Dynamics/crm-customer-center/onboard-your-organization-and-users-to-dynamics-365-online.aspx)  

##

