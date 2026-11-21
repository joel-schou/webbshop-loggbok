# Sprintloggbok

## Fram till Sprint 4

Jag fick äran att börja som Scrum Master för gruppen under Sprint 0. Under den sprinten ansvarade jag för att sätta upp email-service. Jag hjälpte även till med vår lokala utvecklingsmiljö så att alla kunde köra mikrotjänsterna på sina datorer.

Under Sprint 1 och Sprint 2 arbetade vi mycket tillsammans i gruppen. Vi skapade frontend, kopplade ihop den med våra tjänster och arbetade bland annat med inloggning, produkter, kundvagn och adminsidor. En stor del av arbetet gjordes genom Visual Studio Code Live Share. Då kodade en person medan de andra letade information, läste dokumentation och hjälpte till att kontrollera lösningen.

Under Sprint 3 arbetade jag med **FE-24**, där formuläret för nya produkter uppdaterades med kategori och bild, samt **FE-28**, där jag skapade sökfunktionen på produktsidan. Jag arbetade också med **FE-27** och fick email-service att skicka riktiga orderbekräftelser. Gruppen undersökte även olika betalningslösningar tillsammans.

Varje vecka börjar vi med att gå igenom det som har kommit in i backloggen. Vi går igenom de nya uppgifterna tillsammans och använder Planning Poker för att bedöma hur svåra de är. Därefter skriver vi sprintmål och delar upp arbetet. Vi byter Scrum Master efter varje sprint så att alla får prova på rollen.

---

## Sprint 4 – vecka 42

### Vad jag arbetade med

Den här sprinten fokuserade vi på att bygga en gateway mellan frontend och våra mikrotjänster. Uppgiften var ganska stor, så vi bestämde oss för att arbeta mycket tillsammans.

Min uppgift var att skapa grunden till gateway-service och lägga upp projektet på GitHub. Jag bjöd in resten av gruppen så att de kunde börja arbeta vidare med sina delar. Jag deltog även i det gemensamma arbetet med cookie- och JWT-hanteringen.

### Eventuella problem och hur jag löste dem

Vi lyckades få upp våra tjänster på Render, men vi blev inte helt klara med hur de skulle kopplas ihop på rätt sätt. Tiden räckte inte till, så det får bli nästa sprints problem.

### Samarbete och agilt arbete

På måndagen hade vi sprintplanering klockan 10 i vanlig ordning. Vi gick igenom Trello-tavlan och de uppgifter som var aktuella för veckan. När alla hade förstått vad uppgifterna innebar använde vi Planning Poker för att uppskatta hur svåra de var. Därefter fördelade vi arbetet och skrev våra sprintmål. Eftersom gateway-arbetet bestod av flera stora delar bestämde vi oss för att arbeta mycket tillsammans under veckan.

På tisdagar och torsdagar hade vi Daily Scrum efter lektionen. Övriga dagar hade vi mötet klockan 10. Eftersom vi arbetade gemensamt blev mötet ofta starten på dagens arbetspass, och vi fortsatte att arbeta tillsammans efter avstämningen.

Vi använde Live Share när vi arbetade tillsammans. Vi turades om att koda medan de andra letade information, hjälpte till att tolka materialet och kom med förslag på lösningar. På fredagen gjorde vi klart det sista och förberedde demon. Efteråt hade vi retrospektiv med Start, Stop och Continue, där vi pratade om vad som fungerade bra och vad vi kunde förbättra inför nästa sprint.

---

## Sprint 5 – vecka 43

### Vad jag arbetade med

Den här sprinten fortsatte vi med gateway-service och arbetade med att få inloggningen att fungera med JWT i cookies istället för sessionStorage. Målet var att användaren skulle fortsätta vara inloggad även när sidan laddades om och att behörigheterna skulle fungera som de skulle.

Vi arbetade bland annat med endpointen `/auth/me` i gateway-service och auth-service för att kunna hämta information om den inloggade användaren. Vi behövde även göra ändringar i frontend så att den kunde hantera inloggningen på det nya sättet.

Senare under veckan fokuserade vi på tester. Vi använde MSW (Mock Service Worker) för att simulera API-anrop och testa våra funktioner utan att behöva använda de riktiga mikrotjänsterna. Vi satte upp en testmiljö och testade bland annat användarhantering, produkter och felhantering.

Vi fortsatte även med driftsättningen på Render för att få frontend och våra mikrotjänster att fungera tillsammans.

### Eventuella problem och hur jag löste dem

Vi hade en del problem med att få JWT och cookies att fungera tillsammans med frontend. Bland annat slutade adminsidorna att fungera som de skulle efter ändringarna. Vi försökte lösa problemen genom att felsöka tillsammans och läsa dokumentation. Efter att vi fått hjälp under en lektion lyckades vi komma vidare och få inloggningen att fungera.

Vi stötte även på problem med driftsättningen på Render. Vissa delar av applikationen pekade fortfarande mot våra lokala adresser istället för tjänsterna på Render. Efter en del felsökning upptäckte vi även att Docker-imagen för auth-service inte hade uppdaterats med de senaste ändringarna. Vi arbetade därför med att rätta till konfigurationen och uppdatera vårt CI/CD-flöde.

### Samarbete och agilt arbete

På måndagen började vi som vanligt med sprintplanering. Vi gick igenom backloggen, använde Planning Poker för att uppskatta uppgifternas svårighetsgrad och satte upp våra sprintmål.

Vi fortsatte med Daily Scrum under veckan där vi gick igenom vad vi skulle arbeta med och vilka problem vi hade stött på. Eftersom flera uppgifter hängde ihop valde vi att fortsätta arbeta mycket tillsammans.

Vi använde Live Share och hjälptes åt med både kodning, informationssökning och felsökning. När någon fastnade kunde resten av gruppen komma med förslag och hjälpa till att hitta en lösning.

På fredagen gick vi igenom sprintens arbete och hade retrospektiv med Start, Stop och Continue, där vi diskuterade vad som fungerat bra och vad vi kunde förbättra inför nästa sprint.