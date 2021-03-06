---
title: "Skapa XML-portar som baseras på XML-scheman"
description: "Använda XML-scheman för att ange ramverket för datautbyte."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 607d51d929e019662fdc4e17f7bbb064f806f32a
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-use-xml-schemas-to-prepare-data-exchange-definitions"></a>Så här använder du XML-scheman för att förbereda datautbytesdefinitioner
Om du vill aktivera importera/exportera av data i XML-filer via ramverket för datautbyte i [!INCLUDE[d365fin](includes/d365fin_md.md)], kan du använda XML-schema för att definiera vilka dataelement du vill utbyta med [!INCLUDE[d365fin](includes/d365fin_md.md)]. Du utför det här arbetet i fönstret **Visningsprogram för XML-schema** genom att läsa in XML-schemafilen, välja de relevanta dataelementen och sedan att initiera antingen en definition för datautbyte eller en XMLport.  

 När du har definierat vilka dataelement som ska ingå baserat på XML-schemat, kan du använda åtgärden **Generera XMLPort** för att skapa ett XMLport-objekt.  

 Alternativt kan du använda åtgärden **Generera datautbytesdefinition** för att initiera en definition för datautbyte som baseras på de valda dataelementen, som du sedan fyller i i ramverket för datautbyte. Det skapar en post i fönstret **Definitioner för bokföringsbyte** där du fortsätter genom att ange vilka element i filen som mappas till vilka fält i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Mer information finns i [Så här konfigurerar du datautbytesdefinitioner](across-how-to-set-up-data-exchange-definitions.md).  

 Det här avsnittet innehåller följande procedurer:  

-   Så här läser du in en XML-schemafil  

-   Så här markerar eller avmarkerar du noder i ett XML-schema  

-   Så här skapar du en definition för datautbyte baserat på ett XML-schema  

-   Så här skapar du en XMLport för filen som baseras på ett XML-schema  

-   Så här importerar du en XMLport till Object Designer  

### <a name="to-load-an-xml-schema-file"></a>Så här läser du in en XML-schemafil  

1.  Se till att den relevanta XML-schemafilen är tillgänglig. Filnamnstillägget är .xsd.  

2.  I rutan **Sök** anger du **XML-scheman** och väljer sedan relaterad länk.  

3.  På fliken **Start** i gruppen **Ny** väljer du **Ny**.  

4.  Fyll i fälten enligt beskrivningen i följande tabell.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**Kod**|Ange en kod som identifierar XML-schemat.|  
    |**Beskrivning**|Ange beskrivningen av XML-schemat.|  

     Fältet **Målnamnrymd** anger ett namnområde i XML-schemafilen som har laddats för raden.  

5.  Välj **Läs in schema** på fliken **Start** i gruppen **Process** och välj sedan XML-schemafilen.  

     När filen har fylls i fylls resten av fälten på raden i med information från filen, och kryssrutan **Schemat är inläst** markeras.  

    > [!NOTE]  
    >  Trädet med det inlästa xml-schemat är komprimerat som standard. Du expanderar varje nod genom att välja **+** på noden. Välj **Expandera alla** på menyfliken om du vill expandera alla noder.  

### <a name="to-select-or-clear-nodes-in-an-xml-schema"></a>Så här markerar eller avmarkerar du noder i ett XML-schema  

1.  I rutan **Sök** anger du **Visningsprogram för XML-schema** och väljer sedan relaterad länk.  

2.  Fyll i fälten i huvudet enligt beskrivningen i följande tabell.  

    |Fält|Description|  
    |---------------------------------|---------------------------------------|  
    |**XML-schemakod**|Ange den XML schemafil som du läste in i steg 5 i avsnittet ”Ladda XML-schemafilen”.|  
    |**Nytt XML-portnr**|Ange numret på den XMLport som skapas från XML-schemat när du väljer åtgärden **Generera XMLport** i fönstret .|  

     Raderna fylls nu i med noder som representerar alla element i XML-schemat. Noder för element som är obligatoriska i överensstämmelse med XML-schemat markeras som standard.  

3.  På den första raden, i kolumnen **Nodnamn**, expanderar du noden **Dokument** och expandera sedan gradvis underliggande noder som du vill granska.  

     Högerklicka på en nod och välj sedan **Expandera alla**.  

