---
title: "Installera till�gg f�r att anpassa Dynamics NAV"
description: "L�r dig mer om att l�gga till funktioner och anpassa Dynamics NAV genom att installera till�gg."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 07/07/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 109eb8d0e2a38566739878ef513ffa3bec8dcd30
ms.contentlocale: sv-se
ms.lasthandoff: 10/26/2017

---
# <a name="customizing-dynamics-nav-using-extensions"></a>Anpassa Dynamics NAV med till�gg
Du kan �ndra [!INCLUDE[d365fin](includes/d365fin_md.md)] genom att installera till�gg som l�gger till funktioner, �ndrar beteende eller ger dig tillg�ng till nya onlinetj�nster.
N�r du f�rst startar f�rst [!INCLUDE[d365fin](includes/d365fin_md.md)], har du dessutom n�gra till�gg installerade. Med tiden kommer fler till�gg att g�ras tillg�ngliga till dig, och du kan d� v�lja om du vill anv�nda till�gg eller inte.

Till exempel ger Microsoft ett till�gg som ger integrering med PayPal Payments Standard. Detta till�gg instalelras dessutom som standard.
Men om ett annat till�gg �r tillg�ngligt som erbjuder integrering med en annan utbetalningtj�nst, kan du installera det nya till�gget och sedan v�lja vilka av de tv� tj�nsterna som ska anv�ndas.  

Du hanterar till�ggen i f�nstret **Till�ggshantering**. Du kan �ppna det h�r f�nstret fr�n startsidan. I det �vre h�gra h�rnet v�ljer du ikonen **S�k efter sidan eller rapporten** ![S�k efter sidan eller rapporten](media/ui-search/search_small.png "S�k efter sidan eller rapporten") i det �vre h�gra h�rnet anger du **Underh�ll, n�sta service**, och v�lj sedan relaterad l�nk.  

> [!NOTE]  
>   Om du tror att du borde ha �tkomst till ett till�gg, men dess funktioner inte g�r att hitta kontrollerar du f�nstret **till�ggshantering** om till�gget inte finns, kan du installera det enligt vad som beskrivs i f�ljande avsnitt.  

## <a name="installing-an-extension"></a>Installerar till�gg
Du kan f� nya till�gg fr�n marknadsplatsen p� [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1). H�r kan du se alla tillg�ngliga till�gg f�r [!INCLUDE[d365fin](includes/d365fin_md.md)] och du kan f� program, till�gg och inneh�llspaket f�r andra Microsoft-produkter. Ange relevanta filter, ta en titt p� varje till�ggs uppgifter och f� till�gg f�r ditt [!INCLUDE[d365fin](includes/d365fin_md.md)].  
> [!NOTE]  
>   Logga in p� [AppSource.microsoft.com](https://appsource.microsoft.com/) med hj�lp av e-postkonto som du anv�nder f�r [!INCLUDE[d365fin](includes/d365fin_md.md)]. Anv�nd samma e-postkonto f�r andra tj�nster och produkter f�r en bra upplevelse.  

Du kan ocks� komma till marknadsplatsen fr�n [!INCLUDE[d365fin](includes/d365fin_md.md)]. I f�nstret **Till�ggshantering** kan du se till�ggen som installeras f�r n�rvarande, och du kan �ppna sidan **till�ggmarknadsplatsen** som visar till�ggen f�r [!INCLUDE[d365fin](includes/d365fin_md.md)] som f�r n�rvarande finns tillg�ngliga i AppSource. Om du v�ljer l�nken *Fler appar* tas du till [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

Om du v�ljer ett till�gg kan du l�sa om vad till�gget anv�nds till och du kan f� mer information om till�gget. N�r du v�ljer att f� ett till�gg, m�ste du godk�nna anv�ndningsvillkoret. Om du f�r till�gget fr�n AppSource-webbplatsen kommer du att loggas in p� [!INCLUDE[d365fin](includes/d365fin_md.md)] f�r att slutf�ra installationen.  

N�r du installerar till�gget kanske du beh�ver m�ste konfigurera det, till exempel ange ett konto f�r anv�ndning med till�gget **PayPal-standardbetalning f�r [!INCLUDE[d365fin](includes/d365fin_md.md)]**.
Andra till�gg l�gger bara till i f�lt p� en befintlig sida, eller l�gger till en ny sida, till exempel.   

Om du avinstallerar till�gget och du sedan �ndrar dig kan du installera det p� nytt. N�r du avinstallerar till�gg som du har anv�nt, bevaras data s� att de �r tillg�ngliga om du installerar till�gget igen.  

N�gra till�gg ges ut av Microsoft, och andra till�gg ges ut av [andra f�retag](ui-extensions-other.md). Alla till�gg testas innan de g�rs tillg�ngliga f�r dig, men vi rekommenderar att du �ppnar l�nkarna som tillhandah�lls med varje till�gg om du vill veta mer om till�gget innan du v�ljer att installera det.  

Microsoft ger �ven f�ljande till�gg:  

* [Dynamics GP Datamigrering](ui-extensions-dynamicsgp-data-migration.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [QuickBooks datamigrering](ui-extensions-quickbooks-data-migration.md)  
* [F�rs�ljnings- och lagerprognos](ui-extensions-sales-forecast.md)  
* [Ceridian l�ner](ui-extensions-ceridian-payroll.md)  
* [Importera QuickBooks-l�nefil](ui-extensions-quickbooks-payroll.md)  
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)
* [GetAddress.io UK Postcodes](ui-extensions-getaddressio.md)
* [QuickBooks Online datamigrering](ui-extensions-quickbooks-online-data-migration.md)
* [Revisorsportal](ui-extensions-accountant-portal.md)  
* [Image Analyzer](ui-extensions-image-analyzer.md)

> [!NOTE]  
>  Till�gg �r inte tillg�ngliga i AppSource s� snart vi meddelar en uppdatering. Du kan h�lla utkik efter till�gg i [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>Se �ven
[S� h�r aktiverar du kundutbetalning via PayPal](sales-how-enable-payment-service-extensions.md)  
[Migrera verksamhetsdata fr�n andra finanssystem](upload-data.md)    
[[!INCLUDE[d365fin](includes/d365fin_md.md)]-till�gg fr�n andra leverant�rer](ui-extensions-other.md)  
[V�lkommen till [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  

##


