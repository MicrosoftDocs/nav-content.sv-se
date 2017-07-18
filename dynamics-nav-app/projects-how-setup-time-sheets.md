---
title: "Så här kan du skapa tidrapporter"
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
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a>Så här kan du skapa tidrapporter
Tidrapporter i Dynamics NAV administrerar tidregistrering veckovis (sju dagar i taget). Du kan använda dem för att spåra den tid som används för projektet och du kan använda dem för att registrera enkel resurstimregistrering. Innan du kan använda tidrapporter måste du ange hur du vill att de ska registreras och konfigureras.

När du har ställt in hur organisationen ska använda tidrapporter, kan du ange om och hur tidrapporter godkänns. Beroende på organisationens behov kan du ange:

- En eller flera användare som tidrapportsadministratör och godkännare för alla tidrapporter.
- En tidrapportsgodkännare för varje resurs.

När du har konfigurerat tidrapporter, kan du skapa tidrapporter för resurser, tilldela dem till projektplaneringsrader och bokföra tidrapportrader. Mer information finns i [Så här använder du tidrapporter](projects-how-use-time-sheets.md).

## <a name="to-set-up-general-information-for-time-sheets"></a>Så här anger du allmän information för tidrapporter  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resursinställningar** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. För fältet **Tidrapport per projektgodkännande** väljer du ett av följande alternativ.

|Alternativ |Beskrivning|
|---|---|
|**Aldrig**|Användaren i fältet **Användar-ID för tidrapportens godkännare** på resurskortet godkänner tidrapporten.|
|**Alltid**|Användaren i fältet **Ansvarig person** på projektkortet godkänner tidrapporten.|
|**Enbart maskin**|Om maskinens tidrapport är länkad till ett projekt, godkänner användaren i fältet **Ansvarig person** på projektkortet tidrapporten. Om maskinens tidrapport är länkad till en resurs, godkänner användaren i fältet **Användar-ID för tidrapportens godkännare** på resurskortet tidrapporten.

## <a name="to-assign-a-time-sheet-administrator"></a>Så här tilldelar du en tidrapportsadministratör  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Användarinställningar** och välj sedan relaterad länk.  
2.  Lägg till en ny användare om användarlistan inte innehåller den person som du vill ska vara tidrapportsadministratören. För mer information, kontakta administratören.  
3. Välj en användare som ska vara en tidrapportadministratör och välj sedan kryssrutan **Tidrapportadmin.** .  

**Tips**: Vi rekommenderar att du endast anger en användare som tidrapportsadministratör för ett företag. I följande procedur skapar du en tidrapportägare och godkännare där tidrapportgodkännaren tilldelas för varje resurs.  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a>Så här tilldelar du en tidrapportsägare och en godkännare  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Resurser** och välj sedan relaterad länk.
2. Välj den resurs som du vill ställa in möjlighet att använda tidrapporter för och markera sedan kryssrutan **Använd tidrapport**.  
3. I fältet **Användar-ID för tidrapportens ägare** anger du ID för ägaren av tidrapporten. Ägaren kan ange tidförbrukning på en tidrapport och skicka den för godkännande. Vanligtvis, när resursen är en person, är den person också ägare.  
4. I fältet **Användar-ID för tidrapportens godkännare** anger du ID för godkännaren av tidrapporten. Godkännaren kan godkänna, avvisa eller öppna en tidrapport igen.  

**Obs**! Du kan inte ändra ID på tidrapportsgodkännaren om det finns tidrapporter som inte ännu har behandlats och har statusen **Skickad** eller **Öppen**.

## <a name="see-also"></a>Se även
[Ange projekthantering](projects-setup-projects.md)  
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)  

