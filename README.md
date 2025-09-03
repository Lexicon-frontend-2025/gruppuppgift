### **Gruppövning: E-handelsplattform i Next.js**

---

### **Produktbeskrivning**
Uppgiften är att bygga en **minimalistisk e-handelsplattform** för olika produkter med hjälp av **Next.js 15 App Router**. Plattformen ska visa upp ett urval av produkter från ett externt API, vara fullt responsiv och ha interaktiva inslag. Målet är att ni ska få praktisk erfarenhet av att arbeta med **Server Components**, **Client Components**, **statiska och dynamiska routes**, hantering av asynkron data och praktiskt agilt arbete i grupp.

---

### **Ramverk & Teknologier**
* **Next.js 15 (App Router):** Använd det senaste av Next.js för att utnyttja funktioner som Server Components och Server Actions. Se till att optimera med så mycket statiskt och server-renderat som möjligt. 
* **TypesScript:** Använd typescript i projektet
* **DummyJSON API:** Använd API:et `https://dummyjson.com/products` (alternativt `https://fakeapi.platzi.com/`) för att hämta produktdata.
* **React:** Arbeta med React-komponenter, både Server och Client.
* **Valfri styling:** Använd den stylingmetod ni är bekväma med (CSS-moduler/Tailwind CSS).
* **Git & GitHub:** Använd Git för versionskontroll och GitHub för samarbete.
* **Projekthanteringsverktyg:** Använd GitHub Projects (agile/scrum board), Trello (kanban board) eller dylikt som alla i grupper kan komma åt och vara bekväma med att använda. Denna ska hela tiden hållas uppdaterad.
* **WAVE/Tillgänglighet:** Se till att testa tillgängligheten under arbetet med WAVE eller dylikt.

---

### **Funktionalitetskrav**
1.  **Startsida, Om oss, Kontakt:**
    * På startsidan - Visa en översikt av ett urval av produkter (kan vara ett antal som 20 st eller en/flera kategorier av produkter i grupp). Hämta och rendera produktdata på serversidan. Det ska också finnas en Hero med en CTA högst upp på sidan.
    * Om Oss - Gör en Lorem-text eller skriv ihop något bara för att ha något där samt en bild.
    * Kontakt - Ett tomt formulär med lämpliga labels osv (funktionalitet för detta är frivilligt)
2.  **Produktsida:**
    * Skapa en dynamisk route (`/products/[id]`) som visar detaljerad information för en specifik produkt baserat på dess ID. Ni behöver inte ha all info som finns i API här, men titel, beskrivning, bild och pris är minsta kraven.
    * Hämta enskild produktdetalj från API:et och rendera på serversidan.
3.  **Interaktiva element (Client Components):**
    * Lägg till en knapp för att **filtrera produkter** efter en kategori och/eller en fungerande pagineringsfunktion för att bläddra mellan olika sidor (sätt en gräns för antal/sida)
    * Inkludera en knapp för att **"Lägga till i varukorg"** (behöver inte ha en fungerande varukorg, det räcker att den visar en notifikation eller loggar en händelse).
4.    **Kontaktformulär:** Skapa funktionalitet för att skicka formuläret och skapa upp så att personen som skriver i får en visuell indikation på att det lyckats och en bekräftelse via e-post. 
5.    **Frivilligt: Övrigt:** Ev annan funktionalitet som ni ser kan vara intressant som visa recensionser, utvalda produkter eller dylikt. Tänk bara på att inte dra iväg med extra saker innan allt annat är på plats och faktiskt bra utfört.

---

### **Design**
Vi lämnar ingen färdig design på detta, men ni behöver se till att allt som finns i krav är med. För att inte låta det gå för lång tid rekommenderar vi att ni väljer en design utifrån något av förslagen på t ex `https://www.figma.com/community/website-templates/ecommerce?resource_type=mixed&editor_type=all&price=free` eller bildgooglar "e-commerce designs" och väljer en där. Sedan gör ni ev modifieringar för att den ska passa detta syfte. Innan ni sedan börjar koda vill vi att ni skickar oss ert förslag på detta.

---

### **Arbetsflöde & Sprintplan (3-4 veckor)**
Den preliminära planen är på 3 veckor, men ev kommer det en del 2 av arbetet som kommer då vara vecka 3-4. Detta beroende på hur arbetet går i grupperna och vad vi hinner med.
Denna uppgift är därför uppdelad i 3 sprints, en för varje vecka. Varje sprint fokuserar på specifika delmål. Detta är bara förslag och ni kan själva bestämma om ni vill fördela det på annat sätt.

#### **Övergripande arbetsflöde:**
* **Sprintplanering:** I början av varje vecka går ni igenom veckans mål och fördelar ansvar och uppdaterar löpande er scrum board.
* **Löpande arbete:** Arbeta i era egna branches, gör regelbundna `git commit`-operationer och `git push` till er branch.
* **Kodgranskning:** I slutet av varje vecka (t.ex. fredag) presenterar ni era slutförda delmål, skapar **Pull Requests (PRs)** och granskar varandras kod (detta kan också ske löpande under veckan vid behov). När koden är godkänd mergas den in i `main`-branchen.
* **Feedback & Justering:** Efter granskningen ger ni feedback och justerar eventuella brister innan ni påbörjar nästa sprint.

---

### **Sprint 1: Grundläggande struktur (Vecka 1)**
**Mål:** Sätt upp Next.js-projektet och skapa meny och de statiska sidorna.

* Skapa ett nytt Next.js-projekt med App Router.
* Skapa en `page.js` för startsidan (root route).
* Hämta all produktdata från `dummyjson.com/products` och rendera en lista av produkttitel, bild, pris osv på startsidan. Använd en **Server Component** för datahämtningen.
* Skapa en enkel layout/design för startsidan.

---

### **Sprint 2: Dynamisk routing & Interaktion (Vecka 2)**
**Mål:** Bygg de dynamiska sidorna och lägg till de första interaktiva elementen.

* Skapa den dynamiska routen `app/products/[id]/page.tsx` för produktsidorna.
* Hämta en specifik produkts data baserat på ID och rendera detaljerad information.
* Lägg till en **filtreringsfunktion** på startsidan med knappar (t.ex. "Smartphones" och "Laptops"). Använd en **Client Component**.
* Lägg till "Lägg till i varukorg"-knappen på produktsidan som en **Client Component** (inte vara fungerande utan räcker med en indikation bara).

---

### **Sprint 4: Slutputs (Vecka 3)**
**Mål:** Slutför designen och förbereda presentation.
* **Refaktorera** koden för att göra den mer läsbar, återanvändbar och effektiv.
* Se över hela applikationens responsivitet och design för en sista puts.
* Ev redovisning/presentation av projektet (beroende på om det blir en del 2 eller ej)
