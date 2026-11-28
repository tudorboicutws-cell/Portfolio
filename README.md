# Portfolio

Portofoliul lui Tudor Boicu: 3D environment, game art, graphic design și visual storytelling.

**Nu știi GitHub? Citește [GHID-EDITARE.md](GHID-EDITARE.md): totul pas cu pas, doar din browser.**

## Ce e în folder

| Fișier | Ce face |
|---|---|
| `index.html` | Pagina în sine: textele și proiectele |
| `style.css` | Culorile și aranjarea. Culorile se schimbă din primele rânduri |
| `assets/img/` | Pozele proiectelor (jpg, png, webp) |
| `assets/video/` | Clipuri scurte, comprimate (mp4 sub ~20 MB) |

## Pozele proiectelor

Fiecare proiect are:
- o poză de card pe pagina principală: `assets/img/<proiect>-cover.jpg` (960 x 600 px)
- un folder cu pozele lui: `assets/img/<proiect>/` (`hero.jpg` sus, `img-01.jpg`, `img-02.jpg`... în galerie, `ch1-00.jpg`, `ch1-01.jpg`... la capitole). Fiecare poză are și o variantă mică `-thumb.jpg`.
- clipurile, unde există, în `assets/video/`.

Logo-urile programelor și ale firmelor sunt în `assets/logos/`.

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

În `projects/` e câte o pagină pentru fiecare proiect din folderul Portofoliu (26 de pagini): Princely Court, Cultural Tourism, Palace of Culture, cele 6 game props, Unreal Engine 5, CLO 3D, Samdam, flyere, ilustrații, Treasure Hunt și Twinkle Star.
Paginile cu sub-foldere au **capitole** (de exemplu Princely Court, etapele 1-5). Sus pe fiecare pagină sunt logo-urile programelor folosite.
Ca să faci o pagină nouă: copiază una asemănătoare (de exemplu `projects/city-bus.html`), schimbă textele și pozele, apoi adaugă pe pagina principală un card spre ea.

## Culori

Sunt luate din logo-ul KON: bleumarin `#0d152e`, verde mentă `#2fd990`, albastru `#6ba8f6`. Se schimbă din primele rânduri din `style.css`.
