### **Gruppövning: E-handelsplattform i Next.js**

-----

### **Produktbeskrivning**

Uppgiften är att bygga en **minimalistisk e-handelsplattform** för olika produkter med hjälp av **Next.js 15 App Router**. Plattformen ska visa upp ett urval av produkter från ett externt API, vara fullt responsiv och ha interaktiva inslag. Målet är att ni ska få praktisk erfarenhet av att arbeta med **Server Components**, **Client Components**, **statiska och dynamiska routes**, hantering av asynkron data och praktiskt agilt arbete i grupp.

-----

### **Ramverk & Teknologier**

  * **Next.js 15 (App Router):** Använd det senaste av Next.js för att utnyttja funktioner som Server Components och Server Actions. Se till att optimera med så mycket statiskt och server-renderat som möjligt.
  * **TypesScript:** Använd typescript i projektet
  * **DummyJSON API:** Använd API:et `https://dummyjson.com/products` eller `https://fakeapi.platzi.com/` för att hämta produktdata. Titta igenom APIerna tillsammans och se vilka för/nackdelar de har innan ni bestämmer er.
  * **React:** Arbeta med React-komponenter, både Server och Client.
  * **Valfri styling:** Använd den stylingmetod ni är bekväma med (CSS-moduler/Tailwind CSS).
  * **Git & GitHub:** Använd Git för versionskontroll och GitHub för samarbete.
  * **Projekthanteringsverktyg:** Använd GitHub Projects (agile/scrum board), Trello (kanban board) eller dylikt som alla i grupper kan komma åt och vara bekväma med att använda. Denna ska hela tiden hållas uppdaterad.
  * **WAVE:** Se till att ha fokus på och testa tillgängligheten under arbetet med WAVE eller dylikt.

-----

### **Funktionalitetskrav**

1.  **Startsida, Om oss, Kontakt:**
      * På startsidan - Visa en översikt av ett urval av produkter (kan vara ett antal som 20 st eller en/flera kategorier av produkter i grupp). Hämta och rendera produktdata på serversidan. Det ska också finnas en Hero med en CTA högst upp på sidan.
      * Om Oss - Gör en Lorem-text eller skriv ihop något bara för att ha något där samt en bild.
      * Kontakt - Formulär för få kontakt med företaget. Kravet här är rutor för e-post och meddelande till företaget och en knapp för att skicka. Vill man kan man lägga till titel (subject) och ev en drop-down för vilken typ av kontakt man önskar - Support, info, reklamation... Ingen faktiskt funktionalitet av denna krävs förutom tillgänglighet med typer, labels osv.
2.  **Produktsida:**
      * Skapa en dynamisk route (`/products/[id]`) som visar detaljerad information för en specifik produkt baserat på dess ID. Ni behöver inte ha all info som finns i API här, men titel, beskrivning, bild och pris är minsta kraven.
      * Hämta enskild produktdetalj från API:et och rendera på serversidan.
3.  **Interaktiva element (Client Components):**
      * Lägg till en **sökfunktion** och en fungerande **pagineringsfunktion** för att bläddra mellan olika sidor (sätt en fast gräns för antal/sida, om ni vill kan ni lägga till val för detta senare).
      * Inkludera en knapp för att **"Lägga till i varukorg"** (behöver inte ha en fungerande varukorg, det räcker att den visar en notifikation eller loggar en händelse).
4.  **Frivilligt:** Skapa funktionalitet för att skicka kontaktformuläret och skapa upp så att personen som skriver i får en visuell indikation på att det lyckats (ingen funktionalitet med e-post osv behövs).
5.  **Frivilligt:** Ev annan funktionalitet som ni ser kan vara intressant som visa recensioner, utvalda produkter, filtrerar på kategorier, skicka e-post via kontaktformulär eller dylikt. Tänk bara på att inte dra iväg med extra saker innan allt annat är på plats och faktiskt bra utfört.

-----

### **Design**

Vi lämnar ingen färdig design på detta, men ni behöver se till att allt som finns i krav är med. För att inte låta det gå för lång tid rekommenderar vi att ni väljer en design utifrån något av förslagen på t ex `https://www.figma.com/community/website-templates/ecommerce?resource_type=mixed&editor_type=all&price=free` eller bildgooglar "e-commerce designs" och väljer en där. Det finns också sidor som denna som ni kan få inspiration från: `https://www.frontendmentor.io/challenges/product-list-with-cart-5MmqLVAp_d` Sedan gör ni ev modifieringar för att den ska passa detta syfte. Innan ni sedan börjar koda vill vi att ni skickar oss ert förslag på detta. Något liknande detta bör vara helt ok (med lite ändringar) <img width="2533" height="1092" alt="image" src="https://github.com/user-attachments/assets/5809977b-a719-4ec2-b8e7-313d3adb1ec4" />

