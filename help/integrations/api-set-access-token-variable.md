---
title: Marketo How to API Video - Hoe te om het teken van de Toegang in een variabele te plaatsen
description: Leer hoe u de Postman-toepassing instelt en hoe u variabelen kunt gebruiken om gegevens in de variabele op te slaan voor herbruikbaarheidsdoeleinden.
feature: REST API
role: Admin, Developer
level: Experienced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
source-git-commit: 3243c3047efa1bcb92581a58aafe17689ff945fd
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# API Help - Het toegangstoken instellen in een variabele

Leer hoe u de Postman-toepassing instelt en variabelen gebruikt om gegevens in de variabele op te slaan voor herbruikbaarheidsdoeleinden. U zult ook leren hoe te om uw eerste vraag van het Marketo Engage REST API te maken om het toegangstoken te krijgen.

>[!PREREQUISITES]
>
>Voordat u deze video start, moet u een gebruikersnaam met alleen de API maken met een AOI-rol en een Launchpad-service maken. Voer de stappen in de onderstaande artikelen uit:
>
>* [&#x200B; creeer een slechtsAPI Rol van de Gebruiker &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user-role){target="_blank"} 
>
>* [&#x200B; creeer een slechts Gebruiker API &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user){target="_blank"} 
>
>* [&#x200B; creeer een Dienst van de Douane voor Gebruik met REST API &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api){target="_blank"} 

**Verwijzingen die in deze video worden gebruikt:**

* Marketo-eindpunt auth: `{{{}base_url{}}}/identity/oauth/token?grant_type=client_credentials&client_id={{{}client_id{}}}&client_secret={{{}client_secret{}}}`

* JS-script om toegang_token van de hoofdtekst van de reactie op te halen (plaatsen onder het tabblad Scripts:):

```
var jsonData = pm.response.json();
pm.environment.set("access_token", jsonData.access_token);
```

* [&#x200B; documentatie van de Ontwikkelaars van het Marketo Engage &#x200B;](https://experienceleague.adobe.com/nl/docs/marketo-developer/marketo/rest/authentication){target="_blank"} 

>[!VIDEO](https://video.tv.adobe.com/v/3453989/?learn=on&captions=dut)
