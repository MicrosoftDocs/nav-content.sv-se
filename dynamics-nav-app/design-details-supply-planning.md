---
title: Designdetaljer - Leveransplanering
description: "I det här avsnittet innehåller en översikt över de begrepp och metoder som används inom leveransplaneringsfunktionerna [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, planning, reordering, replenishment
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a3a5197ba727404ce7e6dea5ee529ced6dcfa68e
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-supply-planning"></a><span data-ttu-id="41e2a-103">Designdetaljer: Leveransplanering</span><span class="sxs-lookup"><span data-stu-id="41e2a-103">Design Details: Supply Planning</span></span>
<span data-ttu-id="41e2a-104">Dokumentationen innehåller detaljerad teknisk insikt i begreppen och principerna som används i leveransplaneringen i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="41e2a-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Supply Planning features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="41e2a-105">Den förklarar hur planeringssystemet fungerar och hur du justerar algoritmerna för att uppfylla planeringskrav i olika miljöer.</span><span class="sxs-lookup"><span data-stu-id="41e2a-105">It explains how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span> <span data-ttu-id="41e2a-106">Den introducerar först centrala lösningsbegrepp och beskriver sedan logiken för den centrala mekanismen, tillgångsbalansering, innan den fortsätter att förklara hur lagerplanering utförs med partiformningsmetoder.</span><span class="sxs-lookup"><span data-stu-id="41e2a-106">It first introduces central solution concepts and then describes the logic of the central mechanism, supply balancing, before proceeding to explain how inventory planning is performed with the use of reordering policies.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="41e2a-107">I det här avsnittet</span><span class="sxs-lookup"><span data-stu-id="41e2a-107">In This Section</span></span>  
[<span data-ttu-id="41e2a-108">Designdetaljer: Centrala koncept i planeringssystemet</span><span class="sxs-lookup"><span data-stu-id="41e2a-108">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)  
[<span data-ttu-id="41e2a-109">Designdetaljer: Reservation, orderspårning och åtgärdsmeddelanden</span><span class="sxs-lookup"><span data-stu-id="41e2a-109">Design Details: Reservation, Order Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
[<span data-ttu-id="41e2a-110">Designdetaljer: Balansera efterfrågan och tillgång</span><span class="sxs-lookup"><span data-stu-id="41e2a-110">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)  
[<span data-ttu-id="41e2a-111">Designdetaljer: Hantera partiformningsmetoder</span><span class="sxs-lookup"><span data-stu-id="41e2a-111">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)  
[<span data-ttu-id="41e2a-112">Designdetaljer: Planeringsparametrar</span><span class="sxs-lookup"><span data-stu-id="41e2a-112">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)  
[<span data-ttu-id="41e2a-113">Designdetaljer: Planeringstilldelningstabell</span><span class="sxs-lookup"><span data-stu-id="41e2a-113">Design Details: Planning Assignment Table</span></span>](design-details-planning-assignment-table.md)  
[<span data-ttu-id="41e2a-114">Designdetaljer: Efterfrågan vid tomt lagerställe</span><span class="sxs-lookup"><span data-stu-id="41e2a-114">Design Details: Demand at Blank Location</span></span>](design-details-demand-at-blank-location.md)  
[<span data-ttu-id="41e2a-115">Designdetaljer: Överföringar i planering</span><span class="sxs-lookup"><span data-stu-id="41e2a-115">Design Details: Transfers in Planning</span></span>](design-details-transfers-in-planning.md)

