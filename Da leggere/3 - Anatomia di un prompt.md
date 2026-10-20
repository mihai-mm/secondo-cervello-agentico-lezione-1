# Anatomia di un prompt

Prima di salvare un prompt in una skill, conviene sapere cosa ci va dentro perché Claude lavori bene. Qui te lo spiego.

Prima però una correzione di prospettiva. Oggi il problema raramente è **come** formuli la richiesta: i modelli attuali capiscono bene anche frasi scritte male. Il collo di bottiglia è **il contesto che non gli dai**. Per questo chi lavora nel settore ha smesso di parlare di "prompt engineering" e parla di *context engineering*.

Il modello mentale più utile: **un collega brillante al primo giorno di lavoro**. È competente, ma non sa nulla di te, del cliente, di cosa hai già provato e di cosa per te è un buon risultato.

## Le 7 parti di un buon prompt

### 1. Obiettivo e motivazione

Non solo cosa vuoi, ma perché. "Scrivi una mail breve" funziona peggio di "scrivi una mail breve perché il destinatario la legge dal telefono tra una riunione e l'altra". Quando conosce il motivo, Claude prende decisioni sensate anche dove non gli hai dato istruzioni.

### 2. Contesto

Chi sei, per chi è il risultato, in che situazione verrà usato, cosa hai già scartato. Spesso è la parte che vale di più.

### 3. Materiale

Documenti, dati, bozze, screenshot. Se il materiale è lungo, mettilo **prima** e lascia la domanda in fondo. Se è complesso, separalo con etichette chiare: un titolo come `BOZZA ATTUALE:` o un tag come `<contratto>`.

### 4. Criteri di successo

Cosa rende buona la risposta: lunghezza, formato, livello tecnico, tono. Va detto in modo esplicito. "Massimo 200 parole, per un CEO non tecnico" è un criterio che si può controllare; "fammela bella" no.

### 5. Vincoli, detti in positivo

"Scrivi in paragrafi" funziona meglio di "non usare elenchi puntati". Il divieto richiama comunque proprio la cosa che vuoi evitare.

### 6. Esempi, quando conta lo stile

Un esempio vale più di tre aggettivi. Attenzione però: Claude tende a copiarlo troppo da vicino. Danne due o tre diversi tra loro, oppure specifica cosa deve imitare e cosa no.

### 7. Permesso di dissentire

"Se manca qualcosa chiedimelo", "se la premessa è sbagliata dimmelo". Senza questo permesso, Claude tende ad assecondare la richiesta così com'è.

## Cosa non serve più

- **"Sei un esperto di fama mondiale"**: dare un ruolo serve ancora, per fissare prospettiva e pubblico. Non serve più come trucco per ottenere qualità.
- **MAIUSCOLE, "IMPORTANTISSIMO", minacce e mance**: con i modelli recenti peggiorano il risultato. Seguono le istruzioni in modo più letterale e reagiscono troppo all'enfasi. Lo dice anche Anthropic nella sua documentazione.
- **"Ragiona passo passo"**: in gran parte superato, i modelli ragionano già da soli. Resta utile solo se vuoi vedere il ragionamento scritto nella risposta.
- **Mega-template da 2.000 parole copiati da LinkedIn**: rumore. Ogni istruzione che non c'entra annacqua quelle che contano.

## Il prompt è tutta la conversazione

In chat il prompt non è il primo messaggio: è l'intera conversazione. Non serve un primo messaggio perfetto. Serve un buon primo messaggio, seguito da correzioni precise: "troppo formale", "il punto 3 è sbagliato perché...".

Poi conviene distinguere due livelli:

- **Istruzioni stabili** (chi sei, il tuo stile, le tue preferenze): le scrivi una volta sola, così non le ripeti ogni volta. Nel tuo vault stanno in `CLAUDE.md` e in `STYLE.md`.
- **Istruzioni del singolo compito**: vanno nel messaggio.

E quando ti accorgi che stai riscrivendo sempre lo stesso prompt, è il momento di salvarlo una volta per tutte: è una skill.

## Il test finale

Prima di inviare, chiediti: **se mandassi questo messaggio a un professionista competente, saprebbe cosa fare senza chiamarmi?**

Se la risposta è no, al prompt manca contesto, non una formula magica.

## Cosa ti porti a casa oggi

- Il problema quasi mai è come lo chiedi: è il contesto che non dai.
- Le 7 parti: obiettivo e perché, contesto, materiale, criteri di successo, vincoli in positivo, esempi, permesso di dissentire.
- Niente trucchi da "esperto di fama mondiale" o MAIUSCOLE: peggiorano il risultato.
- Le istruzioni stabili si scrivono una volta (`CLAUDE.md`, `STYLE.md`); quelle del compito vanno nel messaggio.
- Un prompt che ripeti sempre uguale diventa una skill.

Il riferimento ufficiale più aggiornato è la guida di Anthropic: https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview
