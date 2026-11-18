# RiderMaker2000

Technikai rider egy helyen: stageplot, csatornalista, kérések és kontaktok, a végén egy tiszta, kinyomtatható PDF.

## 1. Hol vannak az adataid?

**Minden automatikusan mentődik, a böngészőbe, ezen az eszközön.** Nincs fiók, nincs szerver, a ridereidet senki más nem látja, a GitHubra csak maga a program kerül fel.

Ebből három dolog következik:

- **Csinálj néha biztonsági mentést.** A böngésző tárolója törlődhet (böngészési adatok törlése, iPaden a Safari magától is takarít). ☰ menü → **Mentés fájlba…** Itt kiválasztod, mi kerüljön bele: ez a verzió, a projekt minden verziója, minden projekt, és/vagy a presetek.
- **Eszközök között fájllal viszed át.** Mentés fájlba → AirDrop, iCloud Drive vagy e-mail → a másik eszközön **Megnyitás fájlból…** → kipipálod, mit töltsön be. A betöltött projektek újként jönnek létre, a presetek hozzáadódnak a meglévőkhöz. Automatikus szinkron nincs.
- **A kezdőképernyőre tett app külön tároló.** iPaden a kezdőképernyős app nem látja, amit a Safariban csináltál (és fordítva), ezért az adatokat abba töltsd be, amit használni fogsz.

Egyszer megnyitva a program **net nélkül is működik**, netre kapcsolva pedig magától a legfrissebb verzió indul.

## 2. Felépítés

**Projekt = zenekar, verzió = egy rider** (pl. „klubos”, „akusztik”, „fesztivál”). A ⌂ gomb a Projektek oldal: a projektekre kattintva nyílnak le a verziók. Új verzió (másolat) a verziószámot lépteti (v1 → v2), az Új üres verzió tiszta lappal indul. A felső sávban átírod a projekt és a verzió nevét, a ▾ vált a verziók között. Keskenyebb ablakban a fülek lenyíló menüvé válnak. ↶ ↷ visszavonás.

### Stageplot

- **Blokk = egy zenész vagy egy eszköz** a színpadon, valós helyén. A **+** gombbal presetből jön (Dob, Basszus, Billentyű, Gitár, Ének, DJ, Keverő), a saját blokkjaidat „Mentés presetként” elmented.
- **Egy blokk sorai:**
  - **Input:** forrás, típus (mikrofon / DI / egyéb), eszköz típusa (gépelésre javasol, a listát bővítheted és törölheted), helyi vagy saját, RF. Mikrofonnál állvány: a típus alapján magától beáll (ének, OH → nagy; lábdob, láda, tom → kicsi; csiptetős → nincs), kézzel felülírhatod. DI-nél aktív/passzív.
  - **Output:** wedge, IEM, sidefill vagy main, és a cél.
  - **Áram:** „230V áram a jelölt helyekre”, kérésre darabszámmal.
  - **Megjegyzés.**
- **Tömörítés:** sok sorból egy rövid összefoglaló (pl. dob). A **Kiemelt** sor tömörítve is külön látszik.
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

### Kérések

- **Amire szükségünk van:** a program kiszámolja a stageplotból (XLR, DI-box, kis és nagy állvány, mikrofonok, dobmikrofon szett dobtestekkel, rádiós mikrofon külön, áram, stagebox). Minden sor átírható, pipával kivehető a PDF-ből.
- **Backline igény:** dob, gitárláda, basszusláda, billentyűállvány, saját tételekkel bővíthető.
- **Kérések:** + Új kérés, presetből vagy saját szöveggel (router, kommunikáció, keverő stb.), pipa = bekerül a PDF-be.
- **Egyéb megjegyzés:** szabad szöveg a végére.

### Kontaktok

Név, szerep, telefon, e-mail. A ☆ Mentés gombbal kontakt presetet csinálsz, legközelebb egy koppintással hozzáadod. Itt látod a PDF címét, és itt állítod a dátumot (üresen az exportálás napja).

### PDF

**PDF** gomb → az ablak jelzi, ha valami fontos hiányzik (de nem akadályoz). Minden oldalon fejléc: dátum, „Projekt · Verzió – tech rider”, oldalszám. Sorrend: kontaktok, stageplot, csatornalista, amire szükségünk van, backline, kérések, megjegyzés. Van **fekete-fehér** opció (saját = folytonos vonal, helyi = szaggatott). A fájlnév a címből és a dátumból jön, a szöveg kimásolható.

## 3. A filozófia

- **A rider a helyi technikusnak szól.** Csak az kerül bele, ami neki feladat: amit kérünk, és ami a munkájához kell. A saját eszközeid a rajzon jelölve vannak, de a kért listában nem szerepelnek.
- **Minden alapból helyi,** a saját eszközt te jelölöd meg.
- **Ami üres, az nem látszik.** Nincs „—”, nincs „válassz”, nincs felesleges oszlop.
- **A program számol, te döntesz.** Minden javaslat átírható vagy kivehető.
- **Egy irányban egyszerű:** a stageplotból lesz a csatornalista. Ha kell, kézi módba váltasz.
- **Technikai rider, nem szerződés:** nincs benne catering, fény, PA-követelmény. A telefonos egyeztetést nem váltja ki, hanem előkészíti.
