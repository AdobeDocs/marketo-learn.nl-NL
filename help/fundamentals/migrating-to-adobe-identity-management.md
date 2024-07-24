---
title: Migreren naar Adobe Identity Management
description: Beschrijving binnenkort beschikbaar.
role: User
level: Beginner
hide: true
hidefromtoc: true
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: f6ae52b43770789c24237f0bc664d33541469a50
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Migreren naar Adobe Identity Management

Adobe verbetert hoe u uw Adobe Marketo Engage-abonnementen en -gebruikers beheert. Wij brengen verhoogde productiviteit aan u en uw organisatie door uw abonnementen van de Marketo Engage en gebruikers naar Adobe Admin Console te migreren.

Met deze zelfstudie kunt u door de migratie navigeren, zodat u Adobe Marketo Engage samen met andere accounts en producten voor Adoben voor uw gebruikers op een centrale locatie kunt beheren. De migratie is noodzakelijk en heeft geen invloed op uw marketingworkflow, inhoud, integratie of middelen.

## Controlelijst voor migratie voor beheerders van Marketo&#39;s Engage {#pre-migration-checklist-for-marketo-engage-administrators}

Om ervoor te zorgen dat uw organisatie Adobe Marketo Engage naar de Adobe Admin Console kan migreren, raden we u aan de onderstaande checklist te volgen om de komende wijzigingen te beheren.

### 1. Identificeer uw systeembeheerder(s) en bespreek de acties die zij moeten ondernemen {#identify-your-system-administrators}

* Als u niet zeker bent wie de Beheerders van het Systeem binnen uw organisatie zijn, contacteer uw team van de Rekening van de Adobe, of reep aan de Steun van de Adobe `marketocares@marketo.com`.

* Bevestig de Adobe Admin Console (of Adobe Org) waarnaar uw abonnement(en) op het Marketo Engage wordt gemigreerd.  Abonnementen van Marketo&#39;s Engage moeten worden geïmplementeerd in dezelfde organisatie als Dynamic Chat, een native gespreksautomatiseringsprogramma dat is geïntegreerd met Marketo Engage.
  `TBD LINK TO https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete`

* Leer meer over hoe te met uw Beheerders van het Systeem in de [ E-mailsectie van de Steekproef ](#announce-the-migration-timeline) te communiceren.

### 2. Zich bewust maken van de veranderingen en de gevolgen van migratie naar Adobe-identiteit {#familiarize-yourself-with-the-changes}

In de video hieronder, begeleidt het team van het Beheer van het Product van het Marketo Engage u door de migratiereis en wat te verwachten.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?quality=12&learn=on){transcript=true}

Meer hulp op dit onderwerp voor de beheerders van het Marketo Engage kan in de volgende hulpartikelen worden gevonden:

