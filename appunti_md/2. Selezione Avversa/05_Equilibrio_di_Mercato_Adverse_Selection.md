---
tags: [economia-informazione, selezione-avversa, equilibrio, zero-trade]
aliases: [Zero Trade Equilibrium, Equilibrio Zero Scambi, Adverse Selection Equilibrium]
links: [04_Modello_Akerlof_Formale, 06_Variazioni_del_Modello, 07_Inefficienza_e_Implicazioni]
---

# Equilibrio di Mercato sotto Selezione Avversa

## Il Piano $(\mu, p)$: Una Rappresentazione Non Convenzionale

> [!definition]
> L'equilibrio del mercato con selezione avversa viene rappresentato in modo originale da Akerlof/Molho nel piano $(\mu, p)$, dove sull'asse orizzontale si trova la **qualità media** $\mu$ e sull'asse verticale il **prezzo** $p$. Questo piano consente di visualizzare simultaneamente le condizioni di offerta (come la qualità media cambia col prezzo) e di domanda (la qualità minima richiesta per giustificare un dato prezzo).

La scelta di questo piano non è casuale: riflette il fatto che in un mercato con asimmetria informativa, il prezzo determina sia la quantità offerta sia la qualità media offerta. Lavorare nel piano $(\mu, p)$ permette di vedere entrambi gli effetti.

---

## La Curva di Offerta nel Piano $(\mu, p)$

Con qualità $q \sim U[0, 2]$ e regola di vendita $p \geq q$, la qualità media delle auto offerte al prezzo $p$ è:

$$
\mu = \frac{1}{2}p \qquad \text{per } p \leq 2
$$

Nel piano $(\mu, p)$ questa è una **retta con pendenza 2** che parte dall'origine. Al crescere del prezzo offerto, entrano nel mercato auto di qualità crescente, ma la qualità media rimane sempre la metà del prezzo (perché le auto con $q \in [0, p]$ sono distribuite uniformemente).

**Interpretazione**: per ogni prezzo $p$, la qualità media delle auto effettivamente offerte è la metà di $p$. Se un compratore offre $p = 1$, la qualità media delle auto che riceverà sarà solo $\mu = 0{,}5$.

---

## La Curva di Domanda nel Piano $(\mu, p)$

G2 compra solo se $\frac{3}{2}\mu \geq p$, ovvero:

$$
\mu = \frac{2}{3}p
$$

Nel piano $(\mu, p)$ questa è una **retta con pendenza** $\frac{3}{2}$ che parte dall'origine. La pendenza è *minore* di quella della curva di offerta (pendenza 2).

**Interpretazione**: la curva di domanda nel piano $(\mu, p)$ dice qual è la qualità media *minima* necessaria perché i compratori di G2 siano disposti a pagare il prezzo $p$. Se il prezzo è $p = 1$, la qualità minima accettabile è $\mu = \frac{2}{3}$.

---

## Perché Non Esiste Equilibrio con $p > 0$

Confrontando le due rette:

- **Offerta**: $\mu = \frac{1}{2}p$ → pendenza 2 (più ripida)
- **Domanda**: $\mu = \frac{2}{3}p$ → pendenza $\frac{3}{2}$ (meno ripida)

Per ogni valore di $p > 0$:

$$
\mu_{\text{offerta}} = \frac{p}{2} < \frac{2p}{3} = \mu_{\text{domanda}}
$$

La curva di offerta è sempre **a sinistra** della curva di domanda nel piano $(\mu, p)$. Non c'è mai un punto di intersezione con $p > 0$. La supply è sempre troppo a sinistra rispetto alla demand.

Graficamente: se si disegna la regione di offerta positiva (a destra della retta di offerta) e la regione di domanda positiva (a sinistra della retta di domanda), le due regioni non si sovrappongono per $p > 0$.

L'unica intersezione è nell'**origine** $(0, 0)$: equilibrio di zero scambi.

> [M] I compratori (G2) comprano solo se $(3/2)\mu \geq p$. I venditori (G1) vendono solo se $p \geq q$, il che implica qualità media $\mu = (1/2)p$. Sostituendo: $(3/2)(1/2)p \geq p$, ovvero $\frac{3}{4}p \geq p$: falso per ogni $p > 0$.

---

## Caratteristiche dell'Equilibrio di Zero Scambi

> [!definition]
> L'**equilibrio di zero scambi** (*zero-trade equilibrium*) del modello di Akerlof è caratterizzato da:
>
> $$p^* = 0, \quad \mu^* = 0, \quad S^* = D^* = 0$$
>
> - I venditori con $q = 0$ sono indifferenti (vendere a 0 equivale a non vendere)
> - I compratori sono indifferenti tra comprare a $p = 0$ e non comprare (perché $\frac{3}{2} \cdot 0 = 0$)
> - L'offerta coincide con la domanda (entrambe nulle)
> - Il mercato è *tecnicamente* in equilibrio, ma è un equilibrio vuoto

Questo equilibrio è l'unico punto in cui la condizione $S = D$ è soddisfatta. Non si tratta di un "corner solution" in senso classico: è il risultato necessario della dinamica informativa.

---

## L'Aspetto Dinamico: La Spirale della Selezione

