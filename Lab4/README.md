# Lab 4 — OSINT slikom (obrnuto pretraživanje)

U ovoj vježbi fokus je na **obrnutom pretraživanju slike** (*reverse image search*): kada imate fotografiju, možete pokušati otkriti **gdje se pojavljuje na webu**, **stariju pojavu** od trenutne objave ili **srodne verzije** (crop, ogledalo, kompresija). To je standardan alat za **provjeru konteksta** (npr. je li vijest ilustrirana starom ili pogrešnom fotografijom) i za **istraživanje izvora** uz iste etičke granice kao u **Labu 3**.

**Razlika u odnosu na Lab 3:** Lab 3 naglašava **tekstualne tragove** (ime, e-pošta, korisnička imena, dokumenti). Lab 4 naglašava **vizualni trag** i vremensku/logičku provjeru („je li ova slika starija od događaja koji navodno ilustrira?“).

## Upute za studente

**Cilj vježbe:** znati koristiti najmanje **dva** servisa za obrnuto pretraživanje; znati objasniti zašto se rezultati razlikuju; znati dokumentirati izvor i zaključak; povezati s provjerom dezinformacija i s forenzičkim smislom **lanaca dokaza** (slika kao trag, ne kao „automatska istina“).

**Tijek rada:**

1. Pročitajte *Pravila i pravno-etički okvir*.
2. Instalirajte ili isprobajte **dodatke za preglednik** (opcionalno): [RevEye](https://chrome.google.com/webstore/detail/reveye-reverse-image-sear/keaaclcjhehbbapnphnmpiklalfhelgf?hl=en) (Chrome) ili [Image Search Options](https://addons.mozilla.org/en-US/firefox/addon/image-search-options/) (Firefox).
3. Prođite servise u odjeljku *Alati* i usporedite rezultate na **istoj** slici (npr. iz laboratorijskog zadatka).
4. Riješite **laboratorijski zadatak** (slika ili arhiv — vidi *Materijal za zadatak*).
5. Predajte izvještaj prema *Strukturiranoj predaji*.

## Pravila i pravno-etički okvir

- Koristite **samo** slike i zadatke koje vam da nastavnik ili koje su **javno** objavljene za tu svrhu.
- **Zabranjeno:** ciljano otkrivanje i objavljivanje **osjetljivih podataka** o pojedincima iz slika izvan okvira vježbe; zlouporaba nalaza za uznemiravanje; zaobilazenje pristupa privatnim albumima.
- Rezultat obrnutog pretraživanja je **indicija**, ne presuda — uvijek navedite **URL izvora** i **datum pristupa**.

## Alati (obrnuto pretraživanje)

- [Google Images](https://images.google.com/) — učitavanje ili URL slike.
- [Bing Visual Search](https://www.bing.com/images) — sličan princip; rezultati često drugačiji od Googlea.
- [Baidu Images](https://image.baidu.com/) — korisno za sadržaj koji je dominantniji na kineskom webu (s suglasnostima i pravilima nastavnika).
- [TinEye](https://tineye.com/) — drugačiji indeks i algoritam; dobar za „prvu poznatu pojavu“ ako je u indeksu.

**Smjernica za interpretaciju:** ako sliku **ne** pronađete u starijem kontekstu, to **ne dokazuje** nužno da je autentična za današnji događaj — možda nije indeksirana. Ako je **pronađete** u starijem kontekstu, to **jačanje hipoteze** da se ponovno koristi stara fotografija (uz provjeru da je stvarno ista scena).

## Materijal za zadatak

U repozitoriju je predviđena datoteka **`zadatak.zip`** (ili ekvivalent kojeg objavi nastavnik na LMS-u). U njoj je slika ili mali skup slika za vježbu.

**Ako `zadatak.zip` nije u mapi `Lab4/`:** preuzmite ga s mjesta koje označi nastavnik (LMS, e-mail). Bez tog materijala zadatak nije jednak za sve studente — zatražite datoteku prije roka predaje.

**Sadržaj zadatka (cilj):** metodom obrnutog pretraživanja i **dokumentiranih** izvora utvrditi što je moguće pouzdanije:

- **naziv** objekta / zgrade (ili najbliži javno potvrđeni naziv),
- **lokacija** (grad / regija, po mogućnosti s referencom),
- **otvaranje** ili relevantna godina/datum ako se može potkrijepiti javnim izvorom.

Ako nešto **nije** moguće potvrditi, to eksplicitno navedite u predaji (to je valjan dio vježbe).

## Strukturirana predaja

Jedan **PDF** (ili format koji objavi nastavnik).

| Odjeljak | Sadržaj |
|----------|---------|
| **1. Sažetak** | Kratko: što ste zaključili o slici (1–3 rečenice). |
| **2. Koraci** | Koji ste alati korišteni (navedite **najmanje dva**), redoslijed, zašto. |
| **3. Tablica nalaza** | Za svaki važan korak: **upit / slika** \| **alat** \| **ključni rezultat (URL)** \| **datum pristupa**. |
| **4. Odgovori na zadatak** | Naziv zgrade (ili „nije pouzdano utvrđivo“), lokacija, datum/otvaranje — svaka tvrdnja s **izvorom** ili oznakom neizvjesnosti. |
| **5. Ograničenja** | Što obrnuto pretraživanje **nije** moglo riješiti; moguće zamke (reupload, crop, ogledalo). |
| **6. Etika i kontekst** | Jedan odlomak: kako biste istu tehniku upotrijebili u provjeri vijesti bez širenja dezinformacija. |

## Poveznica na ostale vježbe

- **Lab 2:** preciznije tekstualno pretraživanje kad imate tekstualne tragove uz sliku (naziv, mjesto).
- **Lab 3:** ista očekivanja dokumentacije izvora i etike; Lab 4 dodaje **vizualni** kanal.

## Reference

- [Medium — OSINT: How to find information on anyone](https://medium.com/@Peter_UXer/osint-how-to-find-information-on-anyone-5029a3c7fd56) (općenito; uskladite s etičkim okvirom kolegija)
- [Cybrary — OSINT tricks, quick guide image research](https://www.cybrary.it/blog/0p3n/osint-tricks-quick-guide-image-research/)
