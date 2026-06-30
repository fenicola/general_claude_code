---
tags: [economia-informazione, game-theory, giochi-dinamici, backward-induction, SPNE]
aliases: [Giochi Sequenziali, Sequential Games, SPNE, Subgame Perfect Nash Equilibrium, Backward Induction]
links: [03_Nash_Equilibrium, 06_Dilemma_Prigioniero, 08_Giochi_Ripetuti_Finiti, 0. Intro/06_Segnalazione, 0. Intro/07_Screening, 0. Intro/04_Principale_e_agente]
---

# Giochi Dinamici Sequenziali

## Definizione Formale

> [!definition] Gioco Sequenziale e Forma Estesa
> Un **gioco sequenziale** (o *dynamic game*) è un gioco in cui i giocatori muovono in un ordine prestabilito, con ogni mossa successiva potenzialmente condizionata alle mosse precedenti. La rappresentazione naturale è la **forma estesa** (*extensive form* o *game tree*): un albero in cui:
> - I **nodi decisionali** indicano il giocatore che deve muovere
> - I **rami** rappresentano le azioni disponibili
> - I **nodi terminali** riportano i vettori di payoff
>
> Una **strategia** in un gioco sequenziale è un piano completo di azione che specifica cosa fare *in ogni nodo decisionale*, anche quelli che non verranno mai raggiunti in equilibrio.

> [!definition] Subgame Perfect Nash Equilibrium (SPNE)
> Un **SPNE** è una combinazione di strategie che costituisce un Nash Equilibrium in **ogni sottogioco** del gioco complessivo, inclusi i sottogiochi che non vengono raggiunti nel percorso d'equilibrio.
>
> Un **sottogioco** (*subgame*) è una porzione del gioco che:
> - Inizia a un nodo decisionale senza incertezza sulla storia
> - Contiene tutti i rami e i nodi successivi a quel nodo
> - Termina a nodi terminali del gioco complessivo

## Intuizione Economica

> [!intuition]
> In un gioco sequenziale, il Nash Equilibrium da solo non è sufficiente. Perché? Perché un NE può incorporare **minacce non credibili**: un giocatore minaccia di fare qualcosa che, se effettivamente chiamato a farlo, non avrebbe interesse a realizzare.
>
> Immagina un monopolista che minaccia di fare una guerra dei prezzi devastante contro chiunque entri nel suo mercato. Nell'albero del gioco, questa minaccia può tenere lontani i potenziali entranti (è un NE). Ma se qualcuno entrasse davvero, il monopolista subirebbe anche lui perdite enormi — quindi la minaccia non è credibile. Un entrante razionale lo capisce e entra comunque.
>
> Lo SPNE elimina questi equilibri basati su minacce non credibili: richiede che ogni strategia sia razionale *in ogni punto del gioco*, anche nei nodi che "non dovrebbero" essere raggiunti.

## Backward Induction

Il metodo per trovare lo SPNE è l'**induzione a ritroso** (*backward induction*): si parte dai nodi terminali e si lavora a ritroso verso la radice dell'albero, identificando a ogni nodo la mossa razionale del giocatore che muove lì.

> [C, p. 86–90] "Backward induction involves working back through the game checking that the players' strategies specify moves that constitute a Nash equilibrium in every subgame." Solo le minacce che il giocatore porterebbe effettivamente a termine (perché sono nel suo interesse) sono credibili e possono essere parte di uno SPNE.

**Algoritmo:**
1. Identificare i nodi terminali dell'albero
2. A ogni penultimo nodo, il giocatore sceglie l'azione che massimizza il suo payoff tra le alternative disponibili
3. Sostituire quel sottogioco con il payoff risultante
4. Ripetere fino alla radice

## Esempio: Il Gioco FDI (Foreign Direct Investment)

> [!example] Figura 4.1 — FDI Game (Carmichael)
> Alpha muove per prima scegliendo tra *FDI* (investimento diretto estero) o *export only*. Beta osserva la scelta e poi decide se *export* o *not export*.
>
> ```
>                         Alpha
>                        /     \
>                     FDI    Export only
>                    /              \
>                Beta(B₁)        Beta(B₂)
>               /    \           /    \
>          Export  Not exp.  Export  Not exp.
>          (25,-5) (40,10)   (30,30)  (60,10)
> ```
>
> **Backward Induction:**
>
> *Sottogioco a B₁* (Alpha ha scelto FDI):
> - Beta confronta: Export → −5 vs Not export → 10
> - Beta sceglie **Not export** (10 > −5) ✓
>
> *Sottogioco a B₂* (Alpha ha scelto Export only):
> - Beta confronta: Export → 30 vs Not export → 10
> - Beta sceglie **Export** (30 > 10) ✓
>
> *Nodo radice* (Alpha):
> - Sapendo che Beta giocherà (Not export | FDI) e (Export | Export only):
> - Alpha sceglie FDI → payoff 40; Export only → payoff 30
> - Alpha sceglie **FDI** (40 > 30) ✓
>
> **SPNE**: Alpha sceglie *FDI*; Beta sceglie *not export* se Alpha ha scelto *FDI* e *export* se Alpha ha scelto *export only*.
> **Payoff d'equilibrio**: (40, 10).

## La Molteplicità dei Nash e il Raffinamento

