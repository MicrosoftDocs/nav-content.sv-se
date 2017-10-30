---
title: Anpassa sidor i Dynamics Windows-klienten
description: "Lär dig mer om att anpassa användargränssnittet så att det passar ditt sätt att arbeta."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: e22f3464c6a4dd917880ad0b903880fe5f57a37d
ms.contentlocale: sv-se
ms.lasthandoff: 10/23/2017

---
# <a name="personalizing-your-workspace-in-the-dynamics-windows-client"></a>Anpassa din arbetsyta i Dynamics Windows-klienten
Du kan anpassa arbetsytan för att passa ditt arbete och dina inställningar genom att ändra sidor så att de endast visar den information som du behöver när du behöver den. De anpassningar som du gör kommer bara att påverka bara vad som visas, inte vad andra användare ser. Du kan anpassa många delar i användargränssnittet (UI), till exempel åtgärder som ska tas med på menyfliken, hur fält placeras på snabbflikarna eller i faktaboxar och vilka menyobjekt som ska ingå i navigeringsrutan.

> [!NOTE]  
> Du kan också anpassa sidor med [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Information om hur anpassning fungerar mellan två klienter finns i [översikt över anpassning ](ui-personalization-overview.md).

## <a name="how-to-personalize-your-workspace"></a>Hur du anpassar arbetsytan
Du kan utföra det mesta anpassningsarbeten med funktionen **anpassa** som du når från praktiskt taget alla typer av sidor genom att göra följande:

1.  Öppna sidan du vill anpassa.
2.  Längst upp till vänster, välj menyn **Program** ikonen ![Menyknappen Program i menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa** och välj sedan en av anpassningsalternativen.

Det finns vissa grundläggande ändringar i användargränssnittet, till exempel justera storleken på ett fönster eller expandera kolumner som du behöver direkt på sidan utanför alternativet **anpassa**.

## <a name="general-information"></a>Allmän information
Vid anpassning av användargränssnittet är det bra att komma ihåg följande punkter:

-   Du kan registrera flera anpassningar på samma sida baserat på olika åtkomstpunkter till sidan. Till exempel kan fönstret Försäljningsorder anpassas för att se olika ut när det öppnas från fönstret Kundkort än när det öppnas från Rollcenter Försäljningsorderhandläggare. Den punkt varifrån du öppnar sidan som ska anpassas registreras i den specifika sidanpassningen. Det kan alltså uppstå flera sidanpassningsposter i databasen, som du ser i fönstret **Ta bort användaranpassning**.

-   Programmet kan vara konfigurerat för att visa och dölja element i användargränssnittet (till exempel fälten FatTabs och FactBoxes) baserat på din licens eller behörigheter. Du kan bara visa och anpassa elementfält som du har behörighet till.

## <a name="customize-ribbons"></a>Anpassa menyflikar
Menyfliksområdet ger dig tillgång till flera åtgärder. Genom att anpassa menyfliken kan du optimera din för att förenkla arbetsprocesser och preferenser. Till exempel, om du vanligtvis använder fönstret **Dimensioner** kan du lägga till åtgärden **Dimensioner** till åtgärdsgruppen **Process**. Du kan också ta bort åtgärder som du aldrig använder för bättre översikt.  

Du kan utföra följande uppgifter för att anpassa menyflikar på sidor:  

-   Lägga till, byta namn på eller ta bort flikar, grupper, åtgärder och menyer.  
-   Ändra ordning på åtgärder.  
-   Återställa menyfliken till dess standardinställning.  

### <a name="to-customize-a-ribbon"></a>Så här anpassar du en menyflik
1. Öppna sidan du vill ändra.
2. Längst upp till vänster väljer du menyn **Program** ikonen ![knappen programmeny på menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa**, och sedan **Anpassa menyflik**.

Dialogrutan **ordna åtgärder på menyfliken** är uppdelad i två delar. Fönstret **tillgängliga åtgärder** visar alla de åtgärder som du lägger till på sidan. Fönstret **Visa åtgärder i den här ordningen** visar strukturen för alla åtgärder som visas på sidan.

-   Rotnivåartiklar definierar flikar.

    -   Artiklar på andra nivån definierar en grupp i en flik.

        -   Artiklar på tredje nivån definierar en meny med åtgärder i en grupp

### <a name="add-a-group"></a>Lägg till grupp
Klicka på fliken som du vill att grupp ska tillhöra och markera **Skapa grupp**. Du kan inte lägga till en grupp under en meny.

### <a name="add-a-menu"></a>Lägg till en meny
Välj gruppen som du vill att menyn ska tillhöra och markera **Skapa meny**. Du kan bara lägga till en meny till en grupp eller en annan meny.

#### <a name="add-an-action"></a>Lägg till åtgärd
Markerar den i fönstret **tillgängliga åtgärder** väljer du **Lägg till** till i rutan **Visa åtgärder i den här ordningen** och använd knapparna **Flytta upp** och **Flytta ned** för att placera den där du vill ha den.

Du kan inte lägga till en åtgärd till en flike, endast till en grupp eller en meny.

###  <a name="limitations-and-recommendations"></a>Begränsningar och rekommendationer
Observera följande begränsningar när du anpassar menyfliken:  

-   Systemflikar eller grupper till exempel **Hem** eller **Nytt** kan inte flyttas eller bytas namn på. Positionen för alla grupper, till exempel **Nytt dokument** är fasta.  
-   Åtgärder eller grupper, som har dynamisk synlighet kan inte läggas till eller tas bort.
-   Du kan endast skapa menyer inuti grupper, inte inuti flikar.  
-   Du kan kapsla en meny inom en annan meny, men det rekommenderas inte.  
-   Om du ser oväntat beteende med grupper och åtgärder efter att du har anpassat menyfliken, göra följande:  

    1.  Tom men ta inte bort gruppen där det inträffar problem.  
    2.  Stäng dialogen med hjälp av **OK** knappen.  
    3.  Öppna dialogen igen och lägg på nytt till åtgärder i gruppen.  

> [!IMPORTANT]  
>  Alla anpassningar som ändrar menyfliken kan påverka vägledningen som tillhandahålls i [!INCLUDE[navnow_md](includes/navnow_md.md)]-hjälpen, eftersom navigeringsstegen i hjälpen kan referera till en annan menyflikslayout.

## <a name="customize-fasttabs"></a>Anpassa Snabbflikar
Snabbflikar hjälper dig att ordna information om sidor i enkla hanterbara grupper. Du kan anpassa snabbflikar på sidor så att de stöder arbetsflödet. Du kanske vill visa färre snabbflikar eller dölja särskilda fält på snabbflikar. Du kan också göra så att viktiga fält tas med i snabbflikshuvudet när snabbfliken reduceras.  

### <a name="to-customize-a-fasttab"></a>Så här anpassar du en snabbflik:  

1.  Öppna sidan du vill ändra.
2.  Välj menyn **Program**, ikonen ![knappen programmeny på menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa**, och sedan **Anpassa denna sida**.  
3.  I dialogrutan **Anpassa <Page Name>** väljer du **Snabbflikar**.  

### <a name="add-move-or-remove-fasttabs"></a>Lägg till eller ta bort snabbflikar.
Rutan **Visa snabbflikar i den här ordningen** innehåller snabbflikar som redan finns på sidan och den ordning som de visas i. Använd knapparna **Lägg till**, **Ta bort**, **Flytta upp** och **Flytta ned** om du vill ändra.

### <a name="show-and-hide-fields-on-fasttabs"></a>Visa och göm fält på snabbflikar
Markera den snabbflik du vill ändra i rutan **Visa snabbflikar i den här ordningen** och välj sedan **Anpassa snabbflik**. Använd knapparna för att anpassa de fält som du vill visa och deras ordning på sidan.

Ange **vikt** på följande sätt:
-   Om du vill visa fältet i snabbflikens huvud när snabbfliken reduceras anger du **Upphöjd**.
- Om du vill att fältet ska vara dolt om inte användaren väljer åtgärden **visa fler fält** på snabbfliken, anger du **ytterligare**.
-   **Standard** är standard eller normal inställning.

### <a name="set-up-field-for-quick-entry"></a>Ställ in fält för Snabbinmatning
Markera kryssrutan **Snabbinmatning** om du vill lägga till fältet i fältlistan Snabbinmatning. När du arbetar på en sida och trycker på RETUR i ett fält, flyttas pekaren till nästa fält som ska vara ett fält för Snabbinmatning.

## <a name="customize-factboxes"></a>Anpassa faktaboxar
I faktaboxar visas information som hör till den post du har markerat i listan eller öppnat på en uppgiftssida. Från en lista kan du välja vilka faktaboxar du vill visa i rutan Faktabox. Du kan även anpassa faktaboxar så att de bara visar de fält som du behöver.  

### <a name="to-show-or-hide-the-factbox-pane"></a>Visa eller dölj rutan Faktabox
Faktaboxar finns i faktaboxrutan som du kan visa eller dölja på en sida. Detta gör det möjligt att enkelt dölja flera faktaboxar utan att ta bort dem individuellt.

1.  Öppna sidan du vill ändra.
2.  Välj menyn **Program**, ikonen ![knappen programmeny på menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa**, och sedan **Faktaboxar**. En markering i kryssrutan indikerar att faktaboxrutan visas.  

### <a name="to-customize-the-factbox-pane"></a>Så här anpassar du faktaboxrutan  
1.  Öppna sidan du vill ändra.
2.  Välj menyn **Program**, ikonen ![knappen programmeny på menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa**, och sedan **Faktaboxar**.  

### <a name="add-a-factbox"></a>Lägga till en faktabox  

Välj den faktabox som du vill lägga till i faktaboxrutan i **Tillgängliga faktaboxar** och välj sedan knappen **Lägg till**.  

### <a name="remove-a-factbox"></a>Ta bort en faktabox  

I rutan **Visa faktaboxar i den här ordningen**, välj sedan knappen **Ta bort**.   

### <a name="change-the-order-of-the-factboxes"></a>Ändra ordning på faktaboxarna  

I rutan **Visa faktaboxar i den här ordningen** väljer du den faktabox du vill flytta och väljer sedan **Flytta upp** eller **Flytta ned**. Upprepa den här proceduren tills du har placerat faktaboxen rätt.  

### <a name="change-the-fields-in-a-factbox"></a>Ändra fält i en faktabox  

1.  I rutan **Visa faktaboxar i den här ordningen**, väljer du Faktabox och sedan **Anpassa del**.  

2.   Rutan **Tillgängliga fält** visar alla fält som du kan välja mellan. Rutan **Visade fält** visar alla fälten som visas i faktaboxen. Använd knapparna för att lägga till, ta bort och flytta fält.   


## <a name="customize-columns-in-a-list-or-on-document-lines"></a>Anpassa kolumner i en lista eller på dokumentrader
För att få en bättre översikt över den information som du behöver kan du anpassa listsidor och kortsidor genom att lägga till eller ta bort kolumner i rutnäten, flytta kolumner och lägga till en låsning.  

### <a name="to-add-remove-and-arrange-columns"></a>Om du vill lägga till, ta bort och ordna kolumner  

1.  Du kan lägga till, ta bort eller ordna om kolumner på två sätt:

    -   Välj menyn **Program**, ikonen ![knappen programmeny på menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa**, och sedan **Välj kolumner**.
    -   Högerklicka på en kolumnrubrik och klicka sedan på **Välj kolumner**.

2.  I dialogrutan **Välj vilka kolumner som ska visas i listan** i rutan **Tillgängliga kolumner** finns dolda kolumner. Rutan **Visa kolumner i den här ordningen** innehåller kolumnerna som visas. Du flyttar kolumnerna mellan fälten med hjälp av knapparna **Lägg till** och **Ta bort**. Med knapparna **Flytta upp** och **Flytta ned** placerar du kolumnerna där du vill ha dem.

>[!TIP]
>Markera kryssrutan **Snabbinmatning** om du vill lägga till fältet i fältlistan Snabbinmatning. När du arbetar på en sida och trycker på RETUR i ett fält, flyttas pekaren till nästa fält som ska vara ett fält för Snabbinmatning.

### <a name="to-set-the-freeze-pane"></a>Ange låsning
En lista kan ha flera kolumner som kan tvinga dig att bläddra vågrätt för att se alla kolumner. Det kan finnas vissa kolumner som du alltid vill visa även när du bläddrar. För att uppnå detta måste du lägga till en lodrät låsning så att en del kolumner inte bläddras. På så sätt kan du se till att mindre viktiga kolumner flyttas när du bläddrar.

För att ange låsningen markerar du kolumnen som du vill att låsningen ska starta efter och väljer **Lägg till låsning**.

## <a name="customizing-the-navigation-pane"></a>Anpassa navigeringsrutan
I navigeringsrutan visas en meny med länkar till olika listsidor. Länkarna är grupperade under knappar på rotnivå.

### <a name="to-customize-the-navigation-pane"></a>Så här anpassar du navigeringsrutan  

Välj menyn **Program**, ikonen ![knappen programmeny på menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa**, och sedan **Anpassa navigeringsrutan**.  

### <a name="rename-or-rearrange-buttons-in-the-navigation-pane"></a>Byta namn på eller flytta knappar i navigeringsrutan  
Markera knappen som du vill flytta, byta namn på eller ta bort i den vänstra rutan i dialogrutan **Anpassa navigeringsruta**. Välj sedan relevant knapp i mitten av fönstret.

Du kan inte ta flytta, byta namn på eller ta bort knappen **Start**. Knappen **Avdelningar** kan tas bort från navigeringsrutan, men inte bytas namn på eller flyttats.

### <a name="add-a-new-menu-button"></a>Lägga till en ny menyknapp
Du kan skapa en ny knapp på rotnivå och sedan lägga till en meny med länkar under knappen för att öppna olika sidor.

1. Välj **Ny** i dialogrutan **Anpassa navigeringsruta** och skriv ett namn i fältet **Namn**.
2.  Välj knappen **OK**.

Du kan lägga till länkar på knappen.  

### <a name="add-a-link-to-a-button"></a>Lägga till en länk på en knapp   
Om du har behörighet att visa en lista, till exempel en försäljningsorderlista, kan du lägga till en länk till listan från en knapp i navigeringsrutan.  

1.  Markera menyn som du vill lägga till länken på i fältet **Knappar för navigeringsruta** i dialogrutan **Anpassa navigeringsruta**.  

2.  Välj knappen **Lägg till**.  

3.  Bläddra till de länk som du vill lägga till och klicka sedan på **OK**.  
> [!TIP]
> Om länken finns på **Avdelningar**-sidorna kan du också lägga till den i navigeringsrutan. Mer information finns i avsnittet Lägga till en länk från Avdelningar i ditt rollcenter  

### <a name="move-or-copy-a-link-from-one-button-to-another"></a>Flytta eller kopiera en länk från en knapp till en annan  

1.  Markera menyn där länken finns i fältet **Knappar för navigeringsruta** i dialogrutan **Anpassa navigeringsruta**.  

2.  Markera länken som du vill flytta i rutan **Listor** och klicka sedan på **Flytta till** eller **Kopiera till**  

3.  Markera den navigeringsmeny som du vill lägga till länken på och klicka sedan på **OK**.  

### <a name="rearrange-the-order-of-a-links-under-a-button"></a>Ändra ordning på länkar under en knapp  

1.  Markera länken som du vill flytta i rutan **Listor**.  

2.  Med knapparna **Flytta upp** och **Flytta ned** placerar du länkarna där du vill ha dem.

## <a name="adding-department-links-to-the-role-center"></a>Lägga till avdelningslänkar till rollcentret
Ibland kan du hitta en länk på sidan **avdelningar** som du vill lägga till i ditt rollcenter för enkel åtkomst. Där du kan placera länken i rollcentret beror länkens kategori på sidan **avdelningar**.

I tabellen nedan beskrivs de olika typerna av länkar som finns i respektive kategori på sidan **Avdelningar**, och var i rollcentret som du kan lägga till dem.  

|**Kategori**|**Innehåller**|**Lägg till länk på**|  
|------------------|------------------|---------------------|  
|Listor|Listsidor|Knappen **Start** i navigeringsrutan|  
|Uppgifter|Uppgiftssidor, batch-jobb, förslag, journaler|Fliken **Åtgärder** på menyfliken|  
|Rapporter och analyser|Rapporter, batch-jobb, matrisfönster|Fliken **Rapporter** på menyfliken|  
|Dokument |Dokument som fakturor och betalningspåminnelser|**Rapporter** på menyfliken|  
|Arkiv/historik|Bokförda/slutförda dokument, register|Knappen **Start** i navigeringsrutan|  
|Administration|Inställningsfönster|Fliken **Åtgärder** på menyfliken|  

### <a name="to-copy-department-links-to-your-role-center"></a>Så här kopierar du avdelningslänkar till ditt rollcenter:  

1.  Öppna sidan **Avdelningar**.  

2.  Högerklicka på länken och klicka sedan på något av följande (enbart ett av dessa alternativ är tillgängligt).  

    |**Välj**|**Om du vill lägga till länken på**|  
    |----------------|----------------------------|  
    |**Lägg till i navigeringsruta**|Knappen **Start** i navigeringsrutan i Rollcentret.|  
    |**Lägg till åtgärder i menyfliksområdet Rollcenter**|**Åtgärder**-menyn på menyfliken i rollcentret.|  
    |**Lägg till i rapporter på menyfliken Rollcenter**|**Rapporter**-menyn på menyfliken i rollcentret.|  

3.  Bekräfta meddelandet som visas.  

 Den nya länken visas nu på menyn där du har lagt till den. Du kanske emellertid vill flytta länken till en annan plats på menyn. Om du till exempel har lagt till en länk i navigeringsrutan, visas den på **Startsida**-menyn, men du kan flytta den till en annan meny i navigeringsrutan. Mer information finns i avsnittet Anpassa navigeringsrutan.

## <a name="adding-charts-to-role-centers-and-list-pages"></a>Lägga till diagram i rollcentret och listsidor
När du har komplex information, kan det hända att du vill visa en visuell representation av data för att lättare kunna se trender och fatta beslut. Du kanske till exempel vill övervaka saldon per bankkonto för företaget i ett diagram. Du kan använda diagramrutan för att visuellt visa data från en lista på följande typer av sidor:  

-   I rollcentret där du kan välja mellan många olika fördefinierad generiska diagram.  

-   På en listsida, där du kan välja om du vill visa en lista som ett diagram.  

### <a name="to-add-a-generic-chart-to-your-role-center"></a>Så här lägger du till ett generiskt diagram i rollcentret  

1.  I ditt rollcenter, välj menyn **Program**, ikonen ![knappen programmeny på menyfältet](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa**, och sedan **Anpassa denna sida**.  

2.  Välj **Diagramdel** i fältet **Tillgängliga delar** i fönstret **Anpassa Rollcenter** och klicka på **Lägg till**.  

3.  Flytta diagramdelen i ditt rollcenter med knapparna **Flytta upp**, **Flytta ned**, **Flytta vänster** och **Flytta höger**.  

4.  Markera diagramdelen, välj **Anpassa del**.  

5.  Markera det fördefinierade diagram som du vill visa i fönstret **Anpassa diagram** och klicka på **OK**.  

### <a name="to-view-a-list-as-a-chart"></a>Så här visar du en lista som en karta  

1.  På listsidan, välj åtgärden **Visa som diagram**.  

2.  Välj en enhet och en dimension som används för att skapa ett anpassat diagram. Välj en sekundär dimension för att visa ytterligare information. Du kan t.ex. skapa ett enkelt stapeldiagram genom att välja en dimension på X-axeln sedan välja dimensionen **Dimensionsantal** på Y-axeln.  

> [!NOTE]  
>  Diagramrutan är som standard dold eftersom den kan påverka prestandan negativt. Du bör endast visa diagrammet, när du måste ha informationen.  

## <a name="handling-external-files-and-automation-objects"></a>Hanterar externa filer och automatiseringsobjekt
När [!INCLUDE[navnow_md](includes/navnow_md.md)] tar emot en extern fil visas en dialogruta. Förutom att välja vad som ska ske med filen kan du bestämma hur du hanterar filtypen nästa gång som den tas emot.  

När [!INCLUDE[navnow_md](includes/navnow_md.md)] måste köra ett automationsobjekt visas en dialogruta. Du kan välja om du vill att typen av objekt alltid ska eller aldrig ska kunna köras.  

### <a name="to-specify-how-to-handle-external-files"></a>Så här anger du hur externa filer ska hanteras  

1.  När dialogrutan visas avmarkerar du kryssrutan **fråga alltid innan den här filtypen öppnas** om du vill att [!INCLUDE[navnow_md](includes/navnow_md.md)] ska komma ihåg vilket alternativ du väljer i steg 2. Nästa gång filtypen måste hanteras visas inte dialogrutan och filen behandlas som anges i steg 2.  

     Markera kryssrutan **Fråga alltid innan den här filtypen öppnas** för att dialogrutan alltid ska visas när den här filtypen tas emot.  

2.  Välj **Öppna**, **Spara** eller **Avbryt**. Filen hanteras enligt ditt val.  

### <a name="to-specify-how-to-handle-automation-objects"></a>Så här anger du hur automationsobjekt ska hanteras  

När dialogrutan visas markerar du kryssrutan **Tillåt alltid** om du vill att [!INCLUDE[navnow_md](includes/navnow_md.md)] alltid ska köra den typen av automationsobjekt. Nästa gång den typen av automationsobjekt behöver köras kommer dialogrutan inte visas, och automationsobjektet körs direkt.  

Du kan också markera kryssrutan **Tillåt aldrig**. Nästa gång den typen av automationsobjekt behöver köras kommer dialogrutan inte visas, och automationsobjektet körs inte.  

## <a name="CancelPersonalization"></a>Avbryta anpassning
Avbryta anpassning kan delas in i två kategorier:

-   Avbryta ändringar som du gjort med hjälp av funktionen **Anpassa**.
-   Avbryta grundläggande användargränssnittändringar.

### <a name="cancel-customization"></a>Avbryta anpassning
Om du vill annullera all anpassning av användargränssnittet som du har gjort någonsin för en sida under din aktuella användarinloggning, eller sedan du senast annullerad **Ta bort användaranpassning**. Layouten på sidan som du tar bort dina anpassningar för återställs då till standardkonfigurationen för din profilen.  

Om du bara vill annullera anpassning av användargränssnittet som du har gjort på ett specifikt användargränssnittsområde på en sida, till exempel menyfliken, kan du använda knappen **Återställ standardvärden** i fönstret **Anpassa**. Layouten för det specifika användargränssnittsområdet på sidan återställs då till standardkonfigurationen för din profil.  

#### <a name="to-cancel-all-ui-customization-that-you-have-made-to-a-page"></a>Så här annullerar du alla användargränssnittsanpassningar som du har gjort för en sida  

1.  I rutan **Sök**, anger du **Ta bort användaranpassning** och väljer sedan relaterad länk.  

2.  Välj sidan som du vill annullera din anpassning av användargränssnittet för, och sedan, på fliken **Hem** i gruppen **Visa** väljer du **Ta bort**.  

> [!NOTE]  
>  All anpassning av sidans användargränssnitt som du någonsin har gjort under din aktuella användarinloggning eller sedan du senast använde fönstret **Ta bort användaranpassning** avbryts. Layouten på sidan nollställs till standardkonfigurationen för din profil, som den konfigurerats av administratören eller som den installerats med [!INCLUDE[navnow](includes/navnow_md.md)].  

#### <a name="to-cancel-ui-customization-that-you-have-made-to-a-ui-area-on-a-page"></a>Så här annullerar du användargränssnittsanpassningar som du har gjort för ett gränssnittsområde på en sida  

1.  Från sidan där du har anpassat ett användargränssnittsområde på menyfliken, välj menyn **Koppling**, ![Knappen kopplingsmeny på menyfliken](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa** och sedan **Anpassa <UI area>**.  

2.  Välj knappen **Återställ standardvärden** längst ned i fönstret **Anpassa**.  

> [!NOTE]  
>  Alla anpassning av användargränssnittsområdet som du någonsin har gjort för sidan under din aktuella användarinloggning eller sedan du senast använde knappen **Återställ standardvärden** avbryts. Layouten i gränssnittsområdet på sidan nollställs till standardkonfigurationen för din profil, som den konfigurerats av administratören eller som den installerats med [!INCLUDE[navnow](includes/navnow_md.md)].

### <a name="cancel-basic-ui-changes"></a>Avbryta grundläggande användargränssnittändringar.
Du kan annullera de grundläggande användargränssnittsändringarna genom att öppna fönstret **Återställ inställningar som angetts av användaren** från ditt Rollcenter.  

Grundläggande användargränssnittändringarna är bland annat:
 -  Ändra storlek och placering i ett fönster.
 -  Ändra bredd på kolumner
 -  Ändra höjden på kolumnrubriker.
 -  Sortera kolumner i listan.
 -  Visa listor som diagram.
 -  Ange hur externa filer och automationsobjekt ska hanteras  

#### <a name="to-cancel-basic-ui-changes"></a>Så här avbryter du grundläggande användargränssnittändringar.

1.  Gå till ditt Rollcenter.  

     På menyn **Koppling**, ![Knappen Kopplingsmeny på menyfliken](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa** och sedan **Återställ inställningar som angetts av användaren**.  

2.  Välj knappen **Återställ gränssnittsinställningar**. Välj knappen **Återställ alla** för att även avbryta dina beslut för hantering av filer och automatiseringsobjekt.  

 Alla grundläggande UI-ändringar som du någonsin har gjort under ditt aktuella användarinloggning till [!INCLUDE[navnow_md](includes/navnow_md.md)], eller sedan du senast valde knappen **Återställ gränssnittsinställningar** avbryts. Användargränssnittet återställs till standardkonfigurationen för din profil.  

#### <a name="to-cancel-your-decision-for-running-or-saving-external-files"></a>Så här annullerar du beslutet för att köra eller spara externa filer  

1.  Gå till ditt Rollcenter.  

     På menyn **Koppling**, ![Knappen Kopplingsmeny på menyfliken](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa** och sedan **Återställ inställningar som angetts av användaren**.  

2.  Välj knappen **Återställ filhanteringsbeslut**. Välj knappen **Återställ alla** för att även avbryta dina vyändringar och beslut för hantering av automatiseringsobjekt.  

 Alla beslut för standardhantering av filtyper som du någonsin har gjort under din aktuella användarinloggning, eller sedan du senast valde knappen **Åtkomst till klientfil**, avbryts och återställs till standardkonfigurationen för din profil. Nästa gång [!INCLUDE[navnow_md](includes/navnow_md.md)] tar emot en extern fil av någon typ visas en dialogruta med alternativen **spara**, **kör**, och **avbryt**  

### <a name="to-cancel-your-decision-for-handling-automation-objects"></a>Så här annullerar du beslutet för hantering av automationsobjekt  

1.  Gå till ditt Rollcenter.  

     På menyn **Koppling**, ![Knappen Kopplingsmeny på menyfliken](media/applicationmenuicon.png "ApplicationMenuIcon"), välj **Anpassa** och sedan **Återställ inställningar som angetts av användaren**.  

2.  Välj knappen **Återställ automatiseringsbeslut**. Välj knappen **Återställ alla** för att även avbryta dina vyändringar och beslut för att köra eller spara externa filer.  

 Alla beslut om hur automatiseringsobjekt ska köras som du någonsin har tagit under din aktuella användarinloggning eller sedan du senast valde knappen **Återställ automatiseringsbeslut** avbryts. Filhanteringsbeteendet återställs till standardkonfigurationen för din profil. Nästa gång [!INCLUDE[navnow_md](includes/navnow_md.md)] måste köra ett automationsobjekt av någon typ visas en dialogrutan med alternative **Tillåt alltid** och **Tillåt aldrig**.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## <a name="see-also"></a>Se även
[Anpassa din arbetsyta i Dynamics webbklienten](ui-personalization-user.md)  
[Anpassning, översikt](ui-personalization-overview.md)  

