---
title: "Så här skapar du projekt"
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
ms.openlocfilehash: df34c435d07e9526cb4d93e2bfc30162258ba957
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-jobs"></a>Så här skapar du projekt
När du vill starta ett nytt projekt måste du skapa ett projektkort med inbyggda projektaktiviteter och projektplaneringsrader, strukturerade i två lager.  

Det första lagret består av projektaktiviteter. Du måste skapa minst en projektaktivitet per projekt eftersom all bokföring refererar till en projektaktivitet. Med åtminstone en projektaktivitet i ditt projekt kan du lägga upp projektplaneringsrader och bokföra förbrukningen i projektet.

Det andra lagret består av projektplaneringsrader som specificerar detaljerad förbrukning av resurser, artiklar och diverse redovisningskostnader.

Lagerstrukturen gör att du kan dela upp projekt i mindre aktiviteter och specificera budget, offerter och registrering mer i detalj. Dessutom att du får en inblick i hur ett projekt fortlöper. Du kan till exempel spåra om du uppfyller uppsatta milstolpar eller om du är i linje med mål för att uppfylla budget.

**OBS**! Åtgärden **Nytt projekt** på Rollcentret **Projektchef** startar en guidad hjälp som guidar dig genom stegen för att skapa ett projekt med integrerade uppgifter och planeringsrader. Efterföljande procedur beskriver hur du utför stegen manuellt.

## <a name="to-create-a-job-card"></a>Så här skapar du ett projektkort.
Du skapar ett projektkort och sedan skapar projektaktivitetsrader och projektplaneringsrader för det.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny** och fyll sedan i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. Om du vill ange projektet med information om andra projekt väljer du åtgärden **Kopiera projekt**, fyller i fälten efter behov och väljer sedan knappen **OK**.

**OBS**! Om du använder tidrapporter i projektet måste du också ange en person som ansvarar. Denna person kan godkänna tidrapporter för anställdas aktiviteter som är kopplade till projektet. Mer information finns i [Så här skapar du tidrapporter](projects-how-setup-time-sheets.md).

## <a name="to-create-tasks-for-a-job"></a>Så här kan du skapa aktiviteter för ett projekt  
En viktig del när du skapar ett projekt är att ange de olika aktiviteter som ingår i projektet. Du gör detta genom att lägga till nya rader i snabbfliken **Uppgifter** i fönstret **Projektkort**, en aktivitet per rad. Varje projekt måste ha minst en aktivitet.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.
2. Öppna projektkortet för ett relevant projekt.
3. På snabbfliken **Uppgifter** fyller du i fälten efter behov på en ny rad.
4. Om du vill dra in uppgifter och skapa en hierarki väljer du åtgärden **Uppgifter** och sedan väljer du åtgärden **Indrag för projektaktiviteter**.
5. Upprepa steg 3 och 4 för alla de aktiviteter som du behöver för projektet.
6. Om du vill ange projektaktiviteter med information om andra projektaktiviteter väljer du åtgärden **Kopiera projektaktiviteter från**, fyller i fälten efter behov och väljer sedan knappen **OK**.

## <a name="to-create-planning-lines-for-a-job"></a>Så här skapar du en planeringsrad för ett projekt  
Du kan förfina dina nya projektaktiviteter på projektplaneringsrader. En planeringsrad kan används för att samla in den information som du vill spåra för ett projekt. Med planeringsrader kan du lägga till information som vilka resurser som behövs eller för att samla in vilka artiklar som behövs för att utföra projektet. Du kan till exempel ha en aktivitet för att inhämta kundens godkännande av ett projekt, du kan associera den aktiviteten med planeringsrader för objekt som att träffa kunden och tilldela en resurs.  

En projektplaneringsrad kan ha en av följande typer.  

|Kontakttyp|Beskrivning|
|----|-----------|
|**Budget**|Anger uppskattad förbrukning och kostnader för projektet, vanligtvis i tids- och materialtypsprojekt. Planeringsrader av den här typen kan inte faktureras.|
|**Fakturerbart**|Anger uppskattad fakturering till kunden, vanligtvis som ett fastprisprojekt.|
|**Både Budget och Fakturerbart**|Anger budgeterad förbrukning som motsvarar vad du vill fakturera.|  

**Obs**. När du anger information på projektplaneringsrader fylls kostnadsinformationen i automatiskt. T.ex. baseras kostnaden, priset och rabatten för resurser och artiklar inledningsvis på informationen som definieras på resurs- och artikelkort.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Projekt** och välj sedan relaterad länk.
2. Öppna ett relevant projektkort.
3. Markera ett projekt där fältet **Typ av projektaktivitet** innehåller **Bokföring** och klicka sedan på åtgärden **Projektplaneringsrader**.  
4. I fönstret **Projektplaneringsrader**, på en ny rad, fyller du i fält efter behov.
5. Upprepa steg 3 och 4 för alla de planeringsrader som du behöver för projektaktiviteten.

## <a name="see-also"></a>Se även
[Hantera projekt](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Hantera inköp](purchasing-manage-purchasing.md)         
[Hantera försäljning](sales-manage-sales.md)      
[Arbeta med Dynamics NAV](ui-work-product.md)  

