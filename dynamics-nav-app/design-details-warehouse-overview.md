---
title: "Designdetaljer - Översikt över distributionslager"
description: "För att stödja den fysiska hanteringen av artiklar i zonen och på lagerplatsnivån måste all information spåras för varje transaktion eller transport i distributionslagret. Det hanteras i tabellen **Dist.lager transaktion**. Varje transaktion lagras i ett distributionslagerregister."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 36fc951668580b4a74d8642a734f321312aaaab7
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-warehouse-overview"></a>Designdetaljer: Översikt över distributionslager
För att stödja den fysiska hanteringen av artiklar i zonen och på lagerplatsnivån måste all information spåras för varje transaktion eller transport i distributionslagret. Det hanteras i tabellen **Dist.lager transaktion**. Varje transaktion lagras i ett distributionslagerregister.  

Distributionslagerdokument och en distributionslagerjournal används för att registrera artikeltransporter i distributionslagret. Varje gång en artikel i distributionslagret flyttas, tas emot, förs in, plockas, utlevereras eller justeras, registreras distributionslagertransaktioner för att lagra den fysiska informationen om zon, lagerplats och antal. Mer information finns i [Designdetaljer: Ingående distributionslagerflöde](design-details-outbound-warehouse-flow.md).  

Tabellen **Lagerplatsinnehåll** används för att hantera alla olika dimensioner av innehållet i en lagerplats per artikel, t.ex enhet, maximal antal och lägsta antal. Tabellen **Lagerplatsinnehåll** innehåller även flödesfält till distributionslagertransaktionerna, distributionslagerinstruktionerna och distributionslagerjournalraderna, som säkerställer att tillgängligheten för en artikel per lagerplats och en lagerplats för en artikel kan beräknas snabbt. Mer information finns i [Designdetaljer: disposition i distributionslagret](design-details-availability-in-the-warehouse.md).  

När artikeltransaktioner uppstår utanför distributionslagerenheten används en standardjusteringlagerplats per lagerställe för att synkronisera distributionslagerposter med lagerposter. Under inventeringen av distributionslagret registreras alla avvikelser mellan de beräknade och inventerade kvantiteterna på justeringslagerplatsen och sedan bokförs de som korrigerande artikeltransaktioner. Mer information finns i [Designdetaljer: Integrering med lager](design-details-integration-with-inventory.md)  

Följande illustration ger en översikt över typiska distributionslagerflöden.  

![Översikt över lagerprocesser](media/design_details_warehouse_management_overview.png "design_details_warehouse_management_overview")  

## <a name="basic-or-advanced-warehousing"></a>Grundläggande eller avancerad lagerstyrning  
Distributionslagerfunktion i [!INCLUDE[d365fin](includes/d365fin_md.md)] kan implementeras i olika komplexitetsnivåer, beroende på ett företag processer och ordervolym. Den huvudsakliga skillnaden är att aktiviteter utförs order-för-order i grundläggande lagerstyrning, när de konsolideras för flera order i avancerad lagerstyrning.  

 För att skilja mellan de olika komplexitetsnivåerna refererar denna dokumentation till två allmänna benämningar, grundläggande och avancerad lagerstyrning. Den här enkla differentieringen täcker flera olika komplexitetsnivåer som definieras av produktpartiklar och lagerplatsinställningar, där var och en stöds av olika användargränssnittsdokument . Mer information finns i [Designdetaljer: Lagerstyrningsinställningar](design-details-warehouse-setup.md).  

> [!NOTE]  
>  Den mest avancerade nivån av lagerstyrning kallas för ”WMS-installationer” i denna dokumentation, eftersom den här nivån kräver den mest avancerade partikeln, lagerstyrningssystem (Warehouse Management Systems).  

 Följande olika användargränssnittsdokument används i grundläggande och avancerade lagerhantering.  

## <a name="basic-ui-documents"></a>Grundläggande gränssnittsdokument  

-   **Lagerinförsel**  
-   **Lagerplockning**  
-   **Lagertransport**  
-   **Artikeljournal**  
-   **Artikelgrupperingsjournal**  
-   (Olika rapporter)  

## <a name="advanced-ui-documents"></a>Avancerade UI-dokument  

-   **Dist.lager inleverans**  
-   **Artikelinförsel förslag**  
-   **Dist.lager artikelinförsel**  
-   **Plockningsförslag**  
-   **Dist.lager plockning**  
-   **Transportförslag**  
-   **Dist.lager transport**  
-   **Intern dist.lager plockning**  
-   **Intern dist.lager art.införsel<**  
-   **Lagerplatsuppläggning förslag**  
-   **Lagerplatsinnehålluppl förslag**  
-   **Dist.lager artikeljournal**  
-   **Dist.lager Artikelgrupperingsjnl**  
-   (Olika rapporter)  

Se respektive fönsteravsnitt för mer information om varje dokument.  

### <a name="terminology"></a>Terminologi  
För att anpassas till de ekonomiska begreppen för inköp och försäljningar refererar lagerdokumentationen för [!INCLUDE[d365fin](includes/d365fin_md.md)] till följande villkor för objektflöde i distributionslagret.  

|Term|Description|  
|----------|---------------------------------------|  
|Ankommande flöde|Artiklar som transporteras in till distributionslagerplatsen, till exempel inköp och ankommande överföringar.|  
|Internt flöde|Artiklar som transporteras inom distributionslagerplatsen, till exempel produktionskomponenter och utflöde.|  
|Avgående flöde|Artiklar som transporteras ut ur distributionslagerplatsen, till exempel försäljningar och avgående överföringar.|  

## <a name="see-also"></a>Se även  
 [Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)

