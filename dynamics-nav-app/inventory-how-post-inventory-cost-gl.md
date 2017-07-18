---
title: "Så här kan du bokföra lagerkostnader i redovisningen"
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
ms.openlocfilehash: 59815db9c7b435ff585e1174b570029a360dea6e
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Så här kan du bokföra lagerkostnader i redovisningen   
När du bokför lagertransaktioner, till exempel försäljningsutleveranser, inköpsinleveranser eller lagerjusteringar registreras de ändrade kvantiteterna i artikeltransaktioner respektive värdetransaktioner. För att återspegla detta ändringar av lagervärdet i dina ekonomiska böcker måste du bokföra lagerkostnader till de relaterade lagerkontona i redovisningen.

Du kan bokföra lagerkostnader i redovisningen på två sätt.

- Automatiskt, vilket innebär att lagerkostnaderna bokförs i redovisningen varje gång en lagertransaktion bokförs.
- Manuellt, vilket innebär att lagerkostnaderna endast bokförs i redovisningen när du väljer att köra ett batch-jobb.


## <a name="to-post-inventory-costs-automatically"></a>Bokföra lagerkostnader automatiskt
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Lagerinställningar** och välj sedan relaterad länk.
2. I fönstret **Lagerinställningar** väljer du kryssrutan **Automatisk kostnadsbokföring**.

För varje lagertransaktion som bokförs, bokförs lämpliga värden på lagerkontot, justeringskontot och KSV-kontot i redovisningen.

Även om automatisk kostnadsbokföring används bör batch-jobbet Justera kostnad – artikeltrans. fortfarande köras ibland. Detta för att säkerställa att varornas kostnader har vidarebefordrats till lämpliga avgående transaktioner, t.ex. till försäljning eller överföringar. Det är speciellt viktigt i situationer där du säljer varor, innan du fakturerar inköpet av dessa varor.

Om ett fel inträffar i dimensionsinställningarna samtidigt som lagerkostnaden bokförs i redovisningen avslutas bokföringen med ett fel.

## <a name="to-post-inventory-costs-manually"></a>Bokföra lagerkostnader manuellt
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Bokför lagerkostnad i redov.** och välj sedan relaterad länk.
2. Bokför lagerkostnader i redovisningen manuellt genom att köra batch-jobbet. När det här batch-jobbet körs skapas redovisningstransaktioner utifrån värdetransaktioner. Det går att bokföra transaktionerna så att de sammanfattas per bokföringsmall.

**Obs!** När du kör batch-jobbet kan fel påträffas som har att göra med saknad inställning eller inkompatibel dimensionsinställning. Om fel uppstår i batch-jobbets dimensionsinställning ersätter den dessa fel och använder dimensionerna för värdetransaktionen. För andra fel hopar batch-jobbet över att bokföra värdetransaktionerna och anger dem vid slutet av rapporten i avsnittet “Transaktioner som hoppats över”. För att bokföra de här transaktionerna måste du först lösa felen.

Om en lista över felen ska visas innan batch-jobbet för bokföring ska köras kan rapporten **Bokför lagerkostnad i redovisning - test** köras. Alla fel som inträffar under testbokföringen visas i en lista i testrapporten. Därefter går det att korrigera felen och köra batch-jobbet för bokföringen av lagerkostnaden utan att transaktioner hoppas över.

Det går att visa en översikt över de värden som eventuellt bokförs i redovisningen genom att köra batch-jobbet Bokför lagerkostnad i redov., utan att själva bokföringen av värdena utförs i redovisningen. Genom att avmarkera fältet Bokför på sidan för begäran kan översikten visas. Om batch-jobbet körs med de här inställningarna visas värdena som kan bokföras i redovisningen i rapporten, men de bokförs inte.

## <a name="see-also"></a>Se även
[Hantera lager](inventory-manage-inventory.md)    
[Så här justerar du artikelkostnader](inventory-how-adjust-item-costs.md)  
[Hantera försäljning](sales-manage-sales.md)  
[Hantera inköp](purchasing-manage-purchasing.md)

