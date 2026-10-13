# Bologna de Mis Amores – sito web

## Struttura
```
index.html            → home + archivio edizioni
assets/style.css      → stile condiviso da tutte le edizioni
2027/index.html       → edizione 2027
2027/img/             → immagini dell'edizione
```

## Immagini da inserire in `2027/img/`
- `banner.jpg`  → il tuo banner (sfondo dell'hero)
- `badge.png`   → l'immagine circolare/badge (logo, icona, footer)
- opzionali: `dj1.jpg`, `dj2.jpg`, `dj3.jpg`, `citta1.jpg`, `citta2.jpg`, `citta3.jpg`

## Cosa modificare in `2027/index.html`
1. Cerca tutto ciò che è tra `[parentesi quadre]` e sostituiscilo.
2. In fondo al file, nello `<script>`, imposta `DEADLINE` e `DEADLINE_TEXT`.
   Alla scadenza il modulo si nasconde da solo e compare "Iscrizioni chiuse".
3. Iscrizioni: crea un Google Form → Invia → `< >` Incorpora HTML → copia
   l'URL dentro `src` dell'iframe `form-frame`.
4. Mappa: Google Maps → Condividi → Incorpora una mappa → sostituisci `src`.

## Nuova edizione (ogni anno)
1. Copia la cartella `2027` e rinominala `2028`.
2. Aggiorna testi, date, DJ, deadline e immagini.
3. In `index.html` (home) cambia il link del pulsante principale in `2028/`
   e aggiungi la scheda nell'archivio. Le edizioni vecchie restano online.

## Pubblicazione gratuita (Cloudflare Pages o GitHub Pages)
**Cloudflare Pages**: Workers & Pages → Create → Pages → Upload assets →
trascina la cartella. Indirizzo: `nomescelto.pages.dev`.
**GitHub Pages**: crea un repository, carica i file, Settings → Pages →
Deploy from branch (main). Indirizzo: `utente.github.io/repo`.
