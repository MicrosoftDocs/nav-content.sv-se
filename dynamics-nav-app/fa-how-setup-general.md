---
title: "Så här skapr du allmän information för anläggningstillgångar"
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
ms.openlocfilehash: 8c0e33a78d47ccfbe39a78f81e31b69f61fd4f80
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-general-fixed-assets-information"></a>Så här skapr du allmän information för anläggningstillgångar
Innan du kan hantera anläggningstillgångar, måste du skapa standardinställningredovisningskonton, fördelningsnycklar, journalmallar och journaler för bokföring och gruppering av anläggningstillgångar i klasser, som till exempel Materiella och Immateriella.

## <a name="to-set-up-general-default-values-for-fixed-assets"></a>Så här anger du generella standardvärden för anläggningstillgångar
Du definierar det allmänna beteendet eller funktionen för anläggningstillgångarna och ställer in verifikationsnummerserie i fönstret **Inställningar för anläggningstillgångar**.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Inställningar för anläggningstillgångar** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

## <a name="to-set-up-fixed-asset-posting-groups"></a>Så här skapar du bokföringsmallar för anläggningstillgångar  
Du kan använda bokföringsmallar om du vill definiera anläggningstillgångsgrupper. Transaktionerna för de här bokföringsmallarna bokförs på samma redovisningskonton.  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. bokföringsmall** och välj sedan relaterad länk.  
2. Välj åtgärden **Ny**.
3. I fönstret **Anl. bokföringsmallkort** fyller du i fälten efter behov.

    **Obs!**: För att se till att motkonton för olika anläggningstillgångar infogas bokföringar automatiskt när du väljer åtgärden **Infoga anl. motkonto** på journalrader, följer nästa steget som baseras på bokföring av uppskrivning.
4. På snabbfliken **Motkonto** i fältet **Uppskrivning motkonto** anger du vilket redovisningskonto som du vill bokföra mottransaktioner för uppskrivning.

Mer information om hur du använder åtgärden **Infoga anl. motkonto** påanl.tillg. redovisningsjournal, se t.ex. [Så här omvärderar du anläggningstillgångar](fa-how-revalue.md).

## <a name="to-set-up-fixed-asset-allocation-keys"></a>Så här ställer du in fördelningsnycklar för anläggningstillgångar  
Du kan fördela transaktioner på olika avdelningar eller projekt utifrån användardefinierade fördelningsnycklar. Du kan till exempel skapa en fördelningsnyckel om du vill fördela avskrivningskostnader för bilar med 35 % på administrationsavdelningen och 65 % på försäljningsavdelningen. För mer information, se [Så här använder fördelningsnycklar i redovisningsjournaler](ui-how-use-allocation-keys-general-journals.md).

Fördelningsnycklar används för fördelningar av anläggningstillgångar, inte för individuella tillgångar.  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. bokföringsmall** och välj sedan relaterad länk.  
2. I fönstret **Anl. bokföringsmallar** väljer du åtgärden **Fördelningar** och sedan en bokföringstyp.
3. I fönstret **Anl. fördelningar** fyller du i fälten efter behov.
4. Upprepa steg 2 och 3 för varje bokföringstyp som du vill ange fördelningsnycklar för.