-----

### **Arbetsflöde & Sprintplan (3-4 veckor)**

Den preliminära planen är på 3 veckor, men ev kommer det en del 2 av arbetet som kommer då vara vecka 3-4. Detta beroende på hur arbetet går i grupperna och vad vi hinner med.
Denna uppgift är därför uppdelad i 3 sprints, en för varje vecka. Varje sprint fokuserar på specifika delmål. Detta är bara förslag och ni kan själva bestämma om ni vill fördela det på annat sätt. Det finns ingen produktägare i detta projekt så det är upp till er att ha användaren i fokus i arbetet med design och funktionalitet. Det ska vara tydligt och enkelt för den som tittar på sidan att hitta det man vill och behöver (oavsett ev handikapp osv).

**Innan ni börjar att koda se till att allt är förberett i ert SCRUM board, att ni har valt design och beslutat vem som börjar med vad. Vi vill också att ni visar upp detta för oss lärare och får klartecken innan ni sätter igång med något mer.**

#### **Övergripande arbetsflöde:**

  * **Sprintplanering:** I början av varje vecka går ni igenom veckans mål och fördelar ansvar och uppdaterar löpande er scrum board. Varje person väljer själv sina ansvar, vissa kort kommer vara spärrade då PR inte är granskad/mergad ännu och då väljer ni bara ett annat.
  * **Löpande arbete:** Arbeta i era egna branches, gör regelbundna `git commit`-operationer och `git push` till er branch (en för varje feature/card/issue).
  * **Kodgranskning:** I slutet av varje vecka/dag (t.ex. fredag) presenterar ni era slutförda delmål, skapar **Pull Requests (PRs)** och granskar varandras kod (detta kan också ske löpande under veckan vid behov). När koden är godkänd mergas den in i `main`-branchen.
  * **Feedback & Justering:** Efter granskningen ger ni feedback och justerar eventuella brister innan ni påbörjar nästa sprint.

#### **Dagliga rutiner för effektivt samarbete**

För att underlätta samarbetet och säkerställa att ni hela tiden rör er framåt som en grupp, kan ni införa några enkla men effektiva dagliga rutiner. Detta hjälper er att hantera hinder i tid och hålla koll på allas framsteg.

  * **Morgonmöte (ca 10-15 minuter):** Håll ett kort dagligt möte, gärna på morgonen. Varje person delar kort vad de planerar att arbeta med under dagen. Berätta om eventuella problem eller hinder du stött på, så att gruppen kan hjälpa till att lösa dem.
  * **Dedikerad tid för Pull Requests (PR):** Att skicka in en **Pull Request** är inte slutet på en uppgift, utan början på en diskussion och ett samarbete. Bestäm en tid varje dag då ni går igenom aktiva PR:s, lämnar feedback och granskar varandras kod. Detta är helt okej att bara göra i par och i mån av behov.
  * **Arbeta i små, avgränsade delar:** Arbeta gärna med små och hanterbara uppgifter. Bryt ner stora kort som ”Bygg produktsidan” till mindre delar som ”Hämta produktdatan från API:et” eller ”Rendera produktbild och titel”. Detta undviker **merge conflicts** och ger en tydlig känsla av framsteg.

-----

### **Sprint 1: Grundläggande struktur (Vecka 1)**

**Mål:** Planera grunderna. Sätt upp Next.js-projektet och skapa meny och de statiska sidorna.

  * Välj API, UX design att utgå från, ev bibliotek som ni vill använda (t ex Tailwind). **Detta ska förmedlas till oss lärare som ska godkänna innan ni börjar kodandet.**
  * Skapa ett nytt Next.js-projekt med App Router.
  * Rensa bort templatekod (eller alternativt gör ett tomt projekt och skapa själv grundstrukturen).
  * Skapa upp menyer och grundstruktur på projektet
  * Hämta all produktdata från API endpoint för detta och rendera en lista av produkttitel, bild, pris osv på startsidan.
  * Gör grundläggande layout/design för startsidan.

-----

### **Sprint 2: Dynamisk routing & Interaktion (Vecka 2)**

**Mål:** Bygg de dynamiska sidorna och lägg till de första interaktiva elementen.

  * Skapa den dynamiska routen `app/products/[id]/page.tsx` för produktsidorna.
  * Hämta en specifik produkts data baserat på ID och rendera detaljerad information.
  * Lägg till **sökfunktion** och **paginering** där det är aktuellt. Använd client/server-components i samarbete med varandra för att lösa detta.
  * Lägg till "Lägg till i varukorg"-knappen på produktsidan (behöver inte vara fungerande utan räcker med en indikation att en vara lagts till).

-----
### **Sprint 3: Skapa & Ta bort produkter (Vecka 3)**
**Mål:** Implementera grundläggande CRUD-funktioner.

