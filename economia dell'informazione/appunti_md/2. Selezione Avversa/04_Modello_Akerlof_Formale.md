---
tags: [economia-informazione, selezione-avversa, modello-akerlof, molho]
aliases: [Modello Akerlof, Market for Lemons Model, Molho Cap 2]
links: [02_Mercato_dei_Limoni_Intuizione, 03_Modello_Formale_Due_Qualita, 05_Equilibrio_di_Mercato_Adverse_Selection]
---

# Il Modello Formale di Akerlof (Molho, Cap. 2)

## Setup del Modello

> [!definition]
> Il modello di Akerlof (1970) come presentato da Molho (cap. 2) si basa su due gruppi di agenti che interagiscono in un mercato di auto usate:
> - **Gruppo 1 (G1)** — i *proprietari* (*owners*): ciascuno possiede un'auto e ne conosce la qualità
> - **Gruppo 2 (G2)** — i *non-proprietari* (*not-owners*): vogliono acquistare un'auto ma non ne osservano la qualità
> - G2 valorizza le auto mediamente di più rispetto a G1 → esistono **guadagni potenziali dallo scambio**
> - Esiste **un solo prezzo di mercato** $p$ perché la qualità non è osservabile

Assunzione sulla qualità: segue una **distribuzione uniforme** su $[0, 2]$.

$$
q_i \sim U[0, 2] \qquad \Rightarrow \qquad f(q) = \frac{1}{2}, \quad \mu_{\text{tot}} = 1
$$

dove $f(q)$ è la densità di probabilità e $\mu_{\text{tot}}$ è la qualità media totale del parco auto.

---

## Il Gruppo 2: Domanda di Auto Usate

La funzione di utilità dei non-proprietari è:

$$
U_2 = M + \frac{3}{2} q \cdot n
$$

dove:
- $M$ = consumo di altri beni (numerario)
- $q$ = qualità dell'auto acquistata
- $n$ = variabile dummy: $n=1$ se l'auto viene acquistata, $n=0$ altrimenti
- $\frac{3}{2}$ = saggio marginale di sostituzione tra auto e altri beni

Il vincolo di bilancio è:

$$
y_2 = M + p \cdot n \qquad \Rightarrow \qquad M = y_2 - p \cdot n
$$

Sostituendo nella funzione di utilità:

$$
U_2 = y_2 + \left[\frac{3}{2}q - p\right] n
$$

I membri di G2 conoscono la **qualità media** delle auto sul mercato (aspettative razionali), ma non la qualità del singolo esemplare. Quindi massimizzano l'**utilità attesa**:

$$
E(U_2) = y_2 + \left[\frac{3}{2}\mu - p\right] n
$$

dove $\mu = E(q)$ è la qualità media attesa delle auto disponibili al prezzo $p$.

**Regola di decisione di G2:**

$$
\text{Acquista } (n=1) \text{ se e solo se } \frac{3}{2}\mu \geq p \qquad \Longleftrightarrow \qquad \mu \geq \frac{2}{3}p
$$

In altre parole, G2 compra solo se la qualità media attesa, pesata per il loro apprezzamento relativo ($\frac{3}{2}$), supera il prezzo. Riformulato in termini di $\mu$ e $p$, la **curva di domanda** nello spazio $(\mu, p)$ è:

$$
\mu = \frac{2}{3} p \qquad \text{(condizione di indifferenza G2)}
$$

---

## Il Gruppo 1: Offerta di Auto Usate

La funzione di utilità dei proprietari è:

$$
U_1 = M + q \cdot n
$$

dove qui $n=1$ significa *tenere* l'auto (consumarla come bene), $n=0$ significa *venderla*. Nota: possedere un'auto aumenta l'utilità di G1 di $q$ e di G2 di $\frac{3}{2}q$ — da qui i guadagni dallo scambio.