## <a name="to-set-up-fixed-asset-journal-templates"></a>Så här skapar du journalmallar för anläggningstillgångar  
En mall är en fördefinierad layout för en journal. Mallen innehåller information om spårkoder, rapporter och nummerserier. (Mer information finns i [Arbeta medSkapa redovisningsjournaler](ui-work-general-journals.md).

Dynamics NAV skapar automatiskt en journalmall för anläggningstillgångar första gången du öppnar fönstret **Journalmall för anläggningstillgångar** men du kan skapa ytterligare journalmallar.  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. journalmallar** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs.

## <a name="to-set-up-fixed-asset-journal-batches"></a>Så här ställer du in journaler för anläggningstillgångar
Du kan skapa flera journaler, d.v.s. enskilda journaler för varje journalmall. Personalen kan till exempel ha egna journaler som har den anställdes initialer som journalnamn. Mer information finns i [Arbeta medSkapa redovisningsjournaler](ui-work-general-journals.md).  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. journalmallar** och välj sedan relaterad länk.  
2. Välj relevant försäkringsjournalmall och välj sedan åtgärden **Journaler**.
3. I fönstret **Anl.journaler** fyller du i fälten efter behov.

## <a name="to-set-up-fixed-asset-reclassification-journal-templates"></a>Så här ställer du in grupperingsmallar för anläggningstillgångar  
Du kan använda dedikerade grupperingsjournalen när du vill överföra, dela upp och slå ihop anläggningstillgångar. Dynamics NAV skapar Dynamics NAV en grupperingsjournalmall för anläggningstillgångar första gången som du öppnar fönstret **Anl. grupperingsjournal**, men du kan skapa ytterligare grupperingsjournalmallar för anläggningstillgångar. Mer information finns i [Arbeta medSkapa redovisningsjournaler](ui-work-general-journals.md).  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. grupperingsjournalmall** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs.

## <a name="to-set-up-fixed-asset-reclassification-journal-batches"></a>Så här skapar du grupperingsjournaler för anläggningstillgångar  
Du kan skapa flera journaler, d.v.s. enskilda journaler för varje grupperingsjournalmall. Personalen kan till exempel ha egna grupperingsjournaler som använder den anställdes inititaler som journalnamn. Mer information finns i [Arbeta medSkapa redovisningsjournaler](ui-work-general-journals.md).
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. grupperingsjournalmall** och välj sedan relaterad länk.  
2. Välj relevant försäkringsjournalmall och välj sedan åtgärden **Journaler**.
3. I fönstret **Anl. grupper.journaler** fyller du i fälten efter behov.

## <a name="to-set-up-fixed-asset-class-codes"></a>Så här skapar du indelningskoder för anläggningstillgångar:  
Indelningskoder för anläggningstillgångar kan användas för att gruppera anläggningstillgångar, t.ex. materiella och immateriella tillgångar.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. indelningar** och välj sedan relaterad länk.
2. Ange koder och namn för de indelningar som du vill skapa.

## <a name="to-set-up-fixed-asset-subclass-codes"></a>Så här skapar du underindelningskoder för anläggningstillgångar:
Du kan använda underindelningskoden för anläggningstillgångar om du vill gruppera dina tillgångar i kategorier, som exempelvis byggnader, fordon, möbler och maskiner.  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. underindelningar** och välj sedan relaterad länk.
2. Ange koder och namn för de indelningar som du vill skapa.

## <a name="to-set-up-fixed-asset-location-codes"></a>Så här skapar du lagerställekoder för anläggningstillgångar
Du kan använda lagerställekoder för anläggningstillgångar om du vill registrera var en anläggningstillgång är placerad, till exempel försäljningsavdelning, reception, administration, fabrik och lager. Den här informationen är användbar för försäkrings- och lagerändamål.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl. placeringar** och välj sedan relaterad länk.
2. Ange koder och namn för anläggningstillgångens lagerställe som du vill skapa.

## <a name="to-register-opening-entries"></a>Så här registrerar du ingående transaktioner  
Om det är första gången som du använder anläggningstillgångarna Dynamics NAV måste du först ange inställningar för redovisningsmodulen. Hur du genomför detta beror på om anläggningstillgångar är integrerad med redovisningen.  

 Du använder följande procedur om anläggningstillgångstransaktionerna ska bokföras i redovisningen.  

1. Kontrollera att du har avslutat den grundläggande inställningsprocessen för anläggningstillgångar.  
2. Skapa ett anläggningstillgångskort för de befintliga tillgångarna.  
3. Skapa avskrivningsregler för anläggningstillgångar.  
4. Aktivera redovisningintegration, genom att följa stegen.
5. I rutan **Sök**, ange **Avskrivningsregler** och välj sedan relaterad länk.  
6. Välj den relevanta avskrivningsregeln. Välj **Redigera** för att öppna fönstret **Avskrivningsregelkort** på fliken **Start** i gruppen **Hantera**.
7. Kontrollera att alla fält är ofyllda (ta bort markeringar) på snabbfliken **Integration**. Om du har fler än en avskrivningsregel ska du aktivera redovisningsintegrationen för alla reglerna.  
8. Ange följande rader för varje anläggningstillgång i anläggningsjournalen:
    - En rad med anskaffningskostnaden.
    - En rad med den ackumulerade avskrivningen till slutet på föregående räkenskapsår.
    - En rad med den ackumulerade avskrivningen från början av det innevarande räkenskapsåret till det datum då Dynamics NAV anges för att starta beräkningen av avskrivningen.

Om du har andra ingående saldon kan du även ange dessa nu, t.ex. nedskrivning\-uppskrivning.  

Om anläggningstillgången inte är integrerad med redovisningen hoppar du över steg 4 till 7.

## <a name="see-also"></a>Se även
[Skapa anläggningstillgångar](fa-setup.md)  
[Hantera anläggningstillgångar](fa-manage.md)  
[Finans](finance-setup.md)  
[Välkommen till Dynamics NAV](across-get-started.md)

