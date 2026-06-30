---
tags: [economia-informazione, game-theory, equilibrio]
aliases: [Nash Equilibrium, Equilibrio di Nash, NE]
links: [01_Strategia_Dominante, 02_Iterated_Dominance, 04_Giochi_Coordinamento, 05_Chicken_Game, 06_Dilemma_Prigioniero, 0. Intro/02_Mercato_e_Hayek, 0. Intro/04_Principale_e_agente, 0. Intro/05_Selezione_avversa]
---

# Nash Equilibrium

## Definizione Formale

> [!definition] Nash Equilibrium
> Un **profilo di strategie** $(s_1^*, s_2^*, \ldots, s_n^*)$ è un **Nash Equilibrium** (NE) se, per ogni giocatore $i$, la strategia $s_i^*$ è la **miglior risposta** (*best response*) alle strategie degli altri giocatori:
> $$u_i(s_i^*, s_{-i}^*) \geq u_i(s_i, s_{-i}^*) \quad \forall s_i \in S_i, \; \forall i \in N$$
> Formalmente, in un gioco a due giocatori (A e B), il profilo $\{A_i, B_i\}$ è un NE se:
> $$P(A_i, B_i) \geq P(A_{-i}, B_i) \quad \text{e} \quad P(B_i, A_i) \geq P(B_{-i}, A_i)$$

> [C, p. 37–42] Il Nash Equilibrium è il concetto di equilibrio più utilizzato in teoria dei giochi. A differenza della strategia dominante, non richiede che la strategia sia la migliore risposta a *tutte* le possibili mosse avversarie, ma solo alla *specifica* strategia che l'avversario sta effettivamente giocando nell'equilibrio.

## Intuizione Economica

> [!intuition]
> Il Nash Equilibrium può essere interpretato come uno **stato di quiete strategica**: se tutti i giocatori stanno giocando le loro strategie NE, nessuno ha un incentivo *unilaterale* a deviare. È un'autoprofezia che si avvera — se tutti credono che si giocherà un certo profilo, nessuno vuole discostarsi.
>
> Un'interpretazione dinamica (il **Revision Test**): immagina che i giocatori abbiano appena giocato una partita e osservino il risultato. Se, ripensandoci, nessuno vuole cambiare la propria scelta sapendo cosa hanno fatto gli altri, allora il profilo giocato è un Nash Equilibrium.
>
> Il NE può anche essere visto come il **punto finale di un processo di apprendimento**: i giocatori aggiornano progressivamente le proprie credenze sulle altrui strategie; se le credenze convergono e sono verificate nell'equilibrio, il profilo risultante è un NE.

## Il Revision Test (Definizione Informale)

> [!definition] Revision Test
> Siano i giocatori in grado di osservare l'esito del gioco. Se nessun giocatore desidera **unilateralmente** cambiare la propria strategia — dati i payoff osservati e le scelte altrui — il profilo giocato è un Nash Equilibrium.

Questo test è utile per identificare intuitivamente i NE: basta chiedersi, cella per cella, se un giocatore potrebbe migliorare il proprio payoff cambiando solo la propria riga (o colonna), lasciando fissa l'altra.

## Procedura per Trovare il NE: Il Metodo delle Sottolineature

La tecnica standard consiste nel sottolineare, per ogni colonna (strategie di un giocatore), il payoff migliore del *row player*; e per ogni riga, il payoff migliore del *column player*. Le celle in cui *entrambi* i payoff sono sottolineati sono Nash Equilibria.

> [C, p. 38] Questo è un metodo meccanico ma efficiente: identificata la miglior risposta di ciascun giocatore a ciascuna strategia dell'altro, le celle con best responses reciproche costituiscono un NE.

## Esempio: Computer Wars 1

> [!example] Matrix 2.12 — Computer Wars 1 (Carmichael)
> Due aziende di computer (Pin Ltd e Chip Inc) scelgono simultaneamente una promozione: *lower price*, *free printer* o *extended guarantee*.
>
> |  | Chip: *lower price* | Chip: *free printer* | Chip: *extended guarantee* |
> |---|---|---|---|
> | **Pin: *lower price*** | 0, 4 | 4, 0 | **5, 3** |
> | **Pin: *free printer*** | 4, 0 | 0, 4 | **5, 3** |
> | **Pin: *extended guarantee*** | 3, 5 | 3, 5 | **6, 6** |
>
> Applicando le sottolineature: il NE è {*extended guarantee*, *extended guarantee*} con payoff (6, 6). Né Pin né Chip vorrebbero deviare sapendo che l'altro ha scelto la garanzia estesa.

## Esempio: Friends or Enemies 3 (NE Multipli)

