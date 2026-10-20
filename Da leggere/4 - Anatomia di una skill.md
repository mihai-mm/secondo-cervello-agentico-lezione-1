# Anatomia di una skill

Una skill non è una formula magica: è fatta di pochi pezzi, e ogni pezzo ha un mestiere. Qui te li spiego.

Una cosa da tenere a mente per tutto: **una skill, in pratica, è una cartella con dentro un file di testo** (si chiama `SKILL.md`). Niente di esoterico. Un foglio di istruzioni, scritto bene.

Nel tuo pacchetto le skill si chiamano anche **procedure**: è la stessa cosa. `porta-i-tuoi-file`, quella che hai già, è una skill. Ogni skill sta nel tuo vault, in `.claude/skills/nome-della-skill/SKILL.md`, accanto a `porta-i-tuoi-file`. Le skill si richiamano con `/nome`: il menu che si apre scrivendo `/` le elenca.

## I pezzi di una skill

### Il nome / comando

Come richiami la skill. Una parola che inizia con `/`: per esempio `/recap-discovery` o `/crea-proposta`. È anche il nome della cartella.

La digiti nella chat e la skill parte.

### Il corpo: le istruzioni

È il cuore: cosa deve fare la skill e come deve comportarsi. Il "manuale" che il tuo collaboratore legge per fare il lavoro.

Una regola d'oro: **tienilo corto**. Più istruzioni ammucchi, peggio lavora. Un manuale snello e chiaro batte sempre un papiro di mille righe. C'è anche un numero: la guida ufficiale di Claude Code consiglia di stare **sotto le 500 righe** e di mettere il dettaglio in file separati, nella stessa cartella. Quante righe servono dipende dal lavoro: conta che ognuna abbia un motivo per esserci.

### Distillata dal lavoro che fai già a mano

Non è una parte del file, è il principio che decide se la tua skill sarà buona o scadente.

Le skill migliori non si inventano a tavolino: nascono prendendo un lavoro che fai sempre uguale, a mano, e cristallizzandolo. Se il modo in cui lo fai a mano è chiaro, la skill sarà ottima. Se è confuso, lo sarà anche lei.

Regola pratica: se fai una cosa a mano due volte, la terza falla diventare una skill.

## Come te ne crei una, in pratica

Non c'è un solo modo. Ne hai tre, e portano tutti allo stesso punto: un comando `/nome` che riusi all'infinito. Una cosa è comune a tutti e tre: **non la scrivi tu riga per riga: la chiedi a Claude**.

Una volta scritta, la skill è **subito disponibile**, senza riavviare niente: la richiami con `/nome` anche in una conversazione nuova.

### 1. La distilli dal lavoro che fai a mano

Fai il lavoro come lo faresti comunque, a mano, dentro la chat. Leggi il risultato, dici a Claude cosa togliere e cosa aggiungere, e quando ti torna lo approvi. Solo allora dici: "fanne una skill". Lui prende il processo che hai appena fatto, già approvato da te, e lo cristallizza in un comando.

È il modo più naturale: la skill nasce da qualcosa che hai già visto funzionare. **Prima approvi un esempio, poi deleghi gli altri.** È quello che hai visto oggi con `/recap-discovery`.

### 2. La costruisci col Plan Mode

Descrivi a Claude cosa vuoi ottenere. Prima di scrivere qualsiasi cosa, lui ti mostra **il piano**: come ha intenzione di costruirla. Tu lo leggi, lo approvi (o lo correggi), e solo dopo Claude la scrive.

Utile quando la skill è più articolata e vuoi controllare la direzione prima che parta. È il modo che useremo per `/crea-proposta`.

Il Plan Mode è una delle **modalità** dell'app: Manual, Accept edits, Plan, Auto, Bypass permissions. Si sceglie dal selettore accanto al tasto di invio, oppure con Cmd+Shift+M, e vale solo per la conversazione in corso: in quelle nuove non resta attivo.

Attenzione a non confonderlo con un'altra cosa che già succede. Il tuo pacchetto lavora in modalità **Auto**, e il suo `CLAUDE.md` chiede a Claude di annunciare cosa sta per scrivere e di aspettare il tuo sì: lo fa per ogni file, uno alla volta. Il Plan Mode è diverso: approvi **come lo farà**, per intero, prima che cominci a lavorare. Prima il piano, poi il lavoro; non il permesso, file per file.

### 3. La prendi già pronta

Molte skill utili le ha già scritte qualcun altro. Le trovi nella community di **AlchemIA su Skool** o su GitHub, e le metti nel tuo vault, in `.claude/skills/`: sono subito tue. Zero lavoro di scrittura.

Una skill è un file di istruzioni: prima di usare quella di qualcun altro, aprila e leggila, o chiedi a Claude di spiegarti cosa fa.

È così che è stata presa la skill che genera i diagrammi delle slide della lezione. https://github.com/coleam00/excalidraw-diagram-skill

Esiste anche una skill che crea le skill: si installa come **plugin**, un componente aggiuntivo di Claude Code. Non serve per cominciare; sapere che c'è basta.

### Due regole che valgono per tutte e tre

**Se non ti convince, la sistemi parlando.** Non è scolpita nella pietra: provi, dici a Claude cosa cambiare, lui la corregge, riprovi. Finché non ti piace. La aggiusti a parole, non riscrivendo codice.

**Quando NON farne una.** Per cose che fai una volta sola, o che cambiano ogni volta. La skill ha senso solo quando il lavoro si ripete uguale.

## Il principio che vale per tutto

Quando chiedi a Claude di costruire una skill (perché **non la scrivi tu riga per riga**: gliela fai scrivere), vale una sola regola:

**Descrivi il risultato che vuoi, non i passi tecnici per arrivarci.**

Il tuo lavoro è sapere *cosa* vuoi ottenere. Il *come* è il suo mestiere.

## Cosa ti porti a casa oggi

- Una skill (o procedura) è una cartella con un file di istruzioni, nel tuo vault, in `.claude/skills/`.
- Ti bastano: nome/comando, corpo corto e chiaro (sotto le 500 righe), e il principio "distillala dal lavoro che fai già a mano".
- La skill nuova funziona subito, senza riavviare.
- La regola d'oro per chiederla a Claude: descrivi il risultato, non i passi.
- Prima approvi un esempio, poi deleghi gli altri.
