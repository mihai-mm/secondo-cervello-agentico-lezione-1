# Il tuo Account Manager

Lezione 1, Parte B. Qui costruisci il secondo collaboratore: l'account manager, quello che si ricorda di ogni cliente: cosa vi siete detti, cosa avete deciso, a che punto siete. Non più "dove eravamo rimasti?".

## Il problema che risolviamo

Fai una call con un cliente o un collaboratore. Vi dite cose, prendete decisioni, vi date dei compiti. Poi la settimana dopo: cosa avevamo deciso sul prezzo? Chi doveva mandare quel documento?

E quando riprendi un cliente dopo settimane, parti da zero: rileggi le email, cerchi gli appunti, ricostruisci tutto a memoria. Ogni volta.

Il tuo account manager risolve questo: ogni cliente diventa una **cartella che ricorda tutto**.

## L'archivio cliente

L'idea è semplice: **una cartella per ogni cliente**. Lì dentro vive tutto quello che riguarda quel cliente: le call, le decisioni, i documenti.

Quando lavori su quel cliente, apri quella cartella e Claude ha sotto mano tutta la sua storia. Non gli devi rispiegare niente.

La cartella del cliente ha la stessa forma del progetto che hai creato nella Lezione 0 (tappa 3 del pacchetto). Il tuo progetto è un lavoro vero; qui, per vedere come funziona, usiamo come esempio Serramenti Furlan:

```
1-Projects/Serramenti Furlan/
├── CLAUDE.md             →  le regole di questo cliente
├── MEMORY.md             →  le decisioni (con data e motivo), gli insight, i numeri
├── Serramenti Furlan.md  →  la mappa: l'indice di tutti i file
├── calls/                →  le trascrizioni, con accanto i recap (/recap-call salva qui)
├── reports/              →  ciò che produci per il cliente: la proposta
├── materials/            →  i documenti che ricevi dal cliente
└── attivita/             →  il diario del progetto
```

I tre file in alto ci sono sempre. Le cartelle `calls/`, `reports/`, `materials/` e `attivita/` nascono quando servono: non vanno create in anticipo.

L'ultima, `attivita/`, è il diario che usi già dal pacchetto: lo approfondiamo la prossima volta.

## Interroga il tuo archivio

Una cartella che ricorda tutto serve se le fai delle domande. Apri una conversazione nuova nel tuo vault e chiedi, per esempio:

> Cosa avevamo concordato con Serramenti Furlan? Cosa preparo per il prossimo incontro?

Claude legge il `CLAUDE.md` e il `MEMORY.md` del cliente, la trascrizione della call, il recap e la proposta, e risponde dicendoti **da quale file** ha preso ogni informazione. Non scrive niente: legge e risponde.

Tre cose da sapere:

- Se due file dicono cose diverse, te lo dice, con le date.
- Se un'informazione non c'è, ti dice che non c'è: non la inventa.
- Distingue una **richiesta** del cliente da una **decisione** che hai preso tu. Quello che chiede un cliente resta una richiesta finché non decidi.

La stessa domanda funziona sul tuo progetto della Lezione 0: cambia solo il nome.

## Le memorie del tuo collaboratore

Il tuo collaboratore ha due livelli di memoria: quello che vale **sempre** e quello che vale **per un cliente solo**.

**Il livello del vault** (vale ovunque, con qualsiasi cliente). È il `CLAUDE.md` del vault, che a ogni conversazione carica:

- **`_claude/PROFILO.md`**: **chi sei**: il tuo lavoro, con chi lavori. (Fatto nella Lezione 0.)
- **`_claude/SOUL.md`**: **come lavora l'assistente**: franco, concreto, che non decide al posto tuo. (Già scritto nel pacchetto.)
- **`_claude/STYLE.md`**: **come scrivi**: la tua voce. (Lo costruisci con la guida Crea il tuo stile di scrittura.)

**Il livello del cliente** (vale solo per quel cliente, dentro la sua cartella):

- **`CLAUDE.md` del cliente**: **le regole di questo cliente**: cosa fa, come va trattato, le sue particolarità. Si accende quando lavori nella sua cartella.
- **`MEMORY.md`**: **cosa avete deciso**: la memoria storica del cliente. Qui c'è la differenza tra "ricordare le call" e "ricordare le decisioni". Tre sezioni che non invecchiano:
  - **Decisioni** (con data e perché): cosa avete scelto e per quale motivo.
  - **Insight**: cosa hai capito di questo cliente nel tempo.
  - **Numeri**: budget, prezzi, dati concordati.

