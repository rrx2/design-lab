# Area: design

Studio dell'explanatory design su dati e ricerca medica.

## Metodo: See → Name → Copy → Vary

1. **See**: si sceglie un riferimento visivo (articolo, infografica, grafico).
2. **Name**: lo si scompone e si dà un nome ai suoi elementi: palette, font, texture, forme, griglia, ritmo.
3. **Copy**: lo si rifà fedelmente su dati medici.
4. **Vary**: si rifà lo stesso contenuto negli altri stili, per vedere cosa cambia quando il contenuto resta fermo.

## Struttura

- `styles/<stile>.css`: un file per stile (palette, font, texture, forme). È l'atlante degli stili in forma di codice. In cima al file, un commento con il riferimento da cui nasce e cosa lo caratterizza.
- `articoli/<nome>/`: uno studio, con una pagina per ogni stile in cui è stato realizzato.
- `articoli/index.json`: elenco degli studi mostrati nella galleria. Voce: `{ "titolo": "...", "descrizione": "...", "path": "articoli/<nome>/" }`
- `index.html`: la galleria.

## Regole

- Si copia per studiare, citando sempre il riferimento. Non si pubblica come proprio lo stile di altri.
- Gli stili devono funzionare in tema chiaro e scuro e su schermo da telefono.