4.  På fliken **Hem** i gruppen **Visa** väljer du någon av följande åtgärder för att ändra vilka noder som visas.  

    |**Åtgärd**|Description|  
    |----------------|---------------------------------------|  
    |**Visa alla**|Alla noder visas.|  
    |**Dölj ej obligatoriska**|Endast noder som representerar element som krävs enligt XML-schemat visas. Dessa noder har anges vanligtvis med **1** i fältet **MinOccurs**.<br /><br /> Välj **Visa alla** för att återföra vyn.|  
    |**Dölj ej valda**|Endast noder där kryssrutan **Vald** är markerad visas.<br /><br /> Välj **Visa alla** för att återföra vyn.|  

5.  På fliken **Start** i gruppen **Hantera** väljer du **Redigera**.  

6.  I kryssrutan **Vald** anger du för varje nod om du vill att elementet ska stödjas i definitionen för datautbyte för den relaterade SEPA-bankfilen.  

    > [!NOTE]  
    >  När du markerar en obligatorisk underordnad nod markeras även alla överordnade noder ovanför den.  

7.  Välj åtgärden **Markera alla obligatoriska element** för att välja alla noder igen som representerar element som är obligatoriska enligt XML-schemat.  

8.  Välj åtgärden **Avmarkera alla** för att rensa alla val.  

     Fältet **Val** anger att noden har två eller fler syskonnoder som fungerar som alternativ.  

### <a name="to-generate-a-data-exchange-definition-that-is-based-on-an-xml-schema"></a>Så här skapar du en definition för datautbyte baserat på ett XML-schema  

1.  I rutan **Sök** anger du **XML-scheman** och väljer sedan relaterad länk.  

2.  Markera ett lämpligt XML-schema och välj **Öppna XML-schemavisare** på fliken **Hem** i gruppen **Behandla**.  

3.  Se till att de relevanta noderna har markerats. Mer information finns i avsnittet ”Så här markerar eller avmarkerar du noder i ett XML-schema”.  

4.  I fönstret **Visningsprogram för XML-schema** på fliken **Start** i gruppen **Process** väljer du **Generera datautbytesdefinition**.  

 Datautbytesdefinitionen skapas i fönstret **Definitioner för bokföringsbyte** som du kan fylla i genom att ange vilka element i filen som ska mappas till respektive fält i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Mer information finns i [Så här konfigurerar du datautbytesdefinitioner](across-how-to-set-up-data-exchange-definitions.md).  

> [!NOTE]  
>  Du kan också använda funktionen **Hämta filstruktur** från fönstret **Definitioner för bokföringsbyte** som använder funktionen i fönstret **Visningsprogram för XML-schema** för att autofylla snabbfliken **Kolumndefinitioner**.  

### <a name="to-generate-an-xmlport-that-is-based-on-an-xml-schema"></a>Så här skapar du en XMLport som baseras på ett XML-schema  

1.  I rutan **Sök** anger du **XML-scheman** och väljer sedan relaterad länk.  

2.  Markera ett lämpligt XML-schema och välj **Öppna XML-schemavisare** på fliken **Hem** i gruppen **Behandla**.  

3.  I fältet **Nytt XML-portnr** anger du numret som den nya XMLport-artikeln ska få när den skapas.  

4.  Se till att de relevanta noderna har markerats. Mer information finns i avsnittet ”Så här markerar eller avmarkerar du noder i ett XML-schema”.  

5.  Välj **Generera XMLport** och spara objektet som en TXT-fil på ett lämpligt lagerställe på fliken **Hem** i gruppen **Bearbeta**.  

6. Importera nya XML-porten till den [!INCLUDE[d365fin](includes/d365fin_md.md)] development environment och kompilera.

## <a name="see-also"></a>Se även  
[Så här konfigurerar du datautbytesdefinitioner](across-how-to-set-up-data-exchange-definitions.md)   
[Så här exporterar du betalningar till en bankfil](payables-how-export-payments-bank-file.md)   
[Samla in betalningar med SEPA-autogiro](finance-collect-payments-with-sepa-direct-debit.md)   
[Om ramverket för datautbyte](across-about-the-data-exchange-framework.md)

