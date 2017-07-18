---
title: "Använda Dynamics NAV innehållspaket för Power BI"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6351e4819a2f3665cc561b5b1f868eea5d435f75
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="using-the-dynamics-nav-content-pack-for-power-bi"></a>Använda Dynamics NAV innehållspaket för Power BI
Det är enkelt att få insikter om Dynamics NAV-data med Power BI och innehållspaketet för Dynamics NAV. Power BI hämtar dina data och bygger en förinstallerad instrumentbräda och rapporter baserade på den data.  

Innehållspaketet är förkonfigurerat för att arbeta med försäljningsdata och ekonomiska data från demonstrationsföretaget som du får när du registrerar dig på förhandsgranskningen av Dynamics NAV.  

- Välj något visuellt på instrumentbrädan för att få upp en av sju underliggande rapporter.  
- Filtrera rapporten eller lägg till fält som du vill övervaka.  
- Sätt fast den här vyn på instrumentbrädan om du vill fortsätta spårningen.  
Instrumentbrädan och underliggande rapporter uppdateras dagligen. Du kan kontrollera uppdateringsschemat och ändra frekvens på datauppsättningen.  

## <a name="accessing-dynamics-nav-in-power-bi"></a>Öppna Dynamics NAV i Power BI
Om du vill se data för Dynamics NAV i Power BI måste du ha följande:  

- Åtkomst till Dynamics NAV. Mer information finns i [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714).  
- Åtkomst till Power BI. Mer information finns i [Power BI](https://powerbi.microsoft.com).

Du hittar ytterligare information på webbplatsen för Power BI om [lägga till Dynamics NAV ](http://go.microsoft.com/fwlink/?LinkID=760850)-innehållspaket till Power BI.  

Om du vill komma åt Dynamics NAV-innehållspaketet i Power BI, i anslutningsfönstret måste du ange följande information:

| Fält       | Beskrivning              |
|-------------|--------------------------|
|**OData feed URL**|OData-URL så att Power BI kan få åtkomst till data från ditt företag som t.ex. https://mybusiness.com:7048/MS/OData/Company('CRONUS%20US').|
|**Autentiseringsmetod**|Välj **grundläggande**.|
|**Användarnamn**|E-postkontot som du som du använde till att registrera dig för signerar för Dynamics NAV , t.ex. *me@mybusiness.com*.|
|**Lösenord**|Detta är webbtjänståtkomstnyckel för ditt användarkonto i Dynamics NAV. |

Detta innebär dock att du måste ha två enheter av information från Dynamics NAV: OData-URL och webbtjänståtkomstnyckel för ditt användarkonto.  
**Få URL:en**  
När du lägger till Dynamics NAV till Power BI måste du ange en URL, så att Power BI kan komma åt data från företaget. I anslutningsfönstret kommer URL:en att hänvisas till som **OData Feed URL** och måste ha följande format:

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
I det här exemplet är *mybusiness* namnet på din Dynamics NAV-tjänst och *CRONUS US* är namnet på demonstrationsföretaget med *%20* som representerar utrymmet i namnet.   
Om du vill få URL:en söker du efter och öppnar i Dynamics NAV fönstret **Webbtjänster**. I det här fönstret visas webbtjänsterna som för närvarande finns tillgängliga och du kan kopiera länken från fältet **OData-URL** för en av de standardinställda OData-webbtjänsterna.  
**Få webbtjänståtkomstnyckeln**  
För att använda data från Dynamics NAV , i Power BI, i fönstret **Anslut till Dynamics NAV** måste du ange din användarnamn, som är ett e-postkonto, och ett lösenord. Lösenordet är webbtjänståtkomstnyckeln som är konfigurerad för ditt användarkonto i Dynamics NAV.   
Om du vill få en webbtjänståtkomstnyckel, i Dynamics NAV söker du efter fönstret **Användare** och öppnar sedan kortet för ditt användarkonto. På snabbfliken **Webbtjänståtkomst** kopierar du innehållet i fältet **Webbtjänståtkomstnyckel**. Om fältet är tomt, välj **Ändra webbtjänståtkomstnyckel**, välj fältet **Nyckeln upphör aldrig att gälla** och tryck sedan på OK-knappen. Du kan sedan kopiera nyckeln.  

## <a name="getting-data-from-dynamics-nav"></a>Hämta data från Dynamics NAV 
Instrumentbrädan för Dynamics NAV visar de vanligaste rapporterna som du kommer att behöva använda för att spåra verksamheten. Data extraheras från ditt Dynamics NAV-företag med webbtjänster för att läsa realtidsdata. I Dynamics NAV anger fönstret **Webbtjänster** webbtjänsterna som har konfigurerats för dig, inklusive följande som förbrukas av innehållspaketet i Power BI:  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-inställning  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Obs!** Om du ändrar namnet på någon av dessa webbtjänster, kommer data inte att visas i Power BI.  
Om du vill lägga till i andra data i Power BI, måste du hitta tabellerna i Dynamics NAV och exponera dem som webbtjänster och sedan lägga till dem i innehållspaketet. Detta är ett avancerat scenario och vi rekommenderar att du börjar med data som redan är tillgängliga i Power BI.  

## <a name="troubleshooting"></a>Felsökning
Instrumentbrädan för Power BI förlitar sig på de publicerade webbtjänsterna som visas ovan, och kommer att innehålla data från demonstrationsföretaget eller ditt eget företag om du importerar data från den aktuella finansinställningslösningen. Men om något går fel kommer denna sektion att ge en tillfällig lösning för de vanligaste problemen.  

**"Parametervalidering misslyckades. Se till att alla parametrar är giltiga"**  
Om du ser det här felet efter att du har angett Dynamics NAV-URL:en ska du se till att följande krav är uppfyllda:  

- URL:en följer exakt deta mönster:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
- Ta bort all text efter företagsnamnet i parentesen  
- Se till att det inte finns något avslutande snedstreck i slutet av URL:en.  
- Se till att det finns en säker anslutning som anges av URL:en som börjar med *https*.  


**"Inloggningen misslyckades"**  
Om du får felet "Inloggningen misslyckades" när du loggar in på instrumentbrädan med dina autentiseringsuppgifter för Dynamics NAV kan detta orsakas av ett följande problem:

* Kontot som du använder har inte behörighet att läsa data från Dynamics NAV från ditt konto.

    Kontrollera ditt användarkonto i Dynamics NAV och se till att du har använt rätt webbtjänståtkomstnyckel som lösenord och försök sedan igen.  
* Instansen Dynamics NAV som du försöker att ansluta till har inte ett giltigt SSL-certifikat. I så fall visas en mer detaljerat felmeddelande ("det går inte att upprätta betrott SSL-förhållande").

    **Obs!**: Självsignerade certifikat stöds inte.  


**"Hoppsan"**  
Om du ser feldialogen "Hoppsan" när du har passerat autentiseringdialogen, orsakas den oftast av ett problem vid anslutning av data för innehållspaketet.

* Kontrollera att URL:en följer mönstret som angavs tidigare:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
* Ett vanligt fel är att ange den fullständiga URL:en för en viss webbtjänst:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')/powerbifinance-setup  
* Eller så har du glömt att ange företagsnamnet:

    https://mybusiness.projectmadeira.com:7048/MS/OData/  


## <a name="see-also"></a>Se även
[Välkommen till Dynamics NAV](across-get-started.md)  

