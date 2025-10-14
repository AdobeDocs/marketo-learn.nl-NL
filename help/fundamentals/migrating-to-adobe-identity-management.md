---
title: Migreren naar Adobe Identity Management
description: Deze zelfstudie helpt u bij het migreren van uw Marketo Engage-abonnementen en -gebruikers naar de Adobe Admin Console.
role: Admin
level: Intermediate, Experienced
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: dcfffa299cbcfef489f5b618fae29f745b878d26
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Migreren naar Adobe Identity Management

Adobe verbetert hoe u uw Adobe Marketo Engage-abonnementen en -gebruikers beheert. Wij brengen verhoogde productiviteit aan uw organisatie door uw Marketo Engage abonnementen en gebruikers naar Adobe Admin Console te migreren.

Deze zelfstudie helpt u door de migratie te navigeren, zodat u Adobe Marketo Engage samen met andere Adobe-accounts en -producten voor uw gebruikers op een centrale locatie kunt beheren. De migratie is noodzakelijk en heeft geen invloed op uw marketingworkflow, inhoud, integratie of middelen.

## Controlelijst voor migratie voor Marketo Engage-beheerders {#pre-migration-checklist-for-marketo-engage-administrators}

Om ervoor te zorgen dat uw organisatie Adobe Marketo Engage naar de Adobe Admin Console kan migreren, raden we u aan de onderstaande checklist te volgen om de komende wijzigingen te beheren.

### 1. Identificeer uw systeembeheerder(s) en IT-team en bespreek de acties die zij moeten ondernemen {#identify-your-system-administrators}

* Als u niet zeker weet wie de systeembeheerders binnen uw organisatie zijn, neemt u contact op met uw Adobe-accountteam of neemt u contact op met de ondersteuning van Adobe `marketocares@marketo.com` .

