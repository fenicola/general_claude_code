---
tags: [economia-informazione, segnalazione, single-crossing, istruzione, credibilita]
aliases: [Educazione come Segnale, Single Crossing Property, Costo del Segnale]
links: [01_Signalling_vs_Screening, 03_Modello_di_Spence, 05_Equilibrio_Separatore]
---

# L'Istruzione come Segnale Credibile e la Proprietà di Single-Crossing

## Il Problema del Datore di Lavoro

> [!definition]
> Un datore di lavoro deve assumere e remunerare lavoratori in base alla loro **produttività**, che è una *caratteristica nascosta* (non osservabile prima dell'assunzione). La domanda è: esiste una **caratteristica osservabile** correlata a quella non osservabile, su cui basare l'offerta salariale? La proposta di Spence è il **livello di istruzione** ($y$): se chi è più produttivo tende anche ad accumulare più istruzione, allora l'istruzione può fungere da segnale della produttività.

La correlazione "più istruzione ⇒ più produttività" non basta però a rendere l'istruzione un *buon* segnale. Serve qualcosa di più forte.

---

## Perché l'Istruzione è un Segnale Credibile? Perché è Costosa

> [!intuition]
> Un segnale è credibile **non perché sia osservabile, ma perché è costoso — e costoso in modo differenziato**. Il segnale dell'istruzione funziona perché *acquisire istruzione costa di più ai lavoratori meno produttivi*. Per un lavoratore di bassa abilità, ogni anno di scuola richiede più fatica, più tempo, più ripetizioni: il costo (monetario e psicologico) è più alto. Per un lavoratore di alta abilità lo stesso traguardo è più "a buon mercato".
>
> Se il segnale costasse uguale a tutti, chiunque potrebbe imitarlo e il segnale perderebbe ogni valore informativo. È proprio il **differenziale di costo** a impedire l'imitazione e a rendere il segnale informativo.

> [BB, p. 337] La segnalazione è un'attività meno costosa per una parte che offre un prodotto di alta qualità rispetto a una che ne offre uno di bassa qualità.

Nel modello numerico della lezione (vedi [[04_Esempio_Numerico_Casi_Base]]) questo si traduce nei costi:

$$
c_L(y) = y \qquad\qquad c_H(y) = \frac{y}{2}
$$

dove $c_L$ è il costo del lavoratore a bassa produttività e $c_H$ quello del lavoratore ad alta produttività. Per ogni livello di istruzione $y > 0$ vale $c_L(y) > c_H(y)$: l'istruzione costa il doppio al tipo basso.

---

## La Proprietà di Single-Crossing (Spence–Mirrlees)

> [!definition]
> La **proprietà di single-crossing** (o condizione di Spence–Mirrlees) richiede che le curve di indifferenza (o le funzioni di costo) dei due tipi si **incrocino una sola volta** nello spazio segnale–ricompensa. Operativamente: il **costo marginale del segnale è sistematicamente più alto per il tipo che si vuole impedire imiti** il tipo migliore.

Formalmente, indicando con $c_i(y)$ il costo del segnale per il tipo $i$:

$$
\frac{\partial c_L}{\partial y} > \frac{\partial c_H}{\partial y} \quad \text{per ogni } y
$$

Nel nostro esempio: $\frac{\partial c_L}{\partial y} = 1 > \frac{1}{2} = \frac{\partial c_H}{\partial y}$.

Graficamente (slide 25–28), nello schema con il salario sull'asse verticale e $y$ sull'orizzontale, la retta di costo $c_L = y$ è **più ripida** della retta $c_H = y/2$. Le due rette partono dall'origine e divergono: è questo singolo "ventaglio" che permette di trovare un livello-soglia $y^*$ che il tipo alto è disposto a raggiungere ma il tipo basso no.

> [BB, p. 338] Le curve di indifferenza tra ricompensa ($a$) e attività di segnalazione ($b$) sono più piatte per gli individui di alta abilità (linee continue) che per quelli di bassa abilità (linea tratteggiata). Il livello massimo di segnalazione accettabile per un individuo di alta abilità è $b_2$; il minimo richiesto per segnalare alta abilità in presenza di individui di bassa abilità è $b_1$.

---

## La Condizione di Imitazione

La single-crossing è esattamente la condizione che rende **non conveniente l'imitazione**. Perché il tipo basso non finga di essere alto raggiungendo $y^*$, occorre che il guadagno salariale dell'imitazione sia inferiore al suo costo aggiuntivo:

$$
\underbrace{w_H - w_L}_{\text{guadagno dall'imitare}} \;<\; \underbrace{c_L(y^*)}_{\text{costo per il tipo basso}}
$$

mentre per il tipo alto il segnale deve restare conveniente:

$$
w_H - w_L \;\ge\; c_H(y^*)
$$

Poiché $c_L(y^*) > c_H(y^*)$ per single-crossing, esiste un intervallo di soglie $y^*$ che soddisfa entrambe le disuguaglianze. Questo intervallo è il cuore dell'[[05_Equilibrio_Separatore|equilibrio separatore]].

> [!example]
> Il GED (vedi [[08_Test_Empirico_GED]]) illustra perfettamente il principio: *"non si può superare il GED senza un minimo di istruzione e studio"*. Il superamento del test è meno costoso per chi è più capace/maturo, quindi soddisfa la single-crossing e può funzionare da segnale (slide 58, 64).

---

## Un Punto Sottile: il Segnale Può Essere Improduttivo

> [!intuition]
> Nel modello di Spence l'istruzione **non aumenta la produttività**: la produttività è fissata dalla natura e l'istruzione serve *solo* a segnalare. Eppure i lavoratori razionali investono in istruzione. Questo è il risultato più spiazzante della teoria: un'attività socialmente improduttiva (puro spreco di risorse, dal punto di vista dell'output) viene intrapresa razionalmente perché *privatamente* redditizia come segnale. È la radice delle esternalità negative discusse in [[06_Proprieta_Equilibrio_Separatore]].

Questo distingue nettamente il modello di segnalazione dal modello del **capitale umano**, in cui l'istruzione è valuata perché *crea* produttività. Distinguere i due empiricamente è il problema affrontato in [[08_Test_Empirico_GED]].

---

## Take-home message

> [!summary]
> L'istruzione è un segnale credibile della produttività non perché sia osservabile, ma perché è **costosa in modo differenziato**: costa di più ai lavoratori meno produttivi. Questa è la **proprietà di single-crossing** (Spence–Mirrlees): il costo marginale del segnale è più alto per il tipo che si vorrebbe impedire di imitare. Nel modello, $c_L(y)=y > c_H(y)=y/2$. Il differenziale di costo apre un intervallo di soglie $y^*$ in cui il tipo alto trova conveniente segnalare e il tipo basso no, rendendo il segnale informativo. Cruciale: il segnale può funzionare *anche se del tutto improduttivo*, perché ciò che conta è il differenziale di costo, non il valore produttivo.

---

## Vedi anche

- [[01_Signalling_vs_Screening]] — Il quadro in cui si colloca il segnale
- [[03_Modello_di_Spence]] — Come la single-crossing entra nella definizione di equilibrio
- [[05_Equilibrio_Separatore]] — La single-crossing in azione: le condizioni $1 \le y^* \le 2$
- [[08_Test_Empirico_GED]] — La single-crossing del GED e la sua verifica empirica

---

## Connessioni con il Vault

**Da `1. GT`:**
- [[1. GT/05_Chicken_Game|Chicken Game]] — la credibilità del segnale è un caso di **impegno credibile**: un'azione è credibile quando è costoso non onorarla o imitarla. Stessa logica del commitment nei giochi
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — il differenziale di costo determina le mosse ottimali dei due tipi nell'albero del gioco

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/12_Confronto_Utilita_Equilibri_Assicurativi|Confronto Utilità]] — la condizione di Spence–Mirrlees compare anche nello screening assicurativo e nel modello Cabernet–Merlot come vincolo che permette la separazione dei tipi
