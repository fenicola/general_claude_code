---
tags: [economia-informazione, game-theory, giochi-ripetuti, backward-induction]
aliases: [Giochi Ripetuti Finiti, Finitely Repeated Games, Paradosso Backward Induction]
links: [06_Dilemma_Prigioniero, 07_Giochi_Dinamici_Sequenziali, 09_Giochi_Ripetuti_Indefiniti, 0. Intro/08_Azzardo_morale, 0. Intro/03_Beni_comuni]
---

# Giochi Ripetuti Finiti

## Definizione Formale

> [!definition] Gioco Ripetuto Finito
> Un **gioco ripetuto finito** (*finitely repeated game*) è un gioco in cui lo stesso gioco base (*stage game*) viene giocato dagli stessi giocatori per un numero $T$ finito e **noto** di volte. Il gioco complessivo è chiamato **supergame**.
>
> Una **strategia nel supergame** (o *meta-strategia*) specifica l'azione in ogni round condizionatamente alla storia di tutte le azioni passate. Il concetto di equilibrio appropriato è lo [[07_Giochi_Dinamici_Sequenziali|SPNE]], trovato tramite backward induction sul supergame.

## Intuizione Economica

> [!intuition]
> Se il gioco si ripete un numero finito di volte, sembrerebbe che ci sia spazio per la cooperazione: "se cooperi oggi, coopererò domani." Ma la logica dell'induzione a ritroso vanifica questa speranza in modo sorprendente. Sapendo che nell'ultima ripetizione non ci sarà futuro, entrambi defezionano. Ma se nell'ultima ripetizione defezionano entrambi, la penultima diventa effettivamente l'ultima... e così via, fino alla prima ripetizione.
>
> Risultato: in un PD ripetuto un numero finito di volte, l'unico SPNE è defezionare in ogni round. La cooperazione è teoricamente impossibile — eppure gli esperimenti mostrano che le persone cooperano spesso. Questo è il **paradosso dell'induzione a ritroso**.

## Il Paradosso nell'Esempio

> [!example] PD Finito a 3 Round (Matrix 8.1 — Carmichael)
> Il Dilemma del Prigioniero viene ripetuto 3 volte tra John Row e Joe Column.
>
> |  | Joe: *cooperate* | Joe: *defect* |
> |---|---|---|
> | **John: *cooperate*** | 1, 1 | −1, 2 |
> | **John: *defect*** | 2, −1 | 0, 0 |
>
> Struttura: $c=2 > a=1 > d=0 > b=-1$, dunque il PD è strutturalmente corretto.
>
> **Round 3** (ultimo): Senza futuro, entrambi giocano *defect* (è la strategia dominante dello stage game). Payoff: (0, 0).
>
> **Round 2**: Entrambi sanno che nel Round 3 defezionano comunque. Dunque la scelta al Round 2 non influenza il Round 3. I payoff futuri attesi sono gli stessi indipendentemente da ciò che si fa ora. Il Round 2 è quindi identico a un one-shot PD → entrambi defezionano.
>
> **Round 1**: Stesso ragionamento → entrambi defezionano.
>
> **SPNE**: Defezionare in ogni round. Il gioco si svolge come se fosse una serie di one-shot PD indipendenti.

## Il Risultato Generale

Il risultato dell'esempio si generalizza:

> [C, p. 199–204] "Se un gioco one-shot ha un unico Nash Equilibrium (subgame perfect), questo equilibrio verrà giocato in ogni ripetizione del gioco ripetuto finitamente. Questo risultato è chiamato *paradosso dell'induzione a ritroso*."

Formalmente: se lo stage game ha un unico SPNE $\{s^*\}$, allora l'unico SPNE del supergame a $T$ round è giocare $\{s^*\}$ in ogni round, indipendentemente da $T$.

## Implicazioni

**Per il Dilemma del Prigioniero**: la cooperazione non può emergere in un PD finito con un numero noto di round. Questo è in netto contrasto con l'evidenza sperimentale, dove i soggetti tendono a cooperare per molti round prima di defezionare verso la fine.

**Per i giochi di entrata nel mercato** (*entry deterrence*, catena di negozi): anche qui, un incumbent razionale dovrebbe sempre cedere all'entrante, perché la minaccia di combattere è non-credibile a ritroso. Ma nella realtà si osservano strategie di deterrenza anche in giochi finiti.

## Risoluzione del Paradosso

Il paradosso si risolve introducendo **incertezza** nel gioco:

**1. Incertezza sulla durata**: se i giocatori non sanno quando finirà il gioco, l'induzione a ritroso non si può applicare. → Vedi [[09_Giochi_Ripetuti_Indefiniti]]

**2. Incertezza sulla razionalità**: se un giocatore non è sicuro che l'altro sia pienamente razionale (forse c'è una probabilità $P$ che l'altro giochi *tit-for-tat* meccanicamente), allora cooperare per costruire una reputazione di cooperatore diventa razionale anche nel gioco finito.

> [C, p. 215–225] Kreps, Milgrom, Roberts e Wilson (1982) hanno dimostrato che, se c'è incertezza sulla razionalità (o sul tipo di payoff) di almeno un giocatore, la cooperazione può emergere come equilibrio anche in un PD finito, per tutti i round eccetto gli ultimi due.

## Stage Game vs. Supergame

È utile distinguere due concetti:

- **Stage game**: il gioco base che viene ripetuto (es. il PD one-shot)
- **Supergame**: il gioco complessivo della ripetizione; le strategie nel supergame sono *meta-strategie* che specificano l'azione in ogni round in funzione della storia

La strategia "sempre cooperare" o "cooperare finché l'altro coopera, poi defezionare" sono esempi di meta-strategie del supergame. Nell'[[09_Giochi_Ripetuti_Indefiniti|indefinite repetition]] queste meta-strategie possono essere SPNE.

> [C, p. 203] "For a player's strategy to be an equilibrium strategy in a repeated game it needs to be a best response to the other player's move in every repetition of the game. As each repetition is effectively a subgame of the whole game the appropriate equilibrium concept is that of a subgame perfect Nash equilibrium."

> [!summary] Take-home message
> Il risultato chiave dei giochi ripetuti finiti è sconfortante: in un PD con un numero noto e finito di ripetizioni, l'induzione a ritroso porta all'unico SPNE di defezionare in ogni round. La cooperazione non è sostenibile. Questo paradosso tuttavia si risolve non appena si introduce incertezza sulla durata del gioco (passaggio ai [[09_Giochi_Ripetuti_Indefiniti|giochi indefiniti]]) o sul tipo dei giocatori. Nei giochi ripetuti indefinitamente, la prospettiva di interazioni future può rendere la cooperazione razionale.

## 🔗 Connessioni con l'Economia dell'Informazione

Il paradosso dell'induzione a ritroso nei giochi ripetuti **finiti** è particolarmente rilevante per:

- **[[0. Intro/08_Azzardo_morale|Azzardo morale e contratti di lavoro a termine]]**: se il contratto è a scadenza nota, l'agente ha incentivo a ridurre lo sforzo nell'ultimo periodo — e per backward induction in tutti i periodi precedenti. Questo spiega perché i contratti di incentivo (bonus differiti, pensioni, stock options con vesting) sono strutturati per spostare le ricompense verso la fine.
- **[[0. Intro/03_Beni_comuni|Beni comuni e fine del gioco]]**: nelle risorse comuni con un orizzonte temporale noto (concessioni a scadenza, accordi internazionali con termine), ci si aspetta un'escalation di sfruttamento verso la fine — esattamente il paradosso backward induction applicato alla tragedia dei commons.
- **Strategia della "catena di negozi"** (*chain store paradox*, Selten 1978): un incumbent razionale non dovrebbe mai combattere l'entrata in un gioco finito — ma nella realtà la reputation effect (incertezza sul tipo) risolve il paradosso, come discusso in [[09_Giochi_Ripetuti_Indefiniti]].
