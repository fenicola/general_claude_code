---
tags: [economia-informazione, selezione-avversa, wilson, equilibri-multipli, pareto]
aliases: [Modello di Wilson, Equilibri Multipli Selezione Avversa, Wilson 1980]
links: [04_Modello_Akerlof_Formale, 05_Equilibrio_di_Mercato_Adverse_Selection, 07_Inefficienza_e_Implicazioni]
---

# Il Modello di Wilson: Equilibri Multipli e Pareto-Dominanza

## Oltre Akerlof: Ipotesi Più Generali

Il modello di Akerlof (1970), analizzato in [[04_Modello_Akerlof_Formale]], raggiunge conclusioni molto nette grazie a ipotesi molto specifiche: preferenze simmetriche per compratori e venditori, qualità distribuita uniformemente, e un unico rapporto MRS ($t = 3/2$) uguale per tutti i compratori. Wilson (1980) rilassa queste ipotesi e ottiene un quadro molto più ricco e, per certi versi, più realistico.

> [!definition]
> Il **Modello di Wilson (1980)** è un'estensione del modello di Akerlof che, rilassando le ipotesi sulle preferenze degli acquirenti e sulla distribuzione della qualità, mostra l'esistenza di **equilibri multipli Pareto-ordinabili** nel mercato con selezione avversa. In particolare, Wilson dimostra che (a) possono coesistere più equilibri di mercato, (b) questi equilibri sono ordinabili secondo il criterio di Pareto, e (c) i prezzi possono stabilizzarsi *al di sopra* del livello che svuoterebbe il mercato, generando un eccesso permanente di offerta.

[M, ch. 3]

---

## La Struttura del Modello

### Il Lato dell'Offerta (Venditori)

Come in Akerlof, il mercato ha uno stock di auto la cui qualità $q$ è descritta da una funzione di densità $f(q)$ con minimo $q_1$ e massimo $q_2$. La funzione di utilità dei venditori è:

$$U_S = M + q \cdot n$$

soggetta al vincolo di bilancio $Y = M + p \cdot n$. La **regola di vendita ottimale** rimane la stessa del modello base:

$$\text{Vendi se e solo se } p \geq q$$

Questo implica che quando il prezzo sale, la qualità marginale del venditore indotto a vendere sale anch'essa: un prezzo più alto attrae auto di qualità crescente.

### Il Lato della Domanda (Compratori)

Qui Wilson introduce la variazione cruciale. La funzione di utilità dei compratori è:

$$U_B = M + t \cdot q \cdot n$$

dove $t$ è il **saggio marginale di sostituzione** (MRS) tra qualità dell'auto e altri beni. In Akerlof, $t = 3/2$ era uguale per tutti i compratori. Wilson assume invece che $t$ sia eterogeneo: distribuito tra un minimo $t_1$ e un massimo $t_2$ secondo una funzione di densità $h(t)$. **Alcuni compratori valorizzano la qualità molto più di altri.**

Sostituendo il vincolo di bilancio $M = Y - p \cdot n$ nella funzione di utilità:

$$U_B = Y + (t \cdot q - p) \cdot n$$

Poiché i compratori conoscono solo la qualità media $\mu = \mu(p)$ — che dipende dal prezzo attraverso il meccanismo di selezione avversa — l'utilità attesa è:

$$E(U_B) = Y + (t \cdot \mu(p) - p) \cdot n$$

La **regola d'acquisto ottimale** è:

$$\text{Acquista se e solo se } t \cdot \mu(p) \geq p$$

Intuitivamente: il compratore acquista se il valore soggettivo della qualità media ottenibile ($t \cdot \mu(p)$) supera il prezzo pagato ($p$).

> [!intuition]
> Il parametro $t$ rappresenta quanto un compratore è disposto a pagare per unità di qualità. Un compratore con $t$ alto valuta molto la qualità: è più disposto ad acquistare anche a prezzi elevati. Questo crea un meccanismo interessante: quando il prezzo sale, escono dal mercato i compratori con $t$ basso (non giustificano il prezzo elevato), ma entrano potenzialmente compratori con $t$ alto. La composizione della domanda dipende dal prezzo.

---

## La Curva di Domanda Inclinata Positivamente

Nel modello standard (beni omogenei), la curva di domanda è inclinata negativamente: a prezzi più alti, meno persone comprano. Nel modello di Wilson, la domanda può essere **inclinata positivamente** per due ragioni combinate:

**Condizione (a):** La qualità media $\mu(p)$ cresce *più velocemente* del prezzo $p$. In questo caso, il beneficio dell'acquisto $t \cdot \mu(p)$ cresce più rapidamente del suo costo $p$, rendendo l'acquisto più conveniente all'aumentare del prezzo.

**Condizione (b):** Ci sono abbastanza compratori con un MRS sufficientemente alto ($t$ grande) che entrano nel mercato quando il prezzo (e la qualità) salgono. Se il numero di nuovi entranti è sufficiente, la domanda *totale* può aumentare all'aumentare del prezzo.

> [!intuition]
> Questo è il momento cruciale in cui il mercato con asimmetria informativa si comporta in modo radicalmente diverso da un mercato standard. Nei mercati convenzionali, la qualità è presa come data (ceteris paribus) nell'analisi della domanda. Qui, la qualità non è una costante ma una funzione del prezzo: $\mu = \mu(p)$. Aumentare il prezzo non solo aumenta il costo per il compratore, ma *cambia il prodotto che ottiene*, attraendo auto migliori. Se il secondo effetto domina il primo, la domanda è crescente nel prezzo.

[M, ch. 3]

---

## Equilibri Multipli: A, B, C

Quando entrambe le condizioni (a) e (b) sono soddisfatte, la curva di domanda $D(p)$ è inclinata positivamente, come la curva di offerta $S(p)$. Due curve crescenti possono intersecarsi più volte, generando **equilibri multipli**.

Nelle slide della lezione, i tre equilibri sono etichettati A, B e C, con $p_A < p_B < p_C$ e $Q_A < Q_B < Q_C$. A è l'equilibrio a basso prezzo e bassa qualità; C è l'equilibrio ad alto prezzo e alta qualità.

La domanda naturale è: questi equilibri sono ordinabili? C'è uno migliore degli altri?

---

## Pareto-Dominanza: C Domina B Domina A

### Per i Venditori

Passando da A a B, e poi da B a C:
1. I venditori che vendevano già guadagnano di più per le stesse auto (prezzo più alto).
2. Nuovi venditori con auto di qualità superiore entrano nel mercato (prima non vendevano).

Entrambi i gruppi stanno meglio: il criterio di Pareto è soddisfatto per il lato dell'offerta.

### Per i Compratori

L'analisi dei compratori è più sofisticata e richiede di guardare le **curve di indifferenza** nello spazio $(µ, p)$.

L'utilità attesa di un compratore che acquista ($n=1$) è:
$$E(U_B) = Y + (t \cdot \mu - p)$$

Le curve di indifferenza in questo spazio sono **rette con pendenza $t$**: per mantenere la stessa utilità, se il prezzo sale di $\Delta p$, la qualità deve salire di $\Delta \mu = \Delta p / t$. I compratori preferiscono le curve di indifferenza più a *destra* nello spazio $(\mu, p)$ (più qualità a parità di prezzo).

Un compratore che non acquista ($n=0$) si trova all'origine $(0,0)$. La soglia di partecipazione è la curva di indifferenza che passa per l'origine: il compratore entra nel mercato quando $t \cdot \mu(p) \geq p$, ovvero quando il punto $(\mu(p), p)$ si trova a destra della sua curva di indifferenza di riserva $IC_m$.

Passando da B a C, i compratori si dividono in tre categorie:
1. **Compratori che acquistavano in B e acquistano ancora in C**: stanno meglio o uguali (la qualità è aumentata e la loro utilità sale o rimane invariata a seconda del rapporto tra aumento di prezzo e aumento di qualità).
2. **Compratori marginali in B che ora acquistano in C** (i "marginal buyers" entrano al prezzo di C): stanno meglio di prima (erano indifferenti a B, ora sono nel mercato e ottengono surplus).
3. **Compratori che non acquistavano in B e non acquistano in C**: invariati.

> [!summary]
> Nessun compratore sta peggio passando da B a C. Molti stanno meglio. **C Pareto-domina B**, che a sua volta **Pareto-domina A**. Gli equilibri sono Pareto-ordinabili, con C come equilibrio migliore.

[M, ch. 3]

---

## Il Prezzo di Eccesso d'Offerta: Perché il Mercato Può Bloccarsi

Un risultato sorprendente del modello di Wilson è che **il prezzo di mercato può superare il livello che svuoterebbe il mercato** (il prezzo market-clearing). Questo accade perché sia venditori che compratori potrebbero preferire un prezzo più alto, anche se ciò implica un eccesso di offerta e il razionamento di alcuni venditori.

