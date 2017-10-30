---
title: "Hantera anpassning som administratör"
description: "Lär dig mer om att anpassa användargränssnittet så att det passar ditt sätt att arbeta."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e3d088c35efca4d62b7db1f0d44d5ef2958317d4
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="managing-personalization-as-an-administrator"></a>Hantera anpassning som administratör
Användare kan anpassa sin arbetsyta efter eget behov. Som administratör kan du styra och hantera anpassning genom att inaktivera användare för att anpassa egna sidor och ta bort alla anpassningar på sidan som användare har gjort.

## <a name="disable-personalization-for-a-profile"></a>Inaktivera anpassningar för en profil
Du kan förhindra alla användare som tillhör en viss profil från att anpassa sidorna.
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Profiler** och välj sedan relaterad länk.
2.  Välj den profil i listan som du vill ändra.
3.  Välj kryssrutan **Inaktivera anpassning** och välj sedan knappen **OK**.

## <a name="clear-user-personalizations"></a>Rensa användaranpassning

Ta bort sidann för anpassningsändringar gör att sidan återställs till sin ursprungliga layout innan alla anpassningar gjordes. Det finns två sätt att ta bort de anpassningar som användare har gjort på sidor: med hjälp av sidan **Ta bort användaranpassning** och använda sidan **Anv.anpassningskort**.

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>Ta bort användaranpassningar genom att använda sidan ta bort användaranpassning

Sidan **ta bort användaranpassning** låter dig ta bort anpassningen på en per sida, per användare-basis.

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Ta bort användaranpassning** och välj sedan relaterad länk.

    Sidan visar en lista över alla sidor som har anpassats och användaren den tillhör.

    >[!NOTE]
    > En kryssmarkering i kolumnen **Äldre anpassning** anger att anpassningen har gjorts strikt med hjälp av [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] och/eller den har gjorts i [!INCLUDE[nav_web_md](includes/nav_web_md.md)] före [!INCLUDE[navnow_md](includes/navnow_md.md)]. Användare som försöker anpassa sidorna med hjälp av [!INCLUDE[nav_web_md](includes/nav_web_md.md)] är låsta från att göra detta såvida de inte väljer att låsa upp en sida. Mer information finns i [anledningen till att en sida är låst för att anpassa](ui-personalization-locked.md). Mer information om anpassningen mellan [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)]och [!INCLUDE[nav_web_md](includes/nav_web_md.md)], finns i [arbeta med anpassningen mellan Dynamics NAV Windows- och webbklienten](ui-personalization-overview.md#PersonalizationWinWeb).

2. Markera den transaktion som du vill radera och välj sedan åtgärden **Radera**.

    Användaren kommer att se ändringarna nästa gång de loggar in.

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a>Ta bort användaranpassningar genom att använda sidan användaranpassningskort

Sidan **Anv.anpassningskort** låter dig ta bort anpassningen på alla sidor för en specifik användare. Detta kräver skrivbehörighet för tabellen 2000000072 **Profil**.

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Ta bort användaranpassning** och välj sedan relaterad länk.

    Sidan **användaranpassning** visar alla användare som eventuellt har anpassade sidor. Om du inte hittar en användare i listan, innebär det att de inte har några anpassade sidor.

2. Välj den användare från listan, välj åtgärden **Redigera**.

3.  På fliken **Åtgärder**, välj **Ta bort anpassade sidor**.

    Användaren kommer att se ändringarna nästa gång de loggar in.

## <a name="see-also"></a>Se även
[Anpassning, översikt](ui-personalization-overview.md)  
[Anpassa din arbetsyta](ui-personalization-user.md)  
[Arbeta med [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Så här ändrar du rollcentret](change-role.md)  
