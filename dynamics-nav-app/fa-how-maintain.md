---
title: "Så här underhåller du anläggningstillgångar."
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
ms.openlocfilehash: 58077a38433a73b981a6f3d05ce7ed106acf32f4
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-maintain-fixed-assets"></a>Så här underhåller du anläggningstillgångar.
Underhållskostnaderna är rutinmässiga periodiska kostnader som utförs för att bevara värdet på en anläggningstillgång. Till skillnad från kapitalförbättringar ökar de inte värden.

Du kan registrera och underhålla en aktuell fil om underhåll och service av anläggningstillgångarna så att du enkelt har tillgång ett fullständiga underhållsregister för anläggningstillgångar. När en anläggningstillgång skickas på service noterar du all relevant information, som exempelvis servicedatum, leverantörsnummer och serviceföretagets telefonnummer. Underhållsregistrering registreras för varje anläggningstillgång från det aktuella anläggningstillgångskortet.

Indexering används för att anpassa värden till den allmänna prisnivån. Du kan använda batch-jobbet **Indexera anläggningstillgångar** om du vill omberäkna underhållskostnader.

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a>Om du vill registrera underhållsarbete på en anläggningstillgång  
Varje gång som underhåll har utförts, exempelvis ett servicebesök kan du registrera detta för den aktuella anläggningstillgången i fönstret  **Underhållsregistrering**.  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.  
2. Markera den anläggningstillgång som du vill registrera underhåll för och välj sedan åtgärden **Underhållsregistreringar**.
3. I fönstret **Underhållsregistreringar** fyller du i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a>Att bokföra underhållskostnader från en redovisningsjournalen för anläggningstillgångar.
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Avskrivningsregellista** och välj sedan relaterad länk.  
2. Markera den avskrivningsregel som är tilldelad anläggningstillgången och välj sedan åtgärden **Redigera**.
3. I fönstret **Avskrivningsregelkort** ser du till att kryssrutan **Underhåll** inte är markerad. Detta säkerställer att underhållskostnader inte bokförs till redovisningen.
4. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Redovisningsjournaler för anl.tillg.** och välj sedan relaterad länk.  
5. Skapa en första journalrad och fyll i fälten efter behov.
6. Välj **Anskaffningskostnad** i fältet **Underhåll**.
7. Välj åtgärden **Infoga anl. motkonto**. En andra journalrad skapas för motkontot som ställs in för bokföring av underhåll.

    **Obs**: Steg 7 fungerar bara om du har ställt in följande: I fönstret **Anl. bokföringsmallkort** för den fasta anläggningstillgångens bokföringsmall, innehåller fältet **Underhållskonto** redovisningsdebitkontot och fältet **Underhållskontosaldo** innehåller det redovisningskonto där du vill bokföra mottransaktioner för uppskrivning. För mer information, se avsnittet "Att ställa in bokföringsmallar för anläggningstillgångar" i [Så här ställer du in allmän information för anläggningstillgångar](fa-how-setup-general.md).
8. Välj åtgärden **Bokföra**.

## <a name="to-follow-up-on-fixed-assets-service-visits"></a>Så här följer du upp servicebesök för anläggningstillgångar
Du kan skriva ut rapporten **Underhåll – nästa service** om du vill se vilka tillgångar som du har bokat in ett servicebesök för. Du kan även använda den här rapporten när du uppdaterar fältet **Nästa servicedatum** på anläggningstillgångskortet.  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Underhåll, nästa service** och välj sedan relaterad länk.  
2. Fyll i fälten **Startdatum** och **Slutdatum**.  
3. Välj knappen **Skriv ut** eller **Förhandsgranska**.

## <a name="to-monitor-maintenance-costs"></a>Så här övervakar du underhållskostnader:  
Du kan se underhållskostnaderna när du visar statistiken för en anläggningstillgång.  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.
2. Markera den anläggningstillgång som du vill visa underhållskostnader för välj sedan åtgärden **Avskrivningsregler**.
3. I fönstret **Avskrivningsregler för anl.tillg.** väljer du relevant avskrivningsregel för anläggningstillgång åtgärden **Statistik**.
4. I **Anl.tillg.statistik** väljer du fältet **Underhåll**.

Fönstret **Underhållstransaktioner** öppnas och visar de poster som utgör beloppet i fältet **Underhåll**.

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a>Om du vill visa eller skriva ut underhållskostnader för åtskilliga anläggningstillgångar  
I rapporten **Underhållsanalys** kan du välja om du vill visa underhåll baaserat på en, två eller tre underhållskoder för ett angivet datum eller en angiven period. Du kan se summan för alla de markerade tillgångarna eller summan för varje tillgång.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Underhållsanalys** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs.
3. Välj knappen **Skriv ut** eller **Förhandsgranska**.

## <a name="to-view-maintenance-ledger-entries"></a>Så här visar du underhållstransaktioner
Du kan också studera underhållskostnader genom att visa underhållstransaktionerna.  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.
2. Markera den fasta anläggningstillgång som du vill visa transaktioner för välj sedan åtgärden **Avskrivningsregler**.
3. I fönstret **Avskrivningsregler för anl.tillg.** väljer du relevant avskrivningsregel för anläggningstillgång åtgärden **Underhållstransaktioner**.

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a>Om du vill visa eller skriva ut underhållstransaktioner för åtskilliga anläggningstillgångar  
I rapporten **Underhåll - Uppgifter** kan du visa eller skriva ut underhållstransaktioner för en eller flera anläggningstillgångar.  

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Underhållsdetaljer** och välj sedan relaterad länk.
2. Fyll i fälten om det behövs.
3. Välj knappen **Skriv ut** eller **Förhandsgranska**.

## <a name="see-also"></a>Se även
[Hantera anläggningstillgångar](fa-manage.md)  
[Skapa anläggningstillgångar](fa-setup.md)  
[Finans](finance-setup.md)  
[Välkommen till Dynamics NAV](across-get-started.md)

