---
title: "Så här skapar du interaktioner på kontakter och segment"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 459a86ad9674e0d61b045743cbcc99ffdb5cacd9
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---
# <a name="how-to-create-interactions-on-contacts-and-segments"></a>Så här skapar du interaktioner på kontakter och segment
Du kan skapa interaktioner för att registrera all interaktion och kommunikation som du har med dina kontakter och segment, till exempel direktreklam.

Innan du skapar interaktioner måste du lägga upp interaktionsmallar. Mer information finns i  [Skapa interaktionsmallar](marketing-interactions.md#set-up-interaction-templates).

## <a name="to-create-an-interaction"></a>Skapa interaktioner så här
1. Öppna kontakten, säljaren eller interaktionsloggtransaktionen.
2. Välj åtgärden **Skapa interaktion**.
3. Fyll i fälten och välj sedan knappen **OK**.

**Obs!** Om du behöver göra något annat aktivitet i **Avbryt**, innan du avslutar interaktionen, kan du avsluta guiden och välja om du vill avsluta interaktionen senare. Detta senarelägger interaktionen.

## <a name="to-finish-and-delete-postponed-interactions"></a>Så här slutför du och tar bort senarelagda åtgärder
1. Öppna kontakten, säljaren eller interaktionsloggtransaktionen.
2. Välj **Senarelagda interaktioner**.
3. Markera den åtgärd som du vill slutföra och klicka på **Åtgärder**, Fortsätt.

## <a name="to-create-an-interaction-on-a-segment"></a>Så här skapar du interaktioner för segment
1. På startsidan väljer du **Aktiva segment** i det övre högra hörnet väljer du ikonen **Söka efter sida eller rapport**, anger **Segment** och sedan väljer relaterad länk.
2. I fönstret **Segment**, i avsnittet **Interaktion**, fyller du i fälten för att specificera vilken interaktion som du vill tilldela segmentet.

  När du har tilldelat segmentet en interaktion kan du anpassa interaktionen till respektive kontakt i segmentet, exempelvis genom att välja en annan interaktionsmall på raderna i fönstret **Segment**.
3. För att logga segmentet och interaktionerna väljer du åtgärden **Logg**. Fönstret **Loggsegment** öppnas.
4. Om du vill skapa ett nytt segment med samma kontakter markerar du kryssrutan **Skapa uppföljningssegment**. Innan ett uppföljningssegment kan skapas måste du ange en nummerserie för segment i fönstret **Affärsstödsinställning**.

Interaktionen registreras för varje kontakt i segmentet i tabellen **Interaktion loggtrans.** och segmentet loggas. Loggade segment återfinns i fönstret **Segmentlogg**.

Om du har markerat kryssrutan **Skapa uppföljningssegment** skapas automatiskt ett nytt segment med samma kontakter som det segment som du precis har loggat.

## <a name="see-also"></a>Se även
[Registrera interaktioner](marketing-interactions.md)  
[Hantera kontakter](marketing-contacts.md)  
[Hantera Försäljningsmöjligheter](marketing-manage-sales-opportunities.md)  
[Ställ in Marknadsföring och Kontakthantering](marketing-setup-marketing.md)

