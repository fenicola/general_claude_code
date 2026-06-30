---
tags: [economia-informazione, matematica, distribuzioni-probabilita, ripasso]
aliases: [Distribuzione Uniforme, Probabilità Continua, Ripasso Probabilità]
links: [03_Modello_Formale_Due_Qualita, 04_Modello_Akerlof_Formale, 05_Equilibrio_di_Mercato_Adverse_Selection]
---

# Ripasso: Distribuzioni di Probabilità

## Perché Questo Ripasso?

Il modello di Akerlof sul mercato dei limoni usa la **distribuzione uniforme** in modo cruciale: la qualità media delle auto offerte a un dato prezzo si calcola come media condizionata di una distribuzione uniforme. Comprendere i concetti di base delle distribuzioni di probabilità è essenziale per seguire la matematica dei modelli.

---

## Distribuzione Discreta: Due Tipi

Il caso più semplice è quello con soli due valori possibili. Supponiamo che esistano auto di qualità $q = 1$ (bassa) e $q = 2$ (alta).

Se la probabilità di scegliere a caso un'auto di qualità 1 è $\rho$ e di qualità 2 è $(1-\rho)$, con:

$$
\rho + (1-\rho) = 1
$$

La distribuzione è completamente descritta da un solo numero $\rho$. Graficamente si rappresenta come due barre verticali di altezza $\rho$ e $(1-\rho)$ rispettivamente.

Nel modello di BB (cap. 13), si assume $\rho = \frac{1}{2}$: metà delle auto vale \$5.000, metà vale \$10.000. La qualità media è:

$$
\mu = \rho \cdot 5.000 + (1-\rho) \cdot 10.000 = \frac{1}{2} \cdot 5.000 + \frac{1}{2} \cdot 10.000 = 7.500
$$

---

## Distribuzione Discreta: Più Tipi

Con quattro valori possibili ($q = 0.5, 1, 1.5, 2$) e probabilità $\rho_1, \rho_2, \rho_3, \rho_4$:

$$
\rho_1 + \rho_2 + \rho_3 + \rho_4 = 1
$$

La qualità media è:

$$
\mu = 0.5\rho_1 + 1\cdot\rho_2 + 1.5\rho_3 + 2\rho_4
$$

Il passaggio a una distribuzione continua è il limite naturale di questo processo quando i valori possibili diventano infinitamente fini.

---

## Distribuzione Continua: La Densità di Probabilità

Quando la qualità $q$ può assumere qualsiasi valore reale in un intervallo, si usa una **funzione di densità di probabilità** $f(q)$.

La probabilità che la qualità cada in un intervallo $[a, b]$ è l'**area** sotto la curva di densità in quell'intervallo:

$$
P(a \leq q \leq b) = \int_a^b f(q) \, dq
$$

Due proprietà fondamentali:
1. $f(q) \geq 0$ per ogni $q$ (la densità è non negativa)
2. $\int_{-\infty}^{+\infty} f(q) \, dq = 1$ (la probabilità totale è 1)

> [!intuition]
> La densità non è direttamente una probabilità (può superare 1!). È la "concentrazione" di probabilità in un punto. La probabilità si ottiene come area, non come altezza.

---

## La Distribuzione Uniforme

> [!definition]
> La **distribuzione uniforme** su $[a, b]$ assegna uguale probabilità a ogni valore nell'intervallo. La funzione di densità è:
>
> $$f(q) = \frac{1}{b-a} \qquad \text{per } a \leq q \leq b$$
>
> La densità è **costante**: graficamente, la distribuzione è un rettangolo di base $(b-a)$ e altezza $\frac{1}{b-a}$, con area totale = 1.

Per la distribuzione uniforme su $[0, 2]$ (il caso di Akerlof):

$$
f(q) = \frac{1}{2-0} = \frac{1}{2} \qquad \text{per } 0 \leq q \leq 2
$$

Verifica: $\int_0^2 \frac{1}{2} \, dq = \frac{1}{2} \cdot 2 = 1$ ✓

**Media** della distribuzione uniforme su $[0, 2]$:

$$
\mu_{\text{tot}} = \int_0^2 q \cdot \frac{1}{2} \, dq = \frac{1}{2} \cdot \left[\frac{q^2}{2}\right]_0^2 = \frac{1}{2} \cdot 2 = 1
$$

---

## Probabilità di Scegliere un'Auto con $q \leq p$

Se $q \sim U[0, 2]$ e il venditore vende solo se $q \leq p$ (per $p \leq 2$):

La probabilità che un'auto scelta a caso abbia $q \leq p$ è l'area del rettangolo fino a $p$:

$$
P(q \leq p) = \int_0^p \frac{1}{2} \, dq = \frac{p}{2}
$$

Questo significa che se il prezzo offerto è $p = 1$, la metà del parco auto ($\frac{1}{2}$) verrà offerta in vendita. Se $p = 0.4$, solo il $20\%$ delle auto ($\frac{0.4}{2} = 0.2$) viene offerto.

---

## Qualità Media Condizionata: La Formula Chiave

La formula più importante per il modello di Akerlof è la **qualità media condizionata** alle auto effettivamente offerte:

