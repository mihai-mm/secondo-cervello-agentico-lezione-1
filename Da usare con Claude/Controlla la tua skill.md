# Controlla la tua skill

Hai appena creato una skill e vuoi sapere se è fatta bene. Questo file lo dai al tuo Claude: legge la tua skill, risponde a otto domande e ti propone cosa migliorare, una cosa alla volta.

Non devi sapere niente di tecnico, e non devi aprire tu il file della skill.

---

## Le otto domande

Sono le stesse della slide di fine esercitazione.

1. **Il nome dice cosa fa?** Per esempio `/rispondi-preventivo`, non `/skill-1`.
2. **La descrizione dice quando usarla, in una frase?** La situazione di lavoro, per esempio «quando arriva una richiesta di preventivo». È la riga che Claude legge per capire se è la skill giusta.
3. **C'è dentro l'esempio che hai approvato?** La skill deve copiare la forma di quell'esempio, non inventarne una.
4. **Dice cosa le serve per partire?** Per esempio: la richiesta del cliente e il listino.
5. **Dice cosa fa quando manca un dato?** Non inventa: lo chiede a chi ce l'ha, oppure lascia lo spazio da completare. E se senza quel dato il lavoro non ha senso, si ferma e ti chiede cosa fare.
6. **Dice cosa non fa?** Non manda niente a nessuno e non scrive file senza il tuo sì.
7. **Ogni parte serve?** Niente ripetizioni e niente istruzioni fuori tema. Quanto è lunga dipende dal lavoro.
8. **L'hai provata in una conversazione nuova, su un caso diverso dal primo?** Meglio se a quel caso manca un dato.

## Come si usa

1. Questo file deve stare dentro il tuo vault, in `0-Inbox/`. Se hai messo lì l'intera cartella scaricata, è già a posto.
2. Apri nell'app una conversazione nuova nella cartella del vault e scrivi:

> leggi il file "Controlla la tua skill.md" e controlla la mia skill /nome-della-skill

Se non ricordi il nome, scrivi solo «controlla la mia skill»: Claude ti mostra quelle che hai.

## Cosa avrai alla fine

- Le otto risposte, ognuna con un sì o un no e il motivo in una riga.
- Le correzioni, scritte nella skill solo dopo il tuo sì.
- Se non l'avevi ancora provata, un caso nuovo su cui provarla.

## Se qualcosa non va

- **Claude non trova la skill?** Controlla di aver aperto la conversazione nella cartella del vault: la skill sta in `.claude/skills/`, dentro il vault.
- **Dopo una correzione la skill non cambia?** Apri una conversazione nuova e riprova. Se il comando non compare nel menu `/`, scrivi `/reload-skills`.
- Nel dubbio, mostra lo screenshot a Claude o scrivi nel gruppo WhatsApp del corso.

---

## Da qui in giù è per Claude: non devi leggerlo

### Regole

1. **Leggi, poi proponi.** Non modificare la skill senza un sì esplicito, una correzione alla volta. Per ogni correzione mostra la riga com'è e come diventa.
2. **Non riscrivere la skill da capo.** Correggi solo ciò che una delle otto domande ha trovato.
3. **Non cambiare il nome della cartella** senza dire prima che dopo il cambio serve una conversazione nuova, e senza il sì.
4. **Parole semplici**, frasi brevi, niente gergo. Cita la frase della skill da cui viene ogni risposta.
5. **Lascia stare `porta-i-tuoi-file`** e le skill che la persona non ha nominato.
6. Lascia questo file al suo posto: non spostarlo senza un sì esplicito.

### Come condurre

1. **Trova la skill.** Controlla di essere nel vault (contiene `LEGGIMI.md`, `CLAUDE.md` e le cartelle da `0-Inbox` a `4-Archives`). Se la persona ha dato il nome, apri `.claude/skills/<nome>/SKILL.md`. Se no, elenca le skill in `.claude/skills/` e chiedi quale ha creato: non provare a indovinare quali sono del pacchetto della Lezione 0.
2. **Leggi la skill per intero**, compresi gli altri file nella sua cartella.
3. **Rispondi alle otto domande** in una tabella: domanda, sì / in parte / no, motivo in una riga con la frase della skill. Criteri:
   - Domanda 1: dal nome si capisce cosa fa o cosa produce, con parole di tutti i giorni (`/preventivo-rapido` va bene; `/skill-1` o `/aiuto` no).
   - Domanda 2: il campo `description` dice cosa fa e in quale situazione di lavoro usarla («quando arriva una richiesta di preventivo»). Se è vago («aiuta con le email») o dice solo «quando scrivo /nome», è un no.
   - Domanda 3: dentro c'è un esempio di risultato, oppure una descrizione precisa della sua forma (parti, ordine, tono, saluto, firma).
   - Domanda 4: dice cosa chiede in ingresso.
   - Domanda 5: è la domanda più importante. Una skill nata da un solo esempio tende ad applicare il modello alla lettera: inventa il dato, lo chiede alla persona sbagliata o scrive comunque un risultato che senza quel dato non serve. Controlla tre cose: (a) dice cosa fare quando manca un dato; (b) dice **chi ha il dato** (la persona stessa, il cliente, un fornitore) e, se è il cliente, prepara la bozza per lui invece di chiederlo in chat; (c) distingue il dato che si può lasciare in sospeso da quello senza cui il risultato non ha senso: in quel caso non scrive il risultato e chiede cosa fare. Se manca una delle tre, è «in parte».
   - Domanda 6: dice cosa non fa (mandare, scrivere file senza sì, decidere al posto della persona).
   - Domanda 7: non conta il numero di righe: segnala ripetizioni, istruzioni generiche che Claude seguirebbe comunque e parti che non c'entrano con l'attività. Sopra le 500 righe proponi di spostare il dettaglio in un file a parte, nella stessa cartella.
   - Domanda 8: non lo puoi sapere dai file: chiedilo nello stesso messaggio della tabella.
4. **Proponi le correzioni**, partendo dai no e dalla domanda 5. Se per correggere ti serve sapere come lavora la persona (per esempio a chi chiede il dato che manca), chiediglielo: la regola viene dalla sua risposta, non da te. Una alla volta: mostra prima e dopo, aspetta il sì, scrivi, rileggi.
5. **La prova.** Se alla domanda 8 la risposta è no, o se hai corretto qualcosa, chiedi un caso vero recente, meglio se gli mancava un dato; se non ne ha, proponine uno tu sulla sua attività, con un dato mancante, e spiega come provarlo: conversazione nuova nella cartella del vault, `/nome-della-skill`, poi il caso. Chiedi di tornare qui con il risultato, o di incollarlo, se vuole un secondo parere.

### Chiusura

Riepiloga in tre righe: quante domande hanno avuto sì, cosa è stato corretto, cosa resta da provare. Se hai notato altro che le otto domande non coprono, dillo in una riga, senza correggerlo se la persona non lo chiede. Ricorda che la skill si migliora con l'uso: quando sbaglia, basta dire «correggi la skill <nome>: ...».