Consideriamo cosa succede quando il prezzo sale oltre $p_C$ fino a $p^*$:

- **Per i compratori**: la curva $\mu(p)$ continua a salire con il prezzo, portando a una qualità media ancora più alta. Molti compratori si trovano su curve di indifferenza *più alte* che a $p_C$: stanno meglio.
- **Per i venditori**: il prezzo più alto è desiderabile, ma non tutti riescono a vendere (eccesso di offerta). Alcuni venditori vengono razionati.

La logica è che un venditore in eccesso d'offerta affronta un **trade-off** tra prezzo più alto e minore probabilità di vendere. Se il guadagno atteso da un prezzo più alto compensa la probabilità di restare invenduto, il mercato può rimanere stabilmente in una situazione di eccesso d'offerta.

> [!intuition]
> Questo risultato è controintuitivo rispetto alla teoria standard. Normalmente, un eccesso di offerta porta a una riduzione del prezzo fino all'equilibrio. Ma qui, il *taglio* del prezzo *peggiorerebbe* la qualità media, scoraggiando i compratori e peggiorando la situazione di tutti. Il mercato può restare "bloccato" in un eccesso d'offerta perché nessun agente individuale ha l'incentivo a ridurre il prezzo.

---

## Sintesi: Akerlof vs. Wilson

| Dimensione | Akerlof | Wilson |
|---|---|---|
| Preferenze compratori | $t = 3/2$ per tutti | $t$ eterogeneo, distribuito in $[t_1, t_2]$ |
| Numero di equilibri | Unico (zero-trade) | Potenzialmente multipli (A, B, C) |
| Ordinabilità degli equilibri | N/A | Pareto-ordinabili: C > B > A |
| Eccesso d'offerta | Assente | Possibile come equilibrio stabile |
| Direzione della curva di domanda | Decrescente in p | Può essere crescente in p |

> [!summary]
> Il modello di Wilson mostra che i risultati catastrofici di Akerlof (collasso totale del mercato) sono un caso limite, non necessariamente la norma. Quando le preferenze sono eterogenee, possono emergere equilibri multipli ordinabili secondo Pareto. Il mercato con selezione avversa non collassa necessariamente, ma può stabilizzarsi a livelli diversi di prezzo e qualità — tutti migliori se più alti. Paradossalmente, sia venditori che compratori possono preferire prezzi più alti di quelli che svuoterebbero il mercato, anche al costo di un eccesso d'offerta e del razionamento di alcuni venditori.

---

## Vedi Anche

- [[04_Modello_Akerlof_Formale]] — Le ipotesi più restrittive che Wilson rilassa
- [[05_Equilibrio_di_Mercato_Adverse_Selection]] — L'equilibrio di zero-scambio di Akerlof
- [[07_Inefficienza_e_Implicazioni]] — I rimedi istituzionali alla selezione avversa
- [[10_Malpractice_Medica_Selezione_Avversa]] — Applicazione empirica della selezione avversa nel mercato medico

---

## Connessioni con il Vault

**Da `0. Intro`:**
- [[0. Intro/05_Selezione_avversa|Selezione avversa — Introduzione]] — questa nota corrisponde all'"Estensione del modello" accennata nell'introduzione: Wilson mostra che il collasso totale non è l'unico esito possibile

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — gli equilibri multipli A, B, C del modello Wilson sono tutti NE del gioco: in ognuno, nessun agente vuole deviare dati i comportamenti altrui. Il problema è che esistono *troppi* NE e la teoria dei giochi da sola non dice quale si realizzerà
- [[1. GT/04_Giochi_Coordinamento|Giochi di Coordinamento]] — la molteplicità di equilibri Pareto-ordinabili è la caratteristica tipica dei giochi di coordinamento (es. Stag Hunt): tutti preferiscono l'equilibrio B a A, e C a B, ma senza coordinamento il mercato può bloccarsi nell'equilibrio peggiore
- [[1. GT/08_Giochi_Ripetuti_Finiti|Giochi Ripetuti Finiti]] — l'eccesso d'offerta permanente a prezzi alti (tratto caratteristico dell'equilibrio C) può essere sostenuto solo in un contesto ripetuto o con impegno; in un gioco one-shot puro, la pressione competitiva spingerebbe verso il market-clearing
