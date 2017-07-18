---
title: "Så här gör du förutsägande kassaflödesprognoser"
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f657509fc2195674db81f47bc5ae31b7ba1aa40e
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-predictive-cash-flow-forecasts"></a>Så här gör du förutsägande kassaflödesprognoser
Kassaflödesprognoser hjälper dig att se till att företaget har tillräckligt med tillgängliga kontanter för att uppfylla sina ekonomiska skyldigheter och är användbara för att identifiera justeringar. Om du t.ex har ett kontant överskott kan du kan betala vissa fordringar och du kommer att uppskatta en tidig varning om det är för lite tid. 

Cortana Intelligence använder den Azure Machine Learning-tjänst för att göra pålitliga förutsägande prognoser. Prognoser från Cortana Intelligence kan t.ex. hjälpa dig att förutsäga och undvika, kontanta underskott. Tjänsten kombinerar historisk information med aktuella bokföringar för leverantörsreskontra och kundreskontra, inklusive bokföring med förfallodatum som ligger i framtiden. Dessa omfattar:
* Inköpsorder
* Förs.order
* Bokförda försäljnings- och inköpsfakturor
* Kreditnotor

## <a name="before-you-start"></a>Innan du börjar  
Det finns några saker att göra innan du kan använda Cortana Intelligence för kassaflödesprognoser: 
* Om du inte redan använder kassaflödesprognoser kommer du att behöva ange:
    * En eller flera inställningar i **kassaflödeinstallation**. 
    * Konton för kundfordringar, leverantörsskulder, försäljningsorder och inköpsorder. Cortana Intelligence använder bokföringen i dessa konton.
    * En eller flera kassaflödesprognoser i **Kassaflödesprognos**. Se till att inkludera inköpsordern, försäljningsorder, kundreskontra och leverantörsreskontra som källor.  
    För mer information, söker du efter _kassaflödesprognoser_ i hjälpsystemet. 
* Känn till API-URL och API-nyckel för den förutsägande webbtjänsten som ska användas.  
    Du kan använda Azure Machine Learning eller någon annan tjänst om du har någon. Alternativt finns en offentlig modell kallad _Prognosmodellen för Microsoft Dynamics NAV_ tillgänglig online i Cortana Intelligence-galleriet. För att använda modellen gör du följande:

    1. I en webbläsare går du till [Cortana Intelligence-galleriet](https://go.microsoft.com/fwlink/?linkid=828352)
    2. Sök efter _Prognosmodellen för Microsoft Dynamics NAV_ och öppna sedan modellen i Azure Machine Learning Studio.
    3. Använd ditt Microsoft-konto för att registrera dig för en arbetsyta och kopiera sedan modellen.
    4. Kör modellen och publicera den som en webbtjänst.
    5. Gör en anteckning av API-URL och API-nyckel. Du ska använda dessa autentiseringsuppgifter när du installerar Cortana Intelligence i Microsoft Dynamics NAV.  

* Tänk över hur du beräknar prognosen. Azure Machine Learning-tjänsten har begränsningar när det gäller användning. Om du till exempel har många artiklar kan det vara bättre att beräkna mindre ofta. 
* Tilldelas rollcentret Revisor. 

## <a name="set-up-cortana-intelligence"></a>Ställ in Cortana Intelligence
Du kan använda en guide för assisterad installation för att ställa in kassaflödesprognoser. Guiden hjälper dig att ange saker som till exempel hur ofta du uppdaterar prognosen, kontona som du vill basera den på, information om när du betalar skatter och om du ska använda Cortana Intelligence eller inte.  

Om du redan använder kassaflödesprognoser och vill bara ska gå tillbaka till Cortana Intelligence, kan du också använda en manuell process. När du loggar in kommer ett meddelande visas i ett blått fält högst upp i arbetsytan. För att ställa in Cortana Intelligence på en gång trycker du på **ja tack**. Meddelandet visas endast en gång. Om du stänger det använder du den manuella processen för att skapa Cortana Intelligence.  

**Tips:** Beakta längden för perioderna som tjänsten ska använda i dess beräkningar. Ju mer information som du anger, desto mer exakta kommer prognoserna att vara. Se upp för stora avvikelser i perioder. De kommer också att påverka prognoserna. Om Cortana Intelligence inte hittar tillräckligt med data, eller om data varierar mycket, kommer tjänsten inte att utföra någon prognos. 

Så här använder du guiden för assisterad installation:
1. I rollcentret Revisor, under diagrammet **kassaflödesprognos** väljer du åtgärden **Öppna assisterad installation**.
2. Fyll i fälten som behövs i varje steg i guiden.

Så här använder du en manuell process:
1. Sök efter **Kassaflödesinställningar** och välj sedan relaterad länk.
2. Expandera snabbfliken **Cortana Intelligence** och fyll sedan i fälten efter behov.

## <a name="turn-on-cortana-intelligence-for-cash-flow-forecasts"></a>Aktivera på Cortana Intelligence för kassaflödesprognoser
1. Sök efter **Kassaflödesprognoser** och välj sedan relaterad länk.
2. Välj åtgärden **kassaflödekalkylblad**.
3. På sidan **kassaflödekalkylblad** väljer du åtgärden **Föreslå förslagsrader**.  
4. Under **Ursprungstyper att inkludera** markerar du kryssrutan **Cortana Intelligence-prognos**.

## <a name="investigate-a-cash-flow-forecast"></a>Undersök en kassaflödesprognos.
För att ta en ordentlig titt på de uppgifter som ligger bakom prognosen, inklusive avvikelse väljer du kolumnen**Cortana Intelligence**. Den första raden i tabellen visar avvikelsen. De övriga raderna arrangeras av källdokumentet.  

Du kan t.ex se hur prognosen:    
* Hanterar bekräftade försäljningar och inköp 
* Subtraherar leverantörsreskontra och lägger till kundreskontra
* Hoppar över dubbla försäljningsorder och inköpsorder

## <a name="see-also"></a>Se även  
[Arbeta med Dynamics NAV](ui-work-product.md)

