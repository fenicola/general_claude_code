---
tags: [economia-informazione, azzardo-morale, secondo-migliore, contratto-contingente, vincolo-incentivo, vincolo-partecipazione]
aliases: [Secondo Migliore AM, Contratto Contingente, IC Moral Hazard, Second Best]
links: [03_Primo_Migliore_Sforzo_Osservabile, 05_Inefficienza_e_Costi_di_Agenzia]
---

# Il Secondo Migliore: Sforzo Non Osservabile

## Il Problema con l'Azione Nascosta

> [!definition]
> Il **secondo migliore** (*second best*) è la soluzione ottimale al problema del contratto di incentivo quando il Principale **non può osservare lo sforzo** dell'Agente a $t=2$. Il Principale non può quindi contrattare direttamente sullo sforzo: deve usare l'esito osservabile come proxy indiretto per indurre il comportamento desiderato.

Quando lo sforzo non è osservabile, il Principale non riesce a distinguere i due nodi a $t=2$: sa solo che si realizza un esito $X_H$ o $X_L$, ma non sa se quell'esito è dovuto a work o shirk. Di conseguenza, dopo aver accettato il contratto, l'Agente può **liberamente scegliere il proprio livello di sforzo**. Il Principale deve anticipare questa libertà quando progetta il contratto.

Come in precedenza, il Principale cerca il contratto ottimale per ciascun livello di sforzo e poi confronta i profitti. La novità è che per lo sforzo alto deve aggiungere un **vincolo di compatibilità degli incentivi**.

---

## Indurre lo Sforzo Basso: Risultato Sorprendente

Consideriamo prima il caso in cui il Principale voglia indurre lo sforzo basso $e_1$. Il problema di ottimizzazione è:

$$\max_{w_{1,H},\, w_{1,L}} \; V = (1-p)(X_H - w_{1,H}) + p(X_L - w_{1,L}) \tag{16.4}$$

soggetto a:

$$(1-p)\, u(w_{1,H}) + p\, u(w_{1,L}) - e_1 \geq 0 \tag{PC}_1$$

Il Principale massimizza il profitto atteso sotto il vincolo di partecipazione per un Agente che vuole shirk.

> [!intuition]
> Non serve un vincolo di incentivo per lo sforzo basso: il Principale non ha bisogno di garantire che A preferisca shirk a work — A lo preferisce naturalmente, poiché shirk costa meno. Quindi basta soddisfare il PC.

**Risultato**: il contratto ottimale è il **salario uniforme** $w_{1,H} = w_{1,L} = w_1^*$, dove $u(w_1^*) = e_1$. Si tratta **esattamente dello stesso contratto** del caso di sforzo osservabile!

Il motivo è geometrico e intuitivo: il PC$_1$ ha pendenza $-(1-p)/p$ nel piano $(u(w_H), u(w_L))$; la funzione obiettivo (iso-profitto) ha la stessa pendenza quando $w_{1,H} = w_{1,L}$ (sulla retta a 45°). Il punto di tangenza — dove si massimizza il profitto rispettando il PC — cade sulla diagonale a 45°, cioè con salario uniforme. Qualsiasi differenza tra $w_{1,H}$ e $w_{1,L}$ costerebbe al Principale del rendimento atteso senza aumentare l'utilità dell'Agente risk-averse.

> [BB, ch. 16] Lo sforzo basso è quasi-osservabile: il Principale può anticipare perfettamente che A farà shirk, e il contratto ottimale è lo stesso del caso osservabile.

**Implicazione**: lo sforzo basso non crea alcun costo da asimmetria informativa. Il problema nasce solo quando si vuole indurre lo sforzo alto.

---

## Indurre lo Sforzo Alto: Il Vincolo di Incentivo

Per indurre lo sforzo alto $e_2$, il contratto deve soddisfare **due condizioni** simultaneamente:

**Vincolo di partecipazione (PC$_2$)**: l'Agente che lavora sodo deve trovare conveniente accettare il contratto, cioè l'utilità attesa netta deve essere non negativa:

$$p\, u(w_{2,H}) + (1-p)\, u(w_{2,L}) - e_2 \geq 0 \tag{16.7}$$

**Vincolo di compatibilità degli incentivi (IC)**: l'Agente deve preferire work a shirk, dato il contratto offerto. La condizione è che l'utilità attesa con sforzo alto superi quella con sforzo basso:

$$p\, u(w_{2,H}) + (1-p)\, u(w_{2,L}) - e_2 \;\geq\; (1-p)\, u(w_{2,H}) + p\, u(w_{2,L}) - e_1 \tag{16.8}$$

Semplificando la (16.8):

$$u(w_{2,H}) - u(w_{2,L}) \;\geq\; \frac{e_2 - e_1}{2p-1} \tag{16.9}$$

> [!definition]
> La condizione **(16.9)** è il **vincolo di incentivo** nel caso dell'azzardo morale. Essa richiede che il differenziale di utilità tra il salario alto e il salario basso sia almeno uguale al rapporto tra il costo aggiuntivo dello sforzo $(e_2 - e_1)$ e il guadagno probabilistico $(2p-1)$. In altri termini: il "premio" per l'esito alto deve essere sufficientemente grande da compensare lo sforzo aggiuntivo, tenendo conto di quanto lo sforzo influenza le probabilità.

Interpretazione economica della (16.9): il termine $(2p-1)$ è la "potenza" dello sforzo — quanto migliora le probabilità di $X_H$. Più alto è $(2p-1)$, minore deve essere il differenziale salariale necessario per indurre lo sforzo alto.

---

## Il Contratto Ottimale per lo Sforzo Alto

Il problema del Principale è:

$$\max_{w_{2,H},\, w_{2,L}} \; V = p(X_H - w_{2,H}) + (1-p)(X_L - w_{2,L}) \tag{16.6}$$

soggetto a (16.7) e (16.8).

**Risultato fondamentale**: nell'ottimo **entrambi i vincoli legano con uguaglianza** (PC$_2$ e IC sono attivi). Perché?

- Finché il PC non lega, il Principale può ridurre almeno uno dei due salari senza perdere l'Agente — riducendo i costi.
- Finché l'IC non lega, il Principale può ridurre la differenza $w_{2,H} - w_{2,L}$ senza temere lo shirking — ancora riducendo i costi dell'assicurazione.

Risolvendo il sistema con PC$_2$ = 0 e IC = 0:

$$u(w_{2,H}^*) = \frac{p\, e_2 - (1-p)\, e_1}{2p-1} \tag{16.10}$$

$$u(w_{2,L}^*) = \frac{p\, e_1 - (1-p)\, e_2}{2p-1} \tag{16.11}$$

> [!intuition]
> Poiché $p > 1/2$ ed $e_2 > e_1$, si verifica che $u(w_{2,H}^*) > u(w_{2,L}^*)$, cioè $w_{2,H}^* > w_{2,L}^*$. Il contratto ottimale per indurre sforzo alto è un **contratto contingente**: paga un salario alto se l'esito è alto e un salario basso se l'esito è basso. L'Agente viene esposto a rischio — deliberatamente — per dargli l'incentivo di lavorare sodo.

Si può riscrivere il contratto come combinazione di una **componente fissa** $w_{1,L}^*$ e un **bonus** per l'esito alto:

$$w_{2,H}^* = w_{1,L}^* + \text{bonus}$$

Rispetto al contratto first-best, il contratto contingente paga di più se l'esito è alto e di meno se l'esito è basso.

---

## Analisi Grafica nel Piano $(u(w_H), u(w_L))$

L'analisi si conduce nel piano le cui assi misurano l'utilità del salario nei due stati:

**La retta a 45°**: luoghi dove $w_H = w_L$, cioè salario fisso e piena assicurazione.

**PC$_1$** (sforzo basso): pendenza $-(1-p)/p$. Esempio con $p = 3/4$: pendenza $-1/3$. Interseca la diagonale nel punto corrispondente a $u(w_1^*)$.

