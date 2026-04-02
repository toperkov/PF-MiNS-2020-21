# Lab 3 — OSINT (otvoreni izvori)

OSINT (*Open Source Intelligence*) znači prikupljanje i analizu podataka iz **javno dostupnih** izvora: tražilica, društvenih mreža, arhiva stranica, objava, metapodataka dokumenata i sl. U forenzici i sigurnosti to je često prvi korak za **kontekst** i **planiranje** daljnjih postupaka — uz jasnu granicu **ovlasti**, **svrhe** i **etike**.

## Upute za studente

**Cilj vježbe:** znati objasniti tipičan tijek OSINT istraživanja (hipoteza → izvori → korelacija → provjera); znati dokumentirati izvor i pouzdanost nalaza; razumjeti zašto je zlouporaba istih tehnika štetna i često nezakonita.

**Tijek rada (redoslijed):**

1. Pročitajte *Pravila i pravno-etički okvir* prije bilo kakvog praktičnog rada.
2. Pregledajte *referentne slike* (flowchartovi) u nastavku — služe kao podsjetnik na korake, ne kao automat za neovlašteno djelovanje.
3. Odaberite **jedan** od dopuštenih modusa cilja (vidi *Modus cilja*).
4. Prođite odjeljak *Alati i smjernice* i isprobajte **dopuštene** korake unutar odabranog modusa.
5. Izradite predaju prema *Strukturiranoj predaji*.

**Modus cilja (nastavnik objavljuje koji vrijedi u vašoj grupi):**

- **Modus A (preporučeni):** rad isključivo na **fiktivnoj kartici** u [osint_cilj_fiktivno.md](osint_cilj_fiktivno.md). Ne tražite stvarne profile pod tim imenom; zadatak je **analiza fragmentata**, harfa korelacije i metodološki komentar.
- **Modus B:** **Self-OSINT** — dokumentirate **vlastite** javno vidljive tragove (npr. što se vidi o vama kroz tražilicu i javne profile koje sami koristite). U predaju ne stavljajte osjetljive podatke (puno brojeve, adrese); dovoljno je opis razine otkrivanja i popis vrsta izvora.
- **Modus C (samo uz eksplicitno odobrenje nastavnika):** cilj je **stvarna osoba** koja je **pismeno pristala** i dobila **ograničen popis polja** koje smije te predati nastavniku. Bez toga **C se ne provodi**.

## Pravila i pravno-etički okvir

- **Dopušteno:** čitanje **javno** objavljenog sadržaja u okviru modusa koji je odobrio nastavnik; korištenje vlastitih računa i podataka uz suglasnost; vježbanje metapodataka na **fiktivnim** materijalima.
- **Zabranjeno u ovoj vježbi:**
  - bilo kakvo **zaobilazenje sigurnosti računa** (npr. zlouporaba „zaboravili ste lozinku“, brute force, krađa sesije);
  - **prijava na tuđe račune** ili predstavljanje kao netko drugi;
  - prikupljanje ili dijeljenje **osjetljivih osobnih podataka** izvan jasno odobrenog modusa;
  - korištenje **plaćenih baza curenja** ili sličnih servisa protiv **tuđih** identiteta u svrhu laba (osim ako nastavnik eksplicitno organizira **legalnu demonstraciju** na sintetičkim podacima);
  - **doxxing**, uznemiravanje, kontaktiranje trećih osoba u ime vježbe.
