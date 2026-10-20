# Crea una skill dalla tua attività

Questo è un file guidato: lo dai al tuo Claude e lui ti accompagna, un passo alla volta, a trasformare un'attività che ripeti spesso in una **skill** tua (nel tuo pacchetto le skill si chiamano anche procedure): un comando, per esempio `/preventivo-rapido`, che fa quel lavoro sempre allo stesso modo.

È l'esercitazione della lezione: in aula la fai con Mihai che ti aiuta se ti blocchi. Se non finisci, la riprendi a casa da dove eri rimasto: in fondo a questo file c'è il registro dei passi.

Il metodo è quello che hai visto con `/recap-discovery`. Si riassume in una frase: **prima approvi un esempio, poi deleghi gli altri.**

Non devi sapere niente di tecnico. Ti servono un'attività vera e un esempio vero di come la fai oggi.

## Cosa avrai alla fine

- Una skill tua, in `.claude/skills/nome-della-skill/SKILL.md`, accanto a `porta-i-tuoi-file`.
- Un comando `/nome-della-skill` che la fa partire.
- La prova che funziona: l'hai usata in una conversazione nuova, su un secondo caso, e il risultato ha la forma che avevi approvato.

## Cosa ti serve prima di partire

- L'app di Claude per computer, con aperta la cartella del tuo vault (quella della Lezione 0).
- **Un'attività che fai spesso**, sempre quasi uguale: una risposta ai clienti, un preventivo, un report, un verbale, un riepilogo. Se ne hai più di una, scegline una sola.
- **Un esempio vero di come la fai oggi**: il risultato finito (un'email già mandata, un documento già consegnato) e, se ce l'hai, ciò da cui parti (gli appunti, la richiesta del cliente, i dati).

Se non hai un'attività in mente, o non hai finito la Lezione 0, non è un problema: guarda «Se non hai un'attività» più sotto.

## Come si usa

1. Questo file deve stare dentro il tuo vault, in `0-Inbox/`. Se hai messo lì l'intera cartella scaricata, è già a posto. **Claude lavora solo dentro il vault**: un file lasciato in Download non lo legge.
2. Apri nell'app una conversazione nuova nella cartella del vault (non in un'altra cartella: deve contenere il file `LEGGIMI.md` e le cartelle da `0-Inbox` a `4-Archives`).
3. Scrivi:

> leggi il file "Crea una skill dalla tua attività.md" e seguilo

(usa il nome del file come lo vedi nella cartella)

Da lì in poi Claude ti guida lui. Quando vuoi fermarti, basta dire "ci fermiamo qui".

Un'avvertenza: non chiedere di «smistare l'inbox» finché non hai finito. Questo file deve restare in `0-Inbox/`, perché Claude ci scrive il registro dei passi.

## Se non hai un'attività, o non hai finito la Lezione 0

Hai due strade, già pronte, che ti portano comunque a una skill funzionante o a una scheda utile:

- **`/recap-call`**: dalla registrazione di una call, un recap ordinato con i compiti. Guida: Crea la tua skill recap-call. Ti serve una trascrizione: quella di esempio c'è.
- **Lo `STYLE.md`**: la scheda del tuo modo di scrivere. Guida: Crea il tuo stile di scrittura.

Se ti manca anche solo il vault della Lezione 0, finisci prima quella: serve una cartella con `CLAUDE.md`, `_claude/` e `0-Inbox/`.

## Se qualcosa non va

- **In aula**: scrivilo in chat o alza la mano. Se il problema è di molti, lo risolviamo davanti a tutti. Se è solo tuo, ti aiuto a parte o nel gruppo WhatsApp del corso: non serve fermare tutti.
- **A casa**: chiedi a Claude e mostragli lo screenshot, come nella Lezione 0.
- Le richieste che puoi vedere: l'app può chiederti il permesso di scrivere dentro `.claude/` (succede al Passo 5, te lo spiega prima), e il Mac può chiederti se «Claude» può accedere a Documenti, Scrivania o Download (va consentito).

---

## Dove sei

Claude aggiorna queste tre righe alla fine di ogni passo, e il registro in fondo al file.