> [!intuition]
> Il collasso del mercato segue una logica sequenziale intuitiva: immagina di partire con un prezzo alto $p_0 > 0$. A quel prezzo entrano nel mercato auto con $q \leq p_0$, con qualità media $\mu_0 = p_0/2$. Ma i compratori vogliono $\mu \geq \frac{2}{3}p_0 > \mu_0$. Non comprano. Il venditore abbassa il prezzo a $p_1 < p_0$. Ma a $p_1$ le auto offerte hanno $\mu_1 = p_1/2 < \mu_0$: la qualità è peggiorata ancora. I compratori vogliono ancora di più qualità... e così via fino allo zero.
>
> Ogni riduzione di prezzo *peggiora* la qualità media offerta, il che giustifica un'ulteriore riduzione. È una spirale discendente che non si ferma prima di $p = 0$.

Questa dinamica mostra perché il **prezzo non può svolgere il suo ruolo allocativo** in presenza di asimmetria informativa: quando il prezzo scende, invece di aumentare la quantità domandata, riduce la qualità offerta, peggiorando le condizioni di scambio per i compratori.

---

## Paragone con Mercato a Informazione Perfetta

| Caratteristica | Info Perfetta | Info Asimmetrica |
|---|---|---|
| Prezzo di equilibrio | $q_i \leq p_i \leq \frac{3}{2}q_i$ (range) | $p^* = 0$ |
| Qualità media scambiata | Tutta la distribuzione | Solo $q = 0$ |
| Volume scambi | 100% delle auto | 0% |
| Efficienza | First-best (Pareto ottimale) | Minima possibile |
| Guadagni dallo scambio realizzati | 100% | 0% |

Con informazione perfetta, ogni auto con $0 < q \leq 2$ trova un prezzo che soddisfa entrambe le parti (ogni $p$ in $[q, \frac{3}{2}q]$ va bene). Con asimmetria informativa, nessuno scambio avviene.

---

## Il Ruolo dell'Asimmetria (Non dell'Incompletezza)

Un punto cruciale: il collasso del mercato dipende dall'**asimmetria** dell'informazione, non dalla sua incompletezza.

Supponiamo che anche i *venditori* non conoscano la qualità delle proprie auto. Allora:

$$
E(U_1) = y_1 + (\mu_{\text{tot}} - p)n = y_1 + (1 - p)n
$$

poiché $\mu_{\text{tot}} = 1$ (media della distribuzione uniforme su $[0,2]$).

La nuova regola di vendita diventa: **vendi se $p \geq 1$**.

La regola d'acquisto rimane: **compra se $p \leq \frac{3}{2}\mu = \frac{3}{2}$**.

Se G1 = G2 (tutti i trader sono uguali), l'intero parco auto viene scambiato per $1 \leq p \leq \frac{3}{2}$. **Nessuna selezione avversa** quando l'ignoranza è simmetrica!

> [M] L'inefficienza dipende dall'asimmetria dell'informazione, non dalla sua incompletezza. Supponiamo che anche i venditori non possano osservare la qualità delle proprie auto... Nessuna selezione avversa ora, sebbene ci sia informazione incompleta.

---

## Take-home message

> [!summary]
> L'equilibrio del modello di Akerlof nel piano $(\mu, p)$ mostra graficamente e algebricamente perché il mercato collassa completamente. La curva di offerta ($\mu = \frac{1}{2}p$) è sempre a sinistra della curva di domanda ($\mu = \frac{2}{3}p$), il che significa che per ogni prezzo positivo la qualità media offerta è inferiore alla qualità minima richiesta dai compratori. L'unica intersezione è nell'origine. Crucialmente, il collasso dipende dall'*asimmetria* e non dall'*incompletezza* dell'informazione: se anche i venditori ignorassero la qualità, il mercato funzionerebbe normalmente.

---

## Vedi anche

- [[04_Modello_Akerlof_Formale]] — Derivazione delle curve di offerta e domanda
- [[06_Variazioni_del_Modello]] — Quando il mercato sopravvive parzialmente
- [[07_Inefficienza_e_Implicazioni]] — Le implicazioni normative e i rimedi
- [[08_Distribuzioni_di_Probabilita_Richiamo]] — La matematica della distribuzione uniforme

---

## Connessioni con il Vault

**Da `0. Intro`:**
- [[0. Intro/02_Mercato_e_Hayek|Mercato e Hayek]] — l'equilibrio qui analizzato è l'antitesi dell'equilibrio hayekiano: il meccanismo dei prezzi *fallisce* nell'aggregare l'informazione dispersa, producendo un esito Pareto-inefficiente

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — l'equilibrio $(p=0, \mu=0)$ nel piano $(\mu, p)$ è un NE: dati i comportamenti ottimali di tutti gli agenti, nessuno vuole deviare unilateralmente. Il NE è unico ma Pareto-inferiore
- [[1. GT/04_Giochi_Coordinamento|Giochi di Coordinamento]] — il problema della selezione avversa ha anche la struttura di un problema di coordinamento: se *tutti* i compratori credessero alla qualità alta, si formerebbero le aspettative che sostengono il mercato; ma la mancanza di coordinamento sulle credenze porta all'equilibrio pessimo
