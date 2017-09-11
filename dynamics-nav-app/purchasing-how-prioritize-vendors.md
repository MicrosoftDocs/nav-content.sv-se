---
title: "Så här prioriterar du leverantörer"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 3b89bf07e1e9d1839b6c86a01111e936fb62c9f3
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-prioritize-vendors"></a>Så här prioriterar du leverantörer
Dynamics NAV används för att ta fram olika betalningsförslag, t.ex. betalningar som snart förfaller eller betalningar för vilka en rabatt kan erhållas. mer information finns i [Så här föreslår du leverantörsbetalningar](payables-how-suggest-vendor-payments.md).

Först måste du prioritera leverantörerna genom att tilldela nummer till dem.

## <a name="to-prioritize-vendors"></a>Så här prioriterar du leverantörer:
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Leverantörer** och välj sedan relaterad länk.
2. Välj lämplig leverantör och sedan **Redigera**.
3. Ange ett nummer i fältet **Prioritet**.

Dynamics NAV anser lägst nummer (förutom 0) motsvarar högst prioritet. Om du t.ex. använder 1, 2 och 3 har alltså 1 högst prioritet.

Om du inte vill prioritera en leverantör lämnar du fältet **Prioritet** tomt. Om du sedan använder funktionen för betalningsförslag visas den här leverantören sist i listan, efter de leverantörer som har tilldelats ett prioritetsnummer. Du kan ange valfritt antal prioritetsnivåer alltefter behov.

## <a name="see-also"></a>Se även
[Konfigurera inköp](purchasing-setup-purchasing.md)  
[Hantera likviditet](payables-manage-payables.md)