- **Passo attuale**: 1 di 6
- **Ultima sessione**: -
- **Note**: -

---

## Stile di lavoro (regole per Claude)

Queste sono le regole che il tuo Claude deve seguire mentre ti guida. Se le viola, fermalo. Si aggiungono a quelle del `CLAUDE.md` del vault; se qualcosa è in conflitto, valgono quelle del vault, e Claude lo dice.

1. **Sei la guida, un passo alla volta.** Mai fare due passi senza la conferma della persona. Una domanda alla volta, mai più di tre per messaggio. Dopo ogni domanda aspetta la risposta.
2. **Annuncia prima di scrivere.** Prima di creare o modificare un file dici quale file, dove e con cosa, e aspetti il sì in chat. Dopo averlo scritto lo rileggi e dici come verificarlo («apri il file X: se vedi Y ha funzionato»).
3. **Niente letture fuori dal vault.** Non usare lo strumento di lettura, né ricerche per nome o contenuto, su cartelle fuori dal vault. Se l'esempio è altrove sul computer, chiedi di incollarlo in chat o di copiarlo in `0-Inbox/` (lo fa la persona, con il Finder). Non usare `porta-i-tuoi-file` per questo: serve a portare progetti interi.
4. **Spiega ogni termine nuovo** la prima volta: skill (nel pacchetto: procedura), vault, `SKILL.md`, modalità. Niente gergo dato per scontato.
5. **Non inventare l'attività, l'esempio o i fatti della persona.** Se un dato manca, chiedilo; se non c'è, scrivi "da definire". Distingui ciò che è scritto nell'esempio (fonte), ciò che hai verificato e ciò che ipotizzi.
6. **Se un file non si legge**, dillo con il rimedio: un file Word (.docx) non si legge direttamente (copia e incolla il testo, oppure salva come PDF); un PDF oltre 10 pagine chiede un programma in più sul Mac (meglio incollare il testo). **Non ricostruire mai un file dal suo nome.**
7. **Nessun invio, nessuna pubblicazione, nessun contatto con altre persone.** La skill prepara bozze; manda chi le rilegge.
8. **Intoppi.** Se qualcosa non torna, non tirare a indovinare: chiedi cosa vede sullo schermo, di incollare il messaggio o di mandare uno screenshot. Poi rispondi in parole semplici: cosa è successo, perché, l'unica cosa da fare adesso e la strada alternativa. Se un'azione viene bloccata, dillo e proponi un'altra strada: non insistere con lo stesso comando.
9. **Lascia il file al suo posto.** Non spostare né eliminare questo file senza un sì esplicito.

## Come condurre

All'avvio:

1. Di' in quale cartella stai lavorando e controlla che sia il vault: contiene `LEGGIMI.md`, `CLAUDE.md` e le cartelle da `0-Inbox` a `4-Archives`. Se non è la cartella giusta, fermati e dillo.
2. Leggi il registro in fondo a questo file. Se ci sono passi già fatti, **riparti dal primo non spuntato**: non rifare domande a cui la persona ha già risposto (le risposte sono nel registro e nei file scritti). Se il registro è vuoto, comincia dal Passo 1.
3. Mostra il percorso in una riga per passo, poi annuncia il passo: cosa fate, perché serve, cosa ci sarà alla fine.

Dopo ogni passo: **annuncia** l'aggiornamento di questo file, spunta le caselle del passo con la data (`✅ AAAA-MM-GG`; un passo che non si applica si spunta con una nota «saltato: ...»), aggiorna le tre righe di «Dove sei» e aggiungi una riga in cima al registro, con ciò che serve per riprendere (attività scelta, nome del file di esempio, nome della skill, regole approvate). Poi chiedi: «continuiamo con il prossimo passo o ci fermiamo qui?».

Se la persona si ferma: dille che la prossima volta basta aprire una conversazione nuova nella cartella del vault e scrivere la frase della sezione «Se non hai finito in aula».

---

## I sei passi

### Passo 1 - Scegli l'attività

Il lavoro che ripeti sempre uguale. È da lì che nasce una skill.

