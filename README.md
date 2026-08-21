# GoMerch — Obsahový hub

Jednostránkový obsahový hub pre Instagram [@go_merch](https://instagram.com/go_merch):
report zo štatistík, plán obsahu, banka nápadov, story hry a checklist na natáčací deň.

## Otvorenie

Celá stránka je jeden súbor `index.html`. Stačí ho otvoriť v prehliadači — nič sa
neinštaluje a nič sa nekompiluje. Jediná vec, ktorá sa ťahá z internetu, sú fonty
z Google Fonts; bez pripojenia sa stránka zobrazí s náhradnými fontami.

## Verejná adresa

Stránka sa po každej zmene sama nasadí na GitHub Pages cez workflow
`.github/workflows/pages.yml`.

## Čo stránka vie

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
