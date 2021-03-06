---
title: "Så här konfigurerar du arbetsflödesanvändare"
description: "Innan du kan skapa arbetsflöden måste du ställa in de användare som ska ingå i arbetsflödena. Det behövs för att ange till exempel vem som ska ta emot en notering för att agera på ett arbetsflödessteg."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reject, delegate, request
ms.date: 08/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ed7ca6e166f7100bc19a558825e3103170fc000c
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-workflow-users"></a>Så här konfigurerar du arbetsflödesanvändare
Innan du kan skapa arbetsflöden måste du ställa in de användare som ska ingå i arbetsflödena. Det behövs för att ange till exempel vem som ska ta emot en notering för att agera på ett arbetsflödessteg.  

Konfigurera användare under arbetsflödesanvändargrupper i fönstret **Arbetsflödesanvändargrupp** och ange användarna i ordningsföljd i till exempel en godkännarkedja.  

Arbetsflödesanvändare som fungerar som godkännandeanvändare, både den som begär och den som godkänner, måste också ställas in i fönstret **Användarinställningar för godkännande**. Mer information finns i [Så här konfigurerar du godkännandeanvändare](across-how-to-set-up-approval-users.md).  

> [!NOTE]  
>  Om du vill definiera att en godkännandebegäran inte godkänns förrän flera godkännare i en godkännandekedja har godkänt den, ställer du in godkännare i en hierarki. För godkännartypen **godkännare** anger du godkännare i fönstret **Användarinställningar för godkännande**. För godkännartypen **Arbetsflödesanvändargrupp**, ställer du in godkännare i fönstret **Arbetsflödesanvändargrupper** och definierar hierarkin genom att tilldela inkrementella nummer till varje godkännare i fältet **Sekvensnr.** . Mer information finns i [Så här konfigurerar du godkännandeanvändare](across-how-to-set-up-approval-users.md) och i det här avsnittet.  
>   
>  Om du vill definiera att en godkännandebegäran inte godkänns förrän flera likvärdiga godkännare har godkänt den, oberoende av ett hierarki, ställer du in en plan arbetsflödesanvändargrupp. För godkännartypen **Arbetsflödesanvändargrupp**, ställer du in godkännare i fönstret **Arbetsflödesanvändargrupper** och definierar samma nummer till varje godkännare i fältet **Sekvensnr.** . Mer information finns i det här avsnittet.  

### <a name="to-set-up-a-workflow-user"></a>Så här konfigurerar du en arbetsflödesanvändare  

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Arbetsflödesanvändargrupper** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny**. Fönstret **Arbetsflödesanvändargrupp** öppnas.  
3. Ange högst 20 tecken för att identifiera arbetsflödet i fältet **Kod**.  
4. Beskriv arbetsflödet i fältet **Beskrivning**.  
5. Fyll i fälten på den första raden enligt beskrivningen i följande tabell på snabbfliken **Medlemmar i arbetsflödesanvändargrupp**.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Användarnamn**|Ange användaren som ska ingå i arbetsflöden.<br /><br /> Användaren måste finnas i fönstret **Användarinställningar**. Mer information finns i [Så här hanterar du användare och behörigheter](ui-how-users-permissions.md).|  
    |**Sekvensnr**|Ange den ordning som arbetsflödesanvändaren agerar i ett arbetsflöde i förhållanden till andra användare. Detta fält kan användas, till exempel, för att ange när användaren godkänner i förhållande till andra godkännare när du använder alternativet **Arbetsflödesanvändargrupp** i fältet **Godkännartyp** på det relaterade arbetsflödesvaret. **Tips!** Om du vill definiera att en godkännandebegäran inte godkänns förrän flera godkännare har godkänt den, oavsett plats i en hierarki, ställer du in en plan arbetsflödeanvändargrupp genom att tilldela samma sekvensnumret till de relevanta godkännarna.|  
6. Upprepa steg 5 för att lägga till fler arbetsflödesanvändare i användargruppen.  
7. Upprepa steg 2 till 6 för att lägga till fler arbetsflödesanvändargrupper.  

## <a name="see-also"></a>Se även  
[Så här konfigurerar du godkännandeanvändare](across-how-to-set-up-approval-users.md)   
[Konfigurera arbetsflöden](across-set-up-workflows.md)   
[Använda arbetsflöden](across-use-workflows.md)   
[Genomgång: Konfigurera och använda ett arbetsflöde för godkännande av inköp](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Arbetsflöde](across-workflow.md)   

