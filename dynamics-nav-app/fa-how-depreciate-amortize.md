---
title: "Så här skriver du av eller amorterar anläggningstillgångar"
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
ms.openlocfilehash: af71f30681d436ed5da1cd6cb3c2e13f86558631
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-depreciate-or-amortize-fixed-assets"></a>Så här skriver du av eller amorterar anläggningstillgångar
Avskrivning används för att fördela kostnaden för anläggningstillgångar, som exempelvis maskiner och inventarier, över den avskrivningsbara livslängden. För varje anläggningstillgång måste du ange hur den ska avskrivas.  

 Du kan bokföra avskrivning på två sätt:
- Automatiskt genom att köra batch-jobbet **Beräkna avskrivning**.
- Manuellt genom att använda fältet anl.tillg. redovisningsjournal.  

Dynamics NAV kan beräkna daglig avskrivning, vilket innebär att du kan beräkna avskrivning för vilken period som helst. Du kan därmed analysera aktuella operativa resultat på exempelvis månads-, kvartals- eller årsbasis. Beräkningen används ett standardår på 360 dagar och en standardmånad på 30 dagar. Mer information finns i [Avskrivningsmetoder](fa-depreciation-methods.md).

Om en anläggningstillgång används av flera avdelningar kan periodisk avskrivning automatiskt fördelas på avdelningarna utifrån en användardefinierad fördelningstabell.  

Du kan rätta felaktiga avskrivningstransaktioner med hjälp av batch-jobbet **Rätta anl.transaktioner**. Därefter kan du bokföra det korrekta beloppet för avskrivningen genom att på nytt köra batch-jobbet **Beräkna avskrivning**. När du korrigerar fel bokförs de som felaktiga transaktioner för anläggningstillgångar.  

Indexering används för att anpassa värden till den allmänna prisnivån. Du kan använda batch-jobbet **Indexera anläggningstillgångar** om du vill omberäkna avskrivningsbeloppen.  

## <a name="to-calculate-a-depreciation-automatically"></a>Så här beräknar du avskrivning automatiskt
En gång i månaden, eller när du vill, kan du köra batch-jobbet **Beräkna avskrivning**. Anläggningstillgångar som har sålts, tillgångar som är spärrade eller inaktiverade och de anläggningstillgångar som använder den manuella avskrivningsmetoden används ignoreras.    

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Beräkna avskrivning** och välj sedan relaterad länk.  
2. Fyll i fälten om det behövs. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.
3. Välj **OK**.  

    Batch-jobbet beräknar nedskrivningen och skapar rader i redovisningsjournalen för anläggningstillgångar.  
4. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournaler för anl.tillg.** och välj sedan relaterad länk.

    I fönstret **Anl.tillg. redovisningsjournal** i fältet **Antal avskrivningsdagar** kan du se hur många avskrivningsdagar som har beräknats.  
5. Välj åtgärden **Bokföra**.

## <a name="to-post-a-depreciation-manually-from-the-fixed-asset-gl-journal"></a>Att bokföra en avskrivning manuellt från en redovisningsjournalen för anläggningstillgångar.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl.tillg. redovisningsjournal** och välj sedan relaterad länk.  
2. Skapa en första journalrad och fyll i fälten efter behov.
3. Välj **Anskaffningskostnad** i fältet **Avskrivning**.
4. Välj åtgärden **Infoga anl. motkonto**. En andra journalrad skapas för motkontot som ställs in för bokföring av avskrivning. För mer information, se avsnittet "Att ställa in bokföringsmallar för anläggningstillgångar" i [Så här ställer du in allmän information för anläggningstillgångar](fa-how-setup-general.md).
5. På fliken **Start** väljer du **Bokför**.

Om du har skapat fördelningsnycklar för anläggningstillgångar, som fördelar belopp på olika avdelningar eller projekt, kan beloppen fördelas under bokföring. Mer information finns i [Så här ställer du in allmän information för anläggningstillgångar](fa-how-setup-general.md).

