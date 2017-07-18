---
title: "Förstå PIA-metoder"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f21357897dd730d96db7abab469d5958c6fe117c
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="understanding-wip-methods"></a>Förstå PIA-metoder

Dynamics NAV stöder följande metoder för att beräkna och registrera värdet för pågående arbete.

|PIA-metod |Beräkningsformel |Beskrivning av beräkning|
|-----------|--------------------|-----------------------|
|Kostnadsvärde|Bokförd intäkt = Fakturerbart fakturerat pris<br /><br /> Totala uppskattade kostnader = Fakturerbart totalpris x Budget kostnadsgrad<br /><br /> PIA-kostnader = \(Färdigställningsgrad - Fakturerat %\) x Uppskattade totalkostnader<br /><br /> Färdigställningsgrad = Förbrukning totalkostnad/Budget totalkostnad<br /> Fakturerat % = Fakturerbart fakturerat pris<br /><br /> Fakturerbart totalpris bokförda kostnader = Förbrukning totala kostnader - PIA|Kostnadsvärdesberäkningar inleds med att beräkna värdet av vad som har tillhandhållits genom att ta en del av de uppskattade totalkostnaderna baserat på färdigställningsgrad. Fakturerade kostnader subtraheras genom att ta en del av de uppskattade totalkostnaderna baserat på fakturerad procent.<br /><br /> Den här beräkningen kräver att fakturerbart totalpris, budget totalpris och budget totalkostnader anges korrekt för hela projektet.|
|Försäljningskostnad|Bokförd intäkt = Fakturerbart fakturerat pris<br /><br /> Bokförda kostnader = Budget totalkostnad x Fakturerat %<br /><br /> Fakturerat % = Fakturerbart fakturerat pris/Fakturerbart totalpris<br /><br /> \(Fakturerat % finns som kolumn på projektaktivitetsrader\)<br /><br /> PIA-kostnader = Förbrukning totalkostnad - Bokförda kostnader|Beräkningar av försäljningskostnader inleds genom att beräkna bokförda kostnader. Kostnader bokförs proportionellt baserat på budget totalkostnader.<br /><br /> Den här beräkningen kräver att fakturerbart totalpris och budget totalkostnader anges korrekt för hela projektet.|
|Försäljningsvärde|Bokförda kostnader = Förbrukning totalkostnad<br /><br /> Bokförd intäkt = Förbrukning totalpris x Förväntad faktureringsgrad<br /><br /> Kostnadsåterställning % = Fakturerbart totalpris/Budget totalpris<br /><br /> PIA-försäljning = Bokförd försäljning - Fakturerbart fakturerat pris|Beräkningar av försäljningsvärde bokför intäkten proportionellt baserat på totala förbrukningskostnader och förväntad kostnadsåterställningsgrad.<br /><br /> Den här beräkningen kräver att fakturerbart totalpris och budget totalpris anges korrekt för hela projektet.|
|Procent färdigställt|Bokförda kostnader = Förbrukning totalkostnad<br /><br /> Bokförd intäkt = Fakturerbart totalpris x Färdigställningsgrad<br /><br /> Färdigställningsgrad = Förbrukning totalkostnad/Budget totalkostnad<br /><br /> \(Kallas för "Färdigställningsgrad % på projektaktivitetsrader\)<br /> PIA-försäljning = Bokförd försäljning - Fakturerbart fakturerat pris|Beräkningar av färdigställningsgrad bokför intäkter proportionellt baserat på färdigställningsgraden, det vill säga Förbrukning totalkostnad kontra budget kostnader.<br /><br /> Den här beräkningen kräver att fakturerbart totalpris och budget totalkostnader anges korrekt för hela projektet.|
|Slutfört kontrakt|PIA-belopp = PIA-kostnadsbelopp = Förbrukning \(Totalkostnad\)<br /><br /> PIA-försäljningsbelopp = Fakturerbart \(Fakturerat pris\)|Slutfört kontrakt bokför inte intäkter och kostnader förrän projektet är slutfört. Du kan vilja göra detta när det finns en stor osäkerhet kring uppskattningen av kostnader och intäkter för projektet.<br /><br /> All förbrukning bokförs på kontot för PIA-kostnader \(tillgång\) och all fakturerad försäljning bokförs på kontot för fakturerad PIA-försäljning\(skuld\) tills projektet är slutfört.|

## <a name="see-also"></a>Se även
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)  

