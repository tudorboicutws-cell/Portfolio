# Portfolio

Portofoliul lui Tudor: video, animație, design și copywriting.

**Nu știi GitHub? Citește [GHID-EDITARE.md](GHID-EDITARE.md): totul pas cu pas, doar din browser.**

## Ce e în folder

| Fișier | Ce face |
|---|---|
| `index.html` | Pagina în sine: textele și proiectele |
| `style.css` | Culorile și aranjarea. Culorile se schimbă din primele rânduri |
| `assets/img/` | Pozele proiectelor (jpg, png, webp) |
| `assets/video/` | Clipuri scurte, comprimate (mp4 sub ~20 MB) |

## Pozele proiectelor

Salvează câte o imagine (jpg, lată, de preferat 1600 px) în `assets/img/` cu exact aceste nume:

| Proiect | Nume fișier |
|---|---|
| Cultural Tourism in the Digital Age | `cultural-tourism.jpg` |
| 3D Assets for Video Games | `game-assets.jpg` |
| The Knights of the Garden | `knights-of-the-garden.jpg` |
| REVIVE: Historic Towns | `revive.jpg` |
| Heroes on Parallel Fronts | `heroes-parallel-fronts.jpg` |
| Dimitrie Cantemir 300 | `cantemir-300.jpg` |

Princely Court folosește deja imaginea de pe YouTube. Până pui o poză, cardul arată un fundal colorat.

## Cum adaugi un proiect

1. Pune poza în `assets/img/` (de exemplu `afis-tabara.jpg`).
2. În `index.html`, copiază un bloc `<article class="card">...</article>` din secțiunea potrivită.
3. Înlocuiește `<div class="media placeholder">Imagine</div>` cu
   `<img src="assets/img/afis-tabara.jpg" alt="Afiș tabără de vară">`.
4. Schimbă titlul și descrierea.

Pentru video mai lungi, urcă-le pe YouTube (sau Instagram) și pune linkul de embed, ca site-ul să rămână rapid.

## Cum vezi site-ul online

Settings > Pages > Source: "Deploy from a branch" > Branch: `main`, folder `/ (root)` > Save.
După 1-2 minute site-ul apare la https://tudorboicutws-cell.github.io/Portfolio/

## Paginile de proiect (case study)

În `projects/` sunt 3 pagini exemplu: `princely-court.html` (Environment), `game-props.html` (Game Art), `product-branding.html` (Graphic Design).
Pozele lor merg în `assets/img/<nume-proiect>/` (ex: `assets/img/game-props/hero.jpg`, `asset-1.jpg`, `sketch.jpg`...). Numele exacte sunt în fiecare pagină, la `src="..."`.
Ca să faci o pagină nouă: copiază una din ele, schimbă textele și pozele, apoi adaugă pe pagina principală un link `Case study →` spre ea.

## Culori

Sunt luate din logo-ul KON: bleumarin `#0d152e`, verde mentă `#2fd990`, albastru `#6ba8f6`. Se schimbă din primele rânduri din `style.css`.
