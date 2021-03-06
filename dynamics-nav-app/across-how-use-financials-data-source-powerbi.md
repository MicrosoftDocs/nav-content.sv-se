---
title: "Skapa en Power BI-datakälla med din Dynamics NAV"
description: "Du kan göra din Dynamics NAV-data tillgänglig som datakälla i Power BI och bygga kraftfulla rapporter av din verksamhets status."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b1beb7286eb221e5df3e7d5b2050ddcb389a0a07
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="using-included365finincludesd365finmdmd-as-a-power-bi-data-source"></a>Använda [!INCLUDE[d365fin](includes/d365fin_md.md)] som en Power BI-datakälla
Du kan göra din [!INCLUDE[d365fin](includes/d365fin_md.md)]-data tillgänglig som datakälla i Power BI och bygga kraftfulla rapporter av din verksamhets status.  

> [!NOTE]  
>   Du måste ha ett giltigt konto med [!INCLUDE[d365fin](includes/d365fin_md.md)] och med Power BI. Dessutom måste du hämta [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a>Att lägga till [!INCLUDE[d365fin](includes/d365fin_md.md)] som datakälla i Power BI Desktop
1. I Power BI Desktop i den vänstra navigeringsrutan väljer du **hämta data**.
2. I fönstret **Hämta data** väljer du **onlinetjänster**, väljer **Dynamics NAV** och sedan knappen **Anslut**.

   Power BI visar en guide som vägleder dig genom anslutningsprocessen. Första steget är att ange en OData-URL och namnet på företaget som är associerat med ditt [!INCLUDE[d365fin](includes/d365fin_md.md)]-konto.  

   För den *OData-URL*, kan du kopiera OData V4-URL för någon av webbtjänsterna som finns på sidan **webbtjänster** i [!INCLUDE[d365fin](includes/d365fin_md.md)], som t.ex. `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.  

   För *företagsnamn*, använder du namnet som visas i fältet **namn** i fönstret **företagsinformation** i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Om din [!INCLUDE[d365fin](includes/d365fin_md.md)] innehåller flera företag, väljer du relevant företagsnamn i listan i fönstret **företag**. I båda fallen kontrollerar du att namnet som du anger i Power BI-guiden motsvarar exakt den text som visas i [!INCLUDE[d365fin](includes/d365fin_md.md)], som t.ex. `My Company`.
3. När du har angett informationen väljer du knappen OK. Nästa steg i guiden är att ange användarnamn och lösenord.

   > [!NOTE]  
>    Om det finns andra alternativ för användarautentisering i den vänstra navigeringen, väljer du *grundläggande*.
4. Ange ditt användarnamn och lösenord. Du hittar den här informationen i fönstret **Användare** i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Använd **Webbåtkomstnyckel** som lösenord.

   Ditt användarnamn är till exempel *ADMIN* och webbtjänståtkomstnyckeln som fungerar som ditt lösenord och *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.
5. Klicka på knappen **Anslutning** för att fortsätta. Power BI-guiden visar en lista över [!INCLUDE[d365fin](includes/d365fin_md.md)]-datakällor. Dessa datakällor motsvarar de webbtjänster som du har publicerat från ditt [!INCLUDE[d365fin](includes/d365fin_md.md)].

   Du kan också skapa en ny webbtjänst-URL i [!INCLUDE[d365fin](includes/d365fin_md.md)] med hjälp av åtgärden **skapa datauppsättning** på sidan **webbtjänster** med hjälp av den assisterade inställningsguiden **Ställ in rapportering**  eller genom att välja åtgärden **redigera i Excel** i någon lista.

6. Ange de data som du vill lägga till i din datamodell och välj knappen **Läs in**.
7. Upprepa stegen för att lägga till ytterligare [!INCLUDE[d365fin](includes/d365fin_md.md)]-data till Power BI-datamodellen.

   > [!NOTE]  
>    När du har anslutit till [!INCLUDE[d365fin](includes/d365fin_md.md)], kommer du inte att uppmanas till att ge OData-URL, användarnamn och lösenord.

När data har lästs in kommer den att visas i den högra navigeringen på sidan. Nu har du lyckats ansluta till dina Dynamics NAV-data och är redo att börja skapa Power BI-rapporten. Mer information finns i [Power BI dokumentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).

## <a name="see-also"></a>Se även
[Affärsstöd](bi.md)  
[Välkommen till [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Importera verksamhetsdata från andra finanssystem](upload-data.md)  
[Ställa in [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Ekonomi](finance.md)  

