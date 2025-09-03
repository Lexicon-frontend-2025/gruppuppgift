### **Gruppövning: E-handelsplattform i Next.js**

---

### **Produktbeskrivning**
Uppgiften är att bygga en **minimalistisk e-handelsplattform** för olika produkter med hjälp av **Next.js 15 App Router**. Plattformen ska visa upp ett urval av produkter från ett externt API, vara fullt responsiv och ha interaktiva inslag. Dessutom ska ni bygga ett förenklat **admingränssnitt** där ni kan hantera produkter. Målet är att ni ska få praktisk erfarenhet av att arbeta med **Server Components**, **Client Components**, **statiska och dynamiska routeer**, samt hantering av asynkron data och datamutationer med **Server Actions**.

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
    * På startsidan - Visa en översikt av samtliga produkter. Hämta och rendera produktdata på serversidan. Den första produkten på sidan ska ha avvikande design och vara större än de andra t ex spänna över två kolumner/rader. Det ska också finnas en Hero med en CTA högst upp på sidan.
    * Om Oss - Gör en Lorem-text eller skriv ihop något bara för att ha något där samt en bild.
    * Kontakt - Ett tomt formulär med lämpliga labels osv (funktionalitet för detta är frivilligt)
2.  **Produktsida:**
    * Skapa en dynamisk route (`/products/[id]`) som visar detaljerad information för en specifik produkt baserat på dess ID. Ni behöver inte ha all info som finns i API här, men titel, beskrivning, bild och pris är minsta kraven.
    * Hämta enskild produktdetalj från API:et och rendera på serversidan.
3.  **Interaktiva element (Client Components):**
    * Lägg till en knapp för att **filtrera produkter** efter en kategori.
    * Inkludera en knapp för att **"Lägga till i varukorg"** (behöver inte ha en fungerande varukorg, det räcker att den visar en notifikation eller loggar en händelse).
4.  **Admingränssnitt med CRUD-funktionalitet:**
    * Skapa en ny route, t.ex. `/admin`, för att hantera produkter.
    * Implementera en förenklad **CRUD**-funktionalitet (Create, Read, Update, Delete) för produkter. Använd **Server Actions** för att hantera dessa operationer (ni kan simulera att spara/uppdatera data genom att logga händelser till konsolen).
5.  **Frivilligt: Inloggning:**
    * Om ni vill ha en extra utmaning, kan ni göra `/admin`-sidan lösenordsskyddad.
    * **Alternativ 1 (Enklast):** Använd en enkel miljövariabel och ett formulär för att autentisera, som beskrevs i tidigare kommunikation.
    * **Alternativ 2 (Avancerat):** Använd ett befintligt autentiseringsbibliotek som **Clerk**, **Kinde**, eller **Auth0** för att snabbt implementera en robust inloggningsfunktion.
6.    **Frivilligt: Kundvagnsfunktionalitet** Använd useContext och API-endpoints för carts/user. Gör så att man kan lägga till och ta bort produkter från kundvagnen och koppla ev till inloggning om ni vill. Ni kan också göra en simulerad utcheckning om ni vill (eller kör t ex Stripe här).
7.    **Kontaktformulär:** Skapa funktionalitet för att skicka formuläret och skapa upp så att personen som skriver i får en visuell indikation på att det lyckats och en bekräftelse via e-post. 
8.    **Frivilligt: Övrigt:** Ev annan funktionalitet som ni ser kan vara intressant som utökade fält på admingränssnitt, recensionser, tillfälliga rabatter eller dylikt. Tänk bara på att inte dra iväg med extra saker innan allt annat är på plats och faktiskt bra utfört.

---

### **Arbetsflöde & Sprintplan (4 veckor)**

Denna uppgift är uppdelad i 4 sprints, en för varje vecka. Varje sprint fokuserar på specifika delmål. Detta är bara förslag och ni kan själva bestämma om ni vill fördela det på annat sätt.

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

* Skapa den dynamiska routeen `app/products/[id]/page.tsx` för produktsidorna.
* Hämta en specifik produkts data baserat på ID och rendera detaljerad information.
* Lägg till en **filtreringsfunktion** på startsidan med knappar (t.ex. "Smartphones" och "Laptops"). Använd en **Client Component**.
* Lägg till "Lägg till i varukorg"-knappen på produktsidan som en **Client Component** (inte vara fungerande utan räcker med en indikation bara).

---

### **Sprint 3: Skapa & Ta bort produkter (Vecka 3)**
**Mål:** Implementera grundläggande CRUD-funktioner.

* Skapa en ny route, t.ex. `app/admin/page.tsx`, för admingränssnittet.
* **Read (Läs):** På adminvyn, visa en lista över alla produkter.
* **Create (Skapa):** Skapa ett formulär för att lägga till en ny produkt (titel, beskrivning, pris, etc.). Använd en **Server Action** för att hantera formulärdata och "skapa" produkten genom att logga den till konsolen och skicka till korrekt API endpoint. Visa meddelande om detta lyckats för användaren.
* **Delete (Ta bort):** Lägg till en "Ta bort"-knapp vid varje produkt i adminvyn. Använd en **Server Action** för att hantera raderingen.  Använd endpoint för detta och ge användaren återkoppling om detta lyckats.
* **Frivilligt:** Om ni väljer att lägga till inloggning, gör en enkel implementering för detta i samband med detta.

---

### **Sprint 4: Uppdatering & Slutputs (Vecka 4)**
**Mål:** Komplettera CRUD, slutföra designen och förbereda presentation.

* **Update (Uppdatera):** Lägg till en "Redigera"-knapp vid varje produkt. Denna ska leda till ett formulär som fylls i med den befintliga produktens data och som låter er uppdatera den. Använd en **Server Action** för att hantera uppdateringen.
* **Refaktorera** koden för att göra den mer läsbar, återanvändbar och effektiv.
* Se över hela applikationens responsivitet och design för en sista puts.
