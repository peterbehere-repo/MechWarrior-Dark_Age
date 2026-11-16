# MechWarrior: Dark Age — Fan Archive

A static archive of recreated cards, printable clix bases and personnel dossiers for the
MechWarrior: Dark Age collectable game (WizKids, 2002–2008).
**Live site: <https://peterbehere-repo.github.io/MechWarrior-Dark_Age/>**

| Section | Contents | Page |
|---|---|---|
| Clix bases — 'Mechs & quads | 788 builds / 747 units | [`bases.html`](bases.html) |
| Clix bases — infantry | 372 builds / 372 units | [`infantry.html`](infantry.html) |
| Personnel dossiers | 211 dossiers, six sets | [`dossiers.html`](dossiers.html) |
| Card gallery | 2,361 card recreations | [`cards.html`](cards.html) |
| CEC gear recreations | 233 cards, eight sets | [`docs/Index.html`](docs/Index.html) |

## Interactive clix bases

Every base is one self-contained HTML page, printable and clickable: click the cells to
advance the damage dial, hover any value for its rules text, work the heat dial, and watch
the last clicks fill with KO bullet holes. Stats come from Warrenborn unit pages.

**'Mechs and quads** — 788 builds covering 747 units in 22 faction sections, including all
27 quad-class units. Mechs and quads share the locked bi-fold base template; a copy of the
current template lives at `mocks/biped-r2.html`.

**Infantry** — 372 circle-base units in 18 faction sections, built on the locked Fenrir
infantry template: vertical stat strip, per-value and per-equipment tooltips, KO holes
stacked past the last click. Units whose build departs from the template (null speed cells,
full-circle arcs, long names) are listed in the exceptions document linked from the page.

## Personnel dossiers

The printed bi-fold personnel folders, rebuilt as an interactive 3D folder: open it, flip
through the four pages, and turn it over for the filing notes. Each dossier extracts the
name, faction, regiment, 'Mech and date of birth from the original sheet.

| Set | Dossiers |
|---|---|
| Dark Age | 36 |
| Liao Incursion | 44 |
| Death from Above | 31 |
| Counterassault | 29 |
| Falcon's Prey | 32 |
| Fire for Effect | 39 |

211 in total — 165 BattleMech pilots and 46 vehicle crew, 14 factions, service dates from
the 3060s to the 3130s. The gallery searches on name, 'Mech, regiment or faction and
filters by era, unit type, faction and series; each card opens
`Dossiers/Viewer.html?id=<code>`, which renders the folder in 3D from the scan textures.

## Card gallery

2,361 recreated cards, grouped by category and set:

| Category | Cards |
|---|---|
| Unit cards (15 sets) | 1,649 |
| Gunslinger pilots | 412 |
| Gear | 233 |
| Faction pride | 31 |
| Special | 36 |

Unit-card sets: Dark Age, Age of Destruction, Fire for Effect, Annihilation, Domination,
Liao Incursion, Death from Above, Counter Assault, Dropship, Falcons Prey, Fire Power,
Solaris VII, Vanguard, Wolf Strike, Battleforce.

## CEC gear card recreations

Complete recreation of all 233 combat enhancement (gear) cards from the MechWarrior:
Age of Destruction 2.0 clix era, covering eight sets:

| Set | Cards |
|---|---|
| Age of Destruction | 33 |
| Fire for Effect | 25 |
| Annihilation | 32 |
| Domination | 41 |
| Vanguard | 32 |
| Wolf Strike | 30 |
| Solaris VII | 28 |
| BattleForce | 12 |

`docs/Index.html` is the searchable A–Z listing; each `docs/CEC Recreations - <Set>.html`
page renders the full card with its original art. All links are relative and every asset
sits in the repo — this section depends on nothing outside it.

## Art and assets

- `Card Art/` — the 233 CEC gear card-art panels at 600 px
- `Cards/` and `Thumbs/` — full-size card images and their grid thumbnails
- `Dossiers/Tex/<id>/` — seven scan textures per dossier (front, back, liner, four pages);
  `Dossiers/Thumbs/` — gallery thumbnails
- `Bases/` — every 'Mech, quad and infantry base build

## Provenance

Card and dossier art is recovered from the owner's archive of catalog scans and the printed
dossier sheets (upscaled where needed). Card text was recovered verbatim from archived card
database listings; base stats come from Warrenborn unit pages. Frames, typography and
badge placement are typeset in the spirit of the printed designs — no complete card scans
were ever archived, so layouts are faithful reconstructions, not scans. Rarity was not
captured in the recovery and is intentionally absent.

Cards whose text says "Provides X SE" carry a highlighted **SE RULE** block quoting the
complete official definition of that special equipment, from the AoD SEC reference sheet
and the set rules inserts (recovered from the Internet Archive). Base pages use the same
recovered wording for heat effects and special equipment.

## Repo notes

Plain static files, no build step — GitHub Pages serves them as-is (`.nojekyll`). Card
images are referenced through absolute `raw.githubusercontent.com` URLs: Pages' origin
returns 404s for the relative image paths inside `cards/*.html`. Generated pages under
`cards/` therefore also use root-relative navigation links.

*Not affiliated with WizKids, The Topps Company or Catalyst Game Labs. Recovered for
personal archival/reference use.*
