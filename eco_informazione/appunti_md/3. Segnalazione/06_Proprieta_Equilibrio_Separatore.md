---
tags: [economia-informazione, segnalazione, equilibri-multipli, pareto, esternalita]
aliases: [Proprietà Equilibrio Separatore, Pareto Ranking Segnalazione, Esternalità Educazione]
links: [05_Equilibrio_Separatore, 04_Esempio_Numerico_Casi_Base, 07_Equilibrio_Aggregante_Pooling]
---

# Proprietà dell'Equilibrio Separatore

L'intervallo $1 \le y^* \le 2$ trovato in [[05_Equilibrio_Separatore]] non è un dettaglio tecnico: implica una serie di proprietà economiche profonde e in parte sorprendenti (slide 31–34).

---

## 1. È un Equilibrio Separatore (il segnale è informativo)

> [!definition]
> Gli H e gli L vengono **riconosciuti e trattati diversamente**. Il segnale $y$ è informativo e ciascun tipo è pagato secondo la propria produttività: $w_H = 2$, $w_L = 1$. È la proprietà che dà il nome all'equilibrio.

---

## 2. Molteplicità degli Equilibri

> [!definition]
> Esistono **infiniti equilibri separatori**: qualunque soglia $1 \le y^* \le 2$, dato il credo dei datori, ne sostiene uno. Non c'è un'unica soglia "naturale".

Questa indeterminatezza è la firma dei modelli di segnalazione (già vista negli esiti del [[03_Modello_di_Spence]]) e rimanda al problema di coordinamento sulle aspettative.

---

## 3. Gli Equilibri Sono Pareto-Ordinabili

> [!definition]
> Gli equilibri separatori sono **Pareto-ordinabili**: più $y^*$ è vicino a $2$, **peggiore** è la condizione dei tipi H; i tipi L restano *invariati* (prendono comunque $w=1$ con $y=0$).

Il motivo è diretto: il rendimento netto di H è $2 - y^*/2$, **decrescente in $y^*$**. Soglie più alte costringono gli H a **sovra-investire** in istruzione, sprecando risorse senza alcun beneficio aggiuntivo (il salario resta $2$).

> [!intuition]
> Ne segue che $y^* = 1$ (la soglia minima) è l'equilibrio **Pareto-dominante** tra i separatori: minimizza il costo di istruzione sostenuto dagli H, lasciando gli L indifferenti. Tutti gli altri equilibri separatori sono Pareto-inferiori a questo. È un esempio in cui "meno segnale possibile" è socialmente preferibile.

$$
\text{Rendimento netto di } H = 2 - \frac{y^*}{2} \quad\Longrightarrow\quad y^*=1:\ 1{,}5 \;>\; y^*=2:\ 1
$$

---

## 4. Il Risultato Non Dipende dalla Quota $q$

> [!definition]
> L'esistenza dell'equilibrio separatore vale **per ogni valore positivo di $q$**: la proporzione di tipi L e H nella popolazione non entra nelle condizioni $1\le y^* \le 2$.

Questo perché nel separatore ciascuno è pagato *individualmente* alla propria produttività: la composizione della popolazione è irrilevante. (Contrasto con il [[07_Equilibrio_Aggregante_Pooling|pooling]] e con il Caso B, dove invece $q$ è centrale via $w=2-q$.)

---

## 5. L'Informazione Completa Pareto-Domina Tutti i Separatori

> [!definition]
> La soluzione a **informazione completa** (Caso A) **Pareto-domina** tutti gli equilibri separatori ad informazione asimmetrica: i salari sono gli stessi ($w_L=1$, $w_H=2$), ma **non ci sono costi di segnalazione**.

> [!intuition]
> Questo è il punto critico per la valutazione di benessere: la segnalazione **non crea valore**, lo *sposta* — e nel farlo brucia risorse reali (gli anni di istruzione segnaletica degli H). Rispetto al mondo ideale in cui la produttività è osservabile, l'equilibrio separatore è sempre peggiore di una quantità pari a $c_H(y^*)$ per ogni H. La segnalazione è un costo che l'asimmetria informativa impone alla società.

---

## 6. L'Istruzione Genera Esternalità Negative

> [!definition]
> Nell'equilibrio separatore l'istruzione produce **esternalità negative** (slide 33): gli H investono, ne traggono un beneficio privato (salario più alto), ma con ciò **impongono un salario più basso agli L**. L'**output totale dell'economia non cambia** (la produttività è fissa): si tratta di pura redistribuzione, ottenuta consumando risorse.

> [!intuition]
> È la stessa struttura del consumo posizionale ([[10_Easterlin_e_Treadmill_Positional]]): il mio segnale costoso migliora la mia posizione *relativa* a spese degli altri, senza accrescere la "torta" complessiva. La segnalazione è un gioco a somma (quasi) zero in cui però si bruciano risorse per giocarlo.

---

## 7. La Non-Segnalazione Può Pareto-Dominare *Alcuni* Separatori

Il risultato più controintuitivo (slide 33–34): l'equilibrio **senza segnalazione** (Caso B, $w=2-q$ per tutti) può essere *migliore* di alcuni equilibri separatori.

