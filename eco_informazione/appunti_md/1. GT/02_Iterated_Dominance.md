---
tags: [economia-informazione, game-theory, equilibrio]
aliases: [Iterated Dominance, Dominanza Iterata, IESDS]
links: [01_Strategia_Dominante, 03_Nash_Equilibrium, 0. Intro/04_Principale_e_agente, 0. Intro/07_Screening]
---

# Equilibrio per Dominanza Iterata

## Definizione Formale

> [!definition] Iterated-Dominance Equilibrium
> Un gioco ha un **equilibrio per dominanza iterata** se, eliminando progressivamente le strategie dominate (strettamente o debolmente) di ciascun giocatore, rimane un unico profilo di strategie. Questo profilo costituisce l'equilibrio.
>
> La procedura si chiama **IESDS** (Iterated Elimination of Strictly Dominated Strategies) nella versione con dominanza stretta, o **IEWDS** con dominanza debole.
>
> Un gioco ha un iterated-dominance equilibrium se almeno *uno* dei giocatori ha una strategia dominante, anche se non tutti ce l'hanno.

> [C, p. 29–36] L'eliminazione iterativa funziona perché si fonda sulla Common Knowledge of Rationality (CKR): non solo io sono razionale, ma so che l'altro è razionale, e so che lui sa che io sono razionale, e così via. Ogni round di eliminazione sfrutta un livello aggiuntivo di questa catena cognitiva.

## Intuizione Economica

> [!intuition]
> Immagina di giocare a scacchi contro un avversario di cui conosci la razionalità. Puoi eliminare subito le mosse che lui non farebbe mai (perché dominate), poi — data questa eliminazione — puoi eliminare le tue mosse ora dominate, e poi ancora le sue, e così via. Questo processo di "messa a fuoco reciproca" riduce progressivamente lo spazio delle strategie ammissibili fino (talvolta) a identificare un unico esito.
>
> Il punto cruciale: il processo è giustificato solo se la razionalità è *common knowledge*. Se non posso essere sicuro che l'altro sia razionale (o che sappia che io lo so), alcune delle eliminazioni diventano rischiose.

## Modello Formale

Sia $S_i^0 = S_i$ l'insieme originale delle strategie del giocatore $i$. Al passo $k$, eliminare da $S_i^{k-1}$ tutte le strategie $s_i$ per cui esiste $s_i' \in S_i^{k-1}$ tale che:

