---
title: "Översikt över dimensionsuppsättningstransaktioner"
description: "Det här avsnittet beskriver hur dimensionsuppsättningstransaktioner lagras och bokförs i [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dimension
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ce9459785ee39fa89baf61b2e97be41ddde661f6
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="dimension-set-entries-overview"></a><span data-ttu-id="c6d12-103">Översikt över dimensionsuppsättningstransaktioner</span><span class="sxs-lookup"><span data-stu-id="c6d12-103">Dimension Set Entries Overview</span></span>
<span data-ttu-id="c6d12-104">I det här avsnittet beskrivs hur dimensionsuppsättningstransaktioner lagras och bokförs i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="c6d12-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
  
## <a name="dimension-sets"></a><span data-ttu-id="c6d12-105">Dimensionsuppsättningar</span><span class="sxs-lookup"><span data-stu-id="c6d12-105">Dimension Sets</span></span>  
<span data-ttu-id="c6d12-106">En dimensionsuppsättning en är en unik kombination av dimensionsvärden.</span><span class="sxs-lookup"><span data-stu-id="c6d12-106">A dimension set is a unique combination of dimension values.</span></span> <span data-ttu-id="c6d12-107">Den lagras som dimensionsuppsättningstransaktioner i databasen.</span><span class="sxs-lookup"><span data-stu-id="c6d12-107">It is stored as dimension set entries in the database.</span></span> <span data-ttu-id="c6d12-108">Varje dimensionsuppsättningstransaktion representerar ett enstaka dimensionsvärde.</span><span class="sxs-lookup"><span data-stu-id="c6d12-108">Each dimension set entry represents a single dimension value.</span></span> <span data-ttu-id="c6d12-109">Dimensionsuppsättningen identifieras av ett gemensamt dimensionsuppsättnings-ID som tilldelats varje dimensionsuppsättningstransaktion som tillhör dimensionsuppsättningen.</span><span class="sxs-lookup"><span data-stu-id="c6d12-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span></span>  
  
<span data-ttu-id="c6d12-110">Följande exempel visar när en dimensionsuppsättning som har tre dimensionsuppsättningstransaktioner.</span><span class="sxs-lookup"><span data-stu-id="c6d12-110">The following example shows a dimension set that has three dimension set entries.</span></span> <span data-ttu-id="c6d12-111">Dimensionsuppsättningen identifieras av ett dimensionsuppsättnings-ID som är 108.</span><span class="sxs-lookup"><span data-stu-id="c6d12-111">The dimension set is identified by a dimension set ID, which is 108.</span></span>  
  
|<span data-ttu-id="c6d12-112">Dimensionsuppsättnings-ID</span><span class="sxs-lookup"><span data-stu-id="c6d12-112">Dimension Set ID</span></span>|<span data-ttu-id="c6d12-113">Dimensionskod</span><span class="sxs-lookup"><span data-stu-id="c6d12-113">Dimension Code</span></span>|<span data-ttu-id="c6d12-114">Dimensionsvärdekod</span><span class="sxs-lookup"><span data-stu-id="c6d12-114">Dimension Value Code</span></span>|<span data-ttu-id="c6d12-115">Dimensionsvärdesnamn</span><span class="sxs-lookup"><span data-stu-id="c6d12-115">Dimension Value Name</span></span>|  
|----------------------|--------------------|--------------------------|--------------------------|  
|<span data-ttu-id="c6d12-116">108</span><span class="sxs-lookup"><span data-stu-id="c6d12-116">108</span></span>|<span data-ttu-id="c6d12-117">OMRÅDE</span><span class="sxs-lookup"><span data-stu-id="c6d12-117">AREA</span></span>|<span data-ttu-id="c6d12-118">70</span><span class="sxs-lookup"><span data-stu-id="c6d12-118">70</span></span>|<span data-ttu-id="c6d12-119">Nordamerika</span><span class="sxs-lookup"><span data-stu-id="c6d12-119">America North</span></span>|  
|<span data-ttu-id="c6d12-120">108</span><span class="sxs-lookup"><span data-stu-id="c6d12-120">108</span></span>|<span data-ttu-id="c6d12-121">RÖRELSEMALL</span><span class="sxs-lookup"><span data-stu-id="c6d12-121">BUSINESSGROUP</span></span>|<span data-ttu-id="c6d12-122">Home</span><span class="sxs-lookup"><span data-stu-id="c6d12-122">HOME</span></span>|<span data-ttu-id="c6d12-123">Start</span><span class="sxs-lookup"><span data-stu-id="c6d12-123">Home</span></span>|  
|<span data-ttu-id="c6d12-124">108</span><span class="sxs-lookup"><span data-stu-id="c6d12-124">108</span></span>|<span data-ttu-id="c6d12-125">AVDELNING</span><span class="sxs-lookup"><span data-stu-id="c6d12-125">DEPARTMENT</span></span>|<span data-ttu-id="c6d12-126">FÖRSÄLJNING</span><span class="sxs-lookup"><span data-stu-id="c6d12-126">SALES</span></span>|<span data-ttu-id="c6d12-127">FÖRS</span><span class="sxs-lookup"><span data-stu-id="c6d12-127">Sales</span></span>|  
  
