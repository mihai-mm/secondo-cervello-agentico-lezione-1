# Crea la tua skill recap-call

Questo è un file guidato: lo dai al tuo Claude e lui ti accompagna, un passo alla volta, a costruire la skill `/recap-call` (nel tuo pacchetto le skill si chiamano anche procedure): quella che dalla registrazione di una call con un cliente o un collaboratore tira fuori un recap ordinato, sempre con la stessa struttura.

È la stessa strada che hai visto in aula con `/recap-discovery`: il lavoro a mano una volta, lo correggi e lo approvi, poi lo trasformi in un comando.

Non devi sapere niente di tecnico. Devi solo avere una trascrizione di call da usare.

## Cosa otterrai

- La skill `/recap-call`: la richiami con un comando e ti trasforma qualsiasi trascrizione di call in un recap ordinato a sei parti.
- In più, dal recap ti tira fuori già pronta la lista dei compiti da fare (chi fa cosa).
- In più, un controllo: **questa call contraddice una decisione già presa?** Lo fa leggendo il `MEMORY.md` del cliente, senza scriverci niente.
- Il recap salvato nella cartella del cliente, in `calls/`, accanto alla trascrizione: entra nella memoria di quel cliente.

## Cosa ti serve prima di partire

- L'app di Claude per computer, con aperta la cartella del tuo vault (quella della Lezione 0).
- **La trascrizione di una call** con un cliente o un collaboratore: una tua vera, oppure quella di esempio che trovi nella lezione, «Trascrizione - Birrificio Tre Pini». Se hai messo la cartella scaricata in `0-Inbox/`, la trovi già lì dentro. Altrimenti mettila in `0-Inbox/`, oppure tienila pronta da incollare in chat.
- Se usi una tua trascrizione: un file di testo o un testo incollato. Un file Word (.docx) Claude non lo legge direttamente: copia il testo e incollalo in chat. Un PDF lungo più di 10 pagine chiede un programma in più sul Mac: meglio incollare il testo.

> Nota: `/recap-call` è per le call **operative** con clienti o collaboratori già acquisiti (cosa avete deciso, chi fa cosa). È diversa dalla `/recap-discovery`, che è per la call commerciale con un potenziale cliente e serve a fare la proposta.

## Come si usa

1. Questo file deve stare dentro il tuo vault, in `0-Inbox/`. Se hai messo lì l'intera cartella scaricata, è già a posto. **Claude lavora solo dentro il vault**: un file lasciato in Download non lo legge.
2. Apri nell'app una conversazione nuova nella cartella del vault (non in un'altra cartella: deve contenere il file `LEGGIMI.md` e le cartelle da `0-Inbox` a `4-Archives`).
3. Scrivi:

> leggi il file "Crea la tua skill recap-call.md" e seguilo

(usa il nome del file come lo vedi nella cartella)

Da lì in poi Claude ti guida lui. Quando vuoi fermarti, basta dire "ci fermiamo qui".

Un'avvertenza: non chiedere di «smistare l'inbox» finché non hai finito. Questo file deve restare dov'è, perché Claude ci scrive il registro dei passi.

## Piano B: la skill pronta

Nella cartella scaricata trovi anche `skill-pronte/recap-call/`: la skill già fatta. Serve come rete di sicurezza, se ti blocchi o se vuoi solo averla subito. **La strada consigliata resta costruirla con questa guida**: la skill che hai approvato tu, correzione dopo correzione, ti somiglia di più. Come si installa quella pronta è spiegato nel file `skill-pronte/LEGGIMI.md`.

## Se qualcosa non va

- **In aula**: scrivilo in chat o alza la mano. Se il problema è di molti, lo risolviamo davanti a tutti. Se è solo tuo, ti aiuto a parte o nel gruppo WhatsApp del corso: non serve fermare tutti.
- **A casa**: chiedi a Claude e mostragli lo screenshot, come nella Lezione 0.
- Le richieste che puoi vedere: l'app può chiederti il permesso di scrivere dentro `.claude/` (succede al Passo 4, te lo spiega prima), e il Mac può chiederti se «Claude» può accedere a Documenti, Scrivania o Download (va consentito).

