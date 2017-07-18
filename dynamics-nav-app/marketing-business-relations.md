---
title: "Skapa affärsrelationer på kontaktföretag"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 20abe2f08fc726a008719f94389579d02ecbd275
ms.contentlocale: sv-se
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a>Skapa affärsrelationer på kontaktföretag
Affärsrelationer används för att visa vilket affärsförhållande du har till kontakterna, till exempel spekulant, bank, konsult eller serviceleverantör.

Att använda affärsrelationer på kontakter är en två-stegsprocess. Först definierar du affärsrelationskoden. Du måste bara utföra den här steget en gång för varje affärsrelation. När du har en affärsrelation kan du börja koppla koden till kontaktföretag.

**Obs!** Om du tänker synkronisera kontakterna med leverantörer, kunder eller bankkonton i andra delar av programmet vill du kanske skapa en affärsrelation för dem.

## <a name="define-a-business-relation-code"></a>Definiera affärsrelationskod
Affärsrelationkoden definierar en kategori eller en typ av affärsrelation, till exempel BANK eller LAG. Du kan ha flera affärsrelationskoder. För att definiera affärsrelationen använder du fönstret **affärsrelationer**.

1. Välj ikonen **söka efter sida eller rapport** i det övre högra hörnet, gå till **affärsrelationer** och välj sedan relaterad länk.
2. Välj åtgärden **Ny** och fyll i en kod och en beskrivning. Koden kan bestå av högst 11 tecken, både siffror och bokstäver.

## <a name="assign-business-relations-to-a-contact"></a>Så här tilldelar du affärsrelationer till kontakter:
Du kan inte tilldela affärsrelationer till en kontaktperson, endast företag.

1. Öppna kontakten .
2. Välj åtgärden **företag** och sedan **affärsrelationer**.

    Fönstret **Kontakt affärsrelationer** öppnas.
3. I fältet **Affärsrelationskod**, markera den affärsrelation du vill tilldela.

Upprepa stegen för varje affärsrelation du vill tilldela. Affärsrelationer kan också tilldelas i Kontaktlista på samma sätt.

Antalet affärsrelationer som du har tilldelat kontakter anges automatiskt i fältet **Antal affärsrelationer** på avsnittet **Segmentering** på **Kontakt**-fönstret.

När du har tilldelat kontakterna affärsrelationer kan du använda dessa uppgifter för urval av kontakter till segmenten. Mer information finns i [Så här lägger du till kontakter i segment](marketing-add-contact-segment.md).

##<a name="see-also"></a>Se även
[Skapa kontaktföretag](marketing-create-contact-companies.md)