> [!example] Matrix 2.14 — Friends or Enemies 3
> Ms Row e Mr Column: *party* o *club*.
>
> |  | Mr Column: *party* | Mr Column: *club* |
> |---|---|---|
> | **Ms Row: *party*** | **1**, **3** | 2, 0 |
> | **Ms Row: *club*** | **2**, **2** | 1, 2 |
>
> Sottolineando: 
> - Miglior risposta di Row a *party* di Column: *club* (2 > 1)
> - Miglior risposta di Row a *club* di Column: *party* (2 > 1)
> - Miglior risposta di Column a *party* di Row: *party* (3 > 0)
> - Miglior risposta di Column a *club* di Row: sia *party* che *club* (2 = 2)
>
> NE: {*club*, *party*} con payoff (2, 2). È anche un iterated-dominance equilibrium debole.

## Relazione con gli Altri Concetti di Equilibrio

La struttura logica è una gerarchia di implicazioni:

$$\underbrace{\text{Eq. Strategie Dominanti}}_{\text{più forte}} \;\Rightarrow\; \underbrace{\text{Iterated-Dominance Eq.}}_{\text{intermedio}} \;\Rightarrow\; \underbrace{\text{Nash Eq.}}_{\text{più generale}}$$

**Ogni equilibrio in strategie dominanti è un NE.** Dimostrazione: se $(A_i, B_i)$ è un equilibrio in strategie dominanti, allora $A_i$ è la miglior risposta a *qualsiasi* strategia di B, e in particolare alla strategia $B_i$; similmente per B. Dunque la condizione di NE è soddisfatta.

**Non ogni NE è un equilibrio in strategie dominanti.** Come nell'esempio sopra: {*club*, *party*} è un NE perché è la miglior risposta *reciproca*, ma Ms Row non ha una strategia dominante (la sua miglior risposta dipende dalla scelta di Column).

> [C, p. 41] Formalmente: la condizione di NE (2.3) è necessaria ma non sufficiente per la dominanza stretta (condizioni 2.1 e 2.2). Pertanto, la dominanza è una condizione più restrittiva.

## Limiti del Nash Equilibrium

1. **Molteplicità**: molti giochi hanno più di un NE (→ [[04_Giochi_Coordinamento]], [[05_Chicken_Game]]). Come si coordina sui giocatori su quale NE giocare?

2. **Assenza**: alcuni giochi in strategie pure non hanno alcun NE (es. giochi a somma zero come prendere un rigore). Richiedono strategie miste.

3. **Non-credibilità in giochi dinamici**: in giochi sequenziali, alcuni NE incorporano minacce che non sarebbero mai messe in atto da un giocatore razionale. Serve il raffinamento in **Subgame Perfect Nash Equilibrium** (→ [[07_Giochi_Dinamici_Sequenziali]]).

4. **Razionalità e conoscenza**: il NE presuppone che ogni giocatore conosca le strategie dell'equilibrio degli altri. Come si arriva a questa convergenza nelle aspettative?

> [C, p. 51] Il NE ha alcune limitazioni: molti giochi hanno equilibri multipli o nessuno in strategie pure. Il problema dei molteplici equilibri peggiora con giochi più complessi, il che ha spinto i teorici a raffinare il concetto (SPNE, Bayesian NE...).

> [!summary] Take-home message
> Il Nash Equilibrium è il concetto cardine della teoria dei giochi: ogni profilo di strategie che si stabilizza nel tempo, dove nessuno vuole deviare unilateralmente, è un NE. È il concetto più generale tra [[01_Strategia_Dominante|strategia dominante]] e [[02_Iterated_Dominance|dominanza iterata]], e li contiene entrambi. La sua forza — applicarsi a quasi tutti i giochi — è anche la sua debolezza: quando un gioco ha più Nash Equilibria, il concetto da solo non dice quale sarà l'esito effettivo.

## 🔗 Connessioni con l'Economia dell'Informazione

Il **Nash Equilibrium** è il concetto di equilibrio che permea l'intera economia dell'informazione:

- Nei mercati concorrenziali con informazione completa, l'equilibrio di mercato è un NE (e un ottimo paretiano) — questo è il nucleo dell'[[0. Intro/02_Mercato_e_Hayek|ipotesi di Hayek]] verificato da Vernon Smith.
- Nei mercati con asimmetria informativa ([[0. Intro/04_Principale_e_agente|framework P–A]]), l'equilibrio è tipicamente un NE non-efficiente: la [[0. Intro/05_Selezione_avversa|selezione avversa]] porta a un NE con solo beni cattivi in vendita (mercato dei *lemons*).
- I contratti ottimali di [[0. Intro/07_Screening|screening]] e [[0. Intro/06_Segnalazione|signalling]] sono progettati affinché l'auto-selezione dei tipi sia un NE — la condizione di compatibilità con gli incentivi (IC) è esattamente la condizione di NE nel gioco di contrattazione.
- Nei [[09_Giochi_Ripetuti_Indefiniti|giochi ripetuti]], la cooperazione diventa un NE del supergame quando il futuro conta abbastanza — fondamento della reputazione e della governance dei [[0. Intro/03_Beni_comuni|beni comuni]].