---

## Dove sei

Claude aggiorna queste tre righe alla fine di ogni passo, e il registro in fondo al file.

- **Passo attuale**: 1 di 6
- **Ultima sessione**: -
- **Note**: -

---

## Stile di lavoro (regole per Claude)

Queste sono le regole che il tuo Claude deve seguire mentre ti guida. Se le viola, fermalo. Si aggiungono a quelle del `CLAUDE.md` del vault; se qualcosa è in conflitto, valgono quelle del vault, e Claude lo dice.

1. **Un passo alla volta.** Mai fare due passi senza la tua conferma. Una domanda alla volta.
2. **Annuncia prima di scrivere.** Prima di creare o modificare un file, ti dice quale file, dove e con cosa, e aspetta il tuo sì. Dopo, lo rilegge e ti dice come verificarlo.
3. **Niente gergo tecnico** dato per scontato: se usa un termine nuovo, lo spiega.
4. **Mostra prima, automatizza dopo**: prima ti fa vedere il recap a mano, poi lo trasformi in skill.
5. **Il `MEMORY.md` si legge, non si scrive.** In questa guida nessuna decisione viene registrata: la skill le legge soltanto. Fa eccezione solo la riga di prova del Passo 6 (facoltativo), scritta dopo il sì dell'utente.
6. **Una richiesta o una proposta non è una decisione.** Una decisione è quella che hai preso tu, scritta nel `MEMORY.md` con data e motivo.
7. **Niente letture fuori dal vault.** Se la trascrizione è altrove sul computer, chiede di incollarla o di metterla in `0-Inbox/`.
8. **Non inventare.** Se un'informazione non c'è nella trascrizione (una data, una scadenza, un nome), scrive "da definire" e non la ricostruisce.
9. **Intoppi.** Se qualcosa non torna, non tira a indovinare: chiede cosa vedi sullo schermo, di incollare il messaggio o di mandare uno screenshot. Poi risponde in parole semplici: cosa è successo, perché, l'unica cosa da fare adesso e la strada alternativa. Se un'azione viene bloccata, lo dice e propone un'altra strada: non insiste con lo stesso comando.
10. **Lascia il file al suo posto.** Non sposta né elimina questo file senza un sì esplicito.

## Come condurre

All'avvio:

1. Di' in quale cartella stai lavorando e controlla che sia il vault: contiene `LEGGIMI.md`, `CLAUDE.md` e le cartelle da `0-Inbox` a `4-Archives`. Se non è la cartella giusta, fermati e dillo.
2. Leggi il registro in fondo a questo file. Se ci sono passi già fatti, **riparti dal primo non spuntato**: non rifare domande a cui la persona ha già risposto (le risposte sono nel registro e nei file scritti). Se il registro è vuoto, comincia dal Passo 1.
3. Mostra il percorso in una riga per passo, poi annuncia il passo: cosa fate, perché serve, cosa ci sarà alla fine.

Dopo ogni passo: **annuncia** l'aggiornamento di questo file, spunta le caselle del passo con la data (`✅ AAAA-MM-GG`; un passo che non si applica si spunta con una nota «saltato: ...»), aggiorna le tre righe di «Dove sei» e aggiungi una riga in cima al registro, con ciò che serve per riprendere (cliente, data della call, nome del file della trascrizione, cosa è stato approvato). Poi chiedi: «continuiamo con il prossimo passo o ci fermiamo qui?».

Se la persona si ferma: dille che la prossima volta basta aprire una conversazione nuova nella cartella del vault e scrivere la frase della sezione «Se non hai finito».

---

## I sei passi

### Passo 1 - Fatti dare la trascrizione