$$u_i(s_i', s_{-i}) > u_i(s_i, s_{-i}) \quad \forall s_{-i} \in \prod_{j \neq i} S_j^{k-1}$$

Il processo converge quando $S_i^k = S_i^{k-1}$ per tutti gli $i$. Se all'convergenza ogni $S_i^*$ è un singoletto, il profilo $\{s_i^*\}$ è l'iterated-dominance equilibrium.

## Esempi

### Esempio 1: Friends or Enemies 1 (2×2)

> [!example] Matrix 2.6 — Friends or Enemies 1 (Carmichael)
> Ms Row e Mr Column devono scegliere tra *party* e *club*.
>
> |  | Mr Column: *party* | Mr Column: *club* |
> |---|---|---|
> | **Ms Row: *party*** | 1, 3 | 2, 0 |
> | **Ms Row: *club*** | 2, 2 | 1, 1 |
>
> **Analisi di Mr Column:**
> - Se Ms Row va al *party*: Column ottiene 3 (party) vs 0 (club) → preferisce *party*
> - Se Ms Row va al *club*: Column ottiene 2 (party) vs 1 (club) → preferisce *party*
>
> *Party* è strategia strettamente dominante per Mr Column. Eliminata la colonna *club* di Column, Ms Row confronta solo: *party* (→ 1) vs *club* (→ 2). Ms Row preferisce *club*.
>
> **Equilibrio iterato**: {*club*, *party*} con payoff (2, 2).
>
> Notare: Ms Row *non* ha una strategia dominante prima dell'eliminazione — solo dopo l'eliminazione della colonna *club* di Column, la scelta di Ms Row diventa univoca.

### Esempio 2: Political Ambition (2×2 con strategia debole)

> [!example] Matrix 2.7 — Political Ambition (Carmichael)
> Un candidato sfidante (Challenger) decide se presentarsi (Challenge) o non presentarsi (No Challenge). L'incumbent MP decide se restare in carica (Stand) o dimettersi (Resign).
>
> |  | Incumbent: *Stand* | Incumbent: *Resign* |
> |---|---|---|
> | **Challenger: *No challenge*** | 5, 10 | 0, 1 |
> | **Challenger: *Challenge*** | −15, 9 | 15, 1 |
>
> **Analisi dell'Incumbent:**
> - Resign gli dà sempre 1, Stand gli dà 10 o 9. Stand domina strettamente Resign.
>
> Eliminata *Resign*, lo sfidante valuta: No Challenge → 5, Challenge → −15. Quindi No Challenge domina.
>
> **Equilibrio**: {*No challenge*, *Stand*} — lo sfidante non si presenta, l'incumbent resta.

### Esempio 3: Friends or Enemies 2 (3×3)

> [!example] Matrix 2.8 — Friends or Enemies 2
> Versione con tre strategie per ciascun giocatore: *party*, *club*, *wedding*.
>
> |  | *party* | *club* | *wedding* |
> |---|---|---|---|
> | ***party*** | 1, 3 | 2, 0 | 1, 1 |
> | ***club*** | 2, 2 | 1, 1 | 1, 0 |
> | ***wedding*** | 1, 3 | 1, 4 | 0, 5 |
>
> **Passo 1**: *Wedding* di Ms Row è dominata debolmente da *club* (confronto riga per riga: 1≤2, 1=1, 0≤1). Elimino *wedding* di Ms Row.
>
> **Passo 2**: Senza *wedding* di Row, *club* di Column ottiene al massimo 2 (club, club). Ma *party* di Column ottiene 3 quando Row va al party e 2 quando va al club: *party* domina *club* di Column. Elimino *club* di Column.
>
> **Passo 3**: Senza *club* di Column, Ms Row confronta *party* (1 vs 1) e *club* (2 vs 1): *club* domina.
>
> **Equilibrio**: {*club*, *party*} con payoff (2, 2).

## Proprietà e Limiti

**Proprietà chiave:**
- Con dominanza *stretta*, l'ordine di eliminazione non cambia il risultato finale (invarianza dell'ordine)
- Con dominanza *debole*, l'ordine può cambiare e si possono eliminare Nash Equilibria validi — usare con cautela
- L'equilibrio per dominanza iterata è sempre un [[03_Nash_Equilibrium|Nash Equilibrium]], ma non viceversa

**Limiti:**
- Richiede Common Knowledge of Rationality a più livelli: ogni round di eliminazione richiede un livello aggiuntivo di "so che sai che so..."
- Molti giochi non convergono a un singolo profilo attraverso questo processo
- La dominanza debole può eliminare equilibri desiderabili

> [C, p. 35] Cancellare strategie debolmente dominate può portare all'eliminazione di un Nash Equilibrium: è una cautela importante quando si usa l'IEWDS.

> [!summary] Take-home message
> L'eliminazione iterativa delle strategie dominate è uno strumento potente quando esiste, ma richiede la Common Knowledge of Rationality. Funziona a cascata: l'eliminazione della strategia dominata di un giocatore può rendere dominate strategie che prima non lo erano per l'altro. Il risultato — quando unico — è un equilibrio che è anche un [[03_Nash_Equilibrium]], ma più robusto di un Nash generico perché sopravvive a un processo di depurazione progressiva.

## 🔗 Connessioni con l'Economia dell'Informazione

La **dominanza iterata** è rilevante in economia dell'informazione principalmente come fondamento della razionalità reciproca nei meccanismi di contrattazione:

- Nello [[0. Intro/07_Screening|screening]], il Principale anticipa che un Agente razionale sceglierà il contratto che massimizza la sua utilità: questo è esattamente il ragionamento di eliminazione iterata applicato al menù di contratti.
- Nei meccanismi di *revelation principle* (fondamento del mechanism design, Nobel 2007), si argomenta che un meccanismo incentive-compatible rende dominante per ogni tipo rivelare la propria informazione vera — l'analisi usa dominanza iterata per mostrare che il meccanismo è robusto.
- La Common Knowledge of Rationality (CKR) richiesta dall'eliminazione iterata è la stessa ipotesi sottostante al framework [[0. Intro/04_Principale_e_agente|Principale–Agente]] nei modelli di teoria dei contratti.
