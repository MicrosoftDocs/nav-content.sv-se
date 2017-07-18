---
title: "Så här arbetar du med Artikelattribut"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: eaf539f1d4d00c2cd5679f39f29a3428e33ee1fd
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-item-attributes"></a>Så här arbetar du med Artikelattribut
När kunder gör förfrågningar om en artikel, antingen i motsvarande fält eller via en integrerad webbutik kan kunden fråga eller söka efter egenskaper som till exempel höjd och modellår. För att tillhandahålla denna kundservice kan du tilldela artikelattributvärden av andra typer till artiklarna, som sedan kan användas när du söker efter artiklar.

Du kan också tilldela till artikelattribut till artikelkategorier, som sedan kopplas till artiklarna som använder artikelkategorierna. För mer information finns i [Så här kategoriserar du artiklar](inventory-how-categorize-items.md).

## <a name="to-create-item-attributes"></a>Så här skapar du artikelattribut
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Artikelattribut** och välj sedan relaterad länk.
2. I fönstret **Artikelattribut** väljer du åtgärden **Ny**.
3. I fönstret **Artikelattribut** fyller du i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

**Obs!** Om du väljer **Alternativ** i fältet **Typ** kan du välja åtgärden **Artikelattributvärden** för att markera eller skapa artikelattributvärden Mer information finns i avsnittet "Att skapa artikelattributvärden av typen alternativ".  

## <a name="to-create-values-for-item-attributes-of-type-option"></a>Så här skapar du värden för artikelattribut av typen alternativ
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Artikelattribut** och välj sedan relaterad länk.
2. I fönstret **Artikelattribut** markerar du det artikelattribut typen alternativ som du vill tilldela värden på, och väljer sedan åtgärden **Artikelattributvärden**.
3. I fönstret **Artikelattributvärden** fyller du i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

## <a name="to-assign-item-attributes-to-items"></a>Så här tilldelar du ett artikelattribut till en artikel
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Artiklar** och välj sedan relaterad länk.
2. I fönstret **Artiklar** markerar du den artikel som du vill tilldela artikelattribut på, och väljer sedan åtgärden **Attribut**.
3. I fönstret **Artikelattributvärden** väljer du åtgärden **Ny**.
4. I fältet **Attribut** väljer du knappen AssistEdit och väljer ett befintligt artikelattribut. Välj alternativt åtgärden **Ny** för att först skapa en ny artikelattribut som förklaras i avsnittet "Att skapa artikelattribut".
5. I fältet **Värde** anger du artikelattributvärdet , exempelvis "2010" för modellårsattribut.
6. För artikelattribut av typen Alternativ väljer du knappen AssistEditen i fältet **Värde** och väljer sedan ett artikelattributvärde. Välj alternativt åtgärden **Ny** för att först skapa ett nytt artikelattributvärde som förklaras i avsnittet "Att skapa värden för artikelattribut av typen Alternativ".
7. Upprepa steg 4 genom 6 för alla artikelattribut som du vill tilldela artikeln.

## <a name="to-assign-item-attributes-to-item-categories"></a>Så här tilldelar du ett artikelattribut till artikelkategorier
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Artikelkategorier** och välj sedan relaterad länk.
2. I fönstret **Artikelkategorier** markerar du den artikelkategori, som du vill tilldela artikelattributen till och väljer sedan åtgärden **Redigera**.
3. I fönstret **Artikelkategorikort** på snabbfliken **Attribut** väljer du åtgärden **Ny**.
4. I fältet **Attribut** väljer du knappen AssistEdit och väljer ett befintligt artikelattribut. Välj alternativt åtgärden **Ny** för att först skapa en ny artikelattribut som förklaras i avsnittet "Att skapa ett artikelattribut".
5. I fältet **Standaardvärde** väljer du knappen AssistEdit och väljer du ett artikelattributvärde.
6. Upprepa steg 4 genom 5 för alla artikelattribut som du vill tilldela artikelkategorin.

**Obs!**: Artikelattribut för överordnade artikelkategorier kommer att ärvas av underordnade artikelkategorier. Detta indikeras av fältet **Ärvd från** på snabbfliken **Attribut**. För mer information finns i [Så här kategoriserar du artiklar](inventory-how-categorize-items.md).

## <a name="to-filter-by-item-attributes"></a>Filtrera artikel efter attribut
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Artiklar** och välj sedan relaterad länk.
2. I fönstret **Artiklar** väljer du åtgärden **Filtrera efter attribut**.
3. I fönstret **Filtrera artiklar efter attribut** väljer du knappen AssistEdit i fältet **Attribut** och väljer sedan ett artikelattribut.
4. I fältet **Värde** väljer du knappen AssistEdit och väljer du ett befintligt artikelattributvärde att filtrera efter.

    **Obs!** Du kan bara välja värden direkt för artikelattribut som har fasta värden, till exempel färg. För artikelattribut, som har variabelvärden, till exempel bredd, måste du ange artikelattributvärdet, genom att först välja ett villkor. Se steg 5.
5. I fältet **Värde** ett variabelt artikelattribut väljer du knappen AssistEdit.
6. I fönstret **Ange filtervärde** i fältet **Villkor** väljer du villkor med listpilen.
7. I fältet **Värde** anger du ett attributvärde för att filtrera artiklar.

    **Exempel** För att filtrera efter artiklar där materialbeskrivningen börjar med "blå", fyller du i fälten enligt följande: fältet **Attribut**: Materialbeskrivning, fältet **Villkor**: Börjar med, **Värde**: blå.
8. Välj **OK**.   

Artiklarna i fönstret **Artiklar** filtreras efter de angivna artikelattributvärdena.

## <a name="see-also"></a>Se även
[Så här kategoriserar du artikeln](inventory-how-categorize-items.md)    
[Så här registrerar du nya produkter](inventory-how-register-new-products.md)  
[Hantera lager](inventory-manage-inventory.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

