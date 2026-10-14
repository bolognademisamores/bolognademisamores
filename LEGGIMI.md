# Bologna de Mis Amores – sito web

## Struttura
```
index.html            → home (italiano) + archivio edizioni
en/index.html         → home (inglese)
assets/style.css      → stile condiviso da tutte le edizioni
2027/index.html       → edizione 2027 (italiano)
en/2027/index.html    → edizione 2027 (inglese)
2027/img/             → immagini dell'edizione (condivise dalle due lingue)
```

## Immagini da inserire in `2027/img/`
- `banner.jpg`  → il tuo banner (sfondo dell'hero)
- `badge.png`   → l'immagine circolare/badge (logo, icona, footer)
- opzionali: `dj1.jpg`…`dj7.jpg`, `location1.jpg`…`location3.jpg`, `chisiamo1.jpg`…`chisiamo3.jpg`
- foto "Visitare Bologna": `citta1.jpg` (Piazza Maggiore), `citta2.jpg` (Quadrilatero), `citta3.jpg` (Santo Stefano)

## Cosa modificare in `2027/index.html`
1. Cerca tutto ciò che è tra `[parentesi quadre]` e sostituiscilo.
2. Nello `<script>` in fondo imposta `REG_OPEN` (apertura iscrizioni) e `FORM_URL` (link del Google Form).
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

## Date e modulo (in fondo a 2027/index.html e en/2027/index.html)
- EVENT_START: inizio encuentro (27 agosto 2027), usato dal conto alla rovescia.
- REG_OPEN: apertura iscrizioni (10 novembre 2026). Prima di quel giorno il sito mostra l'annuncio; dopo, compaiono prezzi e modulo.
- FORM_URL: incolla qui l'indirizzo del Google Form. Va cambiato in entrambe le lingue.
