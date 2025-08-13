# La Figue Édition – Static Site Starter

Contenuto:
- `index.html` (Home)
- `libri/conversando-con-debussy.html` (pagina libro)
- `press.html` (Press/Contatti con modulo via provider esterno)
- `privacy.html` (informativa base)
- `CNAME` (custom domain GitHub Pages: www.lafigue-ed.com)

## Deploy su GitHub Pages
1. Crea un account GitHub (se non lo hai).
2. Nuovo repository pubblico, es. `lafigue-ed`.
3. Carica i file mantenendo la struttura.
4. Settings → Pages → Source: `Deploy from a branch` → Branch: `main` → Folder: `/ (root)` → Save.
5. Settings → Pages → Custom domain: inserisci `www.lafigue-ed.com` → Save → abilita **Enforce HTTPS**.
6. Nel **pannello DNS** del registrar aggiungi un **CNAME**:
   - Host: `www`
   - Valore: `<tuo-username>.github.io`
   (Non toccare i record **MX** per l'email.)
7. (Opzionale) Redirect 301 dall'apice `lafigue-ed.com` a `https://www.lafigue-ed.com` nel registrar (URL forwarding).

## Modulo inviti (Press)
- In `press.html` sostituisci `YOUR_ACCESS_KEY` con la chiave del provider (Web3Forms/Formspree).
- Configura l'inoltro verso `info@lafigue-ed.com` dal pannello del provider.

## Aggiornare link utili
- Bottone “Acquista il libro”: modifica in `libri/conversando-con-debussy.html`.
- “Scarica press kit (PDF)”: carica un PDF nel repo (es. `press-kit.pdf`) e aggiorna il link.

## Privacy
- Testo base da personalizzare. Se aggiungi Analytics, integra il banner cookie.

— Generato: 2025-08-13
