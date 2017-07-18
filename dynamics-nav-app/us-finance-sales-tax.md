---
title: "Omsättningsskatt och momsgrupper i USA och Kanada"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f70a191fc8392bf1685c08c7e905ac96ba7ed069
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-tax-groups-in-the-us-and-canada"></a>Omsättningsskatt och momsgrupper i USA och Kanada
När du först börjar att använda Dynamics NAV kan du köra en assisterad inställning för att snabbt och enkelt konfigurera information om omsättningsskatt för företaget och alternativt för dina kunder och leverantörer. På några minuter är du klar att skapa försäljningsdokument och inköpsdokument med omsättningsskatt som beräknas korrekt.
Om du flyttar till det tomma Mitt företag, rekommenderar vi att du startar genom att använda alla guider för assisterad installation inklusive den för omsättningsskatt. Om du hellre vill ställa in omsättningsskatt själv förklarar detta inlägg vad du måste ta hänsyn till.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Skattegrupper, skatteområden och skattemyndigheter
I Dynamics NAV är en skattegrupp är en grupp lagerartiklar eller resurser som har identiska skattevillkor. Du kan till exempel skapa en skattegrupp för beskattningsbara artiklar och för andra ej beskattningsbara artiklar. Du måste koppla skattegruppkoder till lagerartiklar och redovisningskonton. På liknande sätt måste du tilldela skatteområdeskoder till kunder, lagerställen och dina egna företaginställningar. Guiden för assisterad installation hjälper dig med detta.  

Varje skatteområde är en gruppering av skattemyndigheterna som baseras på ett visst geografiskt lagerställe. Till exempel innehåller Miami, Florida, skatteområde de tre skattemyndigheterna: ort (Miami), delstat (Dade) och stat (Florida).  Dynamics NAV innehåller en begränsad uppsättning skatteområden med en standardkonfiguration, men du kan ändra dem och lägga till nya skatteområden.  

Om du konfigurerar nya skatteområden och skattemyndigheter, måste du kontrollera att du fyller i fälten korrekt. I USA kan stater, delstater, orter, och kommuner ta ut moms. I Kanada kan federala regeringen och provinser ta ut omsättningsskatt. Företaget samlar in och skickar omsättningsskatt till dessa statliga myndigheter för sålda produkter till slutanvändare. Omsättningsskatt kan även debiteras på befintlig omsättningsskatt. Du kan till exempel beräkna skatten på en försäljningsfaktura som redan innehåller skatter från andra skattemyndigheter.  

I Kanada måste skattbelopp vara detaljerade i dokumentet för varje skattemyndighet. Upp till fyra skattemyndigheter kan visas i ett dokument, och skattemyndigheter som har samma utskriftsorder kombineras när de skrivs ut.

## <a name="tax-details"></a>Skatteuppgifter
Fönstret **Skattdetaljer** visar andra kombinationer av skattemyndigheter och momsgrupper för att fastställa momsskattesatser. För varje skattemyndighet rekommenderar vi att du skapar en skattegrupp för normal omsättningsskatt, en annan skattegrupp för artiklar eller tjänster som inte beskattas och ytterligare en skattegrupp för varje typ av artikel eller tjänst som hanteras med en annan Momssatsen i den skattemyndigheten.  

I Förenta staterna när du säljer till en kund på en plats där du inte har en *plats* eller juridisk plats i den staten kan du inte kräva omsättningsskatt. För platser där du inte har en plats, se till att både **skatt under minimumgräns** och **skatt över maximumgräns** är 0.00.  

## <a name="see-also"></a>Se även
[Finans](finance-setup.md)  
[Konfigurera Ekonomi](finance-setup-setup-finance-setup.md)  
[Omsättningsskatt och moms på varor och tjänster i Kanada](ca-finance-setup-tax.md)  
[Enkel omsättningsskattinstallation](https://madeira.microsoft.com/en-us/blog/sales-tax-setup-made-easy)  

