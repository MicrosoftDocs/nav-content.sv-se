---
title: Administrativa uppgifter i Dynamics NAV
description: "Vissa uppgifter i [!INCLUDE[d365fin](includes/d365fin_md.md)] kräver central administration och inställningar. Se vad de är och lär dig vad du ska göra."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 3ddb647d28a4065be248a265316b38e8d37d28c2
ms.contentlocale: sv-se
ms.lasthandoff: 12/01/2017

---
# <a name="setup-and-administration-in-dynamics-nav"></a><span data-ttu-id="721e4-104">Installation och administration i Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="721e4-104">Setup and Administration in Dynamics NAV</span></span>
<span data-ttu-id="721e4-105">Central administration utförs vanligtvis av en roll i företaget.</span><span class="sxs-lookup"><span data-stu-id="721e4-105">Central administration tasks are usually performed by one role in the company.</span></span> <span data-ttu-id="721e4-106">Omfattningen av dessa uppgifter kan vara beroende av företagets storlek och administratörens ansvarsområden.</span><span class="sxs-lookup"><span data-stu-id="721e4-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span></span> <span data-ttu-id="721e4-107">Dessa uppgifter kan omfatta att hantera databassynkronisering av projekt och e-postköer, konfigurera användare, anpassa användargränssnittet och hantera krypteringsnycklar.</span><span class="sxs-lookup"><span data-stu-id="721e4-107">These tasks can include managing database synchronization of job and email queues, setting up users, customizing the user interface, and managing encryption keys.</span></span>  

<span data-ttu-id="721e4-108">Det är viktigt att ange rätt inställningsvärden från början för att en ny verksamhetsprogramvara ska fungera effektivt.</span><span class="sxs-lookup"><span data-stu-id="721e4-108">Entering the correct setup values from the start is important to the success of any new business software.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="721e4-109"> innehåller ett antal assisterade installationer som hjälper dig att ställa in grundläggande information.</span><span class="sxs-lookup"><span data-stu-id="721e4-109"> includes a number of setup guides that help you set up core data.</span></span> <span data-ttu-id="721e4-110">Mer information finns i [Skapa Dynamics NAV](setup.md).</span><span class="sxs-lookup"><span data-stu-id="721e4-110">For more information, see [Setting Up Dynamics NAV](setup.md).</span></span>

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

<span data-ttu-id="721e4-111">En superanvändare eller administratör kan konfigurera ramverket för datautbyte så att användare kan exportera och importera data i bank- och lönesystemfiler, till exempel för olika processer av likviditetsstyrning.</span><span class="sxs-lookup"><span data-stu-id="721e4-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span></span>  

<span data-ttu-id="721e4-112">I följande tabell beskrivs en serie uppgifter, med länkar till de avsnitt där de beskrivs.</span><span class="sxs-lookup"><span data-stu-id="721e4-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="721e4-113">**Om du vill**</span><span class="sxs-lookup"><span data-stu-id="721e4-113">**To**</span></span>|<span data-ttu-id="721e4-114">**Gå till**</span><span class="sxs-lookup"><span data-stu-id="721e4-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="721e4-115">Lägg till användargrupper och hantera behörigheter, åtkomst till data, tilldela roller.</span><span class="sxs-lookup"><span data-stu-id="721e4-115">Add users, manage permissions and access to data, assign roles.</span></span>|[<span data-ttu-id="721e4-116">Användare, profiler och rollcenter i Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="721e4-116">Users, Profiles, and Role Centers in Dynamics NAV</span></span>](admin-users-profiles-roles.md)|  
|<span data-ttu-id="721e4-117">Spåra alla direkta ändringar som användarna gör av data i databasen för att kunna identifiera var fel och dataändringar härrör från.</span><span class="sxs-lookup"><span data-stu-id="721e4-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span></span>|[<span data-ttu-id="721e4-118">Logga ändringar i Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="721e4-118">Logging Changes in Dynamics NAV</span></span>](across-log-changes.md)|  
|<span data-ttu-id="721e4-119">Stöd inställningsalternativ med rekommendationer för valda fält som eventuellt orsakar att lösningen är ineffektiv, om fältet felaktigt inställt</span><span class="sxs-lookup"><span data-stu-id="721e4-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span></span>|[<span data-ttu-id="721e4-120">Skapa komplexa moduler med hjälp av bästa metoder</span><span class="sxs-lookup"><span data-stu-id="721e4-120">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)|  
|<span data-ttu-id="721e4-121">Visa sidor, kodenheter och frågor som webbtjänster.</span><span class="sxs-lookup"><span data-stu-id="721e4-121">Expose pages, codeunits, and queries as web services.</span></span>|[<span data-ttu-id="721e4-122">Så här: Publicerar du en webbtjänst</span><span class="sxs-lookup"><span data-stu-id="721e4-122">How to: Publish a Web Service</span></span>](across-how-publish-web-service.md)|  
|<span data-ttu-id="721e4-123">Skapa en SMTP-server för att aktivera e-postkommunikation i och utanför Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="721e4-123">Set up an SMTP server to enable e-mail communication in and out of Dynamics NAV</span></span>| [<span data-ttu-id="721e4-124">Så här: Konfigurera e-post manuellt eller med hjälp av Assisterad konfiguration</span><span class="sxs-lookup"><span data-stu-id="721e4-124">How to: Set Up Email Manually or Using the Assisted Setup</span></span>](madeira-how-setup-email.md)|  
|<span data-ttu-id="721e4-125">Ange enstaka eller återkommande begäranden om att köra rapporter eller kodenheter.</span><span class="sxs-lookup"><span data-stu-id="721e4-125">Enter single or recurring requests to run reports or codeunits.</span></span>|[<span data-ttu-id="721e4-126">Använd jobbköer för att schemalägga uppgifter</span><span class="sxs-lookup"><span data-stu-id="721e4-126">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)|  
|<span data-ttu-id="721e4-127">Hantera, ta bort eller komprimera dokument</span><span class="sxs-lookup"><span data-stu-id="721e4-127">Manage, delete, or compress documents</span></span>|[<span data-ttu-id="721e4-128">Hantera dokument</span><span class="sxs-lookup"><span data-stu-id="721e4-128">Manage Documents</span></span>](admin-manage-documents.md)|  

## <a name="see-also"></a><span data-ttu-id="721e4-129">Se även</span><span class="sxs-lookup"><span data-stu-id="721e4-129">See Also</span></span>
[<span data-ttu-id="721e4-130">Översikt över affärsfunktioner</span><span class="sxs-lookup"><span data-stu-id="721e4-130">Overview of Business Functionality</span></span>](madeira-business-functionality.md)  
[<span data-ttu-id="721e4-131">Allmänna affärsfunktioner</span><span class="sxs-lookup"><span data-stu-id="721e4-131">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="721e4-132">[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="721e4-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="721e4-133">[Välkommen till [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="721e4-133">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