- **HIBP ([Have I Been Pwned](https://haveibeenpwned.com/)):** u okviru laba smije se provjeravati **samo vlastita** adresa e-pošte (ili adresa koju vam da nastavnik za demonstraciju), ne adrese nasumičnih osoba.
- **Alati treće strane** (npr. RocketReach, DeHashed, IntelX): tretirajte kao **informativno**; uskladite korištenje s uvjetima pružatelja i uputama nastavnika. Ne unosite tuđe osobne podatke u alate ako to nije dopušteno modusom.

## Referentne slike (flowchart)

*Ako se slike ne učitavaju lokalno, koristite pregled na GitHubu repozitorija — datoteke `Lab3/RealName.png` i `Lab3/Email.png`.*

![OSINT flowchart — ime / identitet](https://raw.githubusercontent.com/toperkov/PF-MiNS-2020-21/main/Lab3/RealName.png)

![OSINT flowchart — e-pošta](https://raw.githubusercontent.com/toperkov/PF-MiNS-2020-21/main/Lab3/Email.png)

## Alati i smjernice (informativno)

### 1. Pretraživanje imena i korelacije

- [Webmii](https://webmii.com/) i slični agregatori — rezultate **provjeravajte**; često su nepotpuni ili zastarjeli.
- Tražilice: Google, Bing, Yandex — koristite znanje iz **Laba 2** (`site:`, `filetype:`, navodnici).

### 2. E-adresa (samo u dopuštenom modusu)

- Pronađeni ili **izmišljeni u fikciji** kontekst: razmislite **gdje bi se** adresa mogla pojaviti (biografije, PDF-ovi, arhive).
- **Permutator e-pošte** (npr. [metricsparrow — email permutator](http://metricsparrow.com/toolkit/email-permutator/)) — koristite **samo** uz jasno odobrenje i etički okvir (npr. vlastiti domen ili fiktivni primjer iz materijala).
- **Have I Been Pwned** — vidi gore; **DeHashed / IntelX** — samo ako nastavnik odredi legalan okvir.

### 3. Korisnička imena

- [knowem.com](https://knowem.com/), [usersearch.org](https://usersearch.org/), [instantusername.com](https://instantusername.com/), [namecheckup.com](https://namecheckup.com/) — korisno za **vlastite** ili **fiktivne** handlove iz [osint_cilj_fiktivno.md](osint_cilj_fiktivno.md), ne za masovno „testiranje“ tuđih nadimaka.

### 4. Preglednik i profesionalni profili

- Dodaci poput **Rapporteur** mogu otkriti veze između tragova — **ne koristite** ih za tuđe račune u ovoj vježbi osim u **modusu C** uz izričitu suglasnost subjekta i upute nastavnika.
- LinkedIn i druge mreže: poštujte uvjete korištenja; ne kombinirajte s **zabranjenim** trikovima za pristup računu.

### Dodatak — kolekcije alata

- [start.me — pers-infra](https://start.me/p/nRl9Ya/pers-infra)
- [start.me — ultimate OSINT collection](https://start.me/p/DPYPMz/the-ultimate-osint-collection)
- [GitHub — oryon-osint / querytool](https://github.com/oryon-osint/querytool)

## Strukturirana predaja

Jedan **PDF** (ili format koji objavi nastavnik) s jasnim naznakom **modusa (A / B / C)**.

| Odjeljak | Sadržaj |
|----------|---------|
| **1. Sažetak** | Cilj istraživanja u jednoj rečenici (što ste pokušali dokazati ili kartografirati). |
| **2. Metodologija** | Kratki popis kategorija izvora (tražilica, društvene mreže, dokumenti, forumi …) koje ste **zapravo** koristili u dopuštenom opsegu. |
| **3. Tablica nalaza** | Za svaki značajan nalaz: **nalaz** (tvrdnja) \| **izvor** (URL ili točan opis dokumenta) \| **datum pristupa** \| **pouzdanost** (npr. visoka/srednja/niska + jedna rečenica zašto). |
| **4. Harfa / shema** | Za modus A: korelacija iz [osint_cilj_fiktivno.md](osint_cilj_fiktivno.md). Za modus B: shema vlastitih **kategorija** tragova (ne kopirajte osjetljive podatke). Za modus C: prema uputama nastavnika. |
| **5. Ograničenja** | Što **niste** mogli potvrditi i zašto (npr. nedostatak javnog izvora, proturječni podaci). |
| **6. Etika** | Jedan odlomak: koja pravila ste poštovali i koja bi opasnost bila od zlouporabe istih tehnika. |

## Poveznica na ostale vježbe

- **Lab 2:** precizni upiti i sužavanje rezultata prije nego što krenete u OSINT.
- **Lab 1:** isti digitalni trag koji „otvara“ OSINT može biti i **rizik** za zaštićenu osobu — znanje o privatnosti i anonimnosti ostaje relevantno.

## Reference (općenito)

- Materijali i alati navedeni u odjeljcima iznad; dodatna literatura po izboru nastavnika.
