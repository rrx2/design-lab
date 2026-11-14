# Area: video

Video explanatory a partire da una ricerca conclusa. Una cartella per video: `video/<argomento>/`, con lo stesso nome del file in `ricerca/`.

## Ruoli

- **L'utente** genera le immagini con Midjourney o Nano Banana e decide il contenuto.
- **Claude** scrive i prompt per le immagini, guida la composizione (ritmo, inquadrature, ordine delle scene) e fa il motion design con HyperFrames: scene in HTML/CSS animate e poi esportate in video. Prima di animare, carica la skill `hyperframes:hyperframes`.

## Passi

1. **Script** (`script.md`): parte da `ricerca/<argomento>.md`. Testo della voce fuori campo diviso in scene; per ogni scena, un messaggio solo.
2. **Storyboard** (`storyboard.md`): per ogni scena durata, immagine, cosa si muove e perché, testo a schermo.
3. **Prompt** (`prompts.md`): un prompt per ogni immagine dello storyboard, con lo stesso stile tra tutte le immagini. Indica per quale strumento è pensato (Midjourney o Nano Banana) e il formato (16:9, 9:16...).
4. **Immagini** (`assets/`): le immagini che l'utente genera e salva qui, con il numero della scena nel nome (`s03-cuore.png`).
5. **Animazione** (`animazione/`): il progetto HyperFrames.
6. **Revisione**: si guarda il render, si corregge, si riesporta.

Non saltare passi senza chiedere: lo storyboard viene approvato prima di scrivere i prompt, i prompt prima di animare.

## Regole

- Le affermazioni del video devono essere sostenute dalla ricerca. Se lo script dice qualcosa che la ricerca non contiene, segnalalo.
- I file video sopra i 50 MB non vanno nel repo (GitHub rifiuta i file oltre i 100 MB). I render finali si tengono fuori o si pubblicano altrove.
- Se il video usa uno stile di `design/styles/`, scrivilo nello storyboard.
