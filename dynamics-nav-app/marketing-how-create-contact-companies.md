---
title: "Skapa kontaktföretag"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: e3490b10039f430137ee35f1a50c73111386fab4
ms.contentlocale: sv-se
ms.lasthandoff: 09/11/2017

---
# <a name="create-contact-companies"></a><span data-ttu-id="82112-102">Skapa kontaktföretag</span><span class="sxs-lookup"><span data-stu-id="82112-102">Create Contact Companies</span></span>
<span data-ttu-id="82112-103">Du kan skapa en kontakt för varje nytt företag som du har förbindelse med, till exempel kund, leverantör, spekulant, bank, jurist, konsult och så vidare.</span><span class="sxs-lookup"><span data-stu-id="82112-103">You can create a contact for each new company you interact with, for example, a customer, vendor, prospective customer, bank, law firm, consultant, and so on.</span></span>

<span data-ttu-id="82112-104">Det finns två sätt att skapa en kontakt: från noll eller från en befintlig kund, leverantör eller bankkonto.</span><span class="sxs-lookup"><span data-stu-id="82112-104">There are two ways to create a contact: from scratch or from an existing customer, vendor, or bank account.</span></span>

<span data-ttu-id="82112-105">Innan du skapar en kontakt kan du kontrollera inställningarna i fönstret **Affärsstödsinställning**.</span><span class="sxs-lookup"><span data-stu-id="82112-105">Before creating a contact, you may want to check the settings in the **Marketing Setup** window.</span></span> <span data-ttu-id="82112-106">Mer information finns i [Ställ in Marknadsföring och Kontakthantering](marketing-setup-marketing.md).</span><span class="sxs-lookup"><span data-stu-id="82112-106">For more information, see [Set Up Marketing and Contact Management](marketing-setup-marketing.md).</span></span>

## <a name="create-a-company-contact-from-scratch"></a><span data-ttu-id="82112-107">Skapa en företagskontakt från noll</span><span class="sxs-lookup"><span data-stu-id="82112-107">Create a company contact from scratch</span></span>
1. <span data-ttu-id="82112-108">Välj ikonen **Söka efter sida eller rapport** i det övre högra hörnet, gå till **Kontakter** och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="82112-108">In the top right corner, choose the **Search for Page or Report** icon, enter **Contacts**, and then choose the related link.</span></span>
2. <span data-ttu-id="82112-109">Välj åtgärden **Ny**.</span><span class="sxs-lookup"><span data-stu-id="82112-109">Choose the **New** action.</span></span>
3. <span data-ttu-id="82112-110">Skriv numret på den artikel som har beställts i fältet **Nr**.</span><span class="sxs-lookup"><span data-stu-id="82112-110">In the **No. field**, enter a number for the contact.</span></span>

  <span data-ttu-id="82112-111">Om du har definierat en nummerserie för kontakter i fönstret **Affärsstödsinställning** kan du i stället trycka på Retur så anges nästa tillgängliga kontaktnummer automatiskt.</span><span class="sxs-lookup"><span data-stu-id="82112-111">Alternatively, if you have set up a number series for contacts in the **Marketing Setup** window, you can press the Enter key to select the next available contact number.</span></span>
4. <span data-ttu-id="82112-112">Ange **Typ** till **Företag**.</span><span class="sxs-lookup"><span data-stu-id="82112-112">Set **Type** to **Company**.</span></span>
5. <span data-ttu-id="82112-113">Fyll i övriga fält enligt behov.</span><span class="sxs-lookup"><span data-stu-id="82112-113">Fill in the other fields as required.</span></span>

## <a name="create-a-company-contact-from-a-customer-vendor-or-bank-account"></a><span data-ttu-id="82112-114">Skapa en företagskontakt från en kund, en leverantör eller ett bankkonto</span><span class="sxs-lookup"><span data-stu-id="82112-114">Create a company contact from a customer, vendor, or bank account</span></span>
<span data-ttu-id="82112-115">Om du redan har lagt upp flera kunder, leverantörer eller bankkonton kan du skapa kontakter baserat på befintliga uppgifter.</span><span class="sxs-lookup"><span data-stu-id="82112-115">If you have already set up a number of customers, vendors, and bank accounts, you can create contacts on the basis of the existing data.</span></span> <span data-ttu-id="82112-116">När du skapar en kontakt på detta sätt, synkroniseras kontaktinformationen med kunden, leverantören eller bankkontotinformationen.</span><span class="sxs-lookup"><span data-stu-id="82112-116">When you create a contact this way, the contact information is synchronized with the customer, vendor, or bank account information.</span></span>

