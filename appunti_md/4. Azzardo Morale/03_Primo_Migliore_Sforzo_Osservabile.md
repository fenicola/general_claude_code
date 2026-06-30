---
tags: [economia-informazione, azzardo-morale, primo-migliore, sforzo-osservabile, salario-fisso, assicurazione]
aliases: [Primo Migliore AM, First Best Moral Hazard, Sforzo Osservabile]
links: [02_Setup_Modello_PA, 04_Secondo_Migliore_Sforzo_Non_Osservabile]
---

# Il Benchmark: Sforzo Osservabile (Primo Migliore)

## Perché Studiare il Caso Osservabile

Prima di analizzare cosa succede quando lo sforzo è nascosto, è essenziale capire cosa succederebbe in un mondo ipotetico in cui il Principale *può* osservare lo sforzo dell'Agente. Questo scenario costituisce il **primo migliore** (*first best*): l'allocazione efficiente massima, quella che massimizza il surplus totale senza il vincolo dell'asimmetria informativa. Ogni distorsione riscontrata nel caso reale (sforzo non osservabile) si misurerà come scarto rispetto a questo benchmark.

> [!definition]
> Il **primo migliore** (*first best*) è la soluzione ottimale al problema del contratto di incentivo quando il Principale può osservare e verificare direttamente il livello di sforzo dell'Agente. In questo caso il contratto può essere scritto direttamente sullo sforzo, eliminando il problema dell'azione nascosta.

---

## Il Contratto con Sforzo Osservabile: Salario Fisso

Se il Principale può distinguere i due nodi a $t=2$ (cioè sa con certezza se A ha lavorato o shirked), **può scrivere un contratto direttamente sullo sforzo**: "ti pago $w$ se lavori sodo, niente se non lavori."

In questo scenario, la scelta ottimale per il Principale risk-neutral è offrire un **salario fisso**: un pagamento costante che non dipende dall'esito $X_H$ o $X_L$.

> [!intuition]
> Il motivo è una questione di vantaggio comparato nel sopportare il rischio. Il Principale è **risk-neutral**: la varianza del pagamento non entra nella sua funzione obiettivo. L'Agente è **risk-averse**: odia la varianza e per sopportarla richiederebbe un compenso extra (premio di rischio). Dunque l'allocazione efficiente del rischio prevede che **tutto il rischio ricada sul Principale**: l'Agente viene completamente assicurato con un salario fisso.

Formalmente, con un salario fisso $w$ (cioè $w_H = w_L = w$), l'Agente è **completamente assicurato** contro l'incertezza dell'esito: il suo compenso non dipende da $X$.

---

## Il Contratto Ottimale per lo Sforzo Basso

Se il Principale vuole che l'Agente scelga lo sforzo basso $e_1$, il contratto deve soddisfare il **vincolo di partecipazione per l'Agente pigro**:

$$u(w_1^*) = e_1 \tag{PC per $e_1$}$$

Il salario fisso minimo $w_1^*$ è quello che rende l'Agente indifferente tra accettare il contratto (e shirk) e rifiutarlo (utilità di riserva = 0). Poiché $u$ è crescente, esiste un unico $w_1^*$ che soddisfa questa condizione.

Il pagamento non dipende dall'esito: $w_{1,H}^* = w_{1,L}^* = w_1^*$.

---

## Il Contratto Ottimale per lo Sforzo Alto

Se il Principale vuole che l'Agente scelga lo sforzo alto $e_2$, il contratto deve soddisfare il **vincolo di partecipazione per l'Agente laborioso**:

$$u(w_2^*) = e_2 \tag{PC per $e_2$}$$

Poiché $e_2 > e_1$, è necessario che $w_2^* > w_1^*$: lavorare di più ha un costo, e l'Agente deve essere compensato per questa disutilità aggiuntiva. Anche in questo caso, il pagamento è fisso: $w_{2,H}^* = w_{2,L}^* = w_2^*$.

> [!intuition]
> Con sforzo osservabile, i due contratti ottimali sono entrambi salari fissi che differiscono solo nell'ammontare: il salario per lo sforzo alto è più alto, perché deve compensare anche la maggiore disutilità. L'Agente riceve esattamente quanto necessario per accettare — nessun surplus informativo, nessun premio di rischio.