- [ ] Chiedi di mettere in `0-Inbox/` la trascrizione di una call con un cliente o un collaboratore (una sua vera, o quella di esempio «Trascrizione - Birrificio Tre Pini») oppure di incollarla in chat. Se la cartella scaricata è già in `0-Inbox/`, la trascrizione di esempio è già lì: chiedi solo di indicarne il nome.
- [ ] Leggila per intero. Di' in due righe chi parla e di cosa.
- [ ] Chiedi **a quale cliente o progetto appartiene** (guarda in `1-Projects/` e in `Home.md` se esiste già).
- [ ] Chiedi **la data della call**, se non è scritta nella trascrizione. Non inventarla: la decide l'utente (per la trascrizione di esempio, che non ha una data, può indicare quella di oggi).
- [ ] Aspetta le risposte prima di proseguire.

**Output atteso**: due righe su chi parla e di cosa, il cliente e la data, scritti nel registro in fondo a questo file. Nessun altro file scritto.
**Verifica**: leggi le due righe. Chi parla e di cosa sono giusti? Il cliente e la data sono quelli che volevi?
**Se non funziona**: se Claude non trova la trascrizione, controlla che sia davvero in `0-Inbox/` oppure incollala in chat. Se è un Word (.docx), incolla il testo; se è un PDF lungo più di 10 pagine, incolla il testo.

### Passo 2 - Fai il recap a mano, una volta