- [ ] Claude chiede: «Quale lavoro ripeti spesso e vorresti non rifare ogni volta da capo?». Se la persona non sa scegliere, propone tre esempi presi da ciò che ha scritto in `_claude/PROFILO.md` (sezione «Cosa mi fa perdere tempo»), senza decidere al posto suo.
- [ ] Verifica che l'attività sia adatta a una skill: la fai **spesso** (almeno una volta alla settimana, o ogni volta che c'è un nuovo cliente), il risultato ha **ogni volta più o meno la stessa forma**, e ne hai già un esempio fatto bene. Se invece la fai una volta sola o cambia ogni volta, è meglio un prompt: lo dice, e ne cerca un'altra insieme alla persona.
- [ ] Se la persona non ha un'attività, o non ha finito la Lezione 0, Claude le propone le due strade della sezione «Se non hai un'attività»: la guida `/recap-call` o la guida allo `STYLE.md`. Si ferma qui, senza forzare.
- [ ] Claude riassume l'attività in quattro righe: **cosa ricevi** (l'input), **cosa produci** (il risultato), **per chi**, **ogni quanto**. Propone un nome per la skill (parole minuscole separate da trattini, per esempio `risposta-richiesta-info`).

**Output atteso**: le quattro righe e il nome proposto, scritti nel registro in fondo a questo file.
**Verifica**: leggi le quattro righe e rispondi «sì, è questa». Se qualcosa non è esatto, correggilo ora: costa meno che dopo.
**Se non funziona**: se non trovi un'attività, pensa all'ultima cosa che hai rifatto con le stesse parole: un'email, un'offerta, un verbale. Oppure scegli una delle due strade.

### Passo 2 - Dai a Claude un esempio vero

Una skill buona parte da un lavoro fatto bene, non da una descrizione.

- [ ] Claude ti chiede **un esempio di come la fai oggi**: il risultato finito e, se ce l'hai, ciò da cui sei partito.
- [ ] Puoi dargli l'esempio in due modi: **incollandolo in chat**, oppure **mettendo il file in `0-Inbox/`** (lo trascini tu, con il Finder, nella cartella `0-Inbox` del vault) e dicendogli il nome. Non dargli un percorso fuori dal vault: non lo legge.
- [ ] Claude legge l'esempio per intero e ti dice, in cinque-otto righe, come ha capito il lavoro: da cosa parti, cosa produci, in che forma, quali parti si ripetono sempre e dove interviene il tuo giudizio. Se ha dubbi su un punto, te lo chiede.

**Output atteso**: la descrizione di «come la fai oggi» in cinque-otto righe, e il nome del file di esempio (o «incollato in chat») nel registro. Nessun altro file scritto.
**Verifica**: la descrizione ti somiglia? Correggi quello che non torna.
**Se non funziona**: se il file è un Word (.docx), incolla il testo in chat o salvalo come PDF; se è un PDF lungo più di 10 pagine, incolla il testo. Se il file non si trova, controlla che sia davvero in `0-Inbox/`.

### Passo 3 - Falla una volta a mano, insieme a Claude

Prima si fa il lavoro, poi si automatizza.

- [ ] Claude fa il lavoro **una volta**, a mano, in chat, partendo da un caso vero: quello dell'esempio, oppure un altro che gli dai. Segue la forma dell'esempio.
- [ ] Ti mostra il risultato in chat. **Non salva niente.** Dove manca un'informazione scrive «da completare», non la inventa.
- [ ] Ti chiede: «È nella forma che ti aspettavi?».

**Output atteso**: un primo risultato in chat, nella forma del tuo esempio.
**Verifica**: confrontalo con il tuo esempio. Se la forma è sbagliata, dillo: non passare al passo dopo con un risultato che non ti convince.
**Se non funziona**: se Claude si inventa dati o frasi che non erano nell'esempio, fermalo: «usa solo quello che ti ho dato, il resto lasciamolo da completare».

### Passo 4 - Correggi e approva

È il passo che conta di più: **prima approvi un esempio, poi deleghi gli altri.** Una skill fatta partire da un risultato che non hai approvato imparerà gli stessi difetti.

