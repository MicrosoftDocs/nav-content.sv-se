---
title: "Omsättningsskatt och moms på varor och tjänster i Kanada"
author: edupont04
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c032a02b545441b927ef5c4facc9f77731f37ab7
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a>Omsättningsskatt och moms på varor och tjänster i Kanada
I Kanada när en leverantör inte har en företagsnärvaro i regionen som inköpet görs i, debiteras leverantören endast för moms på varor och tjänster (GST) eller harmoniserad försäljningsmoms HST). Men om landskapet har en provinsiell omsättningsskatt (PST), måste köparen fortfarande beräkna PST och betala den direkt till regionen. När en skatteområdeskod för regionen markeras använder Dynamics NAV den för att beräkna PST och bokföra den så att det finns en skatteskuld både i redovisningen och i skattetransaktionsposten. Därför bör skatteområdeskoden som markeras här vara en med endast PST och inte GST.  
Mer information om omsättningsskatt finns i [Omsättningsskatt och skattegrupper i USA och Kanada](us-finance-setup-sales-tax.md).  

## <a name="submitting-the-gsthst-file"></a>Skicka GST-/HST-filen
Skatteinformationen i inköpsdokument används för att generera en GST-/HST-internetfilöverföring som du måste tillhandahålla till skattemyndigheterna. Den här filen inkluderar moms för varor och tjänster (GST) och harmoniserad försäljningsmoms HST). Arkivet skapas i ett .tax-filformat, som kan överföras via internet.  

## <a name="see-also"></a>Se även
[Finans](finance-setup.md)  
[Konfigurera Ekonomi](finance-setup-setup-finance-setup.md)  
[Omsättningsskatt och momsgrupper i USA och Kanada](us-finance-setup-sales-tax.md)

