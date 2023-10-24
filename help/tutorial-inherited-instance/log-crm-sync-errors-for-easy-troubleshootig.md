---
title: Logboek CRM-synchronisatiefouten voor eenvoudige probleemoplossing
description: Leer hoe te om een logboek van de fouten van de Synchronisatie van CRM te gebruiken om de synchronisatiekwesties van CRM te onderzoeken en het te houden regelmatig lopend.
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
source-git-commit: 96ec338944d486b74ac77d91aba3ede482abf135
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---


# Logboek CRM-synchronisatiefouten voor eenvoudige probleemoplossing

Als beheerder van het Marketo Engage, zou het controleren of uw instantie synchroon met uw CRM is een zeer belangrijk deel van uw [dagelijkse routine](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (zoek het op de hoogste juiste hoek van uw interface van het Marketo Engage) is waar u begint om frequente synchronisatiekwesties te vinden en te onderzoeken, is er pro tip die u zou kunnen helpen de instantiegezondheid op een georganiseerde manier beheren. De Adobe van Marketo Champion (2019-2022), Amy Goldfine adviseert admin gebruikers een logboek van de fouten van de Synchronisatie van CRM houden om het oplossen van problemen gemakkelijker te maken.

![Screenshot van het tabblad Synchronisatiefouten](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Waarom een overzicht bijhouden van CRM-synchronisatiefouten?

Door de fouten van de Synchronisatie van CRM te registreren, kunnen de beheerders van het Marketo Engage de kwesties en de tendensen met de beheerders van CRM herzien om de worteloorzaak te bevestigen. Volg de onderstaande stappen om uw problemen met CRM Sync voor uw instantie te documenteren.

## Hoe te om een logboek van de Fouten van de Synchronisatie van CRM te houden

Download de [Logsjabloon CRM-synchronisatiefouten](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Stap 1:** Ga naar de *[!UICONTROL Admin]sectie* in Marketo Engage. Onder *[!UICONTROL Integration]*, klikt u op *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]*, of *[!DNL Veeva]*, afhankelijk van welke [!DNL CRM] u gebruikt, dan *[!UICONTROL Sync Errors]* tab.

**Stap 2:** U kunt ervoor kiezen [de records met fouten exporteren als een [!DNL CSV] door het [!UICONTROL Filter] deelvenster](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Als u slechts een paar uur hebt, kopieert en plakt u rechtstreeks vanuit de *[!UICONTROL Sync Errors]* is de manier om te gaan.

**Stap 3:** Let op de datum waarop de fout is opgetreden.

**Stap 4:** Voer het aantal persoonrecords in waarop die fout betrekking heeft. (Soms zal uw CRM slechts een fout voor één persoon veroorzaken. Soms zullen er veel mensen met dezelfde fout tegelijk zijn.)

**Stap 5:** Noteer het e-mailadres van één persoon die door de fout is beïnvloed. Dit maakt het voor u gemakkelijk om de fouten met de beheerder van CRM van verwijzingen te voorzien en te bespreken.

**Stap 6:** Koppelingen naar persoonrecord plakken in [!DNL Marketo Engage] en [!UICONTROL CRM Lead/Contact] een overzicht van die persoon.

**Stap 7:** Plak in de laatste kolom de werkelijke tekst van de fout.

## Wat is de volgende?

**Foutcodes identificeren:** Als u de foutcodes wilt begrijpen, raadpleegt u de beschrijvingen in de documentatie voor ontwikkelaars [Tabel met foutcodes op responsniveau](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} en zoek naar gebruikelijke volgende stappen om de fouten op te lossen.

## Auteurs

**Amy Goldfine**\
Adobe Marketo Champion (2019-2022)
*Oprichter, MarketingOpsAdvice.com*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Beheer van toepassings- en retentiemarketingen bij Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}