### I tipi L stanno meglio senza segnalazione

Nel Caso B l'L riceve $w = 2-q$; nel separatore riceve $w=1$. Quindi:

$$
2 - q > 1 \;\Longleftrightarrow\; q < 1
$$

che è **sempre vero** (la quota è una frazione). Dunque **gli L preferiscono sempre la non-segnalazione**: lì sono sussidiati dagli H, qui sono "smascherati" e pagati solo $1$.

### Anche i tipi H possono stare meglio senza segnalazione

Nel Caso B l'H riceve $2-q$ (nessun costo); nel separatore ottiene rendimento netto $2 - y^*/2$. L'H preferisce la non-segnalazione se:

$$
2 - q > 2 - \frac{y^*}{2} \;\Longleftrightarrow\; \boxed{y^* > 2q}
$$

> [!intuition]
> Quando la soglia richiesta $y^*$ è alta (superiore a $2q$) e/o la quota di L è bassa (poco da guadagnare nel separarsi), **i costi di segnalazione superano i benefici** anche per gli H. In tal caso *tutti* — L e H — preferirebbero un mondo senza segnali. La segnalazione, da rimedio, diventa una trappola collettiva.

### I datori sono sempre indifferenti

In concorrenza i datori fanno **profitti attesi nulli in ogni equilibrio** (separatore, pooling, no-signalling): per loro è indifferente.

> [!example]
> Con $q = 0{,}3$: la non-segnalazione dà $w = 1{,}7$ a tutti. Un separatore con $y^* = 0{,}7$ non esisterebbe (serve $y^*\ge1$); ma confrontando con $y^*=1$, l'H nel separatore ottiene $2 - 0{,}5 = 1{,}5 < 1{,}7$: l'H starebbe **meglio senza segnalare** (infatti $y^*=1 > 2q = 0{,}6$). Qui la non-segnalazione Pareto-domina l'equilibrio separatore con $y^*=1$.

---

## Quadro Riassuntivo delle Proprietà

| # | Proprietà | Implicazione |
|---|---|---|
| 1 | Separatore | Segnale informativo, $w$ = produttività |
| 2 | Molteplicità | Ogni $y^* \in [1,2]$ è un equilibrio |
| 3 | Pareto-ranking | $y^*=1$ domina; $y^*\to2$ danneggia H |
| 4 | Indipendenza da $q$ | Le condizioni non dipendono dalla composizione |
| 5 | Dominanza info completa | Stessi salari, ma senza spreco di segnalazione |
| 6 | Esternalità negative | H danneggia L; output invariato |
| 7 | No-signalling può dominare | Se $y^*>2q$, tutti preferirebbero non segnalare |

---

## Take-home message

> [!summary]
> L'equilibrio separatore esiste per ogni $1\le y^*\le2$, generando **molteplici equilibri Pareto-ordinabili**: $y^*=1$ è il migliore (minimo spreco), valori più alti danneggiano gli H costringendoli a sovra-investire. Il risultato è indipendente da $q$, perché ciascuno è pagato individualmente. La **segnalazione non crea valore**: l'informazione completa domina sempre (stessi salari, nessun costo) e l'istruzione produce **esternalità negative** (gli H abbassano il salario degli L senza accrescere l'output). Il risultato più sorprendente è che la **non-segnalazione può Pareto-dominare alcuni separatori**: gli L preferiscono sempre il Caso B ($q<1$), e gli H lo preferiscono quando $y^*>2q$. La segnalazione, da rimedio all'asimmetria, può trasformarsi in spreco collettivo.

---

## Vedi anche

- [[05_Equilibrio_Separatore]] — La derivazione dell'intervallo $1\le y^*\le 2$
- [[04_Esempio_Numerico_Casi_Base]] — Il Caso B ($w=2-q$) usato per i confronti
- [[07_Equilibrio_Aggregante_Pooling]] — L'esito alternativo
- [[10_Easterlin_e_Treadmill_Positional]] — Le stesse esternalità negative nel consumo posizionale

---

## Connessioni con il Vault

**Da `1. GT`:**
- [[1. GT/04_Giochi_Coordinamento|Giochi di Coordinamento]] — la molteplicità di equilibri Pareto-ordinabili è un problema di coordinamento: quale $y^*$ si realizza dipende dalle aspettative condivise, non dalla teoria
- [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]] — l'esternalità negativa e il caso in cui "tutti preferirebbero non segnalare" hanno la struttura di un PD: l'equilibrio (segnalare) è individualmente razionale ma collettivamente subottimo

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/09_Modello_Wilson_Equilibri_Multipli|Modello di Wilson]] — anche lì equilibri multipli Pareto-ordinabili; stesso tema della non-unicità dell'equilibrio
- [[2. Selezione Avversa/07_Inefficienza_e_Implicazioni|Inefficienza]] — la segnalazione come rimedio *imperfetto*: riduce l'asimmetria ma a costo di uno spreco, esattamente come discusso sui rimedi alla selezione avversa
