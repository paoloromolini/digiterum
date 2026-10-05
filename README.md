# Digiterum

*Sbagliando si impara.* Un'app di touch typing che si concentra sugli errori.

## Uso

Apri `index.html` nel browser. Nessuna installazione né dipendenze.

## Come funziona

- **Niente Backspace**: se sbagli un carattere la parola è bocciata. Finisci di digitarla, premi spazio e la parola ritorna 2-4 posizioni più avanti, finché non la scrivi correttamente.
- **Modalità**: 60s, 30s o libera (senza timer). Il timer parte al primo tasto.
- **Punti deboli**: le parole sbagliate vengono salvate e riproposte nelle sessioni successive. Il pulsante *Solo punti deboli* usa solo quelle.
- **Storico**: a fine sessione vedi WPM, accuratezza, parole sbagliate e il grafico delle ultime sessioni.
- **Lingue**: parole in inglese o italiano.

## Tasti

| Tasto | Azione |
|-------|--------|
| Spazio / Invio | Conferma la parola |
| Tab | Ricomincia |
| Esc | Termina la sessione |

## Dati

Parole deboli e storico sono salvati in `localStorage`, quindi restano nel browser in uso.
