---
title: "Så här använder du godkännande av arbetsflöden"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: e4135aa801b0b507b5f179d02a240a7554ed45cd
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-approval-workflows"></a>Så här använder du godkännande av arbetsflöden
När en post som till exempel ett inköpsdokument eller ett kundkort måste godkännas av någon i organisationen, skickar du en godkännandebegäran som en del av ett arbetsflöde. Beroende på hur arbetsflödet konfigureras meddelas sedan den lämpliga godkännaren om att posten kräver godkännande.

Centrala arbetsflöden för godkännande för inköpsdokument, försäljningsdokument, utbetalningsjournaler, kundkort och artikelkort är klara att starta som assisterad installation. Mer information finns i [Välkommen till Dynamics NAV](across-get-started.md).

## <a name="to-request-approval-of-a-record"></a>Så här begära du godkännande av en post
Efterföljande aktivitet utförs av en godkännaranvändare.

1. I fönstret som visar posten väljer du åtgärden **Skicka godkännandebegäran**.
2. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Transaktioner för godkännandebegäranden** och välj sedan relaterad länk för att se alla dina godkännandebegäran.

Statusen på godkännandetransaktionen uppdateras från **Skapad** till **Öppen**. Statusen på posten, t.ex. en inköpsfaktura, uppdateras från **Öppen** till **Väntar på godkännande** och är låst för bearbetning tills alla godkännare har godkänt transaktionen.

När godkännaren har godkänt transaktionen, ändras statusen till **Släppt**. Därefter kan du fortsätta med dina uppgifter för posten.

## <a name="to-cancel-requests-for-approval"></a>Så här annullerar du begäranden om godkännande
Efterföljande aktivitet utförs av en godkännaranvändare med behörigheten godkännare.

Det kan hända att en kund vill göra ändringar i en order efter att den har skickats till godkännande. I det här fallet kan du annullera godkännandeprocessen och göra nödvändiga ändringar i ordern innan du begär godkännande igen.

1. I fönstret som visar posten väljer du åtgärden **Avbryt godkännandebegäran**.

När godkännandebegäran har annullerats, ändras statusen på den relaterade godkännandeposten till **Annullerad**. Statusen på posten uppdateras från **Väntar på godkännande** till **Öppen**. Godkännandeprocessen kan sedan starta från början igen.

## <a name="to-make-minor-changes-to-approved-records"></a>Så här kan du göra mindre ändringar av godkända poster
Om du vill göra en mindre ändring av en transaktion, när den har godkänts kan du öppna en post igen, ändra den och sedan släppa den. För mindre ändringar gör du detta med knapparna **Öppna igen** och **Släpp**.

1. Öppna fönstret som visar posten, till exempel en inköpsfaktura och välj sedan åtgärden **Öppna igen**.

    Värdet i fältet **Dokumentstatus** ändras till Öppen.
3. Gör de nödvändiga ändringarna i posten, t.ex leverantörens adress.
4. Välj åtgärden **Släppa**.

När du öppnar källposten igen är statusen för den relaterade godkännandetransaktionen fortfarande Godkänd i fönstret **Godkännandetransaktioner**.

## <a name="to-approve-or-reject-requests-for-approval"></a>Så här godkänner eller avvisar du begäranden om godkännande
Efterföljande aktivitet utförs av en godkännaranvändare med behörigheten godkännare.

Du kan bearbeta godkännandebegäran i fönstret **Begäranden att godkänna** till exempel att godkänna flera begäran i taget. Alternativt kan du behandla varje förfrågningsdokument på relaterade post, till exempel fönstret **inköpsfaktura** genom att välja länken i meddelandet som du får.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Begäranden att godkänna** och välj sedan relaterad länk.
2. Markera en eller flera rader för posten eller posterna som du vill godkänna eller avvisa.
3. Välj åtgärden **Godkänna**, **Avvisa**, eller **Delegera**.

När en post har godkänts eller har avvisats ändras godkännandestatus i fältet **Status** till **Godkänd** eller **Avvisad**.

Om en godkännarehierarki har ställts in är poststatusen **Väntar på godkännande** tills alla godkännare har godkänt transaktionen. Sedan ändras statusen till **Släppt**.

Samtidigt ändras godkännandestatus från **Skapad** till **Öppen** så snart som en godkännandebegäran skapas för posten. Om begäran avvisas, ändras godkännandestatus till **Avvisad**. Status står kvar som **Öppen** eller **Avvisad** tills alla godkännare har godkänt begäran.

## <a name="to-delegate-requests-for-approval"></a>Så här delegerar du begäranden om godkännande
Efterföljande aktivitet utförs av en godkännaranvändare med behörigheten godkännare.

För att förhindra att dokument staplas på hög eller blockerar arbetsflödet på något annat sätt kan godkännandeadministratören delegera en godkännandebegäran till en ersättare. Ersättaren kan vara antingen en utsedd ersättare, den direkta godkännaren eller godkännandeadministratören, i den prioritetsordningen. Du kan använda den här funktionen om en godkännare inte är tillgänglig för tillfället och inte kan godkänna begäranden före förfallodatumet.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Begäranden att godkänna** och välj sedan relaterad länk.
2. Markera en eller flera rader för godkännandebegäran som du vill delegera till en ersättande godkännare och välj sedan åtgärden **Delegera**.

Ett meddelande om att godkänna begäran skickas till den ersättande godkännaren.

## <a name="to-manage-overdue-approval-requests"></a>Så här hanterar du förfallna begäranden om godkännande
Efterföljande aktivitet utförs av en godkännaranvändare med behörigheten godkännare.

Med jämna mellanrum måste du påminna godkännandearbetsflödesanvändare om förfallna godkännandebegäranden som de måste agera på. Använd funktionen Skicka meddelanden om förfallna godkännanden för detta.

Med funktionen Skicka meddelanden om förfallna godkännanden görs en kontroll för att hitta alla förfallna öppna godkännandetransaktioner. Varje godkännare som har minst en förfallen godkännandetransaktion får meddelande med en lista över alla förfallna godkännandebegäranden. Meddelandet skickas också till deras godkännare och alla som begärt de förfallna godkännandena. Detta är praktiskt om den förfallna godkännandetransaktionen behöver delegeras till en ersättare.

1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Förfallna begäranden om godkännande** och välj sedan relaterad länk.
2. I fönstret **Förfallna begäranden om godkännande** väljer du åtgärden **Skicka meddelanden om förfallna godkännanden**.

## <a name="see-also"></a>Se även  
[Hantera försäljning](sales-manage-sales.md)    
[Inkommande dokument](across-income-documents.md)  
[Hantera inköp](purchasing-manage-purchasing.md)  
[Arbeta med Dynamics NAV](ui-work-product.md)
