---
title: Hantera profiler och rollcenter
description: "Mer information om hur du hanterar användare och rollcenter i Dynamics NAV."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, roles, role centers, user roles
ms.date: 09/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: a657c409c9cd361a505f1fd61dbb5254b25c5144
ms.contentlocale: sv-se
ms.lasthandoff: 10/26/2017

---
# <a name="managing-profiles-and-role-centers"></a><span data-ttu-id="12215-103">Hantera profiler och rollcenter</span><span class="sxs-lookup"><span data-stu-id="12215-103">Managing Profiles and Role Centers</span></span>
<span data-ttu-id="12215-104">Profiler är samlingar av [!INCLUDE[navnow_md](includes/navnow_md.md)]-användare som delar samma Rollcenter.</span><span class="sxs-lookup"><span data-stu-id="12215-104">Profiles are collections of [!INCLUDE[navnow_md](includes/navnow_md.md)] users who share the same Role Center.</span></span> <span data-ttu-id="12215-105">Ett Rollcenter är en typ av sidan som du kan tillämpa på olika delar.</span><span class="sxs-lookup"><span data-stu-id="12215-105">A Role Center is a type of page on which you can place different parts.</span></span> <span data-ttu-id="12215-106">Varje del är en behållare, i vilken du kan hosta andra sidor eller fördefinierade systemdelar, som till exempel en Outlook-del eller delar för att lägga till uppgifter, meddelanden eller noteringar.</span><span class="sxs-lookup"><span data-stu-id="12215-106">Each part is a container in which you can host other pages or pre-defined system parts, such as an Outlook part or parts for adding tasks, notifications, or notes.</span></span>  

## <a name="about-profiles-and-role-centers"></a><span data-ttu-id="12215-107">Om användare och rollcenter</span><span class="sxs-lookup"><span data-stu-id="12215-107">About profiles and Role Centers</span></span>
<span data-ttu-id="12215-108">Med profiler kan du länka användare till fördefinierade rollcenter.</span><span class="sxs-lookup"><span data-stu-id="12215-108">You use profiles to link users to pre-defined Role Centers.</span></span> <span data-ttu-id="12215-109">Ett rollcenter är en hemsida för alla användare av en profil som har konfigurerats för att reflektera uppgifterna och prioriteringarna för användarna av profilen.</span><span class="sxs-lookup"><span data-stu-id="12215-109">A Role Center is a home page for all users of a profile, which has been configured to reflect the tasks and priorities of users of the profile.</span></span> <span data-ttu-id="12215-110">Till exempel har Rollcentret orderhandläggaren konfigurerats så att de motsvarar uppgifterna och prioriteringarna i en orderhandläggare.</span><span class="sxs-lookup"><span data-stu-id="12215-110">For example, the Order Processor Role Center has been configured to reflect the tasks and priorities of an order processor.</span></span> <span data-ttu-id="12215-111">Ett rollcenter ger enkel åtkomst till information som måste utföras i deras dagliga arbete.</span><span class="sxs-lookup"><span data-stu-id="12215-111">A Role Center provides easy access to information users need to perform their daily work.</span></span> <span data-ttu-id="12215-112">Exempelvis bestämmer rollcentret de stack-ikoner, eller paneler som visar när användare loggar in och länkarna på navigeringssidan.</span><span class="sxs-lookup"><span data-stu-id="12215-112">For example, the Role Center determines the Cues, or tile, that show when isers first sign in, and the links from the navigation page.</span></span>

<span data-ttu-id="12215-113">Profilen som används visas i huvudet på rollcentrets huvudsakliga innehållsområde.</span><span class="sxs-lookup"><span data-stu-id="12215-113">The profile that is used appears in the header of the Role Center’s main content area.</span></span> <span data-ttu-id="12215-114">En administratör kan sedan anpassa det här Rollcentret för att uppfylla behoven för en viss roll i ett visst företag.</span><span class="sxs-lookup"><span data-stu-id="12215-114">An administrator can customize this Role Center to meet the needs of a specific role in a specific company.</span></span> <span data-ttu-id="12215-115">Rollcentret Orderhandläggaren kan sedan vidare anpassas på en enskild dator för att uppfylla behov för en person som utför projekt som en orderhandläggare.</span><span class="sxs-lookup"><span data-stu-id="12215-115">The Order Processor Role Center can then be further personalized on a single computer to meet the needs of a person who is carrying out the job as an order processor.</span></span> <span data-ttu-id="12215-116">Den här person kan anpassa Rollcenter genom att spara frågor, lägga till filter, och lägga till eller ta bort fält.</span><span class="sxs-lookup"><span data-stu-id="12215-116">This person can personalize the Role Center by saving queries, adding filters, and adding or removing fields.</span></span>