* Skapa en ny route, t.ex. `app/admin/page.tsx`, för admingränssnittet.
* **Read (Läs):** På adminvyn, visa en lista över alla produkter. 
* **Create (Skapa):** Lägg till en knapp för att skapa nya produkter på översiktssidan. Skapa ett formulär för att lägga till en ny produkt (titel, beskrivning, pris, etc.). Använd en **Server Action** för att hantera formulärdata och "skapa" produkten genom att logga den till konsolen (om ni inte använder Platzi, då kan ni göra det på riktigt).
* **Delete (Ta bort):** Lägg till en "Ta bort"-knapp vid varje produkt i adminvyn. Använd en **Server Action** för att hantera raderingen.
* **Frivilligt - Update (Uppdatera):** Gör en knapp vid sidan av ta bort för att uppdatera och en sida för det.
* 
-----

### **Sprint 4: Slutputs (Vecka 4)**

**Mål:** Slutför designen, optimering och förbereda presentation.

  * **Refaktorera** koden för att göra den mer läsbar, återanvändbar och effektiv.
  * Se också till att **optimera** med t ex generateStaticParams, lämplig metadata och suspense/loading.tsx.
  * Se över hela applikationens **responsivitet** och **design** för en sista puts.
  * Kontrollera **tillgängligheten** med WAVE eller dylikt
  * Ev redovisning/presentation av projektet (beroende på om det blir en del 2 eller ej)

  -----

### Reflektion
Detta görs individuellt. 

Detta avsnitt ska skrivas individuellt av varje gruppmedlem i README-filen. Syftet är att du reflekterar över ditt bidrag, hur grupparbetet fungerade, samt de tekniska utmaningar du mötte och lärde dig av. Håll dig gärna kortfattad.

1. Bidrag till projektet
* Beskriv kortfattat vad ditt primära bidrag till projektet var. Nämn de viktigaste funktionaliteterna eller sidorna du ansvarade för (t.ex. "Ansvarade för att sätta upp den dynamiska /products/[id]-routen och hämta detaljdata på servern" eller "Implementerade sökfunktionen med useSearchParams i en Client Component").

* Vilka kort/uppgifter i er Scrum Board/Kanban Board var dina viktigaste bidrag?

* Vilka tekniker eller komponenter jobbade du mest med (t.ex. Server Actions, fetch i Server Components, TypeScript-typning, etc.)?

2. Lärdomar och Utmaningar
Reflektera över det som var mest utmanande, spännande eller lärorikt under projektet.

* Tekniskt genombrott: Vilken del av Next.js/TypeScript/React var svårast att greppa i början, men som du nu känner dig mer bekväm med?

* Största utmaningen: Vilket problem tog längst tid att lösa, och hur löste du det?

* Bäst fungerande: Vilken kod/lösning känner du dig mest nöjd med, och varför? (T.ex. ett elegant sätt att hantera state eller en optimerad datahämtning.)


  ---

### **Redovisning**

Ni kommer bli tilldelade tvärgrupper där ni ger en demonstration av er app. Instruktionerna känner ni nog igen från Pokédex-demon. **Kom ihåg att du är en representant för gruppen och inte vad du själv gjort i projektet.**
1. Berätta vilka ni var i ert projekt och vad ert fokus var när det gällde API, design och andra beslut ni tog i början.
2. Gör en översiktligt demonstration av funktionalitet i appen, berätta kort vad ni gjort enligt uppgiftens specifikationer och om det är något ni inte lyckats få till, men gå inte in på detaljer.
3. Därefter väljer ni en eller två funktionaliteter i appen ni vill prata lite mer om. **Det ska inte vara en del du gjort själv, så se till att du förstår koden du ska prata om.** (Det är inte viktigt vem som skrivit koden och du ska inte nämna namn här).
4. Beskriv hur ni i gruppen löst det, men visa inte kod, berätta istället med ord/tekniska termen så gott ni kan. Använd ord som "client components", "searchParams" osv som vi jobbat med.
5. Gruppens medlemmar får också möjlighet att ställa frågor på ett sätt så alla förstår hur du tänkt. Ingen kritik eller förslag till andra lösningar här utan bara klargörande frågor.
6. När allt är tydligt och klart ges möjlighet för alla i gruppen att ge kort, positiv och konstruktiv feedback - om man vill. Det kan vara att ni tyckte det var en intressant lösning med fetch eller att det var snyggt gjort med hur responsiv menyn var osv. Försök att vara mer än bara "snyggt", "bra" då det ofta mest bara blir oklart.
7. Ta sedan en kort runda där ni säger något som ni tyckte var utmanande/spännande/intressant i koden när ni arbetade med den (alltså inte i uppgiften/API i sig utan enbart tekniskt).
   
---



