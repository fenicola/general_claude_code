---
tags: [economia-informazione, azzardo-morale, modello-formale, principale-agente, utilità, sforzo]
aliases: [Modello Contratto di Incentivo, Setup PA Azzardo Morale]
links: [01_Definizione_e_Timing, 03_Primo_Migliore_Sforzo_Osservabile]
---

# Il Modello Formale: Setup del Contratto di Incentivo

## Il Contesto

> [!definition]
> Il **modello di contratto di incentivo** (*incentive contract theory*, o *principal–agent model* con azione nascosta) descrive la relazione tra un Principale risk-neutral e un Agente risk-averse, in cui l'Agente sceglie un livello di sforzo non osservabile che influenza stocasticamente l'esito di un progetto. Il Principale progetta un contratto che massimizza i propri profitti attesi rispettando il vincolo di partecipazione (e, nel secondo migliore, il vincolo di incentivo) dell'Agente.

> [BB, ch. 16] Il modello di base ha un Principale risk-neutral che possiede un progetto con rendimento incerto $X$ e chiede a un Agente risk-averse di gestirlo, offrendogli un contratto take-it-or-leave-it.

---

## Le Assunzioni Fondamentali

### Il Principale (P)
- È **risk-neutral**: massimizza il rendimento atteso, non gli importa la varianza. Formalmente, la sua funzione obiettivo è il valore atteso dei profitti netti.
- Possiede un **progetto con rendimento incerto** $X$, il cui valore dipende sia da fattori casuali sia dall'effort dell'Agente.
- Ha **potere di proposta** (primo mover): offre un contratto take-it-or-leave-it a $t=0$.

### L'Agente (A)
- È **risk-averse**: la sua utilità marginale del reddito è decrescente, cioè $u'(w) > 0$ e $u''(w) < 0$.
- La sua **funzione di utilità totale** è:
$$U = u(w) - e$$
dove $w$ è il salario ricevuto ed $e$ è la disutilità dello sforzo esercitato.

Questa forma additiva cattura un'intuizione fondamentale: il reddito genera utilità, ma lo sforzo genera disutilità; le due dimensioni sono separabili.

- Ha **due livelli di sforzo disponibili**:
  - $e_1$ = sforzo basso ("shirk") — bassa disutilità
  - $e_2$ = sforzo alto ("work") — alta disutilità, con $e_2 > e_1$

### Informazione e Common Knowledge

> [!intuition]
> Tutti gli elementi del gioco — le preferenze del Principale, la funzione di utilità dell'Agente, le probabilità degli esiti, la struttura dei costi dello sforzo — sono **common knowledge**. L'unica informazione privata dell'Agente è l'**azione concreta** che sceglie a $t=2$: non il fatto che possa scegliere tra $e_1$ ed $e_2$, ma quale dei due sceglie effettivamente.

Questo è cruciale: non si tratta di informazione privata sul *tipo* dell'Agente (come nella selezione avversa), ma sulla sua *azione* post-contrattuale.

---

## Il Legame Stocastico tra Sforzo ed Esito

Il progetto ha **due possibili esiti**: $X_H$ (rendimento alto) e $X_L$ (rendimento basso), con $X_H > X_L \geq 0$.

Le probabilità degli esiti dipendono dallo sforzo:

$$\text{Se } e_2 \text{ (work)}: \quad \Pr(X_H) = p > \frac{1}{2}, \quad \Pr(X_L) = 1-p$$

$$\text{Se } e_1 \text{ (shirk)}: \quad \Pr(X_H) = 1-p < \frac{1}{2}, \quad \Pr(X_L) = p$$

Lo sforzo alto **inverte le probabilità**: rende $X_H$ più probabile e $X_L$ meno probabile. Tuttavia, il legame è **stocastico**, non deterministico:

> [!intuition]
> Anche dopo un esito negativo $X_L$, un Agente che ha lavorato sodo (*work*) può sostenere di aver avuto sfortuna. E dopo un esito positivo $X_H$, un Agente pigro (*shirk*) può rivendicare di aver lavorato duro. Il Principale **non può inferire con certezza lo sforzo dall'esito**. Questo è esattamente perché l'azione rimane nascosta.

Dal fatto che $p > 1/2$ e $X_H > X_L$, segue che uno sforzo più alto genera un **rendimento atteso più alto**:

$$p X_H + (1-p) X_L > (1-p) X_H + p X_L$$

La differenza di rendimento atteso tra work e shirk è:

$$[p X_H + (1-p) X_L] - [(1-p) X_H + p X_L] = (2p-1)(X_H - X_L) > 0$$

Il termine $(2p-1)$ misura il **potere informativo dello sforzo**: quanto più $p$ si avvicina a 1, tanto più lo sforzo alto determina quasi certamente l'esito alto.

---

## La Struttura Contrattuale

Il contratto che il Principale può offrire è un **piano di pagamenti contingenti**:

$$\{w_H, w_L\}$$

dove $w_H$ è il salario pagato se l'esito è $X_H$ e $w_L$ è il salario pagato se l'esito è $X_L$.

Notare che il contratto è scritto sull'**esito** (osservabile e verificabile), non sullo **sforzo** (non osservabile). Il meccanismo di incentivo funziona proprio perché l'esito è correlato allo sforzo: rendendo $w_H > w_L$, si crea un incentivo indiretto a lavorare sodo.

> [BB, ch. 16] Le parti contraenti non possono contrattare sullo sforzo non osservabile. Tuttavia, possono contrattare su una variabile osservabile correlata allo sforzo — l'esito $X$. I contratti usano bonus, franchigie, premi dipendenti dalla storia, ecc., con l'obiettivo di indurre A a comportarsi in modo affidabile.

---

## L'Albero del Gioco

Il gioco si rappresenta in forma estesa a quattro stadi (slide 17):

```
         P
         │
      {w₁, w₂}        ← t=0: P offre il contratto
         │
         A
       /   \
   accetta  rifiuta    ← t=1: A decide se accettare
     │          │
     │          0 (payoff di riserva per A)
     │
   ┌─────────┐
  work     shirk       ← t=2: A sceglie lo sforzo (AZIONE NASCOSTA)
  /  \     /  \
 p  1-p  1-p   p       ← probabilità degli esiti
 │    │   │    │
 XH  XL  XH   XL       ← t=3: si realizza l'esito
```

> [!intuition]
> Il Principale non osserva il nodo di scelta a $t=2$: non sa se A è nel ramo "work" o nel ramo "shirk". Nella terminologia dei giochi ad informazione imperfetta, $t=2$ è un **insieme informativo** non singleton per il Principale — vede solo il risultato finale, non l'azione.

### Soluzione per Backward Induction

Il Principale risolve il gioco **all'indietro**:

1. **Da $t=3$ a $t=2$**: dato il contratto $\{w_H, w_L\}$, quale effort sceglierà A? Questo determina la strategia dell'Agente in risposta al contratto.
2. **Da $t=2$ a $t=1$**: A accetterà il contratto solo se la sua utilità attesa (netto del costo dello sforzo) è almeno pari alla sua utilità di riserva — il **vincolo di partecipazione (PC)**.
3. **A $t=0$**: il Principale, anticipando le scelte di A nei periodi successivi, progetta il contratto ottimale per ciascun livello di effort desiderato, poi confronta i profitti attesi per scegliere il livello di effort da indurre.

---

## Take-home Message

> [!summary]
> Il modello ha **un Principale risk-neutral** e **un Agente risk-averse** con utilità $U = u(w) - e$, $u' > 0$, $u'' < 0$. L'Agente sceglie tra sforzo basso $e_1$ e sforzo alto $e_2$ a $t=2$, dopo aver accettato il contratto a $t=1$; l'esito $X \in \{X_H, X_L\}$ si realizza a $t=3$ con probabilità $p$ o $1-p$ a seconda dell'effort. Il legame sforzo→esito è **stocastico**: non è possibile inferire con certezza l'effort dall'esito osservato, ed è questa caratteristica che rende l'azione "nascosta" anche a posteriori. Il contratto è scritto sull'esito e si risolve per backward induction.

---

## Vedi Anche

- [[01_Definizione_e_Timing]] — Definizione di azzardo morale e timing del gioco
- [[03_Primo_Migliore_Sforzo_Osservabile]] — Cosa succederebbe se P potesse osservare lo sforzo?
- [[04_Secondo_Migliore_Sforzo_Non_Osservabile]] — Il contratto ottimale con sforzo nascosto
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — L'albero del gioco e la backward induction
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — L'equilibrio del gioco è un Nash (bayesiano perfetto nei sottogiochi)
