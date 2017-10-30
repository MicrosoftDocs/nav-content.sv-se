---
title: "Konfigurera användargränssnitt (UI) för användare"
description: "Som administratör konfigurerar du företagets standardanvändargränssnitt genom att anpassa sidlayouter för olika användarprofiler i företaget."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize pages, configure user interface, customize UI
ms.date: 07/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ba3d45a856eb38fe99fc5012b4e2f2d8609f9ce
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="configuring-the-user-interface-ui-for-users"></a>Konfigurera användargränssnitt (UI) för användare
Som administratör konfigurerar du företagets standardanvändargränssnitt genom att anpassa sidlayouter för olika användarprofiler i företaget. När du utför det här arbetet måste du vara administratör med behörigheten SUPER. Dessutom måste profiler ställas in och de lämpliga användarna tilldelas till dem. Mer information finns i [hantera användarprofiler och rollcenter](admin-users-profiles-roles.md).  
  
Du konfigurera användargränssnittet för flera användare genom att anpassa sidor för en viss profil som användarna har kopplats till. Du gör detta med hjälp av [!INCLUDE[nav_windows](includes/nav_windows_md.md)] och anpassar på samma sätt som enskilda användare anpassar egna arbetsytor, det vill säga med hjälp av funktionen **anpassa**. Skillnaden är att du öppnar [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurationsläget. Typiska anpassningar är vilka åtgärder som ska tas med på menyfliken, hur fält placeras på snabbflikarna eller i faktaboxar och vilka menyobjekt som ska ingå i navigeringsrutan. 

> [!TIP]  
>  Ett snabbt sätt att implementera gränssnittkonfigurationer för en profil är om du redan har en konfigurerad profil med en annan [!INCLUDE[d365fin](includes/d365fin_md.md)]-databas. Du kan sedan exportera den profilen och sedan importera den till den aktuella databasen. Mer information finns i [Exportera och importera profiler](admin-profiles.md#ExportImportProfile).  
  
## <a name="general-information"></a>Allmän information
Tänk på följande information innan du börjar konfigurera användargränssnittet:
-   Innan du kan börja att konfigurera användargränssnittet, kan programmet konfigureras att visa och dölja element i användargränssnittet (till exempel fälten Snabbflikar och Faktaboxar) baserat på din licens eller behörigheter. Mer information finns i [Ta bort element i användargränssnittet enligt behörigheter](https://msdn.microsoft.com/en-us/dynamics-nav/removing-elements-from-the-user-interface-according-to-permissions).

    Om du vill visa effekten av den alternativet Borttagning av gränssnittselement kan du logga in som provanvändare med behörighetsuppsättningen för den profil som du konfigurerar. Anledningen är att du som administratör har SUPER-behörighet angiven och du kan därför inte visa och testa det resulterande användargränssnittet under din egen inloggning.    
-   När du skapar ändringar för användargränssnittskonfigurationen för en sida som en användare har specialanpassat, bevaras användarens användargränssnittsanpassning och skrivs inte över av den nya sidkonfigurationen. På samma sätt, när du annullerar din användargränssnittskonfiguration av en sida som en användare därefter har specialanpassat annulleras inte användarens användargränssnittsanpassning.
-   Det enda läget där användargränssnittskonfigurationen skriver över användargränssnittsanpassning är när ett element i användargränssnittet tas bort av konfigurationen. Till exempel om administratören tar bort ett fält som användaren har bytt namn på eller har flyttat, kommer fältet fortfarande att tas bort från användarens användargränssnitt.
-   Du kan registrera användargränssnittskonfigurationer på samma sida baserat på olika åtkomstpunkter till sidan. Till exempel kan fönstret **Försäljningsorder** anpassas för att se olika ut när det öppnas från fönstret **Kundkort** än när det öppnas från Rollcenter **Försäljningsorderhandläggare**. Den punkt varifrån du öppnar sidan som ska anpassas registreras i den specifika sidanpassningen. Det kan alltså uppstå flera sidanpassningsposter i databasen, som du ser i fönstret **Ta bort profilkonfiguration**.  
-   Till skillnad från när användaren ändrar storleken på fönstret eller bredden på kolumner på sin egen dator, sparas sådana grundläggande vyändringar som du gör i din konfigurationen av användargränssnittet för en profil inte till profilen och är inte tillgängliga för användare som har tilldelats till profilen. Grundläggande vyändringar är datorspecifika.   

## <a name="configure-a-profile-with-the-includenavwindowsincludesnavwindowsmdmd-in-configuration-mode"></a>Konfigurera en profil med [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurationsläge
1.  Öppna kommandotolken och skriv följande kommando för att ändra installationsmappen för [!INCLUDE[nav_windows](includes/nav_windows_md.md)]. Till exempel:  
  
    ```  
    cd C:\Program Files\(x86)\Microsoft Dynamics NAV\110\RoleTailored Client  
    ```  
  
2.  Skriv följande kommando för att starta den [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurationsläge för en viss profil:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"profileid"  
    ```  
  
     Ersätt **Profil-ID** med namnet på profilen som du vill konfigurera.  
  
     Använd följande kommando för att till exempel konfigurera profilen Redovisningschef:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"Accounting Manager"  
    ``` 

3. Du är nu redo att börja konfigurera användargränssnittet, som du gör på samma sätt som enskilda användare anpassar egna arbetsytor. Mer information finns i [anpassa arbetsytan i [!INCLUDE[nav_windows](includes/nav_windows_md.md)]](ui-personalization-windows-client.md). 

## <a name="cancel-ui-configuration"></a>Annullera gränssnittskonfigurationen
Du kan annullera användargränssnittsanpassningar som du har gjort som konfiguration för en profil på tre sätt:  
  
-   Ångra alla gränssnittsanpassningar som du har gjort för en profil genom att använda knappen **Rensa konfigurerade sidor** i fönstret **Profilkort**.  
  
-   Annullera användargränssnittsanpassningar som du har gjort för specifika sidor för en profil genom att ta bort rader i fönstret **Ta bort profilkonfiguration**.  
  
-   Ångra anpassningar som du har skapat för ett visst användargränssnittsområde för en viss sida för en profil genom att använda knappen **Återställ standardvärden** i fönstret **Anpassa**.  
  
### <a name="general-information"></a>Allmän information  
-   Användare kan göra användargränssnittsanpassningar under sin egen användarinloggning för att anpassa sin användargränssnitt. När du annullerar din användargränssnittskonfiguration av en sida som en användare därefter har specialanpassat annulleras inte användarens användargränssnittsanpassning. På samma sätt, när du skapar den nya användargränssnittskonfigurationen för en sida som en användare har specialanpassat, bevaras användarens användargränssnittsanpassning och skrivs inte över av den nya sidkonfigurationen.  

    Det enda läget där användargränssnittskonfigurationen skriver över användargränssnittsanpassning är när ett element i användargränssnittet tas bort av konfigurationen. Till exempel om administratören tar bort ett fält som användaren har bytt namn på eller har flyttat, kommer fortfarande fältet att tas bort från användarens användargränssnitt.  
  
-   I fönstret **Ta bort användaranpassning** och med knappen **Återställ standardvärden** i **Anpassa** kan användare annullera användargränssnittsanpassningar som de har gjort på sidor under sin egen användarinloggning. När de gör det återställs layouten på de här sidorna till de användargränssnittsanpassningar som administratören har konfigurerat för profilen. Om profilen inte har konfigurerats återställs layouten på användarens sidor till standardprofilkonfigurationen. Mer information om hur användare avbryter anpassning finns i [avbryta anpassning](ui-personalization-windows-client.md#CancelPersonalization).
  
### <a name="to-cancel-all-ui-customization-that-you-have-made-for-a-profile"></a>Så här annullerar du alla användargränssnittsanpassningar som du har gjort för en profil  
  
1.  I rutan **Sök**, ange **Profiler** och välj sedan relaterad länk.  
  
2.  Välj profilen som du vill annullera alla anpassningar av användargränssnittet för, och sedan, på fliken **Hem** i gruppen **Hantera** väljer du **Redigera**.  
  
3.  I fönstret **Profilkort** på fliken **Åtgärder** i gruppen **Funktioner** väljer du **Rensa konfigurerade sidor**.  
  
> [!NOTE]  
>  Alla UI-anpassningar för profilen, både de som har installerats med programmet och de gjordes av administratören, avbryts. Inga sidlayouter som gäller för profilen förblir i databasen.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-specific-page-for-a-profile"></a>Så här annullerar du användargränssnittsanpassningar som du har gjort för en viss sida för en profil  
  
1.  I rutan **Sök**, anger du **Ta bort profilkonfiguration** och väljer sedan relaterad länk.  
  
2.  Välj profilen/siduppsättningen som du vill annullera din anpassning av användargränssnittet för, och sedan, på fliken **Hem** i gruppen **Hantera** väljer du **Ta bort**.  
  
    > [!IMPORTANT]  
    >  Om du har konfigurerat olika gränssnittsanpassningar på samma sida baserat på olika navigeringsökvägar till sidan, visas varje sidanpassning i fönstret **Ta bort profilkonfiguration** med samma information. Det finns inte någon information som kan identifiera vilken rad som är knuten till vilken navigeringsökväg. Därför måste du antingen ta bort rader en i taget följt av visuella kontroller på sidan, och också kan du ta bort alla rader med användargränssnittsanpassningar för profilen/sidan.
    >    
    >  Alla sidans användargränssnittsanpassningar för profilen som du någonsin har gjort för installationen eller sedan du senast använde fönstret **Ta bort profilkonfiguration** avbryts. Layouten på sidan till återställs till standardlayouten för sidobjektet.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-a-specific-ui-area-for-a-specific-page-for-a-profile"></a>Så här annullerar du användargränssnittsanpassningar som du har gjort för ett visst gränssnittsområde för en viss sida för en profil  
  
Du kan annullera ändringar för det som du har gjort i enskilda användargränssnittsområden, till exempel en menyflik, genom att använda knappen **Återställ standardvärden** i fönstret **Anpassa**. Du kan också ångra alla UI-ändringar som du har gjort för en profil med hjälp av fönstret **Ta bort profilkonfiguration**.  
  
Användargränssnittsanpassningen för profilen för det specifik gränssnittsområdet på den specifika sidan har annullerats. Layouten för användargränssnittsområdet på sidan återställs till standardkonfigurationen för din profil, som den skapades av administratören eller installerades med programmet.  
  
## <a name="see-also"></a>Se även  
[Anpassa[!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-customizing-overview.md)   
