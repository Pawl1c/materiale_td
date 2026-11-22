# Protetică Dentară – Ceramică | Site GitHub Pages

Site static interactiv care reunește suporturile de învățare pentru:
- Capitolul 12 – Coroana mixtă metalo-ceramică
- Capitolul 13 – Coroana integral ceramică

## Funcționalități
- capitole și subcapitole generate din cele două documente Word;
- tabele, clasificări, etape de laborator și valori tehnice;
- căutare în material;
- mod Light / Dark;
- quiz pentru fiecare capitol, feedback explicativ și prag de promovare de 70%;
- salvarea progresului în browser (localStorage);
- imagini generate și scheme SVG pentru zirconia și CAD/CAM;
- materiale video externe și linkuri către resurse;
- documentele Word și PDF-urile sursă incluse în `assets/`.

## Publicare pe GitHub Pages

1. Descarcă și dezarhivează `protetica-ceramica-github-pages.zip`.
2. Intră pe GitHub și creează un repository nou, de exemplu `protetica-ceramica`.
3. Încarcă **conținutul folderului** proiectului în rădăcina repository-ului. Fișierul `index.html` trebuie să fie direct în rădăcină, nu într-un subfolder.
4. Deschide repository → **Settings** → **Pages**.
5. La **Build and deployment**, alege **Deploy from a branch**.
6. Selectează branch-ul `main` și folderul `/ (root)`, apoi apasă **Save**.
7. Așteaptă publicarea; adresa va fi de forma `https://NUME-UTILIZATOR.github.io/protetica-ceramica/`.

## Testare locală (opțional)
Nu deschide `index.html` direct prin `file://`, deoarece materialul este încărcat din fișiere JSON. În folderul proiectului rulează:

```bash
python -m http.server 8000
```

Apoi deschide `http://localhost:8000`.

## Personalizare
- Textul cursului: `content.json`
- Întrebările quiz: `quiz.json`
- Stiluri: `styles.css`
- Funcționalități: `app.js`
- Imagini și PDF/Word: `assets/`

## Note importante
- Conținutul educațional este reorganizat pe baza celor două suporturi furnizate. Valorile tehnice din exemple trebuie interpretate în contextul cursului și al instrucțiunilor producătorului.
- Videoclipurile sunt resurse externe și pot fi mutate sau eliminate de platformele-gazdă.
- Progresul este salvat local în browserul utilizatorului, nu într-un cont online și nu se sincronizează între dispozitive.
- Imaginile generate sunt ilustrative, nu fotografii clinice și nu înlocuiesc documentația tehnică a producătorilor.
