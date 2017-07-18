---
title: "Ange skrivarval för rapporter"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 55b48aef2bc108ced7f581f0ff6c11263ee467df
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---
    
# <a name="specify-printer-selection-for-reports"></a>Ange skrivarval för rapporter
Du kan ställa in rapporter så att de måste skrivas ut på en viss skrivare. Följande är några användningsområden för skrivarurvalet: 

- Du kan skriva ut rapporter på ett särskilt företagsbrevhuvud.
- Du kan skriva ut rapporter i olika pappersstorlekar.
- Du kan skriva ut rapporter på standardskrivaren för en viss anställd.

Du använder fönstret **Skrivarval** för att ange olika värden för att få olika utflöden. Om du anger ett visst skrivarval, får det sedan företräde framför mer allmänna skrivarval. Du kan till exempel ange ett skrivarval som har värdena i fälten **Användar-ID**, **Rapport-ID**, och **Skrivarnamn**. Det här skrivarvalet åsidosätter det skrivarval som har tomma transaktioner i fälten **Användar-ID** , eller **Rapport-ID**. 

I följande tabell beskrivs kombinationen av värdena för att ange när du lägger upp skrivarval för en rapport.

|Om du vill                                                 |Ange följande värden                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Skriva ut en rapport till en viss skrivare för alla användare |Ange värden i fälten **Rapport-ID**, och **Skrivarnamn** och lämna fältet **Användar-ID** tomt.|
|Skriva ut alla rapporter till en viss skrivare för en specifik användare|Ange värden i fälten **Användar-ID**, och **Skrivarnamn** och lämna fältet **Rapport-ID** tomt.|
|Ange standardskrivaren för alla rapporter|Ange ett värde i fälten **Skrivarnamn** och lämna fältet **Användar-ID** och **Rapport-ID** tomma.|
|Skriva ut en viss rapport till användarens standardskrivare|Ange ett värde i fälten **Rapport-ID** och lämna fältet **Skrivarnamn** och **Användar-ID** tomma.|
|Skriva ut en viss rapport till en viss skrivare till en viss användare|Ange värden i samtliga tre fält.|

## <a name="see-also"></a>Se även
[Arbeta med Dynamics NAV](ui-work-product.md)

