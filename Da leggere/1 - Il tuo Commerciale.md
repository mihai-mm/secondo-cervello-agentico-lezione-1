# Il tuo Commerciale

Lezione 1, Parte A. Qui costruisci il primo collaboratore del tuo team AI: il commerciale, quello che dalla registrazione di una call tira fuori una proposta pronta da inviare, scritta come la scriveresti tu.

## Il problema che risolviamo

Fai una call commerciale andata bene: il cliente è interessato, c'è feeling, vi siete detti "ci sentiamo per una proposta".

Poi la proposta te la scrivi tu. La sera, quando sei già stanco. Ti rimetti davanti allo schermo e trasformi un'ora di chiacchiere in un documento scritto.

È un lavoro lento e sempre uguale. E ha un costo nascosto: più tardi arriva la proposta, più il cliente si è raffreddato. Il momento giusto per mandargliela era quando era ancora caldo.

Questo lavoro, da oggi, lo fa il tuo commerciale.

## Cosa ti serve: la trascrizione della call

Una cosa sola: il **testo** della call. Quello che vi siete detti, scritto.

Per averlo senza trascrivere a mano, usi uno strumento che sta in sottofondo durante la call (su Zoom, Meet o Teams), la registra e te la trascrive da solo:

- **Fathom**: quello che usiamo nel corso.
- **Granola**: alternativa equivalente.

Funzionano allo stesso modo: apri uno dei due, lo colleghi al tuo calendario, e da lì in poi ogni call diventa testo senza che tu faccia niente. A fine call trovi la trascrizione pronta.

## Il flusso, in pratica

1. Registri la call con Fathom (o Granola).
2. Metti la trascrizione in `0-Inbox/`, la casella in entrata del tuo vault (quella che conosci dalla Lezione 0).
3. Lanci la skill.
4. Da qui non scrivi più niente: la skill ti propone la cartella di quel cliente (nel modello che già conosci: `1-Projects/Nome cliente/`, con `CLAUDE.md`, `MEMORY.md` e la mappa), la crea dopo il tuo sì, ci mette dentro la trascrizione (in `calls/`) e ti scrive il recap. La proposta nasce subito dopo con la seconda skill, `/crea-proposta`, e la trovi in `reports/`.

Tu hai solo messo un testo nella cartella, dato un comando e detto di sì quando te lo chiede. Tutto il resto lo fa il sistema.

## Cos'è una skill

Fin qui hai usato l'AI con i **prompt**: scrivi una richiesta, l'AI risponde, e finisce lì. La volta dopo riscrivi tutto da capo.

Una **skill** (nel tuo pacchetto la chiamiamo anche **procedura**) è un'altra cosa. È un'istruzione che scrivi (o meglio, che fai scrivere a Claude) **una volta sola** e che resta lì, pronta, nel tuo vault: nella cartella `.claude/skills/`, la stessa dove c'è già `porta-i-tuoi-file`. La richiami con un comando (per esempio `/crea-proposta`) e Claude esegue quel lavoro sempre allo stesso modo, con lo stesso metodo.

Il modo più semplice per capire la differenza:

- Un **prompt** è chiedere un favore a qualcuno che passa di lì. Lo fa una volta, poi se ne va.
- Una **skill** è **assumere e formare un collaboratore**. Gli spieghi come si fa una cosa una volta, e da quel momento la sa fare da solo, ogni volta che glielo chiedi.

C'è un'analogia che rende l'idea. Immagina di dover pagare le tasse: preferisci un genio della matematica che non ha mai visto una dichiarazione dei redditi, o un commercialista esperto che ne ha fatte mille? Il genio è bravissimo, ma parte da zero ogni volta. Il commercialista sa già esattamente cosa fare. L'AI da sola è il genio. La skill è quello che la trasforma nel commercialista esperto del tuo lavoro.

Due cose importanti da tenere a mente:

- **La skill non la scrivi tu riga per riga.** La chiedi a Claude: gli spieghi a parole cosa vuoi che faccia, e te la costruisce lui. Il tuo lavoro è sapere *cosa* chiedergli.
- **Una skill nasce dal lavoro che fai già a mano.** Le skill migliori non si inventano a tavolino: si costruiscono prendendo un lavoro che fai sempre uguale e cristallizzandolo. Se il modo in cui lo fai a mano è chiaro, la skill sarà ottima. Se è confuso, anche la skill lo sarà.

Regola pratica: **se fai una cosa a mano due volte, la terza falla diventare una skill.**

## Cosa può fare una skill