<span data-ttu-id="12215-117">Profiler och rollcenter passar med de roller och ansvarsområden som finns i organisationen.</span><span class="sxs-lookup"><span data-stu-id="12215-117">Profiles and Role Centers align with the roles and responsibilities in your organization.</span></span> [!INCLUDE[navnow_md](includes/navnow_md.md)]<span data-ttu-id="12215-118"> innehåller en uppsättning standardprofiler, där var och en motsvarar och länkar till ett rollcenter.</span><span class="sxs-lookup"><span data-stu-id="12215-118"> provides a set of default profiles, which each correspond to and link to a Role Center.</span></span> <span data-ttu-id="12215-119">Administratörer kan ändra befintliga profiler eller skapa nya.</span><span class="sxs-lookup"><span data-stu-id="12215-119">Administrators can modify existing profiles or create new ones.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="12215-120">Profiler länkas inte uttryckligen till de roller och behörigheter som utgör säkerhetssystemet, men profilanvändare måste ha behörighet som passar deras roller i säkerhetssystemet.</span><span class="sxs-lookup"><span data-stu-id="12215-120">Profiles are not explicitly linked to the roles and permissions that constitute the security system, but profile users must have permissions that align with their roles in the security system.</span></span> <span data-ttu-id="12215-121">Mer information finns i [Säkerhet i rollanpassad miljö](http://go.microsoft.com/fwlink?LinkId=147633) i MSDN-biblioteket.</span><span class="sxs-lookup"><span data-stu-id="12215-121">For more information, see [Security in the Role Tailored Environment](http://go.microsoft.com/fwlink?LinkId=147633) in the MSDN Library.</span></span>

## <a name="to-create-a-profile"></a><span data-ttu-id="12215-122">Så här skapar du en profil:</span><span class="sxs-lookup"><span data-stu-id="12215-122">To create a profile</span></span>
1.  <span data-ttu-id="12215-123">Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Profiler** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="12215-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="12215-124">Välj åtgärden **Ny** för att öppna fönstret **Nytt profilkort**.</span><span class="sxs-lookup"><span data-stu-id="12215-124">Choose the **New** action to open the **New Profile Card** window.</span></span>  

3.  <span data-ttu-id="12215-125">I **Profil-ID** fältet, ange ett namn som beskriver den påtänkta rollen för användaren.</span><span class="sxs-lookup"><span data-stu-id="12215-125">In the **Profile ID** field, enter a name that describes the intended role of the user.</span></span>  

4.  <span data-ttu-id="12215-126">I fältet **Beskrivning** anger du en beskrivning av profil-ID:t, t.ex. **Orderhandläggare**.</span><span class="sxs-lookup"><span data-stu-id="12215-126">In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.</span></span>  

5.  <span data-ttu-id="12215-127">Ange fältet **Rollcenter-ID** till det rollcentret som du vill tilldela profilen.</span><span class="sxs-lookup"><span data-stu-id="12215-127">Set the **Role Center ID** field to the Role Center that you want to assign to the profile.</span></span>  

6.  <span data-ttu-id="12215-128">Markera kryssrutan **Standardrollcenter** om du vill att detta rollcenter ska vara standard för profilen.</span><span class="sxs-lookup"><span data-stu-id="12215-128">To make this Role Center the default for the profile, select the **Default Role Center** check box.</span></span>  

7.  <span data-ttu-id="12215-129">Välj knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="12215-129">Choose the **OK** button.</span></span> <span data-ttu-id="12215-130">.</span><span class="sxs-lookup"><span data-stu-id="12215-130">.</span></span>  

<span data-ttu-id="12215-131">Proceduren som används för att ändra en befintlig profil är samma, förutom att du väljer en befintlig profil i profil sidan, i stället för att välja åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="12215-131">The procedure for modifying an existing profile is the same, except you select an existing profile in the Profiles page instead of choosing the **New** action.</span></span>  


##<a name="copying-a-profile"></a><span data-ttu-id="12215-132">Kopiera en profil</span><span class="sxs-lookup"><span data-stu-id="12215-132">Copying a profile</span></span>
<span data-ttu-id="12215-133">Kopiera en profil kan spara tid, om du vill använda liknande inställningar på en profil, och du endast vill ändra några få inställningar.</span><span class="sxs-lookup"><span data-stu-id="12215-133">Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.</span></span>

1.  <span data-ttu-id="12215-134">Öppna den profil som du vill kopiera och välj sedan åtgärden **Kopiera profil**.</span><span class="sxs-lookup"><span data-stu-id="12215-134">Open the profile that you want to copy, and then choose the **Copy Profile** action.</span></span>

2.  <span data-ttu-id="12215-135">Skriv namnet på profilen som du vill kopiera i fältet **Nytt profil-ID**.</span><span class="sxs-lookup"><span data-stu-id="12215-135">In **New Profile ID** field, enter a name for the profile that you want to copy.</span></span>

3.  <span data-ttu-id="12215-136">Ange fältet **Ny profilomfattning** till något av följande:</span><span class="sxs-lookup"><span data-stu-id="12215-136">Set the **New Profile Scope** field to one of the following:</span></span>

    - <span data-ttu-id="12215-137">**Systemet** så att den nya profilen är tillgänglig för alla innehavare av databaser som använder programmet.</span><span class="sxs-lookup"><span data-stu-id="12215-137">**System** to make the new profile available to all tenant databases that use the application.</span></span>
    - <span data-ttu-id="12215-138">**Klientorganisation** så att den nya profilen är tillgänglig bara för den aktuella klientorganisationens databas.</span><span class="sxs-lookup"><span data-stu-id="12215-138">**Tenant** to make the new profile available to just the current tenant database.</span></span>
4. <span data-ttu-id="12215-139">Välj knappen **OK** när du är klar.</span><span class="sxs-lookup"><span data-stu-id="12215-139">Choose the **OK** buttom when done.</span></span>

## <span data-ttu-id="12215-140"><a name="ExportImportProfile"></a>Exportera och importera profiler</span><span class="sxs-lookup"><span data-stu-id="12215-140"><a name="ExportImportProfile"></a>Exporting and importing profiles</span></span>

<span data-ttu-id="12215-141">Du kan exportera och importera profiler som XML-filer till och från en [!INCLUDE[d365fin](includes/d365fin_md.md)]-databas.</span><span class="sxs-lookup"><span data-stu-id="12215-141">You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database.</span></span> <span data-ttu-id="12215-142">Exportera och importera en profil låter dig spara tid när du konfigurerar användargränssnittet eftersom du kan återanvända en befintlig profilkonfiguration i stället för att konfigurera en profil från början.</span><span class="sxs-lookup"><span data-stu-id="12215-142">Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch.</span></span> <span data-ttu-id="12215-143">Om du har en profil som är konfigurerad i en [!INCLUDE[d365fin](includes/d365fin_md.md)]-databas och du vill återanvända hela eller delar av samma profilkonfigurationer i en annan databas, kan du exportera profiler till en XML-fil.</span><span class="sxs-lookup"><span data-stu-id="12215-143">If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file.</span></span> <span data-ttu-id="12215-144">Du kan sedan importera XML-filen för profilen i den andra databasen.</span><span class="sxs-lookup"><span data-stu-id="12215-144">Then, you can import the profile XML file into the other database.</span></span>

-   <span data-ttu-id="12215-145">Om du vill exportera en profil, öppnar du sidan **Exportera profiler**, väljer profilen i listan, och väljer sedan åtgärden **exportera**.</span><span class="sxs-lookup"><span data-stu-id="12215-145">To export a profile, open search for and open the **Export Profiles** page, select the profile from the list, and then choose the **Export** action.</span></span> <span data-ttu-id="12215-146">Spara XML-filen till en plats på datorn eller i nätverket.</span><span class="sxs-lookup"><span data-stu-id="12215-146">Save the XML file to a location on your computer or network.</span></span>

-   <span data-ttu-id="12215-147">Om du vill importera en profil, öppnar du sidan **Importera profiler**, väljer profilens XML-fil och väljer sedan knappen **OK**.</span><span class="sxs-lookup"><span data-stu-id="12215-147">To import a profile, open search for and open the **Import Profiles** page, select the profile XML file, and then choose the **OK** button.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="12215-148">Du kan inte importera en profil som redan finns i databasen, även om XML-filen har ett annat namn eller annat innehåll.</span><span class="sxs-lookup"><span data-stu-id="12215-148">You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content.</span></span> <span data-ttu-id="12215-149">Du måste ta bort den befintliga profilen innan du kan importera den nya profilen.</span><span class="sxs-lookup"><span data-stu-id="12215-149">You must delete the existing profile before you can import the new profile.</span></span>



## <a name="see-also"></a><span data-ttu-id="12215-150">Se även</span><span class="sxs-lookup"><span data-stu-id="12215-150">See Also</span></span>  
[<span data-ttu-id="12215-151">Så här hanterar du användare och behörigheter</span><span class="sxs-lookup"><span data-stu-id="12215-151">How to: Manage Users and Permissions</span></span>](ui-how-users-permissions.md)  
[<span data-ttu-id="12215-152">Anpassa användargränssnittet</span><span class="sxs-lookup"><span data-stu-id="12215-152">Customizing the User Interface</span></span>](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