* Bevestig de Adobe Admin Console (of Adobe Org) waarnaar uw Marketo Engage-abonnement(en) wordt gemigreerd. U hebt waarschijnlijk een Adobe Admin Console voor [&#x200B; Dynamic Chat &#x200B;](/help/dynamic-chat/dynamic-chat-overview.md){target="_blank"}, een inheems hulpmiddel van de gespreksautomatisering in Marketo Engage. Marketo Engage-abonnementen moeten worden geïmplementeerd in dezelfde organisatie als Dynamic Chat.

* Het werk met uw team van IT om alle die domeinen van Adobe te lijsten van gewenste personen [&#x200B; bij de bovenkant van dit artikel &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} worden vermeld om verstoring aan de toegang van Marketo Engage na de migratie aan Identiteit van Adobe te verhinderen.

* **Facultatief:** [&#x200B; voert Enig Sign (SSO) uit &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"} vóór gebruikersmigratie.

  >[!NOTE]
  >
  >Er zijn verschillen tussen door Marketo Engage ondersteunde SSO en Adobe Admin Console SSO. Daarom moeten wijzigingen in uw configuratie mogelijk worden geïmplementeerd.

* **Facultatief:** pas het [&#x200B; gewenste maximumzittingsleven &#x200B;](https://helpx.adobe.com/nl/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} voorafgaand aan gebruikersmigratie voor de gebruikers van Marketo Engage aan authentiek te blijven.

* Leer wat met uw Beheerders van het Systeem in de [&#x200B; E-mailsectie van de Steekproef &#x200B;](#announce-the-migration-timeline) te communiceren.

### 2. Kennis van de veranderingen en gevolgen van migratie naar Adobe Identity {#familiarize-yourself-with-the-changes}

In de onderstaande video bespreekt het Marketo Engage Product Management-team u de migratiereis en wat u verwacht.

>[!VIDEO](https://video.tv.adobe.com/v/3432368/?t=170/?quality=12&learn=on&captions=dut){transcript=true}

Meer hulp over dit onderwerp voor de beheerders van Marketo Engage kan in de volgende hulpartikelen worden gevonden:

* [&#x200B; checklist van de Opstelling van de Gebruiker &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [&#x200B; Adobe Identity Management Overzicht &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [&#x200B; Begrijpend het Abonnement van Marketo en de Migratie van de Gebruiker aan Adobe Admin Console &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [&#x200B; Migrerend aan de Identiteit van Adobe met de Console van de Migratie &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [&#x200B; Begrijp hoe te om Adobe Admin Console &#x200B;](https://helpx.adobe.com/nl/enterprise/using/admin-console.html){target="_blank"} te gebruiken

### 3. Geef uw interne teams een overzicht van het tijdschema en de voorbereiding voor de migratie {#announce-the-migration-timeline}

* Markeer de migratiedatum op de agenda&#39;s van uw Marketo Engage-beheerders en -gebruikers zodra deze gepland zijn.

   * U kunt de migratiedatum in **Admin** wijzigen > **de Console van de Migratie** > **pre-Migratie** om uw interne chronologie beter aan te passen. Leer meer over het opnieuw plannen en de beperkingen van [&#x200B; het wijzigen van uw migratiedatum &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* **verzend een e-mail naar uw Beheerders van het Systeem**

Hieronder ziet u een voorbeeld van een e-mail die u naar uw beheerders wilt verzenden. Meestal beheert uw IT-afdeling al uw Adobe-licenties.

+++ Voorbeeld-e-mail die naar uw systeembeheerders moet worden verzonden

**Onderwerp: Steun nodig-Migratie van de Abonnementen van Marketo Engage aan Adobe Admin Console**

Beste `[IT Administrator/NAME]`,

Ons Marketo Engage-abonnement wordt binnenkort gemigreerd naar het Adobe Identity Management System. `[Marketing Operation team]` heeft uw hulp nodig om enkele vereiste stappen te voltooien voordat de gebruikersmigratie begint, om de gevolgen voor Marketo Engage-gebruikers te minimaliseren.

`1.` Bevestig of de organisatie al andere Adobe-producten beheert in Adobe Admin Console(s) en of Marketo Engage naar dezelfde console wordt gemigreerd.

* Marketo Engage-abonnementen moeten zich in dezelfde organisatie bevinden als Dynamic Chat, een native hulpprogramma voor gespreksautomatisering dat is geïntegreerd met Marketo Engage.

* Neem contact op met Adobe Support op `marketocares@marketo.com` en CC van ons als u vragen of problemen hebt met de Admin Console.

`2.` Zorg dat u op zoek bent naar een e-mailbericht van Adobe met de onderwerpregel &quot;Handeling vereist om gebruikerstoegang tot Adobe Marketo Engage te beheren `[Package Tier]`&quot;. Dit e-mailbericht is verzonden nadat Marketo Engage-licenties zijn ingericht op onze Admin Console. Alleen systeembeheerders ontvangen deze e-mail. Gelieve ons onmiddellijk op de hoogte te brengen wanneer u het ontvangt.

* Adobe kan u, de systeembeheerder van de Admin Console, om toestemming vragen om gebruikers automatisch te migreren naar de bestaande console van onze organisatie. Klik in de e-mail met de onderwerpregel &quot;Handeling vereist om gebruikerstoegang tot Adobe Marketo Engage te beheren `[Package Tier]`&quot; op de knop &quot;Aan de slag&quot; om naar de toestemmingspagina te gaan.

`3.` Na de migratie gaat Marketo Engage van experience.adobe.com naar Adobe Experience Cloud. Gelieve te lijsten van gewenste personen alle die domeinen van Adobe [&#x200B; bij de bovenkant van dit artikel &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} worden vermeld om verstoring aan onze toegang van Marketo Engage te verhinderen.

`4.` **Facultatief:** opstelling SSO (Enig Sign On) in Adobe Admin Console.

* Voor gebruikers die zich bij SSO aanmelden op hun Adobe Identity die zich verder beweegt, dient u hulp te bieden bij de installatie van SSO in de Adobe Admin Console voordat de gebruikersmigratie plaatsvindt.

`5.` **Facultatief:** plaats een langer [&#x200B; maximumzittingsleven &#x200B;](https://helpx.adobe.com/nl/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} in Adobe Admin Console.

* Als u wilt voorkomen dat gebruikers zich vaak moeten aanmelden, past u de levensduur van de sessie in Geavanceerde instellingen met een langere duur aan.

Wij waarderen uw medewerking tijdens deze overgang. Laat me weten wanneer u deze stappen hebt uitgevoerd zodat ik verder kan gaan met de migratie.

met betrekking tot

`[Your Name]`

+++

* **verzend een e-mail naar de gebruikers van Marketo Engage**

Hieronder is een steekproefe-mail voor de gebruikers van Marketo Engage die **&#x200B;**&#x200B;geen beheerdervoorrechten hebben.

+++ Voorbeeld-e-mail met aankondiging van de aanstaande migratie

**Onderwerp: Belangrijke update-Migratie van de Abonnementen van Marketo Engage aan Adobe Admin Console**

Beste Marketo Engage-gebruikers,

We hebben een belangrijke aankondiging over onze Marketo Engage-instantie en hoe u zich gaat aanmelden. Adobe verplaatst Marketo Engage-abonnementen en -gebruikers naar Adobe Admin Console om ons in staat te stellen al hun productbeheer op één locatie te centraliseren. Dit heeft geen invloed op marketingworkflows, inhoud, integraties of elementen.

**Zeer belangrijke Details:**

* **Datum van de Migratie**: `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **Timing**: De migratie begint rond middernacht lokale tijd voor ons abonnement.

* **Effect**: Er zal geen verlies van de producttoegang tijdens gebruikersmigratie zijn. Als u bent aangemeld wanneer uw account wordt gemigreerd, wordt u na de migratie afgemeld en gevraagd u binnen enkele minuten weer aan te melden met Adobe Identity.

* **Voordelen**: Verifieer Marketo Engage en andere producten van Adobe door één enkele identiteit-of Adobe ID of Adobe Federated ID (SSO) te gebruiken.

**wat u moet doen:**

`1.` **voorbereidingen**: De e-mailcontrole wordt vereist voor u om aan een Identiteit van Adobe worden gemigreerd.

i. U hebt een e-mailverificatieaanvraag ontvangen met een koppeling (blijft drie dagen geldig). Als uw verbinding is verlopen, kunt u de verificatie-e-mail van binnen Marketo Engage opnieuw verzenden door uw &quot;Mijn pictogram van het Profiel&quot;te klikken, dan navigerend aan **Mijn Rekening** > **de Montages van de Rekening** > **opnieuw beëindigt Verificatie**.

ii. Een actieve gebruikerssessie is vereist om de e-mailverificatie te voltooien. Meld u eerst aan bij uw Marketo Engage-abonnement via de URL van uw identiteitsprovider (IdP).

`2.` **Onboard**: Zodra uw gebruikersrekening wordt gemigreerd, zult u een e-mail van Adobe betreffende de veranderingen in uw login methode ontvangen.

i. Accepteer de nieuwe uitnodiging door op de knop Uitnodiging accepteren te klikken en u aan te melden met Adobe Identity.

ii. Meld u aan bij een bestaande Adobe ID op de Adobe-aanmeldingspagina.

iii. U moet zich eerst bij de instantie van Marketo Engage voor om het even welke eerder met bladwijzer verklaarde URL op het engage-xx.marketo.com domein aanmelden u aan navigeert.

`3.` **Contact**: Als u om het even welke vragen hebt of hulp nodig nadat uw rekening wordt gemigreerd, of als uw rekening niet wordt gemigreerd en u toegang tot Marketo Engage verliest, te bereiken gelieve uit aan het de migratieteam van Marketo Engage bij `[your internal contact email/phone]`.

Wij waarderen uw medewerking tijdens deze overgang. Dank u voor uw begrip en inzet om onze systemen veilig te houden.

met betrekking tot

`[Your Name]`

+++
