---
title: "Skapa utskicksgrupper för kontakter"
description: "Du kan använda utskicksgrupper för att identifiera grupper av kontakter som ska få samma information, t.ex. för en marknadsföringskampanj."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, campaign, promo, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c7e79ff2b40ecbaa3cbeac926418702b70272d62
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-mailing-groups-for-contacts"></a>Så här: Skapa utskicksgrupper för kontakter
Utskicksgrupper används för att definiera kontaktgrupper som du vill ge samma information. Du kan till exempel skapa en utskicksgrupp med de kontakter du vill skicka flyttkort till eller en annan grupp för att skicka julklappar.

Att använda utskicksgrupper på kontakter är en två-stegsprocess. Först definierar du utskicksgruppkoden. Du måste bara utföra den här steget en gång för varje utskicksgrupp. När du har en utskicksgrupp kan du börja koppla koden till kontaktföretag.

## <a name="to-define-mailing-group-codes"></a>Definiera utskicksgruppkoder
Utskicksgruppkoden definierar typen eller kategorin för den gruppen, till exempel FLYTTA för kontorsflyttning eller GÅVA för julklappar. Du kan ha flera branschgruppkoder. För att definiera branschgrupperna använder du fönstret **utskicksgrupper**.

1. Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Utskicksgrupper** och välj sedan relaterad länk.
2. Välj åtgärden **Ny** och fyll i en kod och en beskrivning. Koden kan bestå av högst 11 tecken, både siffror och bokstäver.

## <a name="AssignMailGroupContact"></a> Så här tilldelar du utskicksgrupp till en kontakt
1. Öppna kontakten .
2. Välj åtgärden **Utskicksgrupper**. Fönstret **Kontakt utskicksgrupp** öppnas.
3. I fältet **Utskicksgruppskod**, markera den utskicksgrupp du vill tilldela.

Upprepa stegen för varje utskicksgrupp du vill tilldela. Utskicksgrupper kan också tilldelas i Kontaktlista på samma sätt.

Antalet utskicksgrupper som du har tilldelat kontakter anges automatiskt i fältet **Antal utskicksgrupper** på avsnittet **Segmentering** på **Kontakt**-fönstret.

När du har tilldelat kontakterna utskicksgrupp kan du använda dessa uppgifter för urval av kontakter till segmenten. Mer information finns i [Så här lägger du till kontakter i segment](marketing-add-contact-segment.md).

## <a name="see-also"></a>Se även
[Skapa kontaktföretag](marketing-create-contact-companies.md)  
[Skapa kontaktpersoner](marketing-create-contact-persons.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

