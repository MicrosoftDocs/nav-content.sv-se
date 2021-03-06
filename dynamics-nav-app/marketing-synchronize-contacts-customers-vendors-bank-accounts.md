---
title: "Synkronisera kontakter med kunder och leverantörer"
description: "Du kan koppla eller synkronisera kontaktinformation för kontakter som också är kunder, leverantörer eller bankkonton, så att du bara uppdaterar informationen på ett ställe."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, CRM, integration, couple
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 44de0d07753871e6dfc38e1ee8240c621174b377
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="synchronizing-contacts-with-customers-vendors-and-bank-accounts"></a>Synkronisera kontakter med kunder, leverantörer och bankkonton
Om några av kontakterna också är kund-, leverantörs- och/eller bankkonton kan du synkronisera deras kontaktinformation med relaterade kund-, leverantörs- och bankkonton. Synkroniseringen gör information som är gemensam mellan kontakter och kunder, leverantörer eller bankkonton densamma.  

Innan du kan synkronisera kontakterna med kund-, leverantörs- och/eller bankkonton måste du ange en affärsrelationskod för dessa i fönstret **Marknadsföringsinställningar**. Mer information finns i [Ställa in e-postmeddelanden](marketing-setup-marketing.md).

## <a name="different-ways-to-synchronize-contacts-with-customers-vendors-and-bank-accounts"></a>Olika sätt att synkronisera kontakter med kunder, leverantörer och bankkonton
Du kan synkronisera kontakterna med kunder, leverantörer eller bankkonton på tre olika sätt:

* Länka kontakterna till befintliga kunder, leverantörer eller bankkonton från kontaktkortet. Mer information finns i [Så här länkar du kontakter med kunder, leverantörer och bankkonton](marketing-how-link-contact.md).
* Skapa kunder, leverantörer och bankkonton från kontakten. Mer information finns i [Skapa en företagskontakt från kund, leverantör eller bankkonto från en kontakt](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).
* Skapa kontakter från kunder, leverantörer eller bankkonton. Mer information finns i [Skapa en företagskontakt från kund, leverantör eller bankkonto](marketing-how-create-contact-companies.md).

## <a name="consequences-of-synchronization"></a>Konsekvenser för synkroniseringen
När kontaken har synkroniserats med kund-, leverantörs- eller bankkontot:

* Du behöver bara uppdatera uppgifterna på ett ställe. Om du till exempel ändrar telefonnumret på kontakten uppdateras telefonnumret med samma ändring på kund-, leverantörs- eller bankkontot.
* Om du har angett nummerserie för kontakter när du skapar kund-, leverantörs- eller bankkontokort, skapas automatiskt ett kontaktkort för kunder, leverantörer eller bankkonton.
* Du kan skapa förs.offerter och försäljningsorder, inköpsofferter och inköpsorder från kontakten.
* Dina interaktioner kan registreras när du utför vissa åtgärder som att skriva ut order eller avropsorder, skapa försäljningsserviceorder, skicka e-post osv.
* Om du raderar en kontakt som är länkad till en kund, leverantör eller bank är det bara kontakten som tas bort från programmet. Kunden, leverantören eller bankkontot återstår.
* Om du raderar en kontakt som är länkad till en kund, leverantör eller ett bankkonto är det bara kontakten som återstår.

> [!NOTE]  
>   Vissa detaljer, t.ex fakturering och bokföringsdetaljer, visas inte på kontaktkortet. Följaktligen kan du behöva lägga till dem manuellt på kund-, leverantörs- och bankkontokort, när du skapar kontakter som kunder, leverantörer eller bankkonton.

## <a name="see-also"></a>Se även
[Hantera kontakter](marketing-contacts.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

