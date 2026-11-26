# Portfolio

Portofoliul lui Tudor: video, animație, design și copywriting.

## Ce e în folder

| Fișier | Ce face |
|---|---|
| `index.html` | Pagina în sine: textele și proiectele |
| `style.css` | Culorile și aranjarea. Culorile se schimbă din primele rânduri |
| `assets/img/` | Pozele proiectelor (jpg, png, webp) |
| `assets/video/` | Clipuri scurte, comprimate (mp4 sub ~20 MB) |

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
