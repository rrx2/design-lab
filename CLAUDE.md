# Design Lab

Un solo repo per tre attività separate. Lavoro in italiano.

| Area | Cartella | Cosa ci si fa |
|---|---|---|
| Ricerca | `ricerca/` | Ricerche su un argomento (scientifico o no), condotte con Claude in più interazioni, fino alle conclusioni |
| Design | `design/` | Studio dell'explanatory design: atlante degli stili e galleria degli studi |
| Video | `video/` | Video explanatory: script, storyboard, immagini (Midjourney / Nano Banana), motion design |

Ogni cartella ha il suo `CLAUDE.md` con il metodo di quell'area: leggilo prima di lavorarci.

## Capire su cosa sta lavorando l'utente

1. Se la richiesta nomina o tocca una cartella, l'area è quella.
2. Altrimenti decidi dalle parole: "ricerca", "fonti", "studi", "conclusioni" → ricerca; "stile", "palette", "font", "riferimento" → design; "video", "scena", "storyboard", "animazione", "prompt per le immagini" → video.
3. Se resta ambiguo, chiedi in una riga: "Ricerca, design o video?"

## Regole tra le aree

- Non mescolare: i file di un'area stanno nella sua cartella.
- Ricerca e video si collegano tramite lo **stesso nome dell'argomento** in kebab-case: `ricerca/fibrillazione-atriale.md` → `video/fibrillazione-atriale/`.
- Non tutte le ricerche diventano video. Un video parte sempre da una ricerca conclusa.
- Uno stile di `design/styles/` può diventare lo stile grafico di un video: in quel caso il video lo cita, non lo copia.
- Il repo è **pubblico** ed è pubblicato su GitHub Pages: niente dati di pazienti né materiale privato.

## Sito

`index.html` alla radice è la pagina principale e porta alle tre aree.
Pubblicato su https://rrx2.github.io/design-lab/