---

## Quale Sforzo è Ottimale per il Principale?

Il Principale confronta i profitti attesi nelle due situazioni:

**Profitto con sforzo basso** (equazione 16.1):
$$\Pi_1 = (1-p) X_H + p X_L - w_1^*$$

**Profitto con sforzo alto** (equazione 16.2):
$$\Pi_2 = p X_H + (1-p) X_L - w_2^*$$

Sottraendo la (16.1) dalla (16.2) si ottiene la **condizione per preferire lo sforzo alto**:

$$\underbrace{(2p-1)(X_H - X_L)}_{\text{Beneficio marginale}} \geq \underbrace{w_2^* - w_1^*}_{\text{Costo marginale}} \tag{16.3}$$

Dove:
- Il **lato sinistro** misura l'**aumento nel rendimento atteso** dovuto allo sforzo alto. Il termine $(2p-1) = p - (1-p)$ è la differenza nelle probabilità dei due esiti tra work e shirk: quanto più $p$ è vicino a 1, tanto più lo sforzo alto determina l'esito.
- Il **lato destro** misura il **costo aggiuntivo in salario** necessario per indurre lo sforzo alto rispetto allo sforzo basso.

Il Principale preferisce lo sforzo alto se e solo se il guadagno marginale in rendimento atteso supera il costo marginale in salario.

> [!example]
> Supponiamo $p = 3/4$, $X_H = 100$, $X_L = 20$, $e_1 = 5$, $e_2 = 10$.
> - Beneficio marginale: $(2 \cdot 3/4 - 1)(100 - 20) = (1/2)(80) = 40$
> - Costo marginale: $w_2^* - w_1^* = u^{-1}(10) - u^{-1}(5)$ — dipende dalla forma di $u$
>
> Se per esempio $u(w) = \sqrt{w}$, allora $w_1^* = 25$ e $w_2^* = 100$. Il costo marginale è 75 > 40, quindi il Principale preferisce lo sforzo basso. Ma se $u(w) = w$ (Agente risk-neutral), $w_1^* = 5$ e $w_2^* = 10$: costo marginale = 5 << 40, e il Principale preferisce lo sforzo alto.

---

## La Proprietà Chiave: Piena Assicurazione

> [!intuition]
> Nel primo migliore, l'Agente è **completamente assicurato**: riceve lo stesso salario indipendentemente dall'esito. Tutto il rischio ricade sul Principale, che è risk-neutral e quindi non subisce costi dalla varianza. Questa è l'allocazione efficiente del rischio. Il surplus totale è massimizzato perché il rischio è sopportato da chi ha costo zero nel sopportarlo.

Questa proprietà di piena assicurazione è il **standard di riferimento** per il secondo migliore. Quando lo sforzo diventa non osservabile, il Principale non potrà più garantire piena assicurazione all'Agente se vuole indurre sforzo alto: dovrà fare una scelta tra **assicurazione** e **incentivo**.

---

## Take-home Message

> [!summary]
> Con sforzo osservabile (primo migliore), il contratto ottimale è un **salario fisso** $w^*$ che soddisfa la condizione $u(w^*) = e$ (il PC lega con uguaglianza). L'Agente è completamente assicurato — nessuna varianza sul suo compenso — e tutto il rischio ricade sul Principale risk-neutral. Il Principale induce sforzo alto se e solo se il beneficio marginale $(2p-1)(X_H - X_L)$ supera il costo marginale $w_2^* - w_1^*$ (condizione 16.3). Questo scenario è il **benchmark di efficienza**: ogni distorsione nel secondo migliore verrà misurata come scarto da questo caso.

---

## Vedi Anche

- [[02_Setup_Modello_PA]] — Il setup del modello (utilità, effort, esiti)
- [[04_Secondo_Migliore_Sforzo_Non_Osservabile]] — Cosa cambia quando lo sforzo è nascosto?
- [[05_Inefficienza_e_Costi_di_Agenzia]] — Il costo della distorsione rispetto al primo migliore
- [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]] — Shirking come strategia dominante senza contratto contingente
