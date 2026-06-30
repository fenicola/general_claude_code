---
tags: [economia-informazione, game-theory, equilibri-multipli, guerra-attrito]
aliases: [Chicken Game, Gioco del Pollo, War of Attrition, Guerra di Attrito]
links: [03_Nash_Equilibrium, 04_Giochi_Coordinamento, 06_Dilemma_Prigioniero, 0. Intro/06_Segnalazione, 0. Intro/01_Coordinamento_e_incentivi]
---

# Chicken Game (Guerra di Attrito)

## Definizione Formale

> [!definition] Chicken Game
> Il **Chicken Game** è un gioco a due giocatori con due Nash Equilibria che **non** sono Pareto-ordinabili: ogni giocatore preferisce un equilibrio diverso, e nessun equilibrio domina l'altro nel senso di Pareto. Esiste un esito non-equilibrio che entrambi i giocatori vogliono evitare perché disastroso per entrambi, e un esito di coordinamento "morbido" che nessuno preferisce ma entrambi tollerano meglio del disastro.
>
> La struttura dei payoff è: $c > a > b > d$ (per il giocatore riga, dove *c* = payoff da "sfidare" contro chi "cede", *a* = payoff da cedere entrambi, *b* = payoff da cedere io contro chi sfida, *d* = payoff dal disastro reciproco).

## Intuizione Economica

> [!intuition]
> Il Chicken Game prende il nome dal gioco adolescenziale in cui due auto si lanciano a velocità verso una scarpata o l'una contro l'altra: chi svolta per primo (il "pollo") perde la faccia, ma chi non svolta rischia la vita. Se nessuno svolta, il risultato è catastrofico per entrambi.
>
> La strategia ottimale dipende crucialmente da ciò che *l'altro* farà: se l'avversario è determinato a non cedere, meglio cedere. Ma se anche tu sei determinato, entrambi finiscono male. A differenza dello [[04_Giochi_Coordinamento|Stag Hunt]], qui il problema non è la fiducia ma la **deterrenza**: come convincere l'altro che non cederai mai.

## Modello Formale

> [!example] Matrix 2.20 — Chicken 1: War of Attrition (Carmichael)
> Smith e Jones sono due ex-pugili che devono decidere se sfidarsi (*challenge*) o cedere (*back down*).
>
> |  | Jones: *back down* | Jones: *challenge* |
> |---|---|---|
> | **Smith: *back down*** | 2, 2 | 0, 5 |
> | **Smith: *challenge*** | 5, 0 | −20, −20 |
>
> **Due Nash Equilibria:**
> - {*challenge*, *back down*}: payoff (5, 0) — Smith sfida, Jones cede. Smith preferisce questo.
> - {*back down*, *challenge*}: payoff (0, 5) — Smith cede, Jones sfida. Jones preferisce questo.
>
> **Esito non-NE peggiore**: {*challenge*, *challenge*} con payoff (−20, −20) — catastrofico per entrambi.
> **Esito non-NE misto**: {*back down*, *back down*} con payoff (2, 2) — nessuno sfida, entrambi moderatamente soddisfatti.
>
> I due Nash Equilibria **non** sono Pareto-ordinabili: Smith preferisce il primo, Jones il secondo. Non c'è un equilibrio che entrambi preferiscano all'altro.

## Caratteristiche Distintive

Il Chicken Game differisce dagli altri giochi con equilibri multipli per alcune proprietà fondamentali:

**1. Asimmetria degli equilibri**: a differenza dello Stag Hunt, i due giocatori hanno preferenze *opposte* sull'equilibrio da raggiungere. Non si tratta di coordinare su un obiettivo comune ma di "chi cede per primo."

**2. Il paradosso dell'impegno**: la forza nel Chicken Game viene dall'essere percepiti come irrazionalmente determinati. Se riesci a convincere l'avversario che *non puoi* cedere (perché hai bruciato i ponti, ti sei legato al volante, ecc.), l'altro è costretto a cedere. Ma questo richiede di rinunciare alla razionalità strumentale — e una minaccia credibile di distruzione reciproca è una minaccia non-credibile, razionalmente.

**3. Relazione con la dissuasione nucleare**: il gioco è largamente utilizzato in politologia internazionale per modellare la deterrenza nucleare e le crisi diplomatiche. La vignetta nelle slide (Washington Post, 2002) ritrae l'escalation militare come esattamente questa trappola: entrambe le parti si convincono di dover attaccare per prime, finendo nel disastro reciproco.

