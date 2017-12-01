---
title: "Så här registrerar du Dynamics NAV i ledningsportalen för Azure"
author: edupont04
manager: edupont
ms.author: edupont
ms.custom: na
ms.date: 11/15/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d41b96ab5807402a342991d5c5bc2d672db09e2f
ms.contentlocale: sv-se
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-dynamics-nav-in-the-azure-management-portal"></a>Så här registrerar du Dynamics NAV i ledningsportalen för Azure
Om du vill använda tjänster som bygger på Microsoft Azure, måste du registrera din Dynamics NAV i ledningsportalen för Azure. Till exempel tillägget [försäljnings- och lagerprognos](ui-extensions-sales-forecast.md)kräver att du anger en API-nyckel och en API-URL och andra tjänster kräver liknande information. Så var hittar du den information?

Du kan använda guiden **Ställa in ledningsportalen för Azure** för att registrera Dynamics NAV i ledningsportalen för Azure och för att extrahera den information som du behöver för att använda tjänster som tillägget för försäljnings- och lagerprognos, Power BI, Office 365, etc. Du måste registrera dig i ledningsportalen för Azure bara en gång, och du måste vara en administratör eller superuser i Dynamics NAV.

Punkten för registrering är att Dynamics NAV och tjänsten som du vill koppla, måste veta information om Azure Active Directory (Azure AD) om varandra.

## <a name="to-register-dynamics-nav-in-the-azure-management-portal"></a>Så här registrerar du Dynamics NAV i ledningsportalen för Azure
1. Logga in på Azure hanteringsportal på [https://portal.azure.com](https://portal.azure.com). Om du inte känner till ledningsportalen för Azure hittar du anvisningar i [Azure dokumentationbibliotek](https://azure.microsoft.com/en-us/documentation/articles).
2. I det vänstra navigeringsfönstret väljer du **Fler tjänster** och väljer sedan **programmarregistreringar**.
3. I den övre menyn väljer du **Lägg till**, och i **Skapa fönster** fyller du i fälten med följande information:
    - **Namn**: Ange ett namn för din Dynamics NAV-lösning till exempel *Dynamics NAV*.
    - **Programtyp**: Välj **Webbprogram* / API**.
    - **Inloggnings-URL**: Ange URL för ditt Dynamics NAV-webbläsarprogram, till exempel *https://MyServer:8080/DynamicsNAV/WebClient/OAuthLanding.htm*.
        Filen OAuthLanding.htm är en fil som hanterar datautbyte mellan Dynamics NAV och andra tjänster via Azure AD.
4. Klicka på **Skapa**.
    Detta lägger till din Dynamics NAV till **programmarregistreringsfönstret**, så du kan nu lägga till inställningar till den.
5. Välj det nya programmet i**programmarregistreringslista**. Om detta inte öppnar fönstret **inställningar** bör du se en åtgärd för att öppna **inställningar**.
6. I fönstret **Inställningar** i avsnittet **API-åtkomst** väljer du **nycklar**.
7. I fönstret **nycklar** anger du en beskrivning och när du cill att nyckeln ska upphöra och väljer sedan **Spara**.
8. Kopiera den skapade nyckeln till en tillfällig plats - du kommer att behöva den i nästa procedur.
9. I avsnittet **API-åtkomst** väljer du **Krävda behörigheter**.
    - Lägg till delegerade behörigheter för visa alla rapporter i Power BI-tjänsten
    - Lägg till delegerade behörigheter för att Logga in och läsa användarprofil till Windows Azure Active Directory
    - Upprepa för andra tjänster som du vill bevilja behörighet till din Dynamics NAV
10. Stäng fönstret **inställningar** och sedan i fönstret **Grundläggande** kopierar du värdet av **Program-ID** till en tillfällig plats.

Du har nu registrerat din Dynamics NAV i ledningportalen för Azure och du har fått åtkomst till relevanta tjänster och du har extraherat information som behövs i Dynamics NAV.  

## <a name="to-add-the-information-to-dynamics-nav"></a>Om du vill lägga till information till Dynamics NAV
1. Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Programinställningsguiden för Azure AD** och välj sedan relaterad länk.
2. Välj **Nästa** i guiden.
3. I fältet **Klient-ID** anger du det innehåll som du kopierade från fältet **Program-ID** tidigare.
4. I fältet **Hemlig nyckel** anger du det innehåll som du kopierade från fönstret **Nycklar** tidigare.
5. Välj **Nästa**. Om du inte ser ett felmeddelande är du nu klar.

Din Dynamics NAV är klar att ansluta till tjänster som till exempel Cortana Intelligence och Power BI.

## <a name="see-also"></a>Se även
[Försäljnings- och lagerprognos](ui-extensions-sales-forecast.md)  
[Konfigurera din Dynamics NAV](setup.md)  

