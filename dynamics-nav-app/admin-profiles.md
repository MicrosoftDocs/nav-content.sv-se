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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 0d99f95d7c90bae55ea139a958ca098ab10a0a7f
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="managing-profiles-and-role-centers"></a>Hantera profiler och rollcenter
Profiler är samlingar av [!INCLUDE[navnow_md](includes/navnow_md.md)]-användare som delar samma Rollcenter. Ett Rollcenter är en typ av sidan som du kan tillämpa på olika delar. Varje del är en behållare, i vilken du kan hosta andra sidor eller fördefinierade systemdelar, som till exempel en Outlook-del eller delar för att lägga till uppgifter, meddelanden eller noteringar.  

## <a name="about-profiles-and-role-centers"></a>Om användare och rollcenter
Med profiler kan du länka användare till fördefinierade rollcenter. Ett rollcenter är en hemsida för alla användare av en profil som har konfigurerats för att reflektera uppgifterna och prioriteringarna för användarna av profilen. Till exempel har Rollcentret orderhandläggaren konfigurerats så att de motsvarar uppgifterna och prioriteringarna i en orderhandläggare. Ett rollcenter ger enkel åtkomst till information som måste utföras i deras dagliga arbete. Exempelvis bestämmer rollcentret de stack-ikoner, eller paneler som visar när användare loggar in och länkarna på navigeringssidan.

Profilen som används visas i huvudet på rollcentrets huvudsakliga innehållsområde. En administratör kan sedan anpassa det här Rollcentret för att uppfylla behoven för en viss roll i ett visst företag. Rollcentret Orderhandläggaren kan sedan vidare anpassas på en enskild dator för att uppfylla behov för en person som utför projekt som en orderhandläggare. Den här person kan anpassa Rollcenter genom att spara frågor, lägga till filter, och lägga till eller ta bort fält.

Profiler och rollcenter passar med de roller och ansvarsområden som finns i organisationen. [!INCLUDE[navnow_md](includes/navnow_md.md)] innehåller en uppsättning standardprofiler, där var och en motsvarar och länkar till ett rollcenter. Administratörer kan ändra befintliga profiler eller skapa nya.  
  
> [!NOTE]  
>  Profiler länkas inte uttryckligen till de roller och behörigheter som utgör säkerhetssystemet, men profilanvändare måste ha behörighet som passar deras roller i säkerhetssystemet. Mer information finns i [Säkerhet i rollanpassad miljö](http://go.microsoft.com/fwlink?LinkId=147633) i MSDN-biblioteket. 

## <a name="to-create-a-profile"></a>Så här skapar du en profil:
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Profiler** och välj sedan relaterad länk.  
  
2.  Välj åtgärden **Ny** för att öppna fönstret **Nytt profilkort**.  
  
3.  I **Profil-ID** fältet, ange ett namn som beskriver den påtänkta rollen för användaren.  
  
4.  I fältet **Beskrivning** anger du en beskrivning av profil-ID:t, t.ex. **Orderhandläggare**.  
  
5.  Ange fältet **Rollcenter-ID** till det rollcentret som du vill tilldela profilen.  
  
6.  Markera kryssrutan **Standardrollcenter** om du vill att detta rollcenter ska vara standard för profilen.  
  
7.  Välj knappen **OK**. .  
  
Proceduren som används för att ändra en befintlig profil är samma, förutom att du väljer en befintlig profil i profil sidan, i stället för att välja **Ny**.  


##<a name="copying-a-profile"></a>Kopiera en profil 
Kopiera en profil kan spara tid, om du vill använda liknande inställningar på en profil, och du endast vill ändra några få inställningar.

1.  Öppna den profil som du vill kopiera och välj sedan åtgärden **Kopiera profil**.

2.  Skriv namnet på profilen som du vill kopiera i fältet **Nytt profil-ID**. 

3.  Ange fältet **Ny profilomfattning** till något av följande:

    - **Systemet** så att den nya profilen är tillgänglig för alla innehavare av databaser som använder programmet.
    - **Klientorganisation** så att den nya profilen är tillgänglig bara för den aktuella klientorganisationens databas. 
4. Välj knappen **OK** när du är klar.

## <a name="ExportImportProfile"></a>Exportera och importera profiler

Du kan exportera och importera profiler som XML-filer till och från en [!INCLUDE[d365fin](includes/d365fin_md.md)]-databas. Exportera och importera en profil låter dig spara tid när du konfigurerar användargränssnittet eftersom du kan återanvända en befintlig profilkonfiguration i stället för att konfigurera en profil från början. Om du har en profil som är konfigurerad i en [!INCLUDE[d365fin](includes/d365fin_md.md)]-databas och du vill återanvända hela eller delar av samma profilkonfigurationer i en annan databas, kan du exportera profiler till en XML-fil. Du kan sedan importera XML-filen för profilen i den andra databasen.

-   Om du vill exportera en profil, öppnar du sidan **Exportera profiler**, väljer profilen i listan, och väljer sedan åtgärden **exportera**. Spara XML-filen till en plats på datorn eller i nätverket. 
  
-   Om du vill importera en profil, öppnar du sidan **Importera profiler**, väljer profilens XML-fil och väljer sedan knappen **OK**. 

    > [!NOTE]  
    >  Du kan inte importera en profil som redan finns i databasen, även om XML-filen har ett annat namn eller annat innehåll. Du måste ta bort den befintliga profilen innan du kan importera den nya profilen. 



## <a name="see-also"></a>Se även  
[Så här hanterar du användare och behörigheter](ui-how-users-permissions.md)  
[Anpassa användargränssnittet](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

