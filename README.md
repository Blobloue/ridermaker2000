# RiderMaker2000

Technikai rider egy helyen: stageplot, csatornalista, kérések és kontaktok, a végén egy tiszta, kinyomtatható PDF.

## 1. Hol vannak az adataid?

**Minden automatikusan mentődik, a böngészőbe, ezen az eszközön.** Nincs fiók, nincs szerver, a ridereidet senki más nem látja, a GitHubra csak maga a program kerül fel.

Ebből három dolog következik:

- **Csinálj néha biztonsági mentést.** A böngésző tárolója törlődhet (böngészési adatok törlése, iPaden a Safari magától is takarít). ☰ menü → **Mentés fájlba…** Itt kiválasztod, mi kerüljön bele: ez a verzió, a projekt minden verziója, minden projekt, és/vagy a presetek.
- **Eszközök között fájllal viszed át.** Mentés fájlba → AirDrop, iCloud Drive vagy e-mail → a másik eszközön **Megnyitás fájlból…** → kipipálod, mit töltsön be. A betöltött projektek újként jönnek létre, a presetek hozzáadódnak a meglévőkhöz. Automatikus szinkron nincs.
- **A kezdőképernyőre tett app külön tároló.** iPaden a kezdőképernyős app nem látja, amit a Safariban csináltál (és fordítva), ezért az adatokat abba töltsd be, amit használni fogsz.

Egyszer megnyitva a program **net nélkül is működik**, netre kapcsolva pedig magától a legfrissebb verzió indul.

## 2. Telepítés és frissítés

- **Első feltöltés:** GitHubon új, publikus repo → feltöltöd a fájlokat (index.html, sw.js, manifest.webmanifest, ikonok, README.md) → Settings → Pages → Deploy from a branch → main, / (root).
- **Frissítés:** csak az új `index.html`-t töltöd fel (Add file → Upload files). Az adataid megmaradnak.
- **iPadre/telefonra:** Safariban megnyitod a címet → Megosztás → Főképernyőhöz adás.

## 3. Felépítés

**Projekt = zenekar, verzió = egy rider** (pl. „klubos”, „akusztik”, „fesztivál”). A ⌂ gomb a Projektek oldal: a projektekre kattintva nyílnak le a verziók. Új verzió (másolat) a verziószámot lépteti (v1 → v2), az Új üres verzió tiszta lappal indul. A felső sávban átírod a projekt és a verzió nevét, a ▾ vált a verziók között. Keskenyebb ablakban a fülek lenyíló menüvé válnak. ↶ ↷ visszavonás.

### Stageplot

- **Blokk = egy zenész vagy egy eszköz** a színpadon, valós helyén. A **+** gombbal presetből jön (Dob, Basszus, Billentyű, Gitár, Ének, DJ, Keverő), a saját blokkjaidat „Mentés presetként” elmented.
- **Egy blokk sorai:**
  - **Input:** forrás, típus (mikrofon / DI / egyéb), eszköz típusa (gépelésre javasol, a listát bővítheted és törölheted), helyi vagy saját, RF. Mikrofonnál állvány: a típus alapján magától beáll (ének, OH → nagy; lábdob, láda, tom → kicsi; csiptetős → nincs), kézzel felülírhatod. DI-nél aktív/passzív.
  - **Output:** wedge, IEM, sidefill vagy main, és a cél.
  - **Áram:** „230V áram a jelölt helyekre”, kérésre darabszámmal.
  - **Megjegyzés.**
- **Tömörítés:** sok sorból egy rövid összefoglaló (pl. dob). A **Kiemelt** sor (input, output vagy áram) tömörítve is külön látszik.
- **Hely:** bármelyik sor rögzíthető a blokk tetejére vagy aljára (pl. az áram mindig alul). A többi sort a blokkon belül szabadon húzod.
- **Szövegméret** beírható, több kijelölt blokknál együtt állítod.
- **Eszköztár:** rendezői/színpadi nézet, mozgatás, snap, méretek, zoom, színpadméret. Shift + klikk: több kijelölés, Option + húzás: másolás, Cmd + húzás: snap nélkül, Delete: törlés, nyilak: finom mozgatás.
- Telefonon a blokk-szerkesztő alul összecsukható sáv.

### Csatornalista

