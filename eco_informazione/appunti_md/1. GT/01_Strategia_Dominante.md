---
tags: [economia-informazione, game-theory, equilibrio]
aliases: [Strategia Dominante, Dominant Strategy, Equilibrio in Strategie Dominanti]
links: [02_Iterated_Dominance, 03_Nash_Equilibrium, 0. Intro/03_Beni_comuni, 0. Intro/06_Dilemma_Prigioniero]
---

# Strategia Dominante

## Definizione Formale

> [!definition] Strategia Strettamente Dominante
> In un gioco a due giocatori (A e B), la strategia $A_i$ è **strettamente dominante** per A se, per tutte le possibili strategie alternative $A_{-i}$ e per tutte le strategie $B_i$ e $B_{-i}$ del giocatore B:
> $$P(A_i, B_i) > P(A_{-i}, B_i) \quad \text{e} \quad P(A_i, B_{-i}) > P(A_{-i}, B_{-i})$$
> dove $P(\cdot)$ indica il payoff. La condizione deve valere **simultaneamente** per ogni possibile scelta dell'avversario.

> [!definition] Strategia Debolmente Dominante
> La strategia $A_i$ è **debolmente dominante** se le disuguaglianze sopra sono *deboli* (≥ anziché >): i payoff con $A_i$ sono almeno tanto buoni quanto quelli con qualsiasi altra strategia, e in almeno un caso sono strettamente migliori.

In un **equilibrio in strategie dominanti** tutti i giocatori scelgono la propria strategia dominante. Un gioco ha tale equilibrio solo se *tutti* i giocatori possiedono una strategia dominante.

> [BB, p. 222] Un equilibrio in strategie dominanti è particolarmente robusto: un giocatore razionale lo sceglie indipendentemente da qualsiasi congettura sulle azioni altrui.

## Intuizione Economica

> [!intuition]
> La strategia dominante libera il giocatore dall'incertezza sulle altrui intenzioni: non importa ciò che fa l'avversario, la mia scelta ottimale è sempre la stessa. È come avere un impermeabile che funziona bene con qualsiasi previsione meteorologica. Il prezzo di questa comodità è che tali strategie esistono solo in pochi giochi.
> 
> Il giocatore razionale *sceglie sempre* la propria strategia dominante, qualora esista. Questo deriva direttamente dall'ipotesi di razionalità: se A è sempre meglio di B nelle stesse circostanze, nessun agente razionale sceglie B.

## Modello Formale

Sia $N = \{1, 2, \ldots, n\}$ l'insieme dei giocatori. Per il giocatore $i$, sia $S_i$ il suo spazio delle strategie e $u_i(s_i, s_{-i})$ la sua funzione di utilità, dove $s_{-i}$ indica le strategie di tutti gli altri giocatori.

La strategia $s_i^* \in S_i$ è **strettamente dominante** se:
$$u_i(s_i^*, s_{-i}) > u_i(s_i, s_{-i}) \quad \forall s_i \neq s_i^*, \; \forall s_{-i} \in S_{-i}$$

Un **equilibrio in strategie dominanti** è un profilo $(s_1^*, s_2^*, \ldots, s_n^*)$ tale che $s_i^*$ è strategia dominante per ogni $i \in N$.

Per la strategia **debolmente** dominante, la disuguaglianza diventa $\geq$ con almeno un caso di $>$.

## Esempio: Il Gioco dei Gestori di Pub

> [!example] Pub Managers Game (Carmichael, Matrix 2.1)
> Due pub concorrenti — Queen's Head e King's Head — decidono simultaneamente se lanciare una promozione (*special offer*) o non farlo (*no offer*).
>
> |  | King's: *special offer* | King's: *no offer* |
> |---|---|---|
> | **Queen's: *special offer*** | 10, 14 | 18, 6 |
> | **Queen's: *no offer*** | 4, 20 | 7, 8 |
>
> *Nota: ogni cella riporta (payoff Queen's Head, payoff King's Head)*
>
> **Verifica per Queen's Head:**
> - Se King's fa *special offer*: Queen's ottiene 10 (special) vs 4 (no) → conviene *special*
> - Se King's non fa offerta: Queen's ottiene 18 (special) vs 7 (no) → conviene *special*
>
> *Special offer* domina strettamente *no offer* per Queen's Head.
>
> **Verifica per King's Head:**
> - Se Queen's fa *special offer*: King's ottiene 14 (special) vs 6 (no) → conviene *special*
> - Se Queen's non fa offerta: King's ottiene 20 (special) vs 8 (no) → conviene *special*
>
> Anche per King's Head, *special offer* è strategia strettamente dominante.
>
> **Equilibrio**: {*special offer*, *special offer*} con payoff (10, 14). Questo è un equilibrio in strategie dominanti — e, come vedremo in [[03_Nash_Equilibrium]], è anche un Nash Equilibrium.