- [ ] Se il progetto del cliente esiste, leggi il suo `CLAUDE.md` e il suo `MEMORY.md`.
- [ ] Produci in chat un recap ordinato in **sei parti**, senza che l'utente ti dia la struttura (gliela mostri tu):
  1. **Di cosa avete parlato**: il riassunto della call.
  2. **I temi, uno per uno**: i punti affrontati, le decisioni prese, le cose lette tra le righe. Le letture tra le righe sono **ipotesi da verificare** con il cliente: marcale come tali, non presentarle come fatti.
  3. **Chi fa cosa**: i compiti, divisi per persona, con la scadenza (se non c'è: "da definire").
  4. **Le domande aperte**: cosa è rimasto in sospeso.
  5. **I prossimi passi**: le tre cose che contano di più.
  6. **Il punto per te**: in due righe, ciò che conta davvero.
- [ ] Dal punto 3, estrai una **lista pulita dei compiti da fare**.
- [ ] Fai il **controllo sulle decisioni**: *questa call contraddice una decisione già presa?*
  - Confronta ciò che è stato detto nella call con le decisioni registrate nel `MEMORY.md` del cliente.
  - Se trovi una contraddizione, scrivila in evidenza: la decisione (con data e motivo), ciò che è stato detto nella call (chi, in quale punto) e il compromesso. **Non decidere tu**: la scelta resta all'utente.
  - Se non ne trovi, scrivi "nessuna contraddizione con le N decisioni registrate".
  - Se il progetto non esiste ancora o il `MEMORY.md` non ha decisioni, scrivi "nessuna decisione registrata da confrontare". Non inventare decisioni.
  - Una richiesta o una proposta emersa nella call non è una decisione: non va fra le decisioni, ma fra le domande aperte.
  - **Non scrivere nel `MEMORY.md`**: qui si legge soltanto.
- [ ] Mostra tutto e chiedi: *"Ti torna? Cosa togli, cosa aggiungi?"*. Aggiusta in base alla risposta, e ripeti finché non dice **«approvato»**. Questo è il modello da cui nascerà la skill: se il recap fatto a mano è buono, la skill sarà buona. Prima approvi un esempio, poi deleghi gli altri.

**Output atteso**: il recap in chat, nelle sei parti, con la lista dei compiti e il controllo sulle decisioni. Finora nessun file scritto, tranne il registro.
**Verifica**: confronta il recap con ciò che ricordi della call. Le letture tra le righe sono marcate come ipotesi? Le scadenze mancanti sono «da definire»? Scrivi «approvato» solo quando ti convince.
**Se non funziona**: se Claude inventa una data, un nome o una decisione che non era nella trascrizione, fermalo: «usa solo quello che c'è scritto, il resto è da definire». Se il recap è troppo lungo o confuso, chiedigli di riscriverlo più corto, sempre nelle sei parti.

### Passo 3 - Salvalo dove va

Adesso fai a mano, una volta, anche il salvataggio: è la stessa cosa che la skill farà ogni volta. **Annuncia ogni file prima di scriverlo** e aspetta il sì.

- [ ] **Se il progetto del cliente non esiste**, proponilo (nome della cartella in `1-Projects/`, di cosa si tratta) e crealo **solo dopo il sì**, con il modello del pacchetto: la cartella con `CLAUDE.md`, `MEMORY.md` e la mappa con lo stesso nome della cartella, più `calls/`. Aggiungi il progetto in `Home.md`. Niente dati inventati: quello che non sai resta "da definire". Se la trascrizione è quella di esempio, dillo: il cliente è inventato e la cartella potrà essere eliminata dall'utente quando ha finito.
- [ ] **La trascrizione** va in `calls/`, con il nome `AAAA-MM-GG - call.md` (per esempio `2026-10-08 - call.md`). Se è in `0-Inbox/`, la sposti solo dopo il sì.
- [ ] **Il recap** va in `calls/`, accanto, con il nome `AAAA-MM-GG - recap.md`. Inizia con il piccolo blocco che dice cos'è il file (`tipo: recap`, `aggiornato:` con la data di oggi). Se esiste già un recap con quel nome, chiedi prima di sostituirlo.
- [ ] **La mappa del progetto**: aggiungi i link ai due file nuovi.
- [ ] Rileggi ogni file che hai scritto e riassumi in tre righe cosa hai salvato e dove.

**Output atteso**: in `calls/` del cliente, la trascrizione e il recap; la mappa del progetto che li cita; se serviva, il progetto nuovo con la sua riga in `Home.md`.
**Verifica**: apri la cartella del cliente in `1-Projects/`: in `calls/` devono esserci i due file con la data nel nome, e la mappa deve avere i due link. Il `MEMORY.md` deve essere com'era.
**Se non funziona**: se un file esiste già con lo stesso nome, Claude deve chiederti prima di sostituirlo: se non lo fa, fermalo. Se i link nella mappa non si aprono, chiedi a Claude di controllare i nomi dei file.

### Passo 4 - Trasformalo in una skill

Quando il recap e il salvataggio ti convincono, il lavoro diventa un comando, così non devi rifarlo ogni volta. **Prima di scrivere, Claude ti spiega due cose.**

- [ ] La prima: la skill nascerà in una cartella nuova del vault, `.claude/skills/recap-call/`, con dentro un file `SKILL.md` (accanto a `porta-i-tuoi-file`). La seconda: scrivendo lì, **l'app mostrerà una richiesta di permesso**, perché `.claude/` è una cartella speciale. È normale: va consentita. Se non compare, bene lo stesso.
- [ ] Claude propone il contenuto in breve e aspetta il sì.
- [ ] Poi crea la skill, **essenziale** (ogni parte serve, mai oltre le 500 righe), a partire dal recap approvato. Nome: `recap-call`. Nell'intestazione, una descrizione che dice quando usarla (per esempio: «Trasforma la trascrizione di una call con un cliente già acquisito o un collaboratore in un recap a sei parti, con la lista dei compiti e il controllo delle decisioni già prese. Usala quando l'utente chiede il recap di una call o scrive /recap-call.»). Il corpo deve dire alla skill di:
  - chiedere o riconoscere la trascrizione e il cliente (guardando in `1-Projects/` e in `Home.md`);
  - se il progetto del cliente non esiste, **proporlo e crearlo solo dopo il sì**, con il modello del pacchetto (`CLAUDE.md`, `MEMORY.md`, mappa, `calls/`), e aggiungerlo in `Home.md`;
  - leggere il `MEMORY.md` del cliente, **senza mai scriverci**;
  - produrre il recap nelle sei parti (Di cosa avete parlato · I temi · Chi fa cosa · Domande aperte · Prossimi passi · Il punto per te), con le letture tra le righe marcate come ipotesi;
  - estrarre la lista dei compiti (chi, cosa, scadenza o "da definire");
  - fare il controllo "questa call contraddice una decisione già presa?", con le stesse regole del Passo 2: porta la decisione con data e motivo, ciò che è stato detto, e lascia la scelta all'utente; se non c'è niente da confrontare, lo dice;
  - salvare in `calls/` del cliente, accanto alla trascrizione, `AAAA-MM-GG - recap.md`, **annunciando prima il file** e aggiungendolo alla mappa; se esiste già, chiedere prima di sostituirlo;
  - non inviare niente a nessuno: il recap lo manda l'utente, se vuole;
  - non inventare: ciò che non c'è nella trascrizione è "da definire".