- **A sorok a stageplotból jönnek** (🔗 jelzi és a zöldes csoportcím). A sorszám a sorrendből jön.
- **Húzással** (⠿) átrendezed a listát, a stageplot nem változik.
- **Szám átírása:** onnan folytatódik a számozás, 📌 jelzi; a 📌-re koppintva újra automatikus. Ugyanez a blokk-szerkesztő „Manuális sorszám” mezője.
- **Input és output sorrend** külön állítható a ☰ menüben, blokkonként húzva.
- **Kézi csatornalista** (☰ menü): a lista leválik a stageplotról, szabadon írod és törlöd, semmi nem tolódik. Visszakapcsolva a meglévő sorok kézi sorok maradnak, csak az új stageplot elemek kapnak csatornát.
- **Kézi sorok** (szürke csoport): csak a listán élnek, a stageploton nem. Blokk törlésekor a program megkérdezi, megtartsa-e a csatornáit kézi sorként.
- Oszlopok ki-be kapcsolhatók, a zöld mező = kitöltve.
- A lista fölött látod, hogyan kerül a PDF-be (pl. „3 hasáb · 24 sor”). A **PDF info** kapcsolóval (Manuális / Auto) választod meg, hogyan kerül az infó a PDF-be. A szerkesztő oszlopai mindkét állásban ugyanazok maradnak.
  - **Manuális:** a név mellett külön Info oszlop.
  - **Auto:** minden egy cellában a név után. Mikrofon: a konkrét típus (pl. SM58), ha nincs megadva, csak „mikrofon”. DI: „aktív DI” vagy „passzív DI”, ha nincs kiválasztva, csak „DI” (megadott típusnál zárójelben mellette). Utána az állvány (kis/nagy), az RF és a megjegyzés, ha ki van töltve.
  - Ha így nem fér el, az előnézet jelzi: kevesebb hasáb lesz, vagy ha egy hasábba sem fér ki egy sorban, kiírja, melyik sor(ok) miatt. Ezek a sorok a listán színes csíkot kapnak a szám előtt.

### Kérések

- **Amire szükségünk van:** a program kiszámolja a stageplotból (XLR, DI-box, kis és nagy állvány, mikrofonok, dobmikrofon szett dobtestekkel, rádiós mikrofon külön, áram, stagebox). Minden sor átírható, pipával kivehető a PDF-ből.
- **Backline igény:** dob, gitárláda, basszusláda, billentyűállvány, saját tételekkel bővíthető.
- **Kérések:** + Új kérés, presetből vagy saját szöveggel (router, kommunikáció, keverő stb.), pipa = bekerül a PDF-be.
- **Egyéb megjegyzés:** szabad szöveg a végére.

### Kontaktok

Név, szerep, telefon, e-mail. A ☆ Mentés gombbal kontakt presetet csinálsz, legközelebb egy koppintással hozzáadod. Itt látod a PDF címét, itt állítod a dátumot (üresen az exportálás napja), és itt töltöd fel a **logót**, ami a PDF minden oldalának tetejére kerül.

### PDF

**PDF** gomb → az ablak jelzi, ha valami fontos hiányzik (de nem akadályoz). Minden oldalon fejléc: dátum, „Projekt · Verzió – tech rider”, oldalszám. Sorrend: kontaktok, stageplot, csatornalista, amire szükségünk van, backline, kérések, megjegyzés. A csatornalista táblázatban a sorszám mellett csak a forrás és egy összegző **Info** oszlop van (pl. „SM58 · nagy állvány”), abba is csak az kerül, ami ki van töltve. A lista 8 soronként hasábot vált: 8 sor egy hasáb, 16 kettő, 24-től három. Ha a szöveg nem fér el, kevesebb hasáb lesz. Egy sor mindig egy sor. Ha a lista nem fér az első oldalra, a stageplot kicsit kisebb lesz. Van **fekete-fehér** opció (saját = folytonos vonal, helyi = szaggatott). A fájlnév a címből és a dátumból jön, a szöveg kimásolható.

## 4. A filozófia

- **A rider a helyi technikusnak szól.** Csak az kerül bele, ami neki feladat: amit kérünk, és ami a munkájához kell. A saját eszközeid a rajzon jelölve vannak, de a kért listában nem szerepelnek.
- **Minden alapból helyi,** a saját eszközt te jelölöd meg.
- **Ami üres, az nem látszik.** Nincs „—”, nincs „válassz”, nincs felesleges oszlop.
- **A program számol, te döntesz.** Minden javaslat átírható vagy kivehető.
- **Egy irányban egyszerű:** a stageplotból lesz a csatornalista. Ha kell, kézi módba váltasz.
- **Technikai rider, nem szerződés:** nincs benne catering, fény, PA-követelmény. A telefonos egyeztetést nem váltja ki, hanem előkészíti.
