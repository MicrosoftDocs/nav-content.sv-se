---
title: "Använda ADCS (Automated Data Capture Systems)"
description: "Du kan använda det automatiska datainsamlingssystemet (ADCS eller Automated Data Capture System) för att registrera förflyttningen av alla artiklar i distributionslagret och för att registrera några journalaktiviteter, däribland kvantitetsjusteringar i artikeljournalen för distributionslagret, inventeringsjournalen och fysisk inventering."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2e5fb701013f75557302b7a26ba8c6f2972806a3
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-automated-data-capture-systems-adcs"></a>Så här: Aktivera automatiskt datainsamlingssystem (ADCS)
Du kan använda det automatiska datainsamlingssystemet (ADCS eller Automated Data Capture System) för att registrera förflyttningen av alla artiklar i distributionslagret och för att registrera några journalaktiviteter, däribland kvantitetsjusteringar i artikeljournalen för distributionslagret, inventeringsjournalen och fysisk inventering.  

Om du ska använda ADCS måste du ge varje artikel i distributionslagret en artikelidentifierare. Du måste även lägga upp miniformulär, handdatorfunktioner, datautbyten och specificeras inställningar för fältet som kontrollerar ADCS. Du anger om du ska använda ADCS på lagerställekortet för ett lager.

Baserat på behovsnivån i lagret definierar du den mängd information som ska visas i miniformulärinställningarna för den aktuella handenheten. Följande är exempel information som du kan visa:  

- Data från tabeller i [!INCLUDE[d365fin](includes/d365fin_md.md)], till exempel en lista över plockningsdokument som användaren kan välja från.  
- Textinformation.  
- Meddelanden som innehåller bekräftelser eller fel om aktiviteter som utförts och registrerats av handenheter användaren.

