<properties
                pageTitle="Så här omvärderar du lager | Dynamics NAV"
                description="Beskriver hur du uppskattar eller skriver av värdet av en eller flera artiklar i lager genom att bokföra deras faktiska, beräknade värde."
                services="project-madeira"
                documentationCenter=""
                authors="SorenGP"
/>
<tags
    ms.service="project-madeira"
    ms.topic="article"
    ms.devlang="na"
    ms.tgt_pltfrm="na"
    ms.workload="na"
    ms.date="11/07/2016"
    ms.author="SorenGP" />


# <a name="how-to-revalue-inventory"></a>Så här omvärderar du lager   
Om du vill öka eller minska värdet för en artikel eller en viss artikeltransaktion, använder du omvärderingsjournalen.

## <a name="to-revalue-inventory"></a>Omvärdera lager
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Omvärderingsjournal** och välj sedan relaterad länk.
2. Välj åtgärden **Beräkna lagervärde**.
3. I fönstret **Beräkna lagervärde** fyller du i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
4. Välj **OK**.
5. På varje rad i fönstret **Omvärderingsjournal** i fältet **Styckkostnad (omvärderad)** anger du den nya styckkostnaden. Du kan alternativt ange det nya totalbeloppet i fältet **Lagervärde (omvärderad)**.

    Relevanta fält uppdateras automatiskt. Lägg märke till att den faktiska förändringen av lagervärdet för den aktuella artikeltransaktionen visas i fältet **Belopp**. Detta belopp utgör skillnaden mellan värdena i fälten **Lagervärde (beräknat)** och **Lagervärde (omvärderat)**.

6. När du har slutfört alla rader i omvärderingsjournalen väljer du åtgärden **Bokför**.

Nya värdetransaktioner skapas nu för att visa omvärderingarna som du har bokfört. Du kan se de nya värdena på respektive artikelkort.

## <a name="see-also"></a>Se även
[Hantera lager](inventory-manage-inventory.md)  
[Hantera försäljning](sales-manage-sales.md)  
[Hantera inköp](purchasing-manage-purchasing.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)

