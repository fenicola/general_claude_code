---
tags: [economia-informazione, azzardo-morale, costi-agenzia, premio-rischio, inefficienza, welfare]
aliases: [Costi di Agenzia, Premio di Rischio AM, Inefficienza Azzardo Morale, Agency Costs]
links: [03_Primo_Migliore_Sforzo_Osservabile, 04_Secondo_Migliore_Sforzo_Non_Osservabile]
---

# Welfare e Costi di Agenzia: Le Conseguenze dell'Asimmetria

## Il Paradosso dell'"Open Secret"

Un aspetto apparentemente paradossale del modello emerge una volta risolto il secondo migliore: il Principale, quando progetta il contratto a $t=0$, **sa perfettamente quale sforzo sceglierà l'Agente** in risposta a ogni contratto. Se offrirà un contratto con differenziale salariale sufficiente, l'Agente lavorerà; altrimenti shirkerà. L'effort non è un mistero per il Principale — è un **segreto di Pulcinella** (*open secret*).

Allora perché l'asimmetria informativa ha un costo?

> [!intuition]
> **Anticipare un'azione e osservarla sono cose diverse.** Il Principale può prevedere il comportamento dell'Agente, ma può farlo **solo al costo di imporre un rischio** all'Agente avverso al rischio. L'asimmetria non impedisce al Principale di "sapere" cosa farà l'Agente — ma rende costoso *indurlo* a farlo nel modo desiderato.

Il caso è analogo alla segnalazione: anche lì l'informazione può essere estratta dall'Agente, ma solo ad un costo. Qui, il "costo di estrazione" dell'information sull'effort prende due forme precise.

> [BB, ch. 16] L'azione nascosta ha un costo anche quando può essere perfettamente prevista. I costi si manifestano in due forme: (1) assicurazione incompleta dell'Agente; (2) scelta inefficiente dello sforzo.

---

## Prima Forma di Inefficienza: Assicurazione Incompleta e Premio di Rischio

Il contratto di incentivo ottimale $\{w_{2,H}^*, w_{2,L}^*\}$ espone l'Agente a variabilità salariale. Poiché l'Agente è risk-averse, un salario variabile con lo stesso valore atteso di un salario fisso genera **meno utilità**. Il Principale deve quindi pagare un salario atteso *più alto* per garantire all'Agente la stessa utilità del caso first-best.

> [!definition]
> Il **premio di rischio** (*risk premium*) $\Delta$ associato al contratto contingente è il costo aggiuntivo che il Principale deve sostenere rispetto al primo migliore per indurre lo stesso livello di sforzo alto. Formalmente:
>
> $$\Delta = p\, w_{2,H}^* + (1-p)\, w_{2,L}^* - \bar{w}_2^* \;\geq\; 0$$
>
> dove $\bar{w}_2^*$ è il salario certo equivalente (*certainty equivalent wage*) del contratto contingente — il salario fisso che darebbe all'Agente la stessa utilità attesa del contratto contingente.

Graficamente: sul piano $u(w)$ vs $w$, per una funzione concava (Agente risk-averse), il valore atteso dell'utilità del contratto contingente è **inferiore** all'utilità del valore atteso del salario. La distanza orizzontale tra il valore atteso del salario e il suo equivalente certo è $\Delta$.

> [!intuition]
> Il premio di rischio **non aumenta l'utilità dell'Agente**: il PC lega con uguaglianza, quindi l'Agente è indifferente tra il contratto contingente (con rischio) e un ipotetico contratto fisso di valore $\bar{w}_2^*$. Il premio di rischio *compensa* l'Agente per il rischio imposto, ma non lo rende meglio off rispetto al caso first-best. È però un **costo reale per il Principale**: un trasferimento di risorse che non genera valore per l'Agente, solo assicurazione contro il rischio.

Questa perdita secca costituisce il **costo di agenzia** (*agency cost*): la perdita di surplus totale causata dall'impossibilità di osservare l'effort.

$$\text{Costo di agenzia} = \Delta \geq 0$$

Il contratto contingente giace su una **iso-profitto più alta** (cioè un profitto più basso per il Principale) rispetto al contratto first-best — proprio della distanza $\Delta$ in termini di salario atteso.

---

## Seconda Forma di Inefficienza: Scelta Inefficiente dello Sforzo

Il premio di rischio rende lo sforzo alto più costoso per il Principale rispetto al caso osservabile. Questa differenza di costo può rendere lo sforzo alto **non conveniente** anche quando lo sarebbe nel primo migliore.

Ricordiamo le due condizioni di confronto:

**Con sforzo osservabile**, il Principale preferisce sforzo alto se (16.3):
$$\underbrace{(2p-1)(X_H - X_L)}_{\text{Beneficio marginale}} \geq \underbrace{w_2^* - w_1^*}_{\text{Costo marginale (first best)}}$$

**Con sforzo non osservabile**, il Principale preferisce sforzo alto se (16.12):
$$(2p-1)(X_H - X_L) \geq \underbrace{p\, w_{2,H}^* + (1-p)\, w_{2,L}^* - w_1^*}_{\text{Costo marginale (second best)}}$$

Poiché il costo nel secondo migliore include il premio di rischio $\Delta$, si ha:

$$p\, w_{2,H}^* + (1-p)\, w_{2,L}^* - w_1^* = (w_2^* - w_1^*) + \Delta$$

