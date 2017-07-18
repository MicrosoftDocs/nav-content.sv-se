---
title: Skapa nummerserier
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
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a>Skapa nummerserier

För varje företag som du lägger upp måste du tilldela unika ID-koder till exempelvis redovisningskonton, kund- och leverantörskonton, fakturor och dokument. Numrering är viktigt inte enbart för identifiering. Ett adekvat numreringssystem gör också företaget mer hanterbart och enkelt att analysera, och kan minska antalet fel som uppstår vid datainmatning.

Du kan lägga upp ett komplett numreringssystem med ett obegränsat antal nummerserier. Du kan använda nummerserier för alla typer av dokument och journaler, samt för huvuddata som kunder, artiklar och projekt.

Du kan kombinera och använda nummerserier vid manuell numrering.

Du skapar ett numreringssystem genom att skapa en eller flera koder för varje typ av huvuddata eller dokument. Du kan till exempel skapa en kod för numrering av kunder, en annan för numrering av försäljningsfakturor och en annan för numrering av dokument i redovisningsjournaler.

När du har skapat en kod måste du skapa minst en nummerserierad. Nummerserieraden innehåller information som första och sista nummer i serien och startdatum. Du kan registrera flera nummerserierader per nummerseriekod, med olika startdatum på varje rad. Nummerserierna används löpande, med början på respektive startdatum.

Om du vill använda mer än en nummerseriekod för en typ av huvuddata, till exempel om du vill använda olika nummerserier för olika kategorier med artiklar, kan du använda nummerseriesamband.

Förutom de nummer som du tilldelar manuellt eller med hjälp av numreringssystemet, tilldelas alla transaktioner automatiskt löpnummer. Dessa nummer visas i **Löpnr.** fält i alla transaktionsfönster. Du kan inte ändra eller ta bort dessa nummer.

## <a name="to-create-relationships-between-number-series"></a>Så här skapar du samband mellan nummerserier
Om du har definierat mer än en nummerseriekod för samma typ av allmän information eller transaktioner kan du skapa samband mellan koderna. Den här funktionen gör det enklare för dig att välja bland koderna när du använder ett nummer.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Nr-serier** och välj sedan relaterad länk.
2. Markera raden med de nummerserier som du vill skapa relationer för och välj sedan **Relationer**.
3. I fältet **Seriekod** anger du koden för nummerserien som du vill koppla till serien du valde i steg 2.
4. Lägg till en rad för varje kod som du vill koppla till den valda nummerserien.
5. Stäng fönstret.

När du hädanefter definierar något för vilket ett nummer krävs kan du använda sambanden som har skapats för att välja bland de kopplade nummerserierna.

## <a name="see-also"></a>Se även
[Arbeta med Dynamics NAV](ui-work-product.md)