- [ ] Tu dici cosa togliere, cosa aggiungere, cosa cambiare («questa frase non la direi», «qui manca il prezzo», «va più corto»). Claude applica le correzioni e ti mostra la versione nuova.
- [ ] Si ripete finché scrivi la parola **«approvato»**. Un «va bene» generico non basta: Claude ti chiede conferma.
- [ ] Quando approvi, Claude ricava dalle tue correzioni **le regole** del lavoro: la forma del risultato, il tono, cosa non fare mai, cosa chiedere se manca. Le scrive in poche righe e te le mostra. Prima di fissare una regola la confronta con il tuo esempio originale: se lo contraddice, la limita al caso in cui è nata.
- [ ] Poi ti chiede: **«E quando il caso non è quello solito, cosa fai? Per esempio quando manca un dato (il prezzo, la quantità, una data) o la richiesta è diversa dal solito.»** Ti chiede anche a chi chiedi il dato che manca: a te stesso, al cliente o a un collega. La risposta diventa una regola: di solito la skill prepara comunque la bozza giusta per quel caso, per esempio un'email al cliente che chiede il dato, invece di riempire il modello con dei buchi o fermarsi.

**Output atteso**: un risultato approvato, e l'elenco delle regole che ne sono uscite, compresa quella per i casi diversi dal solito, scritto nel registro.
**Verifica**: leggi l'elenco. Ogni regola deve essere una cosa che vorresti davvero ogni volta. Togli quelle che valevano solo per questo caso.
**Se non funziona**: se le correzioni si accavallano, chiedi a Claude di riscrivere il risultato da capo con tutte le correzioni insieme, e rileggilo.

### Passo 5 - Trasformalo in una skill

Adesso il lavoro diventa un comando.