La **condizione per scelta inefficiente dello sforzo** è che il Principale scelga sforzo basso nel secondo migliore, pur avendo scelto sforzo alto nel primo migliore. Questo accade quando:

$$w_2^* - w_1^* \;\leq\; (2p-1)(X_H - X_L) \;\leq\; (w_2^* - w_1^*) + \Delta \tag{condizione per inefficienza}$$

In forma compatta, definendo il profitto netto aggiuntivo dello sforzo alto:

$$V_2 - V_1 = (2p-1)(X_H - X_L) - (w_2^* - w_1^*)$$

la condizione diventa:

$$0 \;\leq\; V_2 - V_1 \;\leq\; \Delta$$

> [!definition]
> Lo sforzo è scelto in modo **inefficiente** quando il profitto netto aggiuntivo dello sforzo alto $V_2 - V_1$ è **positivo** (il Principale sceglierebbe sforzo alto se osservabile) ma **inferiore al premio di rischio** $\Delta$ (il Principale sceglie sforzo basso perché il contratto contingente è troppo costoso). Formalmente: $0 \leq V_2 - V_1 \leq \Delta$.

> [!intuition]
> Immaginate uno spettro da "sforzo alto sempre ottimale" a "sforzo basso sempre ottimale": la zona intermedia è quella in cui la scelta dipende dall'asimmetria. Se il guadagno netto dallo sforzo alto è appena positivo (primo migliore: sforzo alto), ma il costo aggiuntivo del contratto contingente supera quel guadagno (secondo migliore: sforzo basso), si ha una **scelta inefficiente**. Il mercato produce meno output di quanto potrebbe, a causa dell'impossibilità di osservare l'effort.

---

## Riepilogo dei Costi dell'Asimmetria Informativa

| Forma di inefficienza | Descrizione | Condizione |
|---|---|---|
| **Assicurazione incompleta** | L'Agente sopporta rischio (non può essere pienamente assicurato) → premio di rischio $\Delta$ come deadweight loss | Sempre presente quando si induce $e_2$ in secondo migliore |
| **Scelta inefficiente dello sforzo** | Il Principale sceglie $e_1$ pur essendo $e_2$ efficiente nel first best | $0 \leq V_2 - V_1 \leq \Delta$ |

---

## Cenni alle Estensioni (Refinements)

Le slide 61–62 anticipano le principali direzioni di estensione del modello di base, che saranno sviluppate nei blocchi successivi:

**Estensioni del problema di base:**
- *Giochi ripetuti e reputazione*: in relazioni di lungo periodo, la reputazione può risolvere (parzialmente) il problema dell'azzardo morale → collegamento con [[1. GT/09_Giochi_Ripetuti_Indefiniti|giochi ripetuti indefiniti]] e [[1. GT/10_Folk_Theorem|Folk Theorem]]
- *Spazio continuo di azioni*: più di due livelli di sforzo, ottimizzazione su un continuum
- *Azioni multidimensionali (multi-tasking)*: l'Agente ha più compiti da svolgere; gli incentivi su una dimensione distorcono le altre (problema classico Holmstrom–Milgrom)
- *Azioni parzialmente osservabili (segnali)*: proxy imperfetti dello sforzo

**Estensioni strutturali:**
- *Competizione tra Principali*: più P che si contendono lo stesso A
- *Competizione tra Agenti*: tornei, gare tra dipendenti (Lazear, 2000)
- *Lavoro di squadra (teamwork)*: problema del free-riding nell'effort collettivo
- *Monitoring*: investimento in sistemi di supervisione per ridurre $\Delta$

**Previsioni comportamentali** (slide 62):
- Più alti incentivi → più alto sforzo (Lazear, 2000)
- Più rumore nell'esito → contratti meno basati sugli incentivi (perché il segnale ha meno valore informativo)
- Valutazioni soggettive: *captatio benevolentiae*, leniency bias, centrality bias
- Profit sharing e incentivi di gruppo

---

## Take-home Message

> [!summary]
> L'asimmetria informativa nell'azzardo morale ha un **costo reale** anche quando il Principale prevede perfettamente il comportamento dell'Agente. I costi si manifestano in due forme: (1) **assicurazione incompleta** — il contratto contingente impone all'Agente un rischio che il Principale deve compensare con un premio di rischio $\Delta \geq 0$, un costo senza controparte in termini di utilità dell'Agente (deadweight loss = costo di agenzia); (2) **scelta inefficiente dello sforzo** — quando $0 \leq V_2 - V_1 \leq \Delta$, il Principale rinuncia allo sforzo alto anche se sarebbe efficiente nel primo migliore. L'asimmetria non blocca la contrattazione, ma la distorce in modi precisi e misurabili.

---

## Vedi Anche

- [[03_Primo_Migliore_Sforzo_Osservabile]] — Il benchmark da cui si misura la perdita di benessere
- [[04_Secondo_Migliore_Sforzo_Non_Osservabile]] — Il contratto contingente che genera il costo di agenzia
- [[2. Selezione Avversa/07_Inefficienza_e_Implicazioni|Inefficienza SA]] — Confronto: costo sociale della SA (mercato vuoto) vs costo di agenzia (AM)
- [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]] — La reputazione come rimedio nei giochi ripetuti
- [[1. GT/10_Folk_Theorem|Folk Theorem]] — Cooperazione sostenibile in equilibrio con interazioni ripetute
