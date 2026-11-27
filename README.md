# GLASSgallery – Technické listy skla (verzia bez prihlásenia)

Statická verzia appky „Technické listy skla“ pre kolegov bez účtu Claude. Beží v prehliadači, netreba sa prihlasovať.

- **Výber skla:** podľa kódu z Logikalu alebo podľa skladby (5 polí). K tomu výmenné tabule s filtrom podľa hrúbky a pozície.
- **Archív:** hotové technické listy s vyhľadávaním podľa textu, nepriezvučnosti Rw a typu skla.
- **Stiahnutie PDF:** technický list v dizajne GLASSgallery sa vytvorí priamo v prehliadači.
- **Chýbajúci list:** tlačidlo „Vyžiadať e-mailom“ otvorí e-mail na sliva@glassgallery.sk s presným zadaním.

## Súbory

| Súbor | Obsah |
|---|---|
| `index.html` | aplikácia |
| `data/archiv.json` | archív technických listov (export z appky v Claude) |
| `data/skla.json` | štandardné sklá z Logikalu |
| `data/funkcne.json` | výmenné tabule |
| `img/logo.png`, `fonts/` | logo a písmo (Carlito = metricky zhodné s Calibri) |

## Zverejnenie na GitHub Pages

1. Na github.com vytvor repozitár, napr. `glassgallery-technicke-listy`.
2. Nahraj doň všetky súbory z tohto priečinka (Add file → Upload files) a potvrď Commit.
3. Choď do Settings → Pages → Build and deployment → Source: **Deploy from a branch**, Branch: **main**, priečinok **/ (root)** → Save.
4. Asi o minútu bude appka dostupná na adrese `https://<účet>.github.io/glassgallery-technicke-listy/`.

Stránka je na internete dostupná každému, kto pozná odkaz. Vyhľadávače ju neindexujú (`noindex`). Neobsahuje ceny.

## Aktualizácia archívu

Keď pribudnú nové listy v appke v Claude, Claude vyexportuje nový `data/archiv.json`. Ten stačí nahradiť v repozitári. Ak je GitHub pripojený ku Claude, nahrá ho Claude sám.