- [ ] **Prima di scrivere**, Claude ti spiega due cose. La prima: la skill nascerà in una cartella nuova del vault, `.claude/skills/<nome>/`, con dentro un file `SKILL.md`, accanto a `porta-i-tuoi-file`. La seconda: scrivendo lì, **l'app mostrerà una richiesta di permesso**, perché `.claude/` è una cartella speciale. È normale: consentila. Se non compare, bene lo stesso.
- [ ] Claude ti propone il **nome** (quello del Passo 1, se ti va ancora), la **descrizione** in una frase (quando usarla) e il **contenuto in breve**, e aspetta il tuo sì. Il contenuto è essenziale (ogni parte serve, mai oltre le 500 righe) e dice: quando si usa, cosa chiede in ingresso, i passi, la **forma del risultato** (l'esempio approvato, senza i nomi e i dati del caso specifico), cosa fa quando il caso non è quello solito o manca un'informazione (la regola del Passo 4: non inventa, e prepara la bozza giusta per quel caso), cosa non fa (non manda niente a nessuno, non scrive dove non gli hai detto di scrivere).
- [ ] Ti chiede **dove salvare il risultato**: in chat, oppure in un file del vault (per esempio `reports/` di un progetto). Lo scrive nella skill. Senza una scelta, la skill mostra il risultato in chat e non scrive file.
- [ ] Con il tuo sì, Claude crea la skill, la **rilegge** e te la mostra.

**Output atteso**: il file `.claude/skills/<nome>/SKILL.md`, corto, che riassume il lavoro approvato.
**Verifica**: scrivi `/` nella chat: nel menu deve comparire il nome della tua skill. Se non compare, scrivi `/reload-skills`. Per vedere il file: `.claude` non compare in Obsidian (nasconde le cartelle che iniziano con un punto, è normale); nel Finder premi Cmd+Maiusc+punto per mostrare i file nascosti, oppure chiedi a Claude di mostrarti il contenuto in chat.
**Se non funziona**: se la richiesta di permesso viene rifiutata, la skill non viene scritta: Claude lo dice e ti chiede di riprovare consentendola. Se il permesso non compare e il file non c'è, incolla il messaggio che vedi: ne parliamo insieme.

### Passo 6 - Provala in una conversazione nuova, su un secondo caso

Una skill vale se funziona senza di te accanto.

- [ ] Apri una **conversazione nuova** nella cartella del vault (la guida resta in `0-Inbox/`, non serve).
- [ ] Scrivi `/nome-della-tua-skill` e dai un **secondo caso**: un altro cliente, un'altra richiesta, un altro dato. Non lo stesso del Passo 3. Meglio ancora se è un caso **a cui manca un dato** o un po' diverso dal solito: è lì che si vede se la skill ragiona o copia il modello.
- [ ] Guarda il risultato: ha la forma che avevi approvato? Ha inventato qualcosa? Se mancava un dato, ha fatto ciò che avevi deciso al Passo 4? Ha chiesto prima di scrivere un file?
- [ ] Se c'è da ritoccare, dillo a Claude nella stessa conversazione («correggi la skill nome: ...»): Claude propone la modifica e la scrive dopo il tuo sì. Poi riprova.
- [ ] Quando ti torna, torna alla conversazione della guida e scrivi «provata» (se l'hai chiusa, apri una conversazione nuova e usa la frase della sezione «Se non hai finito in aula»): Claude spunta il passo.

**Output atteso**: un secondo risultato, prodotto dalla skill da sola, nella forma approvata.
**Verifica**: confrontalo con l'esempio approvato al Passo 4. Non deve essere identico (il caso è diverso): deve avere la stessa forma e lo stesso tono.
**Se non funziona**: se il comando non parte, controlla di essere nella cartella del vault e riprova con `/reload-skills`. Se il risultato è generico, la skill è troppo vaga: chiedi a Claude di aggiungere l'esempio approvato o la regola che manca.

---

## Chiusura

Claude riepiloga in tre righe: quale attività hai trasformato, come si chiama la skill e dove sta, cosa hai verificato. Poi ti ricorda tre cose:

- **Una skill non nasce perfetta, cresce con te.** La usi sul lavoro vero, vedi cosa le manca, e gliela aggiungi a parole.
- **La skill è un file tuo.** Puoi aprirlo e correggerlo, o chiedere a Claude di farlo.
- **Il file di questa guida resta in `0-Inbox/`** finché non decidi tu cosa farne.

### Compito per casa

**Finisci la skill (se non l'hai finita in aula) e usala su un caso vero della settimana.** Non una prova: un lavoro che dovevi fare comunque. È la prova sul tuo lavoro che racconti **entro il 31/10**: cosa hai provato a costruire, cosa ha funzionato, cosa correggeresti. La racconti con un'email a Mihai entro sabato 31 ottobre alle 13:00.

---

## Se non hai finito in aula

Niente panico: la guida è fatta per ripartire. A casa:

1. Apri l'app e una **conversazione nuova** nella cartella del vault.
2. Scrivi:

> Riprendiamo la guida della skill: leggi il file "Crea una skill dalla tua attività.md" in 0-Inbox e riparti dal registro in fondo.

Claude legge il registro, ti dice a che punto sei, e riparte **dal primo passo non spuntato**, senza rifarti le domande a cui hai già risposto.

Scrivi per intero la frase, compreso il nome del file: se scrivi solo «riprendiamo la guida», Claude potrebbe avviare un'altra guida (quella del primo giorno, se è ancora nel vault).

Se hai perso il file, la repo della lezione contiene tutto il materiale: scaricalo di nuovo (vedi Guida a GitHub) e rimettilo in `0-Inbox/`. Il registro riparte da zero, ma la skill che hai già creato in `.claude/skills/` è ancora lì: dillo a Claude al Passo 1.

---

## Registro dei passi

Lo aggiorna Claude alla fine di ogni passo, la voce più recente in cima. Tu non devi fare niente.

Formato di ogni voce:

```
- AAAA-MM-GG - Passo N «nome» - cosa è stato fatto e ciò che serve per riprendere (attività, file di esempio, nome della skill, regole approvate)
```

**Passi**

- [ ] Passo 1 - Scegli l'attività
- [ ] Passo 2 - Dai a Claude un esempio vero
- [ ] Passo 3 - Falla una volta a mano, insieme a Claude
- [ ] Passo 4 - Correggi e approva
- [ ] Passo 5 - Trasformalo in una skill
- [ ] Passo 6 - Provala in una conversazione nuova, su un secondo caso

**Registro**

_(vuoto: le voci compariranno qui mentre procedi)_
