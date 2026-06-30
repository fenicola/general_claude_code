---
tags: [economia-informazione, selezione-avversa, variazioni-modello, robustezza]
aliases: [Conclusioni Meno Estreme, Scambi Positivi, Variazioni Akerlof]
links: [04_Modello_Akerlof_Formale, 05_Equilibrio_di_Mercato_Adverse_Selection, 07_Inefficienza_e_Implicazioni]
---

# Variazioni del Modello: Conclusioni Meno Estreme

## Perché Variare il Modello?

Il modello base di Akerlof produce un risultato drammatico: zero scambi. Nella realtà, i mercati con asimmetria informativa esistono e funzionano — male, sì, ma non si azzera tutto il commercio. È quindi necessario capire in quali condizioni il collasso totale viene attenuato. Le slide presentano due variazioni principali:

- **Caso 1**: diversa funzione di utilità per G2 (maggiore apprezzamento della qualità)
- **Caso 2**: diversa distribuzione di qualità (minimo positivo)

Entrambe le variazioni producono scambi positivi ma inefficienti: il mercato non collassa, ma rimane distante dall'ottimo first-best.

---

## Caso 1: Diversa Funzione di Utilità

### Setup

Supponiamo che la funzione di utilità di G2 sia:

$$
U_2 = M + 3q \cdot n
$$

Il coefficiente passa da $\frac{3}{2}$ a $3$: i compratori valorizzano la qualità il **doppio** rispetto al modello base. Questo può riflettere un'urgenza maggiore nell'acquisto o una maggiore utilità marginale dal possedere un'auto.

### Nuova Regola di Acquisto

Sostituendo nel vincolo di bilancio e prendendo il valore atteso:

$$
E(U_2) = y_2 + [3\mu - p]n
$$

La nuova condizione di acquisto è:

$$
3\mu \geq p \qquad \Longleftrightarrow \qquad \mu \geq \frac{1}{3}p
$$

Questa è la **nuova curva di domanda** nel piano $(\mu, p)$: una retta con pendenza 3 (più ripida rispetto alla pendenza 2 della curva di offerta).

### Confronto delle Pendenze

- **Curva di offerta**: $\mu = \frac{1}{2}p$ (pendenza 2)
- **Nuova curva di domanda**: $\mu = \frac{1}{3}p$ (pendenza 3)
- **Vecchia curva di domanda**: $\mu = \frac{2}{3}p$ (pendenza $\frac{3}{2}$)

