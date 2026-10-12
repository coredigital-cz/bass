# STANA BASS ACADEMY — site

Site static (un singur `index.html`), gata de GitHub Pages. Fără build, fără dependențe.
Design colorat, jucăuș, pentru copii și adolescenți: ecran de încărcare, bas interactiv (apasă pe corzi), animații la scroll, formular de înscriere și buton fix „Înscrie-te" pe telefon.

## Publicare pe GitHub Pages

1. Încarcă tot conținutul acestui folder în rădăcina repository-ului (`index.html`, `assets/`, `.nojekyll`).
2. În repository: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / folder **/ (root)** → **Save**
3. După 1–2 minute site-ul e live la `https://<cont>.github.io/<repo>/`.

Domeniu propriu: **Settings → Pages → Custom domain**, apoi `CNAME` la registrar către `<cont>.github.io`.

## Ce trebuie completat

### 1. Date de contact (important pentru înscrieri)
La începutul `<body>` din `index.html` există blocul `window.SITE`. Completează cel puțin `whatsapp` (ex. `'40712345678'`) sau `email`.
Formularul de înscriere deschide WhatsApp (sau emailul) cu mesajul deja scris. Până nu completezi unul dintre ele, formularul afișează un mesaj că nu e conectat.

### 2. Poze și afișe
- `assets/afise/afis-1.jpg`, `afis-2.jpg` ... → afișele
- `assets/poze/poza-1.jpg`, `poza-2.jpg` ... → poze reale
- `assets/andrei-stan.jpg` → portretul fondatorului (4:5), înlocuiește monograma „AS"

Apar automat în site (secțiunea „Galerie" se afișează doar dacă există imagini).

### 3. Link de partajare
În `<head>`, `og:image` pointează la `https://coredigital-cz.github.io/bass/assets/og-image.png`. Dacă site-ul ajunge la altă adresă, schimbă URL-ul.

## Logo
În `assets/`: `logo.svg` (fundal deschis), `logo-on-dark.svg` (fundal închis), `logo-mark.svg` / `favicon.svg` (doar emblema), plus variante PNG și `og-image.png` (1200×630) pentru rețele sociale.

## Fonturi
Bricolage Grotesque și Nunito, găzduite local în `assets/fonts/` (licență OFL), deci site-ul nu depinde de Google Fonts.