* ](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup) {target="_blank"} checklist van de Opstelling van 0} Gebruiker[

* [ het Overzicht van Identity Management van de Adobe ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview) {target="_blank"}

* [ Begrijpend het Abonnement van Marketo en de Migratie van de Gebruiker aan Adobe Admin Console ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) {target="_blank"}

* [ migrerend aan de Identiteit van de Adobe met de Console van de Migratie ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity) {target="_blank"}

* [ Begrijp hoe te om Adobe Admin Console ](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) te gebruiken {target="_blank"}

### 3. Geef uw interne teams een overzicht van het tijdschema en de voorbereiding voor de migratie {#announce-the-migration-timeline}

* Markeer de migratiedatum op de agenda&#39;s van de beheerders en gebruikers van het Marketo Engage zodra deze gepland zijn.

U kunt de migratiedatum in **Admin** wijzigen > **Console van de Migratie** > **pre-Migratie** om beter met uw interne chronologie te richten. Leer meer over het opnieuw plannen en de beperkingen van [ het wijzigen van uw migratiedatum ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration) {target="_blank"}.

* Verzend een e-mail om met uw Beheerders van het Systeem te communiceren.

Hieronder ziet u een voorbeeld-e-mail die u naar uw systeembeheerders kunt verzenden. Meestal beheert uw IT-afdeling al uw Adobe licenties.

`---------------------------------------------------`

**Onderwerp: Steun nodig-Migratie van de Abonnementen van het Marketo Engage aan Adobe Admin Console**

Beste `[IT Administrator/NAME]`,

Ons abonnement op Marketo&#39;s Engage wordt binnenkort gemigreerd naar het Adobe Identity Management System. Het [ team van de Verrichting van de Marketing ] heeft uw hulp nodig om sommige vereiste stappen te voltooien alvorens de gebruikersmigratie begint, om het effect op de gebruikers van het Marketo Engage te minimaliseren

`1.` Bevestig of de organisatie al andere Adobe producten beheert in Adobe Admin Console(s) en of het Marketo Engage naar dezelfde console wordt gemigreerd.

* Merk op dat de abonnementen van het Marketo Engage in de zelfde organisatie zoals Dynamic Chat moeten zijn, een native gespreksautomatiseringshulpmiddel dat met Marketo Engage wordt geïntegreerd.

* Als u zorgen hebt of vragen hebt over de Admin Console waaraan Marketo Engage wordt toegevoegd, neemt u contact op met het ondersteuningsteam op `marketocares@marketo.com` en neemt u ons op in uw communicatie.

`2.` Ga naar de zoekopdracht voor een e-mailbericht vanuit de Adobe met de onderwerpregel &quot;Handeling vereist voor het beheren van gebruikerstoegang tot Adobe Marketo Engage `[Package Tier]`&quot;. Dit e-mailbericht is verzonden nadat de licenties voor het Marketo Engage op onze Admin Console zijn ingericht. Alleen systeembeheerders ontvangen deze e-mail. Gelieve ons onmiddellijk op de hoogte te brengen wanneer u het ontvangt.

* De Adobe kan om toestemming van u, die de Beheerder van het Systeem van de Admin Console is, vragen om gebruikers automatisch aan de bestaande console van onze organisatie te migreren. Klik in de e-mail met de onderwerpregel &quot;Handeling vereist om gebruikerstoegang tot Adobe Marketo Engage te beheren `[Package Tier]`.&quot; op de knop &quot;Aan de slag&quot; om naar de toestemmingspagina te gaan.

`3.` **Facultatief:** Vestiging SSO (Enige Sign On) op Adobe Admin Console.

* Om onze gebruikers te helpen zich aan te melden bij SSO op hun Adobe Identity die zich verder beweegt, verzoeken wij u om u te helpen bij de installatie van SSO op Adobe Admin Console voordat de gebruikersmigratie plaatsvindt.
Wij waarderen uw medewerking tijdens deze overgang. Laat me weten wanneer u deze stappen hebt voltooid zodat ik met gebruikersmigratie met Marketo Engage kan verdergaan.
met betrekking tot

`[Your Name]`

`---------------------------------------------------`

* Stuur een e-mail naar gebruikers van het Marketo Engage.

Hieronder ziet u een voorbeeld van een e-mail waarmee u de aanstaande migratie kunt aankondigen naar gebruikers van uw Marketo Engage die geen beheerdersrechten hebben.

`---------------------------------------------------`

**Onderwerp: Belangrijke update-Migratie van de Abonnementen van het Marketo Engage aan Adobe Admin Console**

Beste gebruikers van Marketo&#39;s Engage,

We hebben een belangrijke mededeling over ons Marketo Engage-exemplaar en over de manier waarop u zich gaat aanmelden. Adobe verplaatst abonnementen en gebruikers van Marketo&#39;s Engage naar de Adobe Admin Console om hun klanten in staat te stellen al hun productbeheer op één plaats te centraliseren. Dit heeft geen invloed op marketingworkflows, inhoud, integraties of elementen.

Belangrijkste details:

* De Datum van de migratie: [ specificeer de geplande datum - te vinden gelieve dit in Marketo Engage onder **Admin** > **Console van de Migratie** > **pre-migratie**]

* Timing: de migratie begint rond middernacht lokale tijd voor ons abonnement.

* Effect: tijdens de migratie van gebruikers zal de toegang tot het product niet verloren gaan. Als u bent aangemeld wanneer uw account wordt gemigreerd, wordt u na de migratie afgemeld en gevraagd u binnen enkele minuten weer aan te melden met de Adobe Identity.

* Voordelen: Verifieer Marketo Engage en andere producten van de Adobe door één enkele Adobe identiteit, of Adobe ID of Federated ID van de Adobe (SSO) te gebruiken.

Wat u moet doen:

`1.` Voorbereiden: e-mailverificatie is vereist voor migratie naar een Adobe-id.

i. U hebt een e-mailverificatieaanvraag ontvangen met een koppeling (blijft drie dagen geldig). Als uw verbinding is verlopen, kunt u de verificatie-e-mail opnieuw verzenden door **Admin** te gaan > **Mijn Rekening** > **de Montages van de Rekening** en **te klikken herstelt Verificatie**.
ii. Een actieve gebruikerssessie is vereist om e-mailverificatie te voltooien. Meld u eerst aan bij uw abonnement op het Marketo Engage met de URL van uw identiteitsprovider (IdP).

`2.` Aan boord: wanneer uw gebruikersaccount is gemigreerd, ontvangt u een e-mail van de Adobe over de wijzigingen in uw aanmeldingsmethode.

i. Accepteer de nieuwe uitnodiging door op de knop Uitnodiging accepteren te klikken en u aan te melden met Adobe Identity.
ii. Meld u aan bij een bestaande Adobe ID op de aanmeldingspagina van de Adobe.

`3.` Contact: Als u om het even welke vragen hebt of hulp nodig nadat uw rekening wordt gemigreerd of als uw rekening niet wordt gemigreerd en u toegang tot Marketo Engage verliest, te bereiken gelieve uit aan het team van de Marketo Engage van de migratie bij [ uw interne contact e-mail/telefoon ].

Wij waarderen uw medewerking tijdens deze overgang. Dank u voor uw begrip en inzet om onze systemen veilig te houden.

Best

[ Uw Naam ]

`---------------------------------------------------`