$$
\mu = E[q \,|\, q \leq p] = \frac{\int_0^p q \cdot f(q) \, dq}{P(q \leq p)}
$$

Per $q \sim U[0,2]$:

$$
\mu = \frac{\int_0^p q \cdot \frac{1}{2} \, dq}{\frac{p}{2}} = \frac{\frac{1}{2} \cdot \frac{p^2}{2}}{\frac{p}{2}} = \frac{\frac{p^2}{4}}{\frac{p}{2}} = \frac{p}{2}
$$

> [!intuition]
> Il risultato $\mu = \frac{p}{2}$ ha un'interpretazione geometrica immediata: se si prendono solo le auto con $q \leq p$ (distribuite uniformemente su $[0, p]$), la loro qualità media è il punto di mezzo dell'intervallo $[0, p]$, cioè $\frac{p}{2}$. Sempre la metà del prezzo massimo accettato.

---

## Qualità Media Condizionata per $U[t, 2]$

Per la distribuzione uniforme su $[t, 2]$ con $t > 0$ (la variazione del Caso 2 in [[06_Variazioni_del_Modello]]):

- Densità: $f(q) = \frac{1}{2-t}$ per $t \leq q \leq 2$
- Per $p \in [t, 2]$, la qualità media delle auto offerte (con $q \in [t, p]$) è:

$$
\mu = E[q \,|\, t \leq q \leq p] = \frac{t + p}{2}
$$

Questo perché $q$ condizionato a $q \in [t, p]$ è uniformemente distribuito su $[t, p]$, con media $\frac{t+p}{2}$.

La differenza con il caso base è che ora $\mu \geq \frac{t}{2} > 0$ anche per prezzi bassi: c'è sempre una qualità minima garantita.

---

## Esempio Numerico Completo

Supponiamo $q \sim U[0, 2]$ e il compratore offre $p = 1{,}2$.

1. **Quali auto vengono offerte?** Tutte quelle con $q \leq 1{,}2$ (le auto più scadenti, che il venditore è disposto a cedere a quel prezzo).

2. **Quante auto?** Quota $= \frac{p}{2} = \frac{1{,}2}{2} = 0{,}6$, cioè il 60% del parco auto.

3. **Qual è la qualità media?** $\mu = \frac{p}{2} = \frac{1{,}2}{2} = 0{,}6$.

4. **Il compratore accetta?** Condizione: $\frac{3}{2}\mu \geq p$, ovvero $\frac{3}{2} \cdot 0{,}6 = 0{,}9 < 1{,}2$. **No**: il valore atteso (0,9) è inferiore al prezzo (1,2). Il compratore non acquista.

5. **E se il compratore usa la nuova funzione di utilità** ($U_2 = M + 3qn$)? La condizione diventa $3\mu \geq p$, ovvero $3 \cdot 0{,}6 = 1{,}8 > 1{,}2$. **Sì**: il compratore acquista!

---

## Distribuzione Uniforme: Riassunto

| Caratteristica | Distribuzione $U[a,b]$ | Caso Akerlof $U[0,2]$ |
|---|---|---|
| Densità | $\frac{1}{b-a}$ | $\frac{1}{2}$ |
| Media | $\frac{a+b}{2}$ | $1$ |
| Probabilità $q \leq p$ | $\frac{p-a}{b-a}$ | $\frac{p}{2}$ |
| Media condizionata $E[q\|q\leq p]$ | $\frac{a+p}{2}$ | $\frac{p}{2}$ |

---

## Take-home message

> [!summary]
> La distribuzione uniforme è scelta da Akerlof per la sua semplicità: la qualità media condizionata alle auto offerte ($\mu = \frac{p}{2}$) è semplicemente la metà del prezzo di taglio. Questo rende la matematica del modello trasparente. Il risultato cruciale — la curva di offerta nel piano $(\mu, p)$ ha equazione $\mu = \frac{1}{2}p$ — deriva direttamente dalla simmetria della distribuzione uniforme. Con una distribuzione diversa (es. $U[t,2]$), la formula cambia ma la logica rimane la stessa: la qualità media offerta aumenta col prezzo, ma sempre più lentamente di quanto richieda la domanda.

---

## Vedi anche

- [[03_Modello_Formale_Due_Qualita]] — Il caso discreto con due sole qualità
- [[04_Modello_Akerlof_Formale]] — Come la distribuzione uniforme entra nel modello
- [[05_Equilibrio_di_Mercato_Adverse_Selection]] — Come $\mu = p/2$ porta al collasso del mercato
- [[06_Variazioni_del_Modello]] — Il caso $U[t,2]$ e la sua diversa curva di offerta

---

## Connessioni con il Vault

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — le distribuzioni di probabilità sono lo strumento con cui si modellano le *strategie miste* nei giochi (ogni strategia mista è una distribuzione su strategie pure); la distribuzione uniforme della qualità nel modello Akerlof è analoga alla randomizzazione di un giocatore in un equilibrio misto
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — nei giochi bayesiani con informazione incompleta (come quelli di segnalazione), le distribuzioni di probabilità sono le *beliefs* dei giocatori; la distribuzione uniforme $U[0,2]$ rappresenta le credenze a priori del compratore sulla qualità del venditore