> [C, p. 22–29] Il gioco dei gestori di pub è l'esempio paradigmatico di equilibrio in strategie dominanti. Va notato che entrambi i gestori finiscono peggio che se avessero entrambi scelto *no offer* (7, 8 < 10, 14 per Queen's, ma 8 < 14 per King's): la struttura ricorda quella di un Dilemma del Prigioniero.

## Variante: Strategia Debolmente Dominante

> [!example] Pub Managers Game modificato
> Se il payoff di King's Head in {*special offer*, *no offer* di Queen's} diventa 14 anziché 6, allora King's Head è indifferente tra *special offer* e *no offer* quando Queen's non fa offerta (entrambe danno 14 e 8 → ora entrambe danno 14). *Special offer* diventa allora solo **debolmente** dominante per King's.

## Relazione con Altri Concetti di Equilibrio

La relazione logica tra i concetti di equilibrio è la seguente:

$$\text{Equilibrio in strategie dominanti} \;\Rightarrow\; \text{Iterated-Dominance Eq.} \;\Rightarrow\; \text{Nash Eq.}$$

Le implicazioni valgono in una sola direzione: ogni equilibrio in strategie dominanti è anche un [[02_Iterated_Dominance|equilibrio per dominanza iterata]] e un [[03_Nash_Equilibrium|Nash Equilibrium]], ma non viceversa.

> [C, p. 41–42] Formalmente: le condizioni (2.1) e (2.2) di Carmichael per la dominanza stretta implicano la condizione (2.3) del Nash Equilibrium, perché la condizione di Nash è necessaria ma non sufficiente per la dominanza.

## Limiti

Non tutti i giochi hanno un equilibrio in strategie dominanti. La maggior parte dei giochi economicamente interessanti non ce l'ha: è sufficiente che un giocatore non abbia una strategia che sia sempre la migliore risposta per far saltare il concetto. In questi casi occorre ricorrere a [[02_Iterated_Dominance]] o direttamente al [[03_Nash_Equilibrium]].

> [!summary] Take-home message
> La strategia dominante è il criterio di soluzione più potente in teoria dei giochi: chi la possiede dovrebbe sempre giocarla, indipendentemente dalle congetture sugli altri. L'equilibrio in strategie dominanti esiste solo quando *tutti* i giocatori hanno una tale strategia. Quando esiste, fornisce una previsione robusta e convincente dell'esito del gioco.

## 🔗 Connessioni con l'Economia dell'Informazione

La **strategia dominante** è il fondamento logico di molte analisi dell'Economia dell'Informazione:

- Nel [[0. Intro/03_Beni_comuni|dilemma del pescatore]], pescare *sopra* il limite è strategia dominante → tragedia dei beni comuni.
- Nell'[[0. Intro/08_Azzardo_morale|azzardo morale]], ridurre lo sforzo (*shirk*) è la strategia dominante dell'Agente in assenza di incentivi adeguati.
- Nella [[0. Intro/05_Selezione_avversa|selezione avversa]], il venditore di bene cattivo ha come strategia dominante offrirlo al prezzo del bene buono (finché il mercato non collassa).
- Il fatto che la defezione sia dominante nel [[0. Intro/03_Beni_comuni|PD del pescatore]] ma **non** nelle relazioni ripetute (→ [[09_Giochi_Ripetuti_Indefiniti]]) mostra perché la ripetizione e la reputazione sono così importanti nell'economia dell'informazione.