Il gioco FDI ha **due Nash Equilibria** nella forma strategica:
1. {*FDI*, (*not export*, *export*)}: payoff (40, 10) — questo è lo SPNE
2. {*export only*, (*export*, *export*)}: payoff (30, 30)

Il secondo NE richiede che Beta minacci di esportare anche se Alpha ha scelto FDI — ma questo è non credibile perché nel sottogioco B₁, Beta preferirebbe non esportare. Lo SPNE elimina questo secondo equilibrio.

> [C, p. 86] "For a Nash equilibrium to be subgame perfect it has to specify a combination of credible moves in every subgame: moves that are best responses at every decision node."

## Strategie vs. Mosse nei Giochi Sequenziali

Una distinzione cruciale: in un gioco sequenziale, la **strategia** di un giocatore che muove per secondo deve specificare cosa farebbe *in ogni possibile nodo decisionale* — non solo in quello che si raggiunge nell'equilibrio.

Nell'esempio FDI, la strategia completa di Beta è una coppia: (azione a B₁, azione a B₂). Ci sono quattro strategie possibili per Beta:
1. (*export*, *export*) — esporta sempre
2. (*not export*, *not export*) — non esporta mai
3. (*export*, *not export*)
4. (*not export*, *export*) — questa è la strategia dello SPNE

> [!example] Figura 4.2 — Nice-Not So Nice (Carmichael)
> Un esempio aggiuntivo con tre fasi: Giocatore 1 muove per primo (*nice* o *not so nice*), poi Giocatore 2 muove in risposta (nodo 2A o 2B). L'induzione a ritroso identifica: a 2A, Gioc. 2 preferisce *nice* (6 > 0); a 2B, Gioc. 2 preferisce *not so nice* (3 > 2). Quindi Gioc. 1 confronta: *nice* → 2 (con Gioc.2 che risponde *nice*) vs *not so nice* → −6 (con Gioc.2 che risponde *not so nice*). Gioc.1 sceglie *nice*.

## Quanti Sottogiochi?

Un gioco può avere molti sottogiochi. Nell'esempio con quattro nodi decisionali di Beta (Figura 4.6 di Carmichael), ci sono 4 sottogiochi propri più il gioco complessivo. Lo SPNE richiede un NE in ognuno di essi.

> [C, p. 88] Un sottogioco è identificato da un nodo decisionale dove non c'è incertezza sulla storia del gioco. Ogni sottogioco "corretto" (*proper subgame*) inizia a un nodo non-terminale con rami che portano fino ai nodi terminali del gioco complessivo.

## Minacce Credibili e Impegno

Una delle applicazioni più importanti dello SPNE è l'analisi delle **minacce credibili** in contesti come l'entrata nel mercato:

- Un monopolista minaccia di combattere chi entra nel suo mercato (*fight entry*)
- Se la minaccia è credibile (combattere è la miglior risposta anche dopo l'entrata), l'entrante non entra
- Se la minaccia non è credibile (combattere sarebbe costoso per il monopolista), l'entrante entra sapendo che il monopolista cederà

La credibilità si costruisce attraverso l'**impegno preventivo** (*pre-commitment*): investimenti irreversibili, contratti, reputazione. Questi cambiano i payoff in modo da rendere credibile la minaccia.

> [C, p. 103] "The role of credibility and commitment in sequential games was further highlighted in the analysis of the entry deterrence game. In order to deter entry the monopolist threatens to fight entry should it occur. But if the threat to fight is not credible the entrant will enter."

> [!summary] Take-home message
> Nei giochi sequenziali il Nash Equilibrium non basta: occorre il raffinamento in **SPNE**, che eliminina gli equilibri basati su minacce non credibili. Il metodo dell'induzione a ritroso (backward induction) permette di trovare lo SPNE partendo dai nodi terminali e lavorando a ritroso. Il messaggio economico fondamentale: le strategie devono essere credibili a ogni nodo del gioco, non solo sul percorso d'equilibrio. Nei [[08_Giochi_Ripetuti_Finiti|giochi ripetuti]] questo concetto genera il paradosso dell'induzione a ritroso.

## 🔗 Connessioni con l'Economia dell'Informazione

I **giochi sequenziali** e lo SPNE sono gli strumenti formali con cui si analizzano i principali meccanismi dell'economia dell'informazione:

- **[[0. Intro/06_Segnalazione|Signalling]]**: è un gioco sequenziale in cui la parte informata (Agente) muove per prima inviando un segnale; la parte non informata (Principale) osserva il segnale e risponde con un'offerta di contratto. Lo SPNE identifica l'equilibrio separante vs. pooling.
- **[[0. Intro/07_Screening|Screening]]**: gioco sequenziale inverso — il Principale muove per primo con un menù di contratti; l'Agente sceglie e rivela il proprio tipo. Il SPNE è il menù ottimale che soddisfa i vincoli di IC e IR.
- **[[0. Intro/08_Azzardo_morale|Azzardo morale]]**: la forma estesa cattura esplicitamente il timing — contratto → accettazione → azione nascosta → esito. Il SPNE è il contratto che anticipa razionalmente l'azione dell'Agente.
- **Deterrenza all'entrata** (*entry deterrence*): il monopolista che minaccia di combattere ha una minaccia credibile solo se combattere è la sua miglior risposta nel sottogioco rilevante — identico all'analisi del monopolista nel gioco FDI (§4.3 Carmichael).