Mer information finns i [konfigurera ett automatiskt datainsamlingssystem](https://msdn.microsoft.com/en-us/library/dd338742.aspx) på MSDN.

## <a name="to-set-up-a-warehouse-to-use-adcs"></a>Så här konfigurerar ett lager att använda ADCS  
Om du ska använda ADCS måste du ange vilka distributionslagerplatser som använder teknologin.  

> [!NOTE]  
>  Vi rekommenderar att du inte ställer in ett distributionslager som ska använda ADCS, om distributionslagret dessutom har en lagerplats kapacitetsprincip.

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Lagerställen** och välj sedan relaterad länk.
2.  Välj ett lager i listan som du vill aktivera för ADCS och välj **redigera**.
3. I fönstret **lagerställekort** markerar du kryssrutan **använda ADCS**.  

## <a name="to-specify-an-item-to-use-adcs"></a>Ange ett objekt för att använda ADCS  
Varje distributionslagerartiklar som ska användas med ADCS, måste tilldelas en identitetskod för att koppla den till dess artikelnummer. Du kan t.ex använda artikelns Streckkod som identitetskoden. En artikel kan också använda flera identitetskoder. Det kan vara praktisk i de fall där en artikel är disponibel i olika måttenheter, t.ex stycken och pallar. Tilldela varje en identitetskod, i det här fallet.    

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Artiklar** och välj sedan relaterad länk.  
2.  Markera ett objekt i listan som ingår i ADCS-lösningen och välj åtgärden **redigera**.
3. I fönstret **Artikelkort** väljer du åtgärden **Identifierare**.
4. I fönstret **ArtikelIdentifierare** väljer du åtgärden **Ny**.
5. I fältet **Kod** ange identifierare för artikeln. Du kan t.ex använda artikelns Streckkod som identitetskoden.  

    Du kan även definiera ett **Variantkod** och en **Enhet** kod.  

6. Ange flera koder för varje artikel, om det behövs.
7. Välj knappen **OK**.  
8.  För att granska informationen väljer du fältet **identitetskod** för att öppna fönstret **Artikelidentifierare**.

## <a name="to-add-an-adcs-user"></a>Om du vill lägga till en ADCS-användare  
Du kan lägga till användare som en användare av ett ADCS (Automated Data Capture System). När du gör det, måste du även ange ett lösenord. Om du vill kan du även ange en koppling som identifierar ADCS-användaren som distributionslageranvändare. ADCS-användarlösenord kan vara olika från Windows-inloggningslösenord för användaren. Mer information finns i [Så här hanterar du användare och behörigheter](ui-how-users-permissions.md).

1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **ADCS-användare** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny**.  
3.  Ange ett **Namn** på användaren. Namnet kan inte innehålla fler än 20 tecken, inklusive blanksteg.  
4.  Ange ett **Lösenord** i fältet. Lösenord maskeras.  

### <a name="to-specify-that-a-warehouse-employee-is-an-adcs-user"></a>Om du vill ange att lagerpersonalen är en ADCS-användare  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Dist.lager personal** och välj sedan relaterad länk.  
2.  Lägga till en ny lagerpersonalen, om det behövs. Mer information finns i [Så här skapar du Dist.lager personal](warehouse-how-to-set-up-warehouse-employees.md).  
3.  Välj åtgärden **Redigera lista**.  
4.  Välj en lagerpersonal i listan. I fältet **ADCS-användare** väljer du listpilen och sedan namnet på en ADCS-användare i listan.  

> [!NOTE]  
>  Standarddistributionslagret för den anställde ska vara en som använder ADCS.

## <a name="to-create-and-customize-miniforms"></a>Så här: Skapa och anpassa Miniformulär
Du använder miniformulär som beskriver den information som du vill presentera på en handenheter. Du kan till exempel skapa miniformulär för att hantera lageraktiviteten att plocka artiklar. När du har skapat en miniformulär, kan du lägga till funktioner för den vanliga åtgärder för en användare med handenheter, till exempel flytta uppåt eller en rad.  

För att använda eller ändra funktionen i en miniformulärfunktion måste du skapa en ny kodmodul eller ändra befintliga för att utföra lämplig åtgärd eller svar. Du kan få mer information om ADCS-funktioner genom att undersöka kodmoduler till exempel 7705, d.v.s det kodenheten för inloggningar funktioner. Kodmodul 7705 visas hur en miniformulär av korttyp arbetar.  

### <a name="to-create-a-miniform-for-adcs"></a>Så här skapar du en miniformulär för ADCS  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Miniformulär** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny**.  
3.  I fältet **Kod** anger du en kod på Miniformuläret. Ange värden i alla övriga fält, om du vill.  

    Välj **Starta miniformulär** kryssrutan för att ange att miniformuläret är det första formulär som användaren ser i logga in.  

4.  Definiera fälten som visas på miniformuläret på **Rader** Snabbfliken. Ordningen där du anger rader, är den ordning som raderna ska visas på handenheten.  

När du har skapat en miniformulär, nästa steg är att skapa operationer och att koppla funktioner för olika tangentbord indata.  

### <a name="to-add-support-for-a-function-key"></a>Om du vill lägga till stöd för en funktionstangent  
1.  Lägga till koden som liknar följande exempel, till the.xsl-filen för tilläggsprogrammet. Det skapar en operation för **F6** tangent. Tangentsekvensinformation kan erhållas från tillverkaren enhet.  
    ```  
    <xsl:template match="Function[.='F6']">  
      <Function Key1="27" Key2="91" Key3="49" Key4="55" Key5="126" Key6="0"><xsl:value-of select="."/></Function>  
    </xsl:template>  

    ```  
2.  I [!INCLUDE[d365fin](includes/d365fin_md.md)] development environment, öppna tabell 7702 och lägg till en kod som representerar den nya tangenten. Skapa en tangent som heter **F6** i det här exemplet.  
3.  Lägga till C/AL-koden till den aktuella operationen på miniformulärspecifika Codeunit för att hantera funktionen primärnyckel.  

### <a name="to-customize-miniform-functions"></a>Om du vill anpassa miniformulärfunktioner  
1.  Välj ikonen ![Söka efter sida eller rapport](media/ui-search/search_small.png "ikonen Söka efter sida eller rapport"), ange **Miniformulär** och välj sedan relaterad länk.  
2.  Välj ett miniformulär från listan, välj åtgärden **Redigera**.  
3.  Välj åtgärden **Funktioner**.  
4.  I listrutan **Funktionskod** väljer du en kod för att representera en funktion som du vill koppla till miniformuläret. Du kan till exempel välja ESC, som associerar funktionen med att trycka på ESC-tangenten.  

I [!INCLUDE[d365fin](includes/d365fin_md.md)] development environment, redigera koden för fältet **Hantera kodmodul** om du vill skapa eller ändra kod för att utföra lämplig åtgärd eller svar.

Mer information finns i [konfigurera ett automatiskt datainsamlingssystem](https://msdn.microsoft.com/en-us/library/dd338742.aspx) på MSDN.

## <a name="see-also"></a>Se även  
[Lagerstyrning](warehouse-manage-warehouse.md)  
[Lagersaldo](inventory-manage-inventory.md)  
[Ställa in lagerstyrning](warehouse-setup-warehouse.md)     
[Monteringshantering](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyrning](design-details-warehouse-management.md)  
[Arbeta med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

