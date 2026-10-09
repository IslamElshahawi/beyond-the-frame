# Beyond the Frame

Portfolio site for an AI film director. A scroll-driven WebGL film: nine centuries of real public-domain art, with each client film playing on a bending 3D sheet, ending in a 3D wall of all 11 films and a player with sound.

**Live:** deployed by GitHub Actions to GitHub Pages on every push to `main` (`.github/workflows/pages.yml`).

## Structure
| Path | What it is |
|---|---|
| `index.html` | The whole site: content data at the top of the script (`CONFIG`, `FILMS`, `ERAS`), then the engine (three.js r149 from jsDelivr) |
| `art/` | Era artworks, public domain (credited on the page) |
| `pv/`, `pvs/` | Highlight previews of each film (540 px for sheets, 270 px for slices and the wall), muted loops |
| `hero/` | Hero clip (1080 px crop) and poster |
| `full/` | Full films with sound, for the player |
| `fr/`, `lp/` | Poster frames |

## Edit content
- Name and contact links: `CONFIG` at the top of the script.
- Film text (EN/AR): `FILMS`. Era copy and art: `ERAS`.
- Run locally: `python3 -m http.server` in this folder, then open http://localhost:8000.

## Art credits
Yahya al-Wasiti, *Maqamat al-Hariri* (Baghdad, 1237, BnF); Marcellin Auzolle, *Cinématographe Lumière* poster (1896); *See America*, WPA Federal Art Project (c. 1938, Library of Congress); Matson Photo Service, desert caravan, Sinai (Library of Congress); Rick Guidice and Don Davis, space colony interior (NASA Ames, 1975); NASA Earth Observatory, *Black Marble* (2016).

Client films © their respective brands, shown with permission as portfolio work.
