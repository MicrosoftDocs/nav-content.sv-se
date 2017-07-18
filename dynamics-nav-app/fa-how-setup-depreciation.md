---
title: "Så här skapar du avskrivning av anläggningstillgångar"
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
ms.openlocfilehash: 7efc50c673514498de0caa5b3a2dc4b32d4f7f5d
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-depreciation"></a>Så här skapar du avskrivning av anläggningstillgångar
 Du kan använda olika avskrivningsmetoder när du förbereder redovisningsrapporter och självdeklarationer. Många större företag använder linjär avskrivning i redovisningsrapporterna eftersom de då i allmänhet kan rapportera större inkomster. Vad gäller självdeklaration använder många företag däremot en degressiv avskrivningsmetod. Mer information finns i [Avskrivningsmetoder](fa-depreciation-methods.md).

 Efter att du har skapat de avskrivningsregler som behövs måste du koppla en eller flera avskrivningsregler till varje anläggningstillgång. En avskrivningsregel som tilldelats en anläggningstillgång kallas för anläggningstillgångens avskrivningsregel. Därefter kallas fönstret för tilldelade avskrivningsregler **Avskrivningsregler för anl.tillg.**.

## <a name="to-create-a-depreciation-book"></a>Att skapa en avskrivningsregel  
I anläggningstillgångens avskrivningsregel anger du hur en anläggningstillgång ska skrivas av. Om du vill använda olika avskrivningsmetoder kan du skapa flera avskrivningsregler.  
1.  Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Avskrivningsregler** och välj sedan relaterad länk.
2. I fönstret **Lista över avskrivningsregler** väljer du åtgärden **Ny**.
3. I fönstret **Avskrivningsregelkort** fyller du i fälten efter behov. Välj ett fält om du vill få en kort beskrivning av fältet eller länken till mer information.

    **Obs!**: Du kan bokföra in anläggningstillgångstransaktioner i fönstret **Anl.tillg. redovisningsjournal** eller i fönstret **Anlägg.tillg.journal**, beroende på om transaktionerna är för finansiell rapportering eller för intern hantering. Följ nästa steg för att definiera vilken journaltyp som används för de olika anläggningstillgångaktiviteterna som standard.
4. På snabbfliken **Integrering** markerar du kryssrutan för varje anläggningstillgångsaktivitet vars transaktioner du vill bokföra med hjälp av fönstret **Anl.tillg. redovisningsjournal**.
5. Upprepa steg 2 till och med 4 för varje avskrivningmetod eller bokföringsmetod som du vill tilldela till anläggningstillgångar som en avskrivningsregel.

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a>Att tilldela en avskrivningsregel till en anläggningstillgång.  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.
2. Välj anläggningstillgången som du vill skapa avskrivningsregeln för anläggningstillgångar för.
3. I snabbfliken **Avskrivningsregelkort** fyller du i fälten efter behov.
4. Om du vill använda mer än en avskrivningsregel till anläggningstillgången väljer du åtgärden **Lägg till flera avskrivningsregler**.
5. Välj alternativt åtgärden **Avskrivningsregler** för att ange en eller flera avskrivningsregler för anläggningstillgångar.

**Obs!**: När du använder den manuella avskrivningsmetoden måste du föra in avskrivningen manuellt i redovisningsjournalen för anläggningstillgångar. Funktionen **Beräkna avskrivning** utesluter anläggningstillgångar där den manuella avskrivningsmetoden används. Du kan använda den här metoden för tillgångar som du inte längre kan skriva av, exempelvis mark.

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a>Att tilldela en avskrivningsregel till åtskilliga anläggningstillgångar med hjälp av ett batch-jobb
Om du vill tilldela en avskrivningsregel till flera anläggningstillgångar kan du använda batch-jobbet **Skapa anl. avskrivningsregler** så skapas de avskrivningsregler för anläggningstillgångar som behövs automatiskt av Dynamics NAV .  
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Anläggningstillgångar** och välj sedan relaterad länk.
2. Markera den anläggningstillgång som du vill tilldela en avskrivningsregel till och välj sedan åtgärden **Redigera**.
3. I fönstret **Avskrivningsregelkort** väljer du åtgärden **Skapa avskrivningsregler för anl.tillg.**.
4. I fönstret **Välj Avskrivningsregler för anl.tillg.** fyller du i fältet **Avskrivningsregler**.
5. Välj fältet **Kopiera från anl.nr.** och välj sedan det anläggningstillgångsnummer du vill använda som bas för att skapa nya avskrivningsregler för anläggningstillgångar.

    Om du fyller i det här fältet kommer avskrivningsfälten i anläggningstillgångarnas nya avskrivningsregler att innehålla samma information som motsvarande fält i den avskrivningsregel för anläggningstillgång som du kopierar från. Lämna fältet tomt om du vill skapa nya avskrivningsregler för anläggningstillgångar med tomma avskrivningsfält.  
6. På snabbfliken **Anläggningstillgång** kan du ange ett filter så att du kan välja vilka tillgångar du vill skapa avskrivningsregler för anläggningstillgång .
7. Välj **OK**.

## <a name="to-set-up-depreciation-posting-types"></a>Så här skapar du bokföringstyper för avskrivning  
För varje avskrivningsregel måste du ange hur du vill att Dynamics NAV ska hantera olika bokföringstyper. Till exempel om bokföringen ska vara debet eller kredit och om bokföringstypen ska inkluderas i avskrivningsbasen.  
1.  Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Avskrivningsregler** och välj sedan relaterad länk.  
2. Markera den avskrivningsregel som du vill ställa in och välj sedan åtgärden **Anl. inställningar bokföring**.
3. I fönstret **Anl. inställningar bokföring** fyller du i fälten efter behov.

**OBS!**: Du kan inte infoga eller ta bort rader i fönstret **Anl. inställningar bokföring**. Du kan endast ändra de befintliga raderna.

Du bör inte ändra inställningen för avskrivningsregler som transaktioner redan har bokförts för. Ändringarna påverkar inte transaktioner som redan har bokförts, vilket gör att statistiken över avskrivningsregler blir missvisande.

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a>Så här ställer du in standardmallar och journaler för avskrivningsregler för anläggningstillgångar.  
För varje avskrivningsregel anger du en standardinställning för mallar och journaler. Du använder dessa standardinställningar för att:
- Duplicera rader från en journal till en annan.
- Skapa journalrader med hjälp av batch-jobben **Beräkna avskrivning** eller **Indexera anläggningstillgångar**
- Duplicera anskaffningskostnader i försäkringsjournalen.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Avskrivningsregler** och välj sedan relaterad länk.
2. Markera den avskrivningsregel som du vill skapa standardjournaler för och välj sedan åtgärden **Anl. journalinställningar**.
3. Om du vill ha en standardinställning för varje användare väljer du fältet **Användar-ID** så visas fönstret **Användare**.
4. Välj journalmallen eller journalen som ska användas som standard i de andra fälten.

## <a name="see-also"></a>Se även
[Skapa anläggningstillgångar](fa-setup.md)  
[Hantera anläggningstillgångar](fa-manage.md)  
[Finans](finance-setup.md)  
[Välkommen till Dynamics NAV](across-get-started.md)

