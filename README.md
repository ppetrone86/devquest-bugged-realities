# DevQuest: Bugged Realities

### Il gioco di carte multiplayer dove i Dev non combattono draghi, ma clienti, bug e deadline folli.

---

## Introduzione

Benvenuti in **DevQuest: Bugged Realities**, il gioco dove ogni developer ha un obiettivo semplice e crudele: **completare task senza impazzire**, superando bug, PM incomprensibili, colleghi sabotatori, e soluzioni rubate da StackOverflow.

Ogni giocatore ha uno **Sprint personale**, con una **board stile Jira/Trello** divisa in:
- `To Do`: task da iniziare
- `Doing`: task in corso
- `Done`: task completati

Il gioco è un mix di **gestione tempo**, **sabotaggio tra dev**, e **black humor IT**.

---

## Setup

- **2–6 giocatori**
- Durata: **15–30 minuti**
- Ogni giocatore riceve:
  - 1 carta **Ruolo Dev**
  - 3 carte **Task**
  - 3 carte **Azione/Eventi**
  - Karma iniziale: **10**
  - Bug iniziali: **0**

---

## Obiettivo

Completare il maggior numero possibile di **task** nel proprio **Sprint personale**, mantenendo il Karma alto e il numero di bug basso.

Alla fine dello sprint vince chi ha:
- Più **punti task completati**
- Meno **bug accumulati**
- Karma sopra lo zero

---

## Struttura del turno

Ogni giocatore al suo turno:

1. **Pesca** una carta dal mazzo Azioni/Eventi  
2. **Gioca** (facoltativamente) una carta Azione o Evento  
3. **Lavoro**:
   - Se ha un task in `Doing`, riduce la sua durata residua di **1 turno**
   - Se la durata raggiunge **0**, sposta il task in `Done` e ottiene i punti

Può iniziare un nuovo task spostandolo da `To Do` a `Doing` (max 1 attivo alla volta)

---

## Tipologie di Carte

### TASK

| Attributo     | Descrizione |
|---------------|-------------|
| Nome          | Tipo di attività |
| Durata        | Turni necessari (1–5) |
| Valore        | Punti assegnati al completamento |
| Categoria     | Dev, DevOps, UI, Bugfix, ecc. |

### AZIONE

Carte che **aiutano sé stessi**:
- Accelerano task
- Curano bug
- Aumentano karma
- Permettono scambi con altri dev

### EVENTO

Carte che **sabotano gli altri**:
- Aggiungono bug (con severità)
- Costringono a scartare o rimescolare task
- Accorciano deadline
- Fanno perdere karma

---

## Bug e severità

I **bug** sono penalità permanenti fino alla fine dello sprint.

### Severità bug:

| Severità | Effetto |
|----------|---------|
| 🐞 Minor  | +1 turno al task in corso |
| 🐛 Major  | +2 turni al task |
| 💣 Critical | Task azzerato o annullato |

Bug si ricevono tramite carte Evento o per fallimenti epici (es. deploy senza test).

---

## Ruoli Dev (Archetipi)

Ogni player ha un **Ruolo Dev** unico con bonus e malus.

| Nome               | Abilità                                | Malus                                 |
|--------------------|-----------------------------------------|----------------------------------------|
| **Frontend Alchemist** | I task UI durano 1 turno in meno        | +1 bug se compila con warning          |
| **Backend Sorcerer**   | Ignora il primo bug ricevuto             | I task di refactor durano +1 turno     |
| **Junior Prometteur**  | Può completare un task semplice istantaneamente 1 volta | -1 karma se usa StackOverflow          |
| **DevOps Ninja**       | Può evitare 1 evento contro di sé a partita | Se gioca 2 eventi di fila, crasha e perde un turno |
| **FullStack Nomade**   | Può scambiare un task con un altro player | Se ha più di 3 task in Doing, ne fallisce 1 |
| **QA Esoterico**       | Può annullare 1 bug critico per partita | Ma ogni task dura +1 se non ha test |

---

## Esempi Carte

### Task Cards

| Nome                     | Durata | Valore |
|--------------------------|--------|--------|
| Scrivere Test            | 1      | 1      |
| Fixare Bug Critico       | 2      | 3      |
| Ottimizzare Query SQL    | 2      | 2      |
| Refactor Legacy Code     | 3      | 3      |
| Deploy in Produzione     | 4      | 4      |
| Documentare una API REST| 1      | 1      |
| Migrare a TypeScript     | 3      | 3      |

---

### Azione Cards

| Nome                     | Effetto |
|--------------------------|---------|
| Copia da StackOverflow   | Completa un task semplice subito (ma -1 karma per Junior) |
| Pair Programming         | Il task in Doing avanza di 2 turni anziché 1 |
| Ask ChatGPT              | Pesca 2 task extra ma uno è sbagliato (penalità random) |
| Automatizza Deploy       | I task DevOps costano -1 turno |
| Meditazione Agile        | +2 karma, ignora la prossima carta evento |
| Refactor Zen             | Rimuovi 1 bug e guadagni 1 punto extra su un task completato |

---

### Evento Cards

| Nome                        | Effetto |
|-----------------------------|---------|
| “Funziona sul mio PC”       | Sposta un task completato di un altro player di nuovo in Doing |
| Deploy Fallito              | Il task attivo di un altro giocatore viene azzerato |
| Riunione con 7 Manager      | Tutti perdono 1 turno e -1 karma |
| PM Visionario               | Anticipa la deadline: il task in Doing richiede -1 turno, ma -2 karma |
| Chat con GPT Male Addestrato| Il player pesca una carta bug casuale (es. “Risposta Hallucination”) |
| Merge Conflict Infinito     | Blocco del turno successivo e +1 bug Major |

---

## Sprint individuali

Ogni giocatore:
- Ha una **board personale** con task (`To Do`, `Doing`, `Done`)
- Può avere **1 solo task attivo alla volta**
- Riceve punti solo dai task completati nella **propria board**
- Può interagire con gli altri solo tramite le **carte Evento**

---

## Fine Sprint

Alla fine degli **8 turni**:

### Punteggio

- + Punti dai task completati
- -1 punto per ogni bug Minor
- -2 per Major, -4 per Critical
- -2 se Karma < 5

### Vincitore

Il dev con più punti **vince lo sprint**.  
In caso di pareggio, vince chi ha ricevuto più "reaction" dagli altri (ovvero: il dev più divertente o sabotato).

---

## Estensioni & Community

### Ruoli Custom
- Nome, abilità, malus
- Proposti dai giocatori → approvati via PR

### Decreti Personali
> "Non sopporto il PM"  
→ Ogni volta che si gioca una carta PM, guadagno +1 karma.

---

## Summary

- Gioco da 2–6 giocatori dev
- Ognuno ha uno sprint individuale con board ToDo/Doing/Done
- Task hanno durata (turni)
- Bug aumentano la durata dei task
- Karma rappresenta la stabilità mentale
- Carte evento sabotano gli altri, azione aiutano sé stessi
- Vince chi completa più task, gestisce meglio bug e karma

---

## License & Credits

Creato da dev, per dev.  
Forka. Rompi. Estendi.  
Trolla il tuo amico con stile.