## <a name="to-calculate-allocations-in-the-fixed-asset-gl-journal"></a>Så här beräknar du fördelningar i redovisningsjournaler för anläggningstillgångar
Om en anläggningstillgång används av flera avdelningar kan periodisk avskrivning automatiskt fördelas på avdelningarna utifrån en användardefinierad fördelningstabell.  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl.tillg. redovisningsjournal** och välj sedan relaterad länk.   
Skapa en första rad och fyll i fälten efter behov.
3. Välj **Anskaffningskostnad** i fältet **Fördelning**.
4. Välj åtgärden **Infoga anl. motkonto**. En andra journalrad skapas för motkontot som ställs in för bokföring av fördelning.
5. På fliken **Start** väljer du **Bokför**.

## <a name="use-duplication-lists-to-prepare-to-post-to-multiple-depreciation-books"></a>Använd dubblettlistor för att förbereda att bokföra åtskilliga avskrivningsregler  
När du fyller i journalrader som ska bokföras enligt en avskrivningsregel kan du kopiera raderna till en separat journal och bokföra dem enligt en annan avskrivningsregel. För mer information, se avsnittet "Så här bokför du transaktioner enligt olika avskrivningsregler".

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Avskrivningsregler** och välj sedan relaterad länk.  
2. Öppna relevant avskrivningsregel och markera sedan kryssrutan **Ingår i dubblettlista**.  

**Viktigt!**: Om du har markerat fältet **Använd dubblettlista** ska du inte använda nummerserien för journalen. Anledningen är att nummerserien för redovisningsjournalen för anläggningstillgångar gör inte nummerserien för anläggningstillgångsjournalen.

## <a name="to-post-entries-to-different-depreciation-books"></a>Så här bokför du transaktioner enligt olika avskrivningsregler  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl.tillg. redovisningsjournal** och välj sedan relaterad länk.
2. I journalen som du vill bokföra avskrivning med markerar du kryssrutan **Använd dubblettlista**.
3. Fyll i återstående fält om det behövs.
4. Välj åtgärden **Bokföra**.
5. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anl.journaler** och välj sedan relaterad länk.

    Fönstret **Anlägg.tillg.journal** innehåller nya rader för olika avskrivningsregler enligt dublettlistan.   

6. Granska och redigera raderna och välj sedan åtgärden **bokför**.

**Obs!**: Ett alternativt sätt att kopiera en transaktion enligt en annan regel är att ange en avskrivningsregelkod i fältet **Dubblett i avskrivningsregel** när du fyller i en journalrad.

Du kan kopiera transaktioner från en avskrivningsregel till en annan med hjälp av batch-jobbet **Kopiera avskrivningsregel**. Batch-jobbet skapar journalrader i den journal som du har angett i fönstret **Anl. journalinställningar** för den avskrivningsregel som du vill kopiera till. Mer information finns i följande procedur:

## <a name="to-copy-fixed-asset-ledger-entries-between-depreciation-books"></a>Om du vill kopiera anläggningstillgångstransaktioner mellan avskrivningsregler  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Avskrivningsregler** och välj sedan relaterad länk.
2. Öppna relevant avskrivningsregelkort och välj sedan åtgärden **Kopiera avskrivningsregel**.  
3. I fönstret **Kopiera avskrivningsregelkort** fyller du i fälten efter behov.  
4. Välj **OK**.  

De kopierade raderna skapas antingen i redovisningsjournalen för anläggningstillgångar eller i anläggningstillgångsjournalen, beroende på om avskrivningsregeln som du kopierar har integrering med redovisningen.

## <a name="see-also"></a>Se även
[Hantera anläggningstillgångar](fa-manage.md)  
[Skapa anläggningstillgångar](fa-setup.md)  
[Finans](finance-setup.md)  
[Välkommen till Dynamics NAV](across-get-started.md)

