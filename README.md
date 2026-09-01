# Stránky

Statické stránky, ktoré sa nasadzujú na GitHub Pages cez
`.github/workflows/pages.yml`. Každá je jeden HTML súbor — nič sa neinštaluje
a nič sa nekompiluje.

| Stránka | Súbor | Adresa |
| --- | --- | --- |
| GoMerch — obsahový hub | `index.html` | `/` |
| Riadiaci panel Kolektívu | `kolektiv/index.html` | `/kolektiv/` |
| Minifestival — plán stanovíšť | `minifestival/index.html` | `/minifestival/` |
| E-mail marketing Kolektívu | `email/index.html` | `/email/` |

---

## Riadiaci panel Kolektívu

Panel na správu obsahu pre Kolektív: pozícia značky, myšlienky, rubriky, plán
obsahu, banka tém, analytika, mesačný report, úlohy a otvorené otázky.

Stránku otvorí ktokoľvek s odkazom, bez prihlásenia. Tlačidlom **Režim úprav**
sa dá každý text prepísať priamo v prehliadači; zmeny sa priebežne ukladajú do
prehliadača toho, kto ich urobil.

Panel nemá spoločné úložisko — každý má vlastnú kópiu. Na výmenu zmien slúži:

- **Export dát** — uloží súbor `.json` so všetkým obsahom
- **Načítať dáta** — načíta taký súbor od druhej strany
- **Uložiť stránku** — uloží celý panel aj s obsahom ako jeden HTML súbor
- **Tlač / PDF** — vytlačí alebo uloží aktuálnu sekciu

---

## E-mail marketing Kolektívu

Panel na e-mailovú komunikáciu Kolektívu: pozícia kanála a hlas, zbieranie
kontaktov a súhlas, uvítacia séria, mesačný list, predajná vlna na otvorenie
sezóny, automatické e-maily, kalendár rozposielok, čísla a checklist pred
odoslaním.

Texty e-mailov sú napísané, nie len naznačené — tlačidlom **Kopírovať e-mail**
sa celý e-mail (predmet, preheader, telo, výzva) prenesie do schránky a vloží do
Ecomailu či Mailchimpu. V **Banke predmetov** skopíruje predmet kliknutie naň.

Ovláda sa rovnako ako riadiaci panel Kolektívu: **Režim úprav** prepíše
ktorýkoľvek text priamo v prehliadači, zmeny sa ukladajú do prehliadača toho,
kto ich urobil, a vymieňajú sa cez **Export dát** / **Načítať dáta**. **Uložiť
stránku** uloží celý panel aj s obsahom ako jeden HTML súbor, **Tlač / PDF**
vytlačí aktuálnu sekciu.

Na stránke **Čísla** stačí po každej rozposielke zapísať štyri čísla (odoslané,
otvorenia, prekliky, odhlásenia) — miery aj porovnanie s vlastným mediánom sa
dopočítajú samy.

---

## GoMerch — obsahový hub

Jednostránkový obsahový hub pre Instagram [@go_merch](https://instagram.com/go_merch):
report zo štatistík, plán obsahu, banka nápadov, story hry a checklist na natáčací deň.

### Otvorenie

Celá stránka je jeden súbor `index.html`. Stačí ho otvoriť v prehliadači — nič sa
neinštaluje a nič sa nekompiluje. Jediná vec, ktorá sa ťahá z internetu, sú fonty
z Google Fonts; bez pripojenia sa stránka zobrazí s náhradnými fontami.

### Čo stránka vie

- päť záložiek: Report, Plán obsahu, Banka nápadov, Story a hry, Natáčací deň
- filtrovanie nápadov podľa cieľa (dosah / dôvera / predaj)
- kliknutie na hook ho skopíruje do schránky
- generátor hookov
- odškrtávací zoznam záberov na natáčací deň
- režim **Upraviť** — texty sa dajú prepísať priamo v prehliadači a tlačidlom
  **Stiahnuť** sa uloží kópia stránky aj so zmenami (zmeny sa neukladajú samy,
  po zatvorení karty sú preč)
- `Ctrl/Cmd + P` vytlačí alebo uloží celý hub do PDF vrátane všetkých záložiek

## Minifestival — plán stanovíšť

Plán stanovíšť minifestivalu Kolektiv × Bača Customs (29. 8. 2026, Bunky na
Lookach): odškrtávací zoznam, kto čo nesie, časová os doobeda, režim **Upraviť**
a tlač do PDF. Zmeny sa ukladajú do prehliadača návštevníka, takže po návrate
na stránku ostávajú.

---

## Nasadenie

Pages nasadzuje iba vetvu `claude/public-webpage-url-qw00o5` — prostredie
`github-pages` iné vetvy odmieta. Nová stránka sa na verejnú adresu dostane až
po zlúčení do tejto vetvy, alebo po pridaní pravidla v *Settings → Environments
→ github-pages → Deployment branches and tags*.