Ora la nuova curva di domanda ha pendenza 3 > 2 (la pendenza dell'offerta): la curva di domanda è **più ripida** della curva di offerta. Le due rette si intersecano — ci sono punti in cui la qualità offerta supera la qualità minima richiesta!

### L'Equilibrio

Nel piano $(\mu, p)$, la nuova domanda ($\mu = \frac{1}{3}p$) è a destra dell'offerta ($\mu = \frac{1}{2}p$) per valori di $p$ tra certi limiti. In particolare:

Per $p = 1$: $\mu = \frac{1}{2}$. La condizione di acquisto richiede $\mu \geq \frac{1}{3}$, e $\frac{1}{2} > \frac{1}{3}$ ✓

Per $p = \frac{1}{2}$ e $p = \frac{3}{2}$, le due curve si incrociano, delimitando l'intervallo di equilibri possibili.

**Verifica**: Con $p = 1$, $\mu = \frac{1}{2}$ → $3\mu = \frac{3}{2} > 1 = p$ ✓ (G2 vuole comprare). I venditori offrono tutte le auto con $q \leq 1$ → esiste un equilibrio con scambi positivi.

> [M] Con $p = 1$, $\mu = \frac{1}{2}$ e per $\frac{1}{2} \leq p \leq \frac{3}{2}$ ci sono scambi!

L'equilibrio "di mercato" si trova nell'**area rossa** del grafico: la zona tra le due curve per valori di $p$ nell'intervallo $[\frac{1}{2}, \frac{3}{2}]$. Qui coesistono offerta positiva e domanda positiva.

### Interpretazione

Quando i compratori apprezzano molto la qualità (coefficiente 3 invece di $\frac{3}{2}$), anche una qualità media relativamente bassa giustifica un prezzo positivo. Il mercato non collassa, ma — crucialmente — **rimane inefficiente**: solo le auto di qualità inferiore alla metà del range vengono scambiate.

---

## Caso 2: Diversa Distribuzione di Qualità (Minimo Positivo)

### Setup

Supponiamo ora di tornare alla funzione di utilità originale di Akerlof, ma di modificare la distribuzione di qualità: anziché $q \sim U[0,2]$, si assume:

$$
q \sim U[t, 2] \qquad \text{con } t > 0
$$

Il minimo della distribuzione è ora $t > 0$: non esistono auto di qualità zero. Tutte le auto hanno almeno una qualità base.

### Nuova Funzione di Offerta

Con $q \sim U[t, 2]$:
- La densità è $f(q) = \frac{1}{2-t}$
- Per $p \geq t$, la qualità media delle auto offerte è la media di $U[t, p]$:

$$
\mu = \frac{t + p}{2} \qquad \text{per } t \leq p \leq 2
$$

La nuova curva di offerta è una retta parallela alla vecchia ma traslata verso l'alto di $\frac{t}{2}$: passa per il punto $(\frac{t}{2}, t)$ invece che per l'origine.

### Confronto con il Modello Base

| Caratteristica | Modello base ($t=0$) | Modello con $t>0$ |
|---|---|---|
| Distribuzione | $U[0,2]$ | $U[t,2]$ |
| Curva di offerta | $\mu = \frac{p}{2}$ | $\mu = \frac{t+p}{2}$ |
| Curva di domanda | $\mu = \frac{2}{3}p$ | $\mu = \frac{2}{3}p$ (invariata) |
| Equilibrio | $p = 0$ | $p \in [t, 3t]$ |

### L'Equilibrio con $t > 0$

La condizione di equilibrio è: la qualità media offerta soddisfa la condizione di acquisto.

Dalla curva di domanda: $\mu = \frac{2}{3}p$. Dalla curva di offerta: $\mu = \frac{t+p}{2}$.

Eguagliando: $\frac{t+p}{2} = \frac{2p}{3}$, ovvero $3(t+p) = 4p$, da cui $p = 3t$.

Ma c'è anche un limite inferiore: i venditori vendono solo se $p \geq t$ (il prezzo deve almeno coprire la qualità minima). Dunque l'intervallo di equilibri è $t \leq p \leq 3t$.

**Esempio**: se $t = 0,5$, l'equilibrio esiste per $p \in [0,5; 1,5]$.

La **traslazione verso l'alto** della curva di offerta (dovuta al fatto che la qualità minima è $t > 0$ invece di 0) crea una zona di sovrapposizione tra le regioni di offerta positiva e domanda positiva nel piano $(\mu, p)$.

> [M] Con minimo $t > 0$: densità $\frac{1}{2-t}$ e qualità media $\mu = \frac{t}{2} + \frac{p}{2}$ per $p \geq t$. La domanda è positiva per $(3/2)\mu > p$, vero per $t \leq p \leq 3t$ (consistente con $p > 0$ dato che $t > 0$).

---

## Confronto dei Tre Scenari

| Scenario | Condizione | Equilibrio | Efficienza |
|---|---|---|---|
| Modello base | $U_2 = M + \frac{3}{2}qn$, $q \sim U[0,2]$ | Zero scambi ($p = 0$) | Massima inefficienza |
| Caso 1: Utilità alta | $U_2 = M + 3qn$, $q \sim U[0,2]$ | Scambi per $p \in [\frac{1}{2}, \frac{3}{2}]$ | Parzialmente inefficiente |
| Caso 2: Min positivo | $U_2 = M + \frac{3}{2}qn$, $q \sim U[t,2]$ | Scambi per $p \in [t, 3t]$ | Parzialmente inefficiente |

In tutti i casi con scambi positivi, rimane una **inefficienza**: le auto di alta qualità non vengono scambiate, pur essendo valorizzate di più dai compratori rispetto ai venditori.

---

## Cosa Determina Se Il Mercato Collassa?

Dalla comparazione dei due casi emerge una regola intuitiva:

> [!intuition]
> Il mercato collassa completamente quando la "curva di offerta" nel piano $(\mu, p)$ è sempre a sinistra della "curva di domanda" per ogni $p > 0$. Questo accade quando:
> 1. I compratori non apprezzano abbastanza la qualità (basso coefficiente nella funzione di utilità), oppure
> 2. La distribuzione di qualità parte da zero (non c'è un minimo positivo garantito)
>
> Se i compratori apprezzano molto la qualità *o* se la qualità minima è positiva, esiste un margine in cui scambiarsi i beni conviene a entrambi.

---

## Take-home message

> [!summary]
> Il collasso totale del mercato non è una conclusione universale della teoria della selezione avversa: dipende dalle ipotesi specifiche sul grado di apprezzamento della qualità da parte dei compratori e sulla distribuzione di qualità. Se i compratori valorizzano molto la qualità (Caso 1) o se la distribuzione di qualità ha un minimo positivo (Caso 2), il mercato sopravvive parzialmente. In entrambi i casi, però, l'esito rimane inefficiente rispetto al benchmark di informazione perfetta: le auto di alta qualità rimangono invendute nonostante esistano potenziali guadagni dallo scambio. La selezione avversa non deve essere necessariamente "totale" per essere economicamente rilevante e welfare-riducente.

---

## Vedi anche

- [[04_Modello_Akerlof_Formale]] — Il modello base da cui si parte
- [[05_Equilibrio_di_Mercato_Adverse_Selection]] — L'equilibrio di zero scambi nel dettaglio
- [[07_Inefficienza_e_Implicazioni]] — Implicazioni e rimedi
- [[08_Distribuzioni_di_Probabilita_Richiamo]] — La matematica delle distribuzioni

---

## Connessioni con il Vault

**Da `0. Intro`:**
- [[0. Intro/05_Selezione_avversa|Selezione avversa — Introduzione]] — questa nota approfondisce il punto accennato nell'introduzione: la selezione avversa non porta *sempre* al collasso totale; dipende dai parametri

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — i "casi 1 e 2" di questa nota producono equilibri di Nash *diversi* (mercato parzialmente attivo) rispetto al caso Akerlof base (mercato vuoto); i NE multipli nell'equilibrio parziale rispecchiano la struttura dei [[1. GT/04_Giochi_Coordinamento|Giochi di Coordinamento]]
- [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]] — la reputazione come rimedio alla selezione avversa (citata in [[07_Inefficienza_e_Implicazioni]]) funziona esattamente come la cooperazione nei giochi ripetuti: il valore futuro deve essere abbastanza alto (fattore di sconto $\delta$ alto) da rendere la qualità conveniente