<span data-ttu-id="82112-117">**Obs!** Innan du kan skapa kontaktföretag på detta sätt måste du ange en affärsrelationskod för bankkonton, kunder eller leverantörer i fönstret **Marknadsföringsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="82112-117">**Note**: Before you can create contact companies this way, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window.</span></span> <span data-ttu-id="82112-118">Om du vill skapa kontakter från bankkonton måste du även ange nummerserien för bankkonton i fönstret **Redovisningsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="82112-118">If you will be creating contacts from a bank accounts, you must also specify numbers series for bank accounts in the **General Ledger Setup** window.</span></span>

1. <span data-ttu-id="82112-119">I övre högra hörnet väljer du ikonen **Sök efter sida eller rapport** och anger ett av följande, beroende på varifrån du vill skapa kontakter och välj sedan relaterad länk.</span><span class="sxs-lookup"><span data-stu-id="82112-119">In the top right corner, choose the **Search for Page or Report** icon, enter one of the following, depending on from where you want to create contacts, and then choose the related link.</span></span>
  * <span data-ttu-id="82112-120">**Skapa kontakter från kunder**</span><span class="sxs-lookup"><span data-stu-id="82112-120">**Create Contacts from Customers**</span></span>
  * <span data-ttu-id="82112-121">**Skapa kontakter från leverantörer**</span><span class="sxs-lookup"><span data-stu-id="82112-121">**Create Contacts from Vendors**</span></span>
  * <span data-ttu-id="82112-122">**Skapa kontakter från bankkonton**</span><span class="sxs-lookup"><span data-stu-id="82112-122">**Create Contacts from Bank Accounts**</span></span>
2. <span data-ttu-id="82112-123">I batch-jobbfönstret som öppnas i avsnittet **Kund**, **Leverantör** eller **Bankkonto** kan du ställa in filter om du endast vill skapa kontakter från vissa kunder, leverantörer eller bankkonton.</span><span class="sxs-lookup"><span data-stu-id="82112-123">In the batch job window that opens, in the **Customer**, **Vendor**, or **Bank Account** section, set filters if you want to create contacts from specific customers, vendors, or bank accounts.</span></span>
3. <span data-ttu-id="82112-124">Klicka på **OK** för att börja skapa kontakter.</span><span class="sxs-lookup"><span data-stu-id="82112-124">Choose the **OK** button to start creating contacts.</span></span>

  <span data-ttu-id="82112-125">Nästa kontaktnummer i nummerserien kopplas till de nya kontakterna.</span><span class="sxs-lookup"><span data-stu-id="82112-125">The next contact numbers in the number series are assigned to the new contacts.</span></span> <span data-ttu-id="82112-126">De nyskapade kontakterna tilldelas den affärsrelation för leverantörer som angetts i fönstret **Affärsstödsinställning**.</span><span class="sxs-lookup"><span data-stu-id="82112-126">The business relation for vendors that is specified in the **Marketing Setup** window is assigned to the newly created contacts.</span></span>

<span data-ttu-id="82112-127">**Tips** Du kan också skapa en kund, en leverantör eller ett bankkonto från en kontakt.</span><span class="sxs-lookup"><span data-stu-id="82112-127">**Tip**: You can also create a customer, vendor, or bank account from a contact.</span></span> <span data-ttu-id="82112-128">Mer information finns i [Skapa en företagskontakt från kund, leverantör eller bankkonto från en kontakt](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="82112-128">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>
##<a name="see-also"></a><span data-ttu-id="82112-129">Se även</span><span class="sxs-lookup"><span data-stu-id="82112-129">See Also</span></span>
[<span data-ttu-id="82112-130">Synkronisera kontakter med kunder, leverantörer och bankkonton</span><span class="sxs-lookup"><span data-stu-id="82112-130">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="82112-131">Så här tilldelar du affärsrelationer till kontakter</span><span class="sxs-lookup"><span data-stu-id="82112-131">Assign Business Relations to a Contact</span></span>](marketing-business-relations.md#assign-business-relations-to-a-contact)  
[<span data-ttu-id="82112-132">Så här tilldelar du industrigrupper till en kontakt</span><span class="sxs-lookup"><span data-stu-id="82112-132">Assign Industry Groups to a Contact</span></span>](marketing-industry-groups.md#assign-industry-groups-to-a-contact)  
[<span data-ttu-id="82112-133">Tilldela utskicksgrupp till en kontakt</span><span class="sxs-lookup"><span data-stu-id="82112-133">Assign Mailing Groups to a Contact</span></span>](marketing-mailing-groups.md#assign-mailing-groups-to-a-contact)  
[<span data-ttu-id="82112-134">Så här skapar du kontaktpersoner</span><span class="sxs-lookup"><span data-stu-id="82112-134">How to: Create Contact Persons</span></span>](marketing-create-contact-persons.md)  

