# Ghid: cum modifici portofoliul pe GitHub (fără programe, doar din browser)

Tot ce e aici se face pe **github.com**, logat pe contul tău. Nu instalezi nimic.
Orice salvare se numește **Commit**. După fiecare Commit, site-ul se actualizează singur în 1-2 minute.

---

## 0. Cuvinte pe care le vei vedea

| Cuvânt | Ce înseamnă |
|---|---|
| **Repository (repo)** | Folderul proiectului, pe GitHub. Al tău se numește `Portfolio`. |
| **Commit** | „Salvează”. Fiecare salvare rămâne în istoric, deci poți reveni oricând. |
| **main** | Versiunea principală. Ce e pe `main` apare pe site. |
| **Pages** | Serviciul GitHub care transformă repo-ul în site. |

---

## 1. Schimbi un text (de exemplu titlul mare sau o descriere)

1. Intră în repo-ul `Portfolio`.
2. Apasă pe fișierul **`index.html`** (pagina principală).
   Paginile de proiect sunt în folderul **`projects`**.
3. Sus în dreapta apasă pe **creionul ✏️** (Edit this file).
4. Apasă **Ctrl + F** și caută textul pe care vrei să-l schimbi (de exemplu `I build worlds`).
5. Schimbă **doar textul dintre semne**, nu și ce e între `<` și `>`.
   - Bine: `<h1>`**Textul tău nou**`</h1>`
   - Greșit: să ștergi `<h1>` sau `</h1>`
6. Sus în dreapta apasă butonul verde **Commit changes...**
7. În fereastra care apare lasă bifat **Commit directly to the main branch** și apasă **Commit changes**.
8. Așteaptă 1-2 minute și dă refresh la site.

---

## 2. Pui poze (cel mai des o să faci asta)

1. În repo, intră în folderul **`assets`** > **`img`** > folderul proiectului (de exemplu `game-props`).
2. Sus în dreapta: **Add file** > **Upload files**.
3. Trage pozele în pagină.
   **Important:** pozele trebuie să aibă exact numele cerut de pagină (de exemplu `hero.jpg`, `asset-1.jpg`).
   Lista de nume e în `README.md` și în fiecare pagină de proiect.
4. Jos apasă **Commit changes**.

Sfaturi pentru poze:
- Format **.jpg**, lățime în jur de **1600 px**, sub **1 MB** fiecare (le micșorezi gratuit pe squoosh.app).
- Numele: litere mici, fără spații și fără diacritice (`asset-1.jpg`, nu `Asset 1 final.JPG`).
- Ca să **înlocuiești** o poză, urci una nouă cu **același nume**. GitHub o suprascrie.

---

## 3. Adaugi un proiect nou pe pagina principală

1. Deschide `index.html` > creionul ✏️.
2. Caută (Ctrl + F) `<article class="card"`. Fiecare proiect e un bloc care începe cu `<article class="card"` și se termină cu `</article>`.
3. Selectează un bloc întreg, de la `<article` până la `</article>` inclusiv, copiază-l (Ctrl + C) și lipește-l (Ctrl + V) imediat sub el.
4. În copie schimbă: numele pozei din `src="assets/img/....jpg"`, eticheta (`tag`), titlul (`<h3>`), descrierea și linkurile.
5. La `data-cat="..."` pune categoria pentru filtre: `game`, `env`, `design` sau `story` (poți pune mai multe, cu spațiu între ele).
6. **Commit changes**.

## 4. Faci o pagină de proiect nouă

1. Intră în folderul `projects` și deschide pagina cea mai apropiată ca tip (de exemplu `game-props.html`).
2. Apasă pe iconița **Copy raw file** (două pătrățele, sus în dreapta) ca să copiezi tot.
3. Întoarce-te în folderul `projects` > **Add file** > **Create new file**.
4. Scrie numele, de exemplu `tavern-scene.html` (litere mici, cu cratimă), și lipește tot (Ctrl + V).
5. Schimbă textele și numele pozelor. Pozele lor merg într-un folder nou: `assets/img/tavern-scene/`.
6. **Commit changes**.
7. Pe pagina principală, la cardul proiectului, adaugă linkul:
   `<a class="case" href="projects/tavern-scene.html">Case study →</a>`

---

## 5. Ștergi ceva

- **Un fișier:** deschide-l > cele trei puncte **...** sus în dreapta > **Delete file** > **Commit changes**.
- **Un proiect de pe pagina principală:** în `index.html` șterge tot blocul `<article ...> ... </article>` > **Commit changes**.

## 6. Ai greșit ceva? Nu te panica

Nimic nu se pierde. Fiecare Commit e salvat în istoric.
1. Deschide fișierul stricat > butonul **History** (sus în dreapta, cu un ceas).
2. Apasă pe ultima versiune bună > cele trei puncte **...** > **View file**.
3. Copiază tot textul de acolo (Copy raw file), apoi editează fișierul actual (creionul ✏️), șterge tot (Ctrl + A, Delete), lipește versiunea bună și dă **Commit changes**.

Dacă site-ul arată ciudat după o modificare, de obicei ai șters din greșeală un `<` sau un `>`. Folosește pasul de mai sus.

## 7. Multe modificări deodată (opțional)

Pe pagina repo-ului apasă tasta **.** (punct). Se deschide un editor ca un program (github.dev), cu toate fișierele în stânga. Modifici ce vrei, apoi în stânga apeși iconița cu ramuri (Source Control), scrii un mesaj scurt și apeși **Commit & Push**.

---

## 8. Mutarea pe contul tău personal

**Varianta 1 (recomandată): Transfer**
1. Pe contul vechi: repo `Portfolio` > **Settings** > jos de tot **Danger Zone** > **Transfer ownership**.
2. Scrii username-ul contului personal, apoi numele repo-ului ca să confirmi > **I understand, transfer this repository**.
3. Pe contul personal primești un email: accepți transferul.
4. Pe contul personal: **Settings** > **Pages** > Branch: `main`, folder `/ (root)` > **Save**.
5. Site-ul va fi la `https://USERNAME.github.io/Portfolio/`.

**Varianta 2: din ZIP**
1. Pe repo-ul vechi: butonul verde **Code** > **Download ZIP**. Salvează-l pe stick sau în Google Drive.
2. Acasă, pe contul personal: **+** (sus dreapta) > **New repository** > nume `Portfolio`, **Public**, fără README > **Create repository**.
3. Apasă linkul **uploading an existing file**.
4. Dezarhivează ZIP-ul, intră în folder, selectează **tot ce e înăuntru** (nu folderul în sine) și trage în pagină.
5. **Commit changes**, apoi pornește Pages ca la pasul 4 de mai sus.

---

## 9. Cum te ajuți de un Claude gratuit sau de orice AI

1. Deschide fișierul pe GitHub > **Copy raw file**.
2. Lipește-l în chat și scrie ce vrei, de exemplu:
   *„Acesta e fișierul index.html al portofoliului meu. Adaugă un proiect nou în secțiunea Selected work, numit X, cu descrierea Y, categoria game. Dă-mi fișierul întreg înapoi.”*
3. Copiază răspunsul, editează fișierul pe GitHub (creionul ✏️), Ctrl + A, lipește, **Commit changes**.

Cere mereu **fișierul întreg**, nu bucăți, ca să nu greșești la lipit.