Una skill non scrive solo testo. Può:

- **Leggere** file e documenti che le dai (una trascrizione, un PDF, un foglio di calcolo).
- **Scrivere col tuo tono**, sempre allo stesso modo.
- **Seguire un formato fisso** ogni volta (es. una proposta con sempre le stesse sezioni).
- **Estrarre informazioni** da un testo lungo (date, numeri, decisioni, prossimi passi).
- **Riassumere e sintetizzare** ore di materiale in poche righe.
- **Creare cartelle e organizzare i file** al posto tuo.
- **Ricordarsi cosa ha già fatto** e non rifarlo due volte.
- **Partire con un comando solo**: digiti `/nome-skill` e parte.

## Come nasce la tua prima skill

Il metodo è sempre lo stesso, e lo vedrai dal vivo:

1. **Fai il lavoro a mano una volta, bene.** Prendi una trascrizione e chiedi a Claude di elaborarla: un riassunto pulito di cosa serve al cliente.
2. **Correggi e approva.** Leggi il risultato e dì a Claude cosa togliere e cosa aggiungere. Quando ti torna, lo approvi. È il passaggio che fa la differenza: **prima approvi un esempio, poi deleghi gli altri.**
3. **Cristallizzalo.** Con l'esempio approvato in mano, dici a Claude: *"trasforma questo lavoro in una skill"*.
4. **Ora hai un comando.** Da lì in poi quel lavoro lo richiami con una parola, e viene sempre uguale a come l'hai approvato.

La prima skill che costruiamo così è **`/recap-discovery`**: prende la trascrizione di una call commerciale e ne tira fuori un recap ordinato di cosa vuole il cliente.

## La skill si migliora: da verbale a commerciale esperto

Il recap che ottieni all'inizio è ordinato e completo, ma è un **verbale**: ti dice cosa è stato detto nella call. Utile, però è solo metà del lavoro. La parte che chiude un cliente è un'altra: dove conviene fare leva con *questa* persona, a cosa devi stare attento, e le cose che il cliente non ha detto a voce ma che si capiscono tra le righe. Quella lettura la fa un commerciale con anni di esperienza, non chi si limita a trascrivere.

La cosa importante: per averla **non riscrivi la skill da capo**. Le insegni una cosa in più, parlandole. Esattamente come faresti con un collaboratore dopo le prime settimane: "il recap va bene, ma da adesso aggiungimi anche la tua lettura della trattativa".

Questo è un principio che vale per tutte le tue skill: **una skill non nasce perfetta, cresce con te.** La fai nascere minima, la usi sul lavoro vero, vedi cosa le manca, e gliela aggiungi a parole. Non c'è un momento in cui "finisci" una skill: la migliori quando ti accorgi che potrebbe fare di più.

Per far crescere `/recap-discovery`, dopo averla usata, le dai un messaggio come questo:

> Questo recap va bene, ma voglio che la skill faccia un passo in più. Oltre a riassumere cosa è stato detto, voglio che legga la call come la leggerebbe un commerciale esperto: dove conviene fare leva con questo cliente, a cosa devo fare attenzione, e le cose importanti che il cliente non ha detto ma che si capiscono tra le righe. Presentami la lettura tra le righe come ipotesi da verificare con il cliente, non come fatti.

Da quel momento, ogni volta che lanci `/recap-discovery` ottieni due cose invece di una:

1. **L'osso**: il recap ordinato di sempre: chi è il cliente, i suoi problemi, cosa vuole, cosa gli hai promesso, i prossimi passi. Sono **fatti**: sta scritto nella trascrizione.
2. **La lettura del commerciale**: dove fare leva, a cosa fare attenzione, cosa si legge tra le righe. Sono **ipotesi**: Claude le deduce, non le sa. Prima di costruirci sopra la proposta, le verifichi con il cliente.

È la stessa distinzione che il tuo pacchetto fa già (`_claude/livelli-di-prova.md`): ciò che è scritto in un documento è una **[fonte]**, ciò che hai verificato è **[osservato]**, ciò che è una deduzione è un'**[ipotesi]**. Una lettura tra le righe è un'ipotesi anche quando suona convincente: è un motivo in più per fare una domanda al cliente, non per dare la cosa per certa.

Il secondo punto è quello che ti fa arrivare alla proposta sapendo già dove premere, non più a naso.

## Dalla prima skill alla seconda

