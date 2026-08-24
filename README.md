# Stránky

Statické stránky, ktoré sa nasadzujú na GitHub Pages cez
`.github/workflows/pages.yml`. Každá je jeden HTML súbor — nič sa neinštaluje
a nič sa nekompiluje.

| Stránka | Súbor | Adresa |
| --- | --- | --- |
| GoMerch — obsahový hub | `index.html` | `/` |
| Riadiaci panel Kolektívu | `kolektiv/index.html` | `/kolektiv/` |

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

## Ďalšie stránky

- `minifestival/index.html` — plán stanovíšť minifestivalu Kolektiv × Bača Customs
  (29. 8. 2026, Bunky na Lookach). Verejná adresa: `.../minifestival/`.
  Odškrtávací zoznam, kto čo nesie, časová os doobeda, režim **Upraviť** a tlač do PDF.
  Zmeny sa ukladajú do prehliadača návštevníka, takže po návrate na stránku ostávajú.

Pages nasadzuje iba tú vetvu, ktorá je v nastaveniach repozitára zvolená ako zdroj
stránky (teraz `claude/public-webpage-url-qw00o5`). Nová stránka sa na verejnú adresu
dostane až po zlúčení do tejto vetvy — alebo po prepnutí zdroja v *Settings → Pages*.