## <a name="dimension-set-entries"></a><span data-ttu-id="c6d12-128">Dimensionsuppsättningstrans.</span><span class="sxs-lookup"><span data-stu-id="c6d12-128">Dimension Set Entries</span></span>  
<span data-ttu-id="c6d12-129">Dimensionsuppsättningar lagras i tabellen **Dimensionsuppsättnings transaktion** som dimensionsuppsättningstransaktioner med samma dimensionsuppsättnings-ID.</span><span class="sxs-lookup"><span data-stu-id="c6d12-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span></span>  
  
<span data-ttu-id="c6d12-130">![Dimension – översikt](media/dimensionentrynav7.png "DimensionEntryNAV7")</span><span class="sxs-lookup"><span data-stu-id="c6d12-130">![Dimension Entry overview](media/dimensionentrynav7.png "DimensionEntryNAV7")</span></span>  
  
<span data-ttu-id="c6d12-131">När du skapar en ny journalrad, dokumenthuvud eller dokumentrad kan du ange en kombination av dimensionsvärden.</span><span class="sxs-lookup"><span data-stu-id="c6d12-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span></span> <span data-ttu-id="c6d12-132">I stället för att uttryckligen lagra varje dimensionsvärde i databasen tilldelas ett dimensionsuppsättnings-ID till journalraden, dokumenthuvudet eller dokumentraden för att specificera dimensionsuppsättningen.</span><span class="sxs-lookup"><span data-stu-id="c6d12-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span></span>  
  
<span data-ttu-id="c6d12-133">När du redigerar och stänger fönstret **Redigera dimensionsuppsättningstrans.**utförs en kontroll för att se om kombinationen av dimensionsvärden finns som en dimensionsuppsättning i tabellen.</span><span class="sxs-lookup"><span data-stu-id="c6d12-133">When you edit and close the **Edit Dimension Set Entries** window, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span></span> <span data-ttu-id="c6d12-134">Om kombinationen finns i tabellen tilldelas motsvarande dimensionsuppsättnings-ID till journalraden, dokumenthuvudet eller dokumentraden.</span><span class="sxs-lookup"><span data-stu-id="c6d12-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span></span> <span data-ttu-id="c6d12-135">Annars läggs en ny dimensionsuppsättning till tabellen och det nya dimensionsuppsättnings-ID:t tilldelats journalraden, dokumenthuvudet eller dokumentraden.</span><span class="sxs-lookup"><span data-stu-id="c6d12-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span></span>  
  
## <a name="performance-improvement"></a><span data-ttu-id="c6d12-136">Prestandaförbättring</span><span class="sxs-lookup"><span data-stu-id="c6d12-136">Performance Improvement</span></span>  
<span data-ttu-id="c6d12-137">Genom att lagra dimensionsuppsättningar en gång i databasen bevaras databasplats och allmänna prestanda förbättras.</span><span class="sxs-lookup"><span data-stu-id="c6d12-137">By storing dimension sets once in the database, database space is preserved, and overall performance is improved.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="c6d12-138">Se även</span><span class="sxs-lookup"><span data-stu-id="c6d12-138">See Also</span></span>  
<span data-ttu-id="c6d12-139">[Designdetaljer: Söka efter dimensionskombinationer](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="c6d12-139">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
<span data-ttu-id="c6d12-140">[Designdetaljer: Tabellstruktur](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="c6d12-140">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
<span data-ttu-id="c6d12-141">[Designdetaljer: Kodenhet 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span><span class="sxs-lookup"><span data-stu-id="c6d12-141">[Design Details: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span></span>  
<span data-ttu-id="c6d12-142">[Designdetaljer: Kodexempel på ändrade mönster i ändringar](design-details-code-examples-of-changed-patterns-in-modifications.md) </span><span class="sxs-lookup"><span data-stu-id="c6d12-142">[Design Details: Code Examples of Changed Patterns in Modifications](design-details-code-examples-of-changed-patterns-in-modifications.md) </span></span>  
[<span data-ttu-id="c6d12-143">Designdetaljer: Dimensionsuppsättningstransaktioner</span><span class="sxs-lookup"><span data-stu-id="c6d12-143">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)   

