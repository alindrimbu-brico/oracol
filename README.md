# Oracolul celor Cinci Cercuri · The Five Circles Oracle

Site interactiv (52 de cărți, RO/EN) sub brandul **Focul care cunoaște**.

## Cum îl publici pe GitHub Pages

### Varianta simplă (din browser, fără git)
1. Creează un repository nou (ex. `oracol`), **Public**.
2. **Add file → Upload files** → trage aici `index.html`, `og-oracol.jpg` și `.nojekyll`.
3. **Commit changes**.
4. **Settings → Pages** → *Source*: „Deploy from a branch" → *Branch*: `main` / folder `/ (root)` → **Save**.
5. Așteaptă ~1 minut. Site-ul e live la:
   `https://<utilizator>.github.io/oracol/`

### Varianta din terminal (git)
```bash
git init
git add index.html og-oracol.jpg .nojekyll
git commit -m "Oracolul celor Cinci Cercuri"
git branch -M main
git remote add origin https://github.com/<utilizator>/oracol.git
git push -u origin main
```
Apoi activează **Settings → Pages** ca mai sus.

## Un singur retuș (pentru partajări pe rețele)
După ce știi adresa finală, în `index.html` înlocuiește în cele două locuri
`og-oracol.jpg` cu adresa completă, ex.:
`https://<utilizator>.github.io/oracol/og-oracol.jpg`
(la `og:image` și `twitter:image`). Fără asta, imaginea de previzualizare
poate să nu apară la distribuire pe Facebook/WhatsApp/X.

## Domeniu propriu (opțional)
Dacă vrei `oracol.reverb.ro`: Settings → Pages → *Custom domain* →
scrie domeniul, apoi adaugă la DNS un `CNAME` către `<utilizator>.github.io`.

---
Ține toate fișierele în același folder. Nimic de instalat — e un singur HTML.