- [ ] Claude ti spiega che non la state scrivendo riga per riga: la fate costruire a lui descrivendo il risultato voluto. Dopo averla scritta, **rilegge il file** e te lo fa vedere.

**Output atteso**: il file `.claude/skills/recap-call/SKILL.md`, corto, che riassume il lavoro approvato.
**Verifica**: scrivi `/` nella chat: nel menu deve comparire `/recap-call`. Se non compare, scrivi `/reload-skills`. Per vedere il file: `.claude` non compare in Obsidian (nasconde le cartelle che iniziano con un punto, è normale); nel Finder premi Cmd+Maiusc+punto per mostrare i file nascosti, oppure chiedi a Claude di mostrarti il contenuto in chat.
**Se non funziona**: se la richiesta di permesso viene rifiutata, la skill non viene scritta: Claude lo dice e ti chiede di riprovare consentendola. Se non riesci a farla nascere, **piano B**: usa la skill pronta in `skill-pronte/recap-call/` (le istruzioni sono in `skill-pronte/LEGGIMI.md`), poi prosegui con il Passo 5. Il comando funziona allo stesso modo.

### Passo 5 - La prova che si ripete

- [ ] Apri una **conversazione nuova** nella cartella del vault (la guida resta dov'è, non serve).
- [ ] Scrivi `/recap-call` indicando una **seconda** trascrizione (o la stessa di esempio). Invece di rifare il lavoro a mano, la skill lo fa da sola.
- [ ] Se c'è da ritoccare, dillo a Claude nella stessa conversazione: l'utente dice cosa cambiare ("correggi la skill recap-call: ..."), Claude propone la modifica e la scrive dopo il sì. Poi riprova.
- [ ] Quando ti torna, torna alla conversazione della guida e scrivi «provata» (se l'hai chiusa, apri una conversazione nuova e usa la frase della sezione «Se non hai finito»): Claude spunta il passo.

**Output atteso**: un recap prodotto dalla skill da sola, salvato in `calls/` del cliente.
**Verifica**: controlla che:
- [ ] il recap ha le sei parti, la lista dei compiti e la riga del controllo sulle decisioni;
- [ ] il recap è in `calls/` del cliente, accanto alla trascrizione, e la mappa del progetto lo cita;
- [ ] il `MEMORY.md` è come prima: la skill non ci ha scritto niente;
- [ ] l'ha chiesto prima di scrivere, e non ha mandato niente a nessuno.

**Se non funziona**: se il comando non parte, controlla di essere nella cartella del vault e riprova con `/reload-skills`. Se il risultato è generico o manca qualcosa, la skill è troppo vaga: chiedi a Claude di correggerla come sopra. Se non riesci a sistemarla, usa la skill pronta (piano B, vedi Passo 4).

### Passo 6 (facoltativo) - Provare il controllo sulle decisioni

Con il Birrificio Tre Pini il controllo non ha niente da confrontare: è un cliente appena nato e il suo `MEMORY.md` non ha decisioni. Per vederlo in azione ci sono due strade.

- [ ] **Sul tuo progetto della Lezione 0**: se il suo `MEMORY.md` ha già delle decisioni, usa `/recap-call` con una tua trascrizione recente e guarda se segnala qualcosa.
- [ ] **Con una prova guidata sul Tre Pini**: l'utente dice di registrare nel `MEMORY.md` del Birrificio Tre Pini, **come decisione di prova**, che si parte dal sito e dalle schede prodotto e gli ordini dei locali vengono dopo. Claude annuncia la riga, aspetta il sì e la scrive marcandola "(di prova)". Poi si lancia `/recap-call` sulla stessa trascrizione: la skill deve segnalare che la call, dove si decide di partire dagli ordini, contraddice quella decisione. Alla fine l'utente elimina la riga di prova dal `MEMORY.md` (a mano o chiedendolo a Claude).

**Output atteso**: il recap con, in evidenza, la contraddizione con la decisione registrata (data e motivo, ciò che è stato detto, il compromesso), senza una scelta fatta al posto tuo.
**Verifica**: la riga «(di prova)» è stata tolta dal `MEMORY.md` alla fine, e il resto del file è com'era.
**Se non funziona**: se la skill non segnala niente, controlla che la riga di prova sia davvero nel `MEMORY.md` del Tre Pini e rilancia. Se la segnala ma decide al posto tuo, correggi la skill: la scelta è dell'utente.

---

## Chiusura

Claude riepiloga: ora hai la skill `/recap-call`, la richiami quando vuoi, e ti dà sempre il recap a sei parti, la lista dei compiti e il controllo sulle decisioni già prese. Il recap sta nella cartella del cliente, così entra nella sua memoria storica: la volta dopo puoi chiedere «cosa avevamo concordato?» e Claude risponde dai file (vedi Il tuo Account Manager).

Questo file resta dov'è finché non decidi tu cosa farne.

### Note

- Se la skill non ti convince, la sistemi parlando: dici a Claude cosa cambiare e lui la corregge. Non si riscrive il codice a mano.
- Più la userai, più la affinerai. È normale che la prima versione non sia perfetta.
- Registrare le decisioni nel `MEMORY.md` è un altro lavoro: lo affrontiamo la prossima volta. Per ora la skill le legge e ti avvisa.

---

## Se non hai finito

Niente panico: la guida è fatta per ripartire. Apri l'app e una **conversazione nuova** nella cartella del vault, poi scrivi:

> Riprendiamo la guida della skill recap-call: leggi il file "Crea la tua skill recap-call.md" e riparti dal registro in fondo.

Claude legge il registro, ti dice a che punto sei, e riparte **dal primo passo non spuntato**, senza rifarti le domande a cui hai già risposto. Scrivi per intero la frase, compreso il nome del file: se scrivi solo «riprendiamo la guida», Claude potrebbe avviare un'altra guida.

Se hai perso il file, la repo della lezione contiene tutto il materiale: scaricalo di nuovo (vedi Guida a GitHub). Il registro riparte da zero, ma i file che hai già salvato nel vault restano lì: dillo a Claude al Passo 1.

---

## Registro dei passi

Lo aggiorna Claude alla fine di ogni passo, la voce più recente in cima. Tu non devi fare niente.

Formato di ogni voce:

```
- AAAA-MM-GG - Passo N «nome» - cosa è stato fatto e ciò che serve per riprendere (cliente, data della call, file della trascrizione, cosa hai approvato)
```

**Passi**

- [ ] Passo 1 - Fatti dare la trascrizione
- [ ] Passo 2 - Fai il recap a mano, una volta
- [ ] Passo 3 - Salvalo dove va
- [ ] Passo 4 - Trasformalo in una skill
- [ ] Passo 5 - La prova che si ripete
- [ ] Passo 6 (facoltativo) - Provare il controllo sulle decisioni

**Registro**

_(vuoto: le voci compariranno qui mentre procedi)_
