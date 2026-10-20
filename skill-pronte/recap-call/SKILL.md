---
name: recap-call
description: >
  Trasforma la trascrizione di una call con un cliente già acquisito o un collaboratore in un recap
  a sei parti, con la lista dei compiti e il controllo delle decisioni già prese. Usala quando
  l'utente chiede il recap di una call o scrive /recap-call. Non è per la call commerciale con un
  potenziale cliente.
---

# Recap di una call

Dalla trascrizione di una call operativa (cosa avete deciso, chi fa cosa) un recap sempre con la stessa struttura, salvato nella cartella del cliente. **Un passo alla volta**: annuncia ogni file prima di scriverlo e aspetta il sì.

## Regole fisse

- **Il `MEMORY.md` si legge, non si scrive.** Mai.
- **Non inventare.** Data, scadenza, nome o orario che non sono nella trascrizione: «da definire». Una deduzione si scrive come tale («*Deduzione:* …»).
- **Una richiesta o una proposta non è una decisione.** Decisione è solo ciò che è registrato nel `MEMORY.md`, con data e motivo.
- **Niente invii.** Il recap lo manda l'utente, se vuole.
- **Niente letture fuori dal vault.** Se la trascrizione è altrove, chiedi di incollarla o di metterla in `0-Inbox/`.

## Passi

1. **Trascrizione.** Prendi quella indicata, cercala in `0-Inbox/` o chiedi di incollarla. Leggila per intero e di' in due righe chi parla e di cosa.
2. **Cliente e data.** Riconosci il cliente guardando in `1-Projects/` e in `Home.md`; se hai dubbi, chiedi. Se la data della call non è scritta, chiedila: puoi suggerire un indizio dal testo, ma decide l'utente.
3. **Progetto.** Se il cliente non ha un progetto, proponilo (nome della cartella, di cosa si tratta) e crealo **solo dopo il sì**, con il modello del vault: `CLAUDE.md`, `MEMORY.md` (sezioni Decisioni, Insight, Numeri vuote), la mappa con lo stesso nome della cartella, `calls/`; aggiungi una riga in `Home.md`. Ciò che non sai resta «da definire».
4. **Leggi** il `CLAUDE.md` e il `MEMORY.md` del progetto.
5. **Recap in chat**, in sei parti:
   1. **Di cosa avete parlato**: il riassunto della call.
   2. **I temi, uno per uno**: punti affrontati, numeri, decisioni prese in call (con il minuto). In fondo le **letture tra le righe**, ognuna marcata «*Ipotesi:*», da verificare con il cliente.
   3. **Chi fa cosa**: tabella Chi · Cosa · Scadenza («da definire» se manca).
   4. **Le domande aperte**: ciò che è rimasto in sospeso, comprese richieste e proposte non decise.
   5. **I prossimi passi**: le tre cose che contano di più.
   6. **Il punto per te**: due righe su ciò che conta davvero.

   Poi la **Lista dei compiti** (caselle `- [ ]`, «**Chi:** cosa (scadenza)») e il **Controllo sulle decisioni**:
   - confronta la call con le decisioni del `MEMORY.md`;
   - se c'è una contraddizione, mettila in evidenza: la decisione (data e motivo), cosa è stato detto (chi, a che minuto), il compromesso. **Non decidere**: la scelta è dell'utente;
   - se non ce ne sono: «nessuna contraddizione con le N decisioni registrate»;
   - se il progetto è nuovo o il `MEMORY.md` non ha decisioni: «nessuna decisione registrata da confrontare».

   Chiedi: «Ti torna? Cosa togli, cosa aggiungi?». Correggi finché l'utente non dice «approvato».
6. **Salva**, annunciando prima i file:
   - la trascrizione in `calls/AAAA-MM-GG - call.md` (se è in `0-Inbox/`, spostala senza modificarla; se è incollata in chat, salvala così com'è);
   - il recap in `calls/AAAA-MM-GG - recap.md`, che inizia con:
     ```
     ---
     tipo: recap
     aggiornato: AAAA-MM-GG
     ---
     ```
     e con il link alla trascrizione. Se il file esiste già, chiedi prima di sostituirlo;
   - nella mappa del progetto, sotto «Chiamate», i link ai file nuovi, e aggiorna la sua data.
7. **Rileggi** ciò che hai scritto e riassumi in tre righe cosa hai salvato e dove, con il modo per verificarlo.