> [C, p. 46–47] Carmichael sottolinea che nel Chicken Game la previsione dell'esito è particolarmente difficile perché entrambi i Nash Equilibria sono ugualmente "validi" teoricamente, ma i giocatori hanno preferenze opposte. Nessun argomento razionale indica quale si realizzerà. Questo è precisamente il caso in cui le strategie miste diventano interessanti.

## Applicazioni Economiche e Sociali

Il Chicken Game modella diversi scenari reali:

- **Negoziazioni sindacali**: il sindacato minaccia lo sciopero (costoso per entrambi), l'impresa minaccia il licenziamento. Chi cede per primo?
- **Standard tecnologici**: due aziende in guerra per imporre il proprio standard (VHS vs Betamax, Blu-ray vs HD-DVD). Se entrambe persistono a lungo, entrambe perdono.
- **Crisi diplomatiche**: la Crisi dei Missili di Cuba del 1962 è spesso analizzata come un Chicken Game tra USA e URSS.
- **Regolamentazione ambientale**: un paese attende che un altro agisca per primo (free riding), ma se nessuno agisce il risultato è il disastro ambientale.

## Strategie di Soluzione

In assenza di un equilibrio naturalmente selezionato, i giocatori possono ricorrere a:

1. **Impegno preventivo** (*pre-commitment*): "bruciare i ponti" rimuovendo la possibilità di cedere. In questo modo si fa del proprio atteggiamento rigido una *credibile minaccia*.

2. **Comunicazione** (*cheap talk*): segnalare la propria determinazione. Ma, a differenza di segnali costosi, la sola comunicazione verbale non è credibile.

3. **Strategie miste**: randomizzare tra *challenge* e *back down* con probabilità calibrate in modo che l'altro sia indifferente. Questo genera un terzo equilibrio (in strategie miste) ma richiede calcolo sofisticato.

4. **Meccanismi istituzionali**: arbitri, regole del gioco esterne o strutture legali che impongono chi deve cedere (es. regolamentazione antitrust).

> [BB, p. 234] Birchler & Bütler discutono come in mercati con esternalità negative la struttura del Chicken Game possa spiegare il ritardo nell'adozione di norme ambientali o nella regolamentazione finanziaria: ogni operatore attende che altri facciano il passo.

## Confronto con altri Giochi a NE Multipli

| Caratteristica | [[04_Giochi_Coordinamento\|Stag Hunt]] | Chicken Game |
|---|---|---|
| NE Pareto-ordinabili? | Sì | No |
| I giocatori concordano su quale NE preferire? | Sì | No |
| Problema centrale | Fiducia / sicurezza | Deterrenza / impegno |
| Esito peggiore | Cacciare il cervo da soli | Sfidare entrambi |

> [!summary] Take-home message
> Il Chicken Game è il modello paradigmatico della **guerra di attrito**: due parti in conflitto su chi debba cedere, con la consapevolezza che nessuno dei due cedere è un disastro. A differenza dei giochi di coordinamento "puri", i due Nash Equilibria non sono Pareto-ordinabili e i giocatori hanno preferenze opposte su quale si realizzi. Il risultato pratico è l'indeterminazione: la teoria predice che *un* equilibrio si realizzerà, ma non *quale*. Soluzioni praticabili richiedono impegni pre-credibili, istituzione di arbitri o strategie miste.

## 🔗 Connessioni con l'Economia dell'Informazione

Il **Chicken Game** (guerra di attrito) ha applicazioni significative nell'economia dell'informazione:

- **[[0. Intro/06_Segnalazione|Signalling e impegno credibile]]**: il cuore del Chicken Game è la credibilità dell'impegno — chi riesce a convincere l'avversario che non cederà vince. Questa è esattamente la logica del segnale credibile: il segnale funziona perché è costoso da imitare, rendendo l'impegno credibile. Il *Handicap Principle* in biologia è la versione evolutiva del Chicken Game.
- **Standard tecnologici e lock-in**: le battaglie tra standard tecnologici incompatibili (VHS vs Betamax, ecc.) sono Chicken Games in cui entrambe le imprese preferirebbero che l'altra cedesse, ma se entrambe persistono indefinitamente nessuno standard emerge (esito peggiore per tutti).
- **Negoziazione e contratti**: molte trattative contrattuali hanno la struttura del Chicken Game — entrambe le parti vogliono che l'altra faccia la prima concessione. I [[0. Intro/01_Coordinamento_e_incentivi|meccanismi istituzionali]] (arbitrato, mediazione) servono a rompere questa simmetria e identificare chi deve cedere.
