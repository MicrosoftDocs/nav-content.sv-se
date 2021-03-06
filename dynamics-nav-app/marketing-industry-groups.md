---
title: "Skapa Branschgrupper för kontaktföretag"
description: "Beskriver hur du definierar en branschgrupp och koppla den till ett företag, till exempel detaljhandel eller bilindustri."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 62d946155cb65a3e976771bc5029878893bd4797
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-industry-groups-for-contact-companies"></a>Så här: Skapa branschgrupper på kontaktföretag
Branschgrupper används för att visa vilken bransch kontakterna tillhör, exempelvis detaljhandel eller bilBransch.

Att använda Branschgrupper på kontakter är en två-stegsprocess. Först definierar du Branschgruppkoden. Du måste bara utföra den här steget en gång för varje Branschgrupp. När du har en Branschgrupp kan du börja koppla koden till kontaktföretag.

> [!NOTE]  
>   Om du tänker synkronisera kontakterna med leverantörer, kunder eller bankkonton i andra delar av programmet vill du kanske skapa en affärsrelation för dem.

## <a name="to-define-an-industry-group-code"></a>Definiera en Branschgruppskod
Koden för branschgruppen definierar typen eller kategorin för den gruppen, till exempel ANNONS för annonsering eller PRESS för TV och radio. Du kan ha flera branschgruppkoder. För att definiera branschgrupperna använder du fönstret **branschgrupper**.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Branschgrupper** och välj sedan relaterad länk.
2. Välj åtgärden **Ny** och fyll i en kod och en beskrivning. Koden kan bestå av högst 11 tecken, både siffror och bokstäver.

## <a name="AssignIndustryGroupContact"></a> Så här tilldelar du industrigrupper till en kontakt
Du kan inte tilldela branschgrupper till en kontaktperson, endast företag.

1. Öppna kontakten .
2. Välj åtgärden **företag** och sedan **branschgrupper**. Fönstret **Kontakt branschgrupper** öppnas.
3. I fältet **branschgruppkod**, markera den branschgrupp du vill tilldela.

Upprepa stegen för varje branschgrupp du vill skapa. Branschgrupper kan också tilldelas i Kontaktlista på samma sätt.

Antalet branschgrupper som du har tilldelat kontakter anges automatiskt i fältet **Antal branschgrupper** på avnisttet **Segmentering** på **Kontakt**-fönstret.

När du har tilldelat kontakterna branschgrupper kan du använda dessa uppgifter för urval av kontakter till segmenten. Mer information finns i [Så här lägger du till kontakter i segment](marketing-add-contact-segment.md).

## <a name="see-also"></a>Se även
[Skapa kontaktföretag](marketing-create-contact-companies.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