Con lo stesso metodo costruirai poi la seconda skill, **`/crea-proposta`**, che dal recap genera la proposta vera e propria. Questa seconda la costruiamo col **Plan Mode**: Claude ti mostra il piano prima di scrivere, così correggi prima e non dopo. Il Plan Mode è una delle modalità dell'app (le altre sono Manual, Accept edits, Auto e Bypass permissions): lo scegli dal selettore accanto al tasto di invio, oppure con Cmd+Shift+M. Vale solo per la conversazione in corso. I dettagli, e la differenza con quello che il tuo pacchetto fa già in Auto, sono in Anatomia di una skill.

## La proposta: le 6 sezioni, sempre le stesse

La proposta che mandi al cliente ha sempre la stessa struttura. Sei sezioni: una volta che le sai, ogni proposta è solo un riempimento.

1. **Il problema**: i suoi dolori concreti, ripresi uno per uno dal recap. Gli dimostri che hai ascoltato: parli dei suoi problemi, non dei tuoi servizi.
2. **La proposta**: la tua soluzione al suo problema: l'idea di fondo e come la realizzi. Ogni dolore di prima trova qui la sua risposta.
3. **Il perimetro**: cosa fai concretamente e, soprattutto, cosa **non** fai. È la sezione che ti salva dai malintesi: senza, il cliente dà per scontato che tu faccia anche cose mai previste.
4. **Deliverable**: cosa riceve concretamente, nero su bianco.
5. **Prezzo**: una cifra chiara, niente range. Più la scadenza dell'offerta.
6. **Termini**: tempi, modalità di pagamento, prossimo passo.

Due sezioni fanno la differenza tra una proposta che chiude e una che resta nel cassetto: il **perimetro** (ti protegge) e il **prezzo** (una cifra sola: il range "tra i 2 e i 4 mila" fa sembrare che tu non sappia quanto vale il tuo lavoro).

La proposta si salva nella cartella del cliente, in `reports/`.

## Scrivere col tuo tono: perché l'email AI si riconosce

Intorno alla proposta c'è tutto il resto: email, messaggi, presentazioni. Se chiedi a Claude "scrivimi l'email per Marco", esce un testo corretto ma generico, e il cliente capisce lontano un miglio che non l'hai scritto tu.

I segnali che tradiscono un'email scritta dall'AI:

- **Sempre lo stesso ordine**: richiamo alla call, "trovi in allegato", "rimango a disposizione", proposta di call, firma.
- **Frasi-fatte da manuale**: "prenderla in rassegna con calma", "rimango a disposizione per qualsiasi dubbio", "definire i prossimi passi". Suonano bene e non dicono niente.
- **Va bene per chiunque**: zero riferimento a cosa vi siete detti davvero. Se la mandi a cento clienti diversi funziona uguale, e quando un'email va bene per tutti non parla a nessuno.

Attenzione: se vedi dei buchi tipo `[Nome]` o `[recapiti]`, quelli non sono il difetto: sono solo dati che non hai dato all'AI. **Il difetto resta anche dopo averli riempiti: è il tono.** Generico, medio, da manuale. Perché l'AI non sa ancora come scrivi tu.

## Le due schede: chi sei e come scrivi

Nella Lezione 0 hai raccontato a Claude **chi sei**: il tuo lavoro, con chi lavori, come preferisci lavorare. Sta in `_claude/PROFILO.md`, accanto a `_claude/SOUL.md` (come lavora l'assistente). Il `CLAUDE.md` del vault li carica da solo a ogni conversazione, con due righe in cima: `@_claude/SOUL.md` e `@_claude/PROFILO.md`.

Quello che gli manca è una scheda in più: **come scrivi**, cioè la tua voce, le parole che usi e quelle che eviti, quanto vai dritto al punto. Questa scheda si chiama **STYLE.md** e sta nello stesso posto: `_claude/STYLE.md`.

Due schede dello stesso collaboratore: una sa chi sei, l'altra come suoni.

Per farla leggere sempre a Claude basta una riga nel `CLAUDE.md` del vault, sotto le altre due:

```
@_claude/STYLE.md
```

Da quel momento lo STYLE.md si carica da solo a ogni conversazione, come il profilo: ogni volta che gli chiedi di scrivere qualcosa, Claude ha già in testa il tuo modo di scrivere. Non devi dirgli di andarlo a leggere e non ci pensi più.

Per costruire il tuo STYLE.md passo dopo passo segui la guida Crea il tuo stile di scrittura: la trovi già in `0-Inbox/`, nella cartella che hai scaricato: la dai a Claude e lui ti guida. Scrive anche la riga nel `CLAUDE.md`, dopo il tuo sì.