Una cosa importante da capire: i due livelli **si sommano**. Quando lavori su un cliente, Claude ha in testa tutto insieme: chi sei, come lavora, come scrivi, le regole di quel cliente e le sue decisioni. Non scegli quale usare, le ha tutte.

## La skill `/recap-call`

È la gemella della `/recap-discovery` che hai costruito nella Parte A, ma per uno scopo diverso:

- `/recap-discovery` = call **commerciale con un potenziale cliente**: serve a fare la **proposta**.
- `/recap-call` = call **operativa con un cliente o un collaboratore già acquisito**: serve a sintetizzare cosa vi siete detti.

Prende la trascrizione della call e ne tira fuori un recap ordinato, sempre con la stessa struttura. **Sei parti:**

1. **Di cosa avete parlato**: il riassunto della call in un colpo d'occhio.
2. **I temi, uno per uno**: i punti affrontati, le decisioni prese e le cose lette tra le righe (queste ultime sono ipotesi: da verificare con il cliente, non fatti).
3. **Chi fa cosa**: i compiti, divisi per persona, con la scadenza. È il cuore: è quello che dopo una call ti dimentichi sempre.
4. **Le domande aperte**: cosa è rimasto in sospeso, da chiarire.
5. **I prossimi passi**: le tre cose che contano di più.
6. **Il punto per te**: in due righe, ciò che conta davvero di quella call.

E due passi in più. Dai compiti del punto 3 ti tira fuori la **lista delle cose da fare**, già organizzata. E fa un **controllo sulle decisioni**: *questa call contraddice una decisione già presa?* Legge il `MEMORY.md` del cliente e confronta.

Un esempio. A giugno Marco, di Serramenti Furlan, e Luca hanno deciso di partire da tre cose: preventivi, email e storia dei clienti; il sito è "una cosa per dopo". A settembre, nella call di avvio, Marco dice: "già che ci siamo, rifacciamo anche il sito?". Tutti annuiscono. Nel recap, in evidenza, compare una riga:

> Attenzione: questo contraddice quello che avevate deciso il 10 giugno (si parte da preventivi, email e storia dei clienti; il sito dopo).

Claude ti porta la decisione, con la data, e ti dice cosa è stato detto nella call. **Non decide lui**: la scelta resta a te. Magari avete davvero cambiato idea; l'importante è che sia una scelta, non una dimenticanza.

Il controllo **legge** il `MEMORY.md` e non ci scrive. Se nel cliente non ci sono ancora decisioni registrate, te lo dice: non ha niente da confrontare.

Il recap si salva dentro la cartella del cliente, in `calls/`, accanto alla trascrizione: così non è un'email che si perde, ma entra nella memoria di quel cliente. Se il cliente non ha ancora una cartella, la skill te la propone e la crea solo dopo il tuo sì.

## Come la costruisci

In aula vedi il concetto e lo schema; la skill la costruisci tu. Il metodo l'hai già visto con `/recap-discovery`: il recap a mano una volta, lo correggi e lo approvi, poi dici "trasformalo in una skill". Per essere condotto passo dopo passo hai una guida: Crea la tua skill recap-call. La trovi già in `0-Inbox/`, nella cartella che hai scaricato: la dai a Claude e lui ti accompagna.

Nell'esercitazione finale fai la stessa cosa con una skill tua, partendo da un'attività che ripeti spesso: la guida è Crea una skill dalla tua attività.

## Cosa ti porti a casa oggi

- Ogni cliente è una cartella che ricorda tutto: call, decisioni, documenti. E la interroghi: ti risponde dicendo da quale file prende ogni cosa.
- Il collaboratore ha due livelli di memoria: quello del vault (chi sei, come lavora, come scrivi: sempre) e quello del cliente (le sue regole, le sue decisioni: solo nella sua cartella). Si sommano.
- `MEMORY.md` non è il diario delle call: è il registro delle **decisioni, insight e numeri** del cliente.
- `/recap-call` trasforma una call con un cliente in un recap ordinato a 6 parti, ti lascia già pronta la lista dei compiti e ti avvisa se la call contraddice una decisione già presa.
