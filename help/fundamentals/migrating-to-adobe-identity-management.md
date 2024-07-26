---
title: Migreren naar Adobe Identity Management
description: Deze zelfstudie helpt u bij het migreren van uw abonnementen op Marketo's Engage en gebruikers naar de Adobe Admin Console.
role: User
level: Beginner
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: a1248a4367a283bd1922269db3be8ed146f85648
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 0%

---

# Migreren naar Adobe Identity Management

Adobe verbetert hoe u uw Adobe Marketo Engage-abonnementen en -gebruikers beheert. Wij brengen verhoogde productiviteit aan uw organisatie door uw abonnementen van de Marketo Engage en gebruikers naar Adobe Admin Console te migreren.

Deze zelfstudie helpt u om door de migratie te navigeren, zodat u Adobe Marketo Engage samen met andere Adobe-accounts en -producten voor uw gebruikers op een centrale locatie kunt beheren. De migratie is noodzakelijk en heeft geen invloed op uw marketingworkflow, inhoud, integratie of middelen.

## Controlelijst voor migratie voor beheerders van Marketo&#39;s Engage {#pre-migration-checklist-for-marketo-engage-administrators}

Om ervoor te zorgen dat uw organisatie Adobe Marketo Engage naar de Adobe Admin Console kan migreren, raden we u aan de onderstaande checklist te volgen om de komende wijzigingen te beheren.

### 1. Identificeer uw systeembeheerder(s) en bespreek de acties die zij moeten ondernemen {#identify-your-system-administrators}

* Als u niet zeker bent wie de Beheerders van het Systeem binnen uw organisatie zijn, contacteer uw team van de Rekening van de Adobe, of reep aan de Steun van de Adobe `marketocares@marketo.com`.

* Bevestig de Adobe Admin Console (of Adobe Org) waarnaar uw abonnement(en) op het Marketo Engage wordt gemigreerd.  Abonnement(s) van het Marketo Engage moet in de zelfde organisatie zoals [ worden opgesteld Dynamic Chat ](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview) {target="_blank"}, een inheemse hulpmiddel van de gespreksautomatisering die met Marketo Engage wordt geïntegreerd. [ leer meer ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete) {target="_blank"}

* **Facultatief:** [ voert Enig Ondertekenen (SSO) uit ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete) {target="_blank"} vóór gebruikersmigratie.

* Leer wat met uw Beheerders van het Systeem in de [ E-mailsectie van de Steekproef ](#announce-the-migration-timeline) te communiceren.

### 2. Zich bewust maken van de veranderingen en de gevolgen van migratie naar Adobe-identiteit {#familiarize-yourself-with-the-changes}

In de video hieronder, begeleidt het team van het Beheer van het Product van het Marketo Engage u door de migratiereis en wat te verwachten.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?t=170/?quality=12&learn=on){transcript=true}

Meer hulp op dit onderwerp voor de beheerders van het Marketo Engage kan in de volgende hulpartikelen worden gevonden:

* ](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup) {target="_blank"} checklist van de Opstelling van 0} Gebruiker[

* [ het Overzicht van Identity Management van de Adobe ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview) {target="_blank"}

* [ Begrijpend het Abonnement van Marketo en de Migratie van de Gebruiker aan Adobe Admin Console ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) {target="_blank"}

* [ migrerend aan de Identiteit van de Adobe met de Console van de Migratie ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity) {target="_blank"}

* [ Begrijp hoe te om Adobe Admin Console ](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) te gebruiken {target="_blank"}

### 3. Geef uw interne teams een overzicht van het tijdschema en de voorbereiding voor de migratie {#announce-the-migration-timeline}

* Markeer de migratiedatum op de agenda&#39;s van de beheerders en gebruikers van het Marketo Engage zodra deze gepland zijn.

   * U kunt de migratiedatum in **Admin** wijzigen > **de Console van de Migratie** > **pre-Migratie** om uw interne chronologie beter aan te passen. Leer meer over het opnieuw plannen en de beperkingen van [ het wijzigen van uw migratiedatum ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration) {target="_blank"}.

* **verzend een e-mail naar uw Beheerders van het Systeem**

Hieronder ziet u een voorbeeld-e-mail die u naar uw systeembeheerders kunt verzenden. Meestal beheert uw IT-afdeling al uw Adobe licenties.

`---------------------------------------------------`

**Onderwerp: Steun nodig-Migratie van de Abonnementen van het Marketo Engage aan Adobe Admin Console**

Beste `[IT Administrator/NAME]`,

Ons abonnement op Marketo&#39;s Engage wordt binnenkort gemigreerd naar het Adobe Identity Management System. `[Marketing Operation team]` heeft uw hulp nodig om sommige vereiste stappen te voltooien alvorens de gebruikersmigratie begint, om de gevolgen voor de gebruikers van de Marketo Engage te minimaliseren.

`1.` Bevestig of de organisatie al andere Adobe producten beheert in Adobe Admin Console(s) en of het Marketo Engage naar dezelfde console wordt gemigreerd.

* Abonnementen van Marketo&#39;s Engage moeten zich in dezelfde organisatie bevinden als Dynamic Chat, een native hulpprogramma voor gespreksautomatisering dat is geïntegreerd met Marketo Engage.

* Neem contact op met de Adobe Support op `marketocares@marketo.com` en CC ons als u vragen of problemen hebt met de Admin Console.

`2.` Ga naar de zoekopdracht voor een e-mailbericht vanuit de Adobe met de onderwerpregel &quot;Handeling vereist voor het beheren van gebruikerstoegang tot Adobe Marketo Engage `[Package Tier]`&quot;. Dit e-mailbericht is verzonden nadat de licenties voor het Marketo Engage op onze Admin Console zijn ingericht. Alleen systeembeheerders ontvangen deze e-mail. Gelieve ons onmiddellijk op de hoogte te brengen wanneer u het ontvangt.

* De Adobe kan om toestemming van u, de Beheerder van het Systeem van de Admin Console, verzoeken om gebruikers automatisch aan de bestaande console van onze organisatie te migreren. Klik in de e-mail met de onderwerpregel &quot;Handeling vereist om gebruikerstoegang tot Adobe Marketo Engage te beheren `[Package Tier]`&quot; op de knop &quot;Aan de slag&quot; om naar de toestemmingspagina te gaan.

`3.` **Facultatief:** Vestiging SSO (Enige Sign On) op Adobe Admin Console.

* Om onze gebruikers te helpen die zich bij SSO aanmelden op hun Adobe Identity die zich verder beweegt, verzoeken wij u om u te helpen bij de installatie van SSO op de Adobe Admin Console voordat de gebruikersmigratie plaatsvindt.

Wij waarderen uw medewerking tijdens deze overgang. Laat me weten wanneer u deze stappen hebt uitgevoerd zodat ik verder kan gaan met de migratie.

met betrekking tot

`[Your Name]`

`---------------------------------------------------`

* **verzend een e-mail naar de gebruikers van het Marketo Engage**

Hieronder ziet u een voorbeeld van een e-mail waarmee u de aanstaande migratie kunt aankondigen naar gebruikers van uw Marketo Engage die geen beheerdersrechten hebben.

`---------------------------------------------------`

**Onderwerp: Belangrijke update-Migratie van de Abonnementen van het Marketo Engage aan Adobe Admin Console**

Beste gebruikers van Marketo&#39;s Engage,

We hebben een belangrijke mededeling over ons Marketo Engage-exemplaar en over de manier waarop u zich gaat aanmelden. Adobe verplaatst abonnementen en gebruikers van Marketo&#39;s Engage naar de Adobe Admin Console om ons in staat te stellen al hun productbeheer op één locatie te centraliseren. Dit heeft geen invloed op marketingworkflows, inhoud, integraties of elementen.

**Zeer belangrijke Details:**

* **Datum van de Migratie**: `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **Timing**: De migratie begint rond middernacht lokale tijd voor ons abonnement.

* **Effect**: Er zal geen verlies van de producttoegang tijdens gebruikersmigratie zijn. Als u bent aangemeld wanneer uw account wordt gemigreerd, wordt u na de migratie afgemeld en gevraagd u binnen enkele minuten weer aan te melden met de Adobe Identity.

* **Voordelen**: Verifieer Marketo Engage en andere producten van de Adobe door één enkele Adobe te gebruiken identiteit-of Adobe ID of Federated ID van de Adobe (SSO).

**wat u moet doen:**

`1.` **voorbereidingen treffen**: De e-mailcontrole wordt vereist voor u om aan een Identiteit van de Adobe worden gemigreerd.

i. U hebt een e-mailverificatieaanvraag ontvangen met een koppeling (blijft drie dagen geldig). Als uw verbinding is verlopen, kunt u de verificatie-e-mail van binnen Marketo Engage opnieuw verzenden door uw &quot;Mijn pictogram van het Profiel&quot;te klikken, dan navigerend aan **Mijn Rekening** > **de Montages van de Rekening** > **opnieuw beëindigt Verificatie**.

ii. Een actieve gebruikerssessie is vereist om de e-mailverificatie te voltooien. Meld u eerst aan bij uw abonnement op het Marketo Engage met de URL van uw identiteitsprovider (IdP).

`2.` **Onboard**: Zodra uw gebruikersrekening wordt gemigreerd, zult u een e-mail van Adobe betreffende de veranderingen in uw login methode ontvangen.

i. Accepteer de nieuwe uitnodiging door op de knop Uitnodiging accepteren te klikken en u aan te melden met Adobe Identity.

ii. Meld u aan bij een bestaande Adobe ID op de aanmeldingspagina van de Adobe.

`3.` **Contact**: Als u om het even welke vragen hebt of hulp nodig nadat uw rekening wordt gemigreerd, of als uw rekening niet wordt gemigreerd en u toegang tot Marketo Engage verliest, te bereiken gelieve uit aan het team van de Marketo Engage bij `[your internal contact email/phone]`.

Wij waarderen uw medewerking tijdens deze overgang. Dank u voor uw begrip en inzet om onze systemen veilig te houden.

met betrekking tot

`[Your Name]`

`---------------------------------------------------`
