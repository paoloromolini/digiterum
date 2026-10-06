# Digiterum

*Sbagliando si impara.* Un'app di touch typing che si concentra sugli errori.

## Uso

Apri `index.html` nel browser. Nessuna installazione né dipendenze. Dentro l'app il pulsante **? Aiuto** (o `F1` / `?`) spiega come funziona.

## Come funziona

### Il gioco
- Scrivi la parola evidenziata e premi spazio o Invio per confermarla.
- **Niente Backspace**: se sbagli anche un solo carattere la parola è bocciata e **ritorna dopo 2-4 parole**, finché non la scrivi correttamente.
- **Modalità**: 60s, 30s o Libera (senza timer, chiudi con Esc). Il timer parte al primo tasto.
- **WPM**: conta solo le parole corrette (5 caratteri = 1 parola). L'accuratezza è la percentuale di tasti giusti.
- **Lingue**: parole in inglese o italiano.
- **Suoni**: click a ogni tasto giusto, tonfo sordo su quello sbagliato (sintetizzati, nessun file audio). Il pulsante **Suono** li spegne.

### Punti deboli
- Le parole sbagliate vengono salvate e riproposte nelle sessioni successive (circa il 35% delle parole, quando ne hai almeno 3).
- Ogni errore dà 2 punti di debolezza alla parola (massimo 6), ogni scrittura corretta ne toglie 1. A zero la parola esce dalla lista.
- Il pulsante **Solo punti deboli** usa soltanto quelle parole.

### Fermati e concentrati
Alla **4ª volta** che sbagli la stessa parola nella sessione (e poi alla 8ª, 12ª…) si apre un esercizio a schermo intero. Il timer è in pausa e le battute non contano nelle statistiche.
1. **Replay al rallentatore** dei tuoi errori su quella parola: ogni tasto premuto compare uno alla volta, con il tasto giusto, le dita coinvolte, le esitazioni e il tipo di errore (tasto vicino o lontano, lettere invertite, lettera saltata o in più, parola troppo corta), accompagnato da un click d'orologio a ogni tasto (si spegne con `M`).
2. **Ripetizioni**: devi scrivere la parola **4 volte di fila** senza errori. Un errore azzera il conteggio. Una tastiera con i tasti colorati per dito indica il prossimo tasto e quale dito usare.

### Dita
Il pulsante **Dita** mostra, sotto il testo, la tastiera con il prossimo tasto evidenziato e il dito da usare (disposizione QWERTY standard a dieci dita). Si può spegnere.

### Fine sessione
Alla fine vedi WPM, accuratezza, le parole sbagliate e il grafico delle ultime sessioni (WPM e accuratezza), con record personale e media.

## Tasti

| Tasto | Azione |
|-------|--------|
| Spazio / Invio | Conferma la parola |
| Tab | Ricomincia |
| Esc | Termina la sessione |
| F1 / ? | Apre l'aiuto |

## Dati

Parole deboli, storico e preferenze sono salvati in `localStorage`, quindi restano nel browser in uso (non sono sincronizzati tra dispositivi). L'app chiede al browser di non eliminarli automaticamente.

## Pubblicazione

È un singolo file statico, quindi funziona su GitHub Pages senza build.