**PC$_2$** (sforzo alto): stessa forma ma **più ripida** (pendenza $-p/(1-p) = -3$ per $p = 3/4$) e più a destra. PC$_2$ è più ripida perché con sforzo alto le probabilità sono invertite: $p$ è la probabilità di $X_H$. Anche PC$_2$ interseca la diagonale nello stesso punto di PC$_1$: se il salario è fisso, il costo dell'assicurazione è lo stesso indipendentemente dallo sforzo.

**IC** (linea degli incentivi): corre **parallela alla diagonale a 45°** con uno spostamento orizzontale (o verticale) di $\frac{e_2 - e_1}{2p-1}$. I contratti ammissibili per lo sforzo alto devono trovarsi **a destra di IC** (differenziale salariale sufficiente).

**Il contratto ottimale** $(w_{2,H}^*, w_{2,L}^*)$ si trova all'**intersezione di PC$_2$ e IC**: il punto "angolare" dell'area ammissibile (sopra PC$_2$ e a destra di IC) che minimizza i costi salariali, cioè che giace sulla iso-profitto più vicina all'origine.

> [!intuition]
> L'intersezione di PC$_2$ e IC è l'unico punto che contemporaneamente: (a) mantiene l'Agente sul suo livello di utilità di riserva (PC lega) e (b) lo rende indifferente tra work e shirk (IC lega). È il contratto meno costoso che induce sforzo alto.

**Confronto chiave**: il punto $(w_{2,H}^*, w_{2,L}^*)$ si trova **sotto e a destra** del punto sulla diagonale corrispondente al contratto first-best per sforzo alto. In altre parole, l'Agente riceve un salario basso più basso ($w_{2,L}^* < w_1^*$) e un salario alto più alto ($w_{2,H}^* > w_1^*$) rispetto al caso osservabile.

---

## Scelta dell'Effort Ottimale con Sforzo Non Osservabile

Come nel caso osservabile, il Principale confronta i profitti attesi. Con effort non osservabile, il Principale preferisce indurre sforzo alto se:

$$(2p-1)(X_H - X_L) \;\geq\; p\, w_{2,H}^* + (1-p)\, w_{2,L}^* - w_1^* \tag{16.12}$$

La differenza rispetto alla condizione (16.3) del primo migliore è che ora il costo del lavoro è $p\, w_{2,H}^* + (1-p)\, w_{2,L}^*$ (salario atteso contingente), che è **maggiore** del salario fisso $w_2^*$ del primo migliore: bisogna pagare un premio di rischio aggiuntivo per trasferire il rischio sull'Agente e creare gli incentivi.

---

## Take-home Message

> [!summary]
> Con sforzo non osservabile (**secondo migliore**): indurre lo sforzo basso non crea costi aggiuntivi — il contratto ottimale è identico al primo migliore. Indurre lo sforzo alto richiede invece un **contratto contingente** $\{w_{2,H}^*, w_{2,L}^*\}$ con $w_{2,H}^* > w_{2,L}^*$, determinato dall'intersezione di **PC$_2$** (16.7) e **IC** (16.9), entrambi attivi. Formalmente: $u(w_{2,H}^*) = [pe_2 - (1-p)e_1]/(2p-1)$ e $u(w_{2,L}^*) = [pe_1 - (1-p)e_2]/(2p-1)$. Il differenziale salariale è lo strumento di incentivo: l'Agente viene esposto a rischio deliberatamente. Questo ha un **costo** — il premio di rischio e una possibile distorsione nella scelta dello sforzo — analizzato nella nota successiva.

---

## Vedi Anche

- [[03_Primo_Migliore_Sforzo_Osservabile]] — Il benchmark da cui misurare le distorsioni
- [[05_Inefficienza_e_Costi_di_Agenzia]] — I costi reali del contratto contingente
- [[3. Segnalazione/05_Equilibrio_Separatore|Equilibrio Separatore]] — Anche lì PC e IC legano simultaneamente
- [[1. GT/01_Strategia_Dominante|Strategia Dominante]] — Shirking è dominante senza vincolo IC