Con il vincolo di bilancio $M = y_1 - p \cdot n$ (dove vendere significa ricevere $p$ e cedere l'auto):

$$
U_1 = y_1 + (q - p) n
$$

I membri di G1 **conoscono** la qualità $q$ della propria auto e non affrontano incertezza.

**Regola di decisione di G1:**

$$
\text{Vendi } (n=0) \text{ se e solo se } p \geq q
$$

Un proprietario vende solo se il prezzo che riceve supera il valore (soggettivo) che attribuisce all'auto.

---

## Collegamento tra Prezzo e Qualità Media Offerta

Con la regola di vendita $p \geq q$ e la distribuzione uniforme $q \sim U[0,2]$:

- Per $p \leq 2$: vengono offerte tutte le auto con $q \leq p$
- Queste auto rappresentano una quota del parco auto pari a $\frac{p}{2}$
- La loro qualità media è la metà del punto di taglio:

$$
\mu = E[q \,|\, q \leq p] = \frac{p}{2}
$$

**Derivazione**: se $q$ è uniforme su $[0,2]$, allora $q$ condizionato a $q \leq p$ è uniforme su $[0,p]$, con media $p/2$.

Il numero di auto offerte è:

$$
S = \frac{p}{2} \cdot N
$$

dove $N$ è il numero totale di proprietari. La funzione $\mu = \frac{1}{2}p$ è la **curva di offerta** nel piano $(\mu, p)$: descrive la qualità media delle auto offerte al variare del prezzo.

> [M] La probabilità che un'auto scelta a caso abbia qualità $q \leq p$ è l'area della distribuzione uniforme fino a $p$, pari a $\frac{1}{2} \cdot p = \frac{p}{2}$.

---

## Rappresentazione Grafica dell'Equilibrio

Nel piano $(\mu, p)$:

- **Curva di offerta**: $\mu = \frac{1}{2}p$ (retta che passa per l'origine con pendenza 2)
- **Curva di domanda**: $\mu = \frac{2}{3}p$ (retta che passa per l'origine con pendenza $\frac{3}{2}$)

Le due rette si intersecano solo nell'origine: $\mu = 0$, $p = 0$.

Poiché la curva di offerta ($\mu = \frac{1}{2}p$) è **sempre a sinistra** della curva di domanda ($\mu = \frac{2}{3}p$) nel piano $(\mu, p)$ (cioè per ogni $p > 0$, la qualità media offerta è inferiore alla qualità minima richiesta dai compratori), non esiste alcun equilibrio con $p > 0$.

**Verifica algebrica:**

La condizione di acquisto è $\frac{3}{2}\mu \geq p$, con $\mu = \frac{1}{2}p$:

$$
\frac{3}{2} \cdot \frac{1}{2}p \geq p \qquad \Longleftrightarrow \qquad \frac{3}{4}p \geq p
$$

Questa disequazione è **falsa** per ogni $p > 0$. L'unica soluzione è $p = 0$.

---

## L'Unico Equilibrio: Zero Scambi

> [!definition]
> **Equilibrio di zero scambi (zero-trade equilibrium)**: l'unico equilibrio del modello di Akerlof con le ipotesi originali è $p = 0$, $\mu = 0$, $S = D = 0$.
>
> A questo equilibrio: i venditori con $q = 0$ sono indifferenti tra vendere e tenere l'auto (perché $p = q = 0$). I compratori sono indifferenti tra comprare e non comprare (perché $\frac{3}{2}\mu = 0 = p$). L'offerta coincide con la domanda (entrambe nulle), e il mercato è tecnicamente in equilibrio — ma a un volume di scambi pari a zero.

Questo risultato sembra paradossale: esistono **guadagni dallo scambio** (G2 valorizza le auto $\frac{3}{2}$ volte più di G1), eppure non avviene nessuno scambio. L'asimmetria informativa distrugge completamente il mercato.

> [M] Solo un equilibrio in questo modello: quando $p = 0$. Quando $q = 0$ i venditori sono indifferenti rispetto a vendere al prezzo $p = 0$ e i compratori sono indifferenti rispetto a comprare quando $\frac{3}{2}\mu = 0$. Equilibrio: $S = D$ con $p = 0$ e $q = \mu = 0$.

---

## Due letture intuitive del collasso

Il meccanismo dello zero-trade equilibrium può essere riassunto con due immagini ricorrenti:

> [!quote] La legge di Gresham
> *"Bad money drives out good"* — la moneta cattiva scaccia quella buona. Nel mercato delle auto usate vale l'analogo: le **auto cattive (i lemons) scacciano quelle buone**. Poiché il prezzo riflette solo la qualità *media*, i proprietari di auto di alta qualità non trovano conveniente vendere (per loro $q > p$) ed escono dal mercato; restano solo le auto peggiori, il che abbassa ulteriormente la qualità media attesa e quindi il prezzo, in un avvitamento.

> [!quote] Il paradosso di Groucho Marx
> *"Non vorrei mai entrare in un club disposto ad accettare uno come me."* Il compratore razionale ragiona così: **se quell'auto è in vendita, probabilmente il proprietario conosce un difetto nascosto.** Il fatto stesso che un bene venga offerto a quel prezzo è un *segnale negativo* sulla sua qualità — l'offerta diventa essa stessa cattiva notizia.

Entrambe le letture sottolineano il **doppio ruolo del prezzo** in un mercato con asimmetria informativa: non solo equilibra domanda e offerta, ma **segnala la qualità media** dei beni presenti. Ridurre il prezzo può peggiorare la qualità media offerta e quindi ridurre ancora la domanda — un effetto perverso assente nei mercati ordinari (sviluppato poi nel [[09_Modello_Wilson_Equilibri_Multipli|modello di Wilson]]).

---

## Il Mercato con Informazione Perfetta (Benchmark)

Per capire l'entità del fallimento del mercato, è utile confrontare con il caso di informazione perfetta e simmetrica:

- G1: $U_1 = y_1 + (q-p)n$ → Vende se $p \geq q$
- G2: $U_2 = y_2 + [\frac{3}{2}q - p]n$ → Compra se $p \leq \frac{3}{2}q$

Con informazione perfetta, per ogni auto di qualità $q_i$, esiste un range di prezzi che soddisfa entrambi:

$$
q_i \leq p_i \leq \frac{3}{2}q_i
$$

Qualunque prezzo in questo intervallo fa sì che il venditore venda e il compratore compri. Quindi, con informazione completa, **tutte le auto vengono scambiate** (i mercati si svuotano) a prezzi diversi per qualità diverse.

Il confronto è netto:
- Informazione simmetrica → tutti gli scambi possibili si realizzano
- Informazione asimmetrica → zero scambi (nel modello base di Akerlof)

---

## Take-home message

> [!summary]
> Il modello formale di Akerlof, come presentato da Molho (cap. 2), usa funzioni di utilità esplicite per ricavare le regole ottimali di vendita e acquisto. La regola del venditore è $p \geq q$; quella del compratore è $p \leq \frac{3}{2}\mu$. Con qualità uniformemente distribuita su $[0,2]$, la qualità media offerta è $\mu = \frac{1}{2}p$. Sostituendo nella condizione di acquisto si ottiene $\frac{3}{4}p \geq p$, che è impossibile per $p > 0$. L'unico equilibrio è dunque a $p = \mu = 0$: il mercato collassa completamente, nonostante esistano guadagni dallo scambio. L'asimmetria informativa — non la sua incompletezza — è la causa del fallimento.

---

## Vedi anche

- [[03_Modello_Formale_Due_Qualita]] — La versione semplificata con due sole qualità (BB cap. 13)
- [[05_Equilibrio_di_Mercato_Adverse_Selection]] — Analisi dettagliata dell'equilibrio grafico
- [[06_Variazioni_del_Modello]] — Quando il mercato non collassa del tutto
- [[08_Distribuzioni_di_Probabilita_Richiamo]] — Come calcolare $\mu = p/2$ dalla distribuzione uniforme

---

## Connessioni con il Vault

**Da `0. Intro`:**
- [[0. Intro/04_Principale_e_agente|Principale e Agente]] — le funzioni di utilità di venditore (Agente) e compratore (Principale) qui derivate sono il contenuto formale delle preferenze nel framework P–A con informazione asimmetrica ex-ante

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — la condizione $p = \mu = 0$ è il NE del gioco: dati i comportamenti di vendita ottimale ($p \geq q$) e acquisto ottimale ($p \leq \frac{3}{2}\mu$), nessuno devia. Si tratta di un NE in strategie miste con aspettative razionali
- [[1. GT/02_Iterated_Dominance|Iterated Dominance]] — si può derivare il collasso del mercato anche iterando l'eliminazione di strategie dominate: a ogni round di iterazione, il prezzo massimo che il compratore paga scende, il che riduce la qualità media offerta, il che riduce il prezzo massimo...
