---
title: "Azzardo morale: azioni nascoste e contratti ottimali"
tags:
  - economia-informazione
  - azzardo-morale
  - moral-hazard
  - azioni-nascoste
  - contratti-ottimali
  - credence-goods
created: 2026-06-20
related:
  - "[[04_Principale_e_agente]]"
  - "[[05_Selezione_avversa]]"
  - "[[01_Coordinamento_e_incentivi]]"
  - "[[09_Nobel]]"
  - "[[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali (SPNE)]]"
  - "[[1. GT/09_Giochi_Ripetuti_Indefiniti|Reputazione e Giochi Ripetuti]]"
  - "[[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]]"
---

# Azzardo morale (*moral hazard*)

L'**azzardo morale** è la conseguenza tipica delle **azioni nascoste** (*hidden
actions*): a differenza della [[05_Selezione_avversa|selezione avversa]],
l'asimmetria informativa emerge **ex post**, cioè **dopo** l'accettazione del
contratto.

## Da informazione simmetrica a asimmetrica

> [!definition] Azioni nascoste
> Scenario in cui l'informazione è inizialmente **simmetrica** ma diventa
> **asimmetrica durante** la relazione. L'agente compie, **dopo** la firma,
> un'azione **non verificabile** (*hidden action*).
>
> Esempio: contratto di lavoro in cui lo **sforzo non è verificabile**. Il
> lavoratore (agente) **conosce** il proprio sforzo; non esiste *hard evidence* che
> lo provi. Anche se il datore (principale) lo intuisse, **non potrebbe andare in
> tribunale** per mancanza di prova verificabile.

## La sequenza temporale (*timing*)

> [!definition] Timing dell'azzardo morale
> $$
> \text{Principale offre un contratto}
> \;\to\;
> \text{Agente accetta / rifiuta}
> \;\to\;
> \boxed{\text{Agente esercita sforzo (o no)}}
> \;\to\;
> \text{L'esito si realizza}
> $$
> L'azione (lo sforzo) avviene **dopo** la firma ed è privata. (In [BB], fig. 16.1,
> $t=0$ offerta, $t=1$ accettazione, $t=2$ sforzo non osservabile, $t=3$ esito.)

$$
\text{azioni nascoste} \;\Longrightarrow\; \text{azzardo morale}
$$

## Il problema dello *shirking*

> [!intuition] Perché il salario fisso fallisce
> Un **salario fisso** non dà incentivo a esercitare alto sforzo: l'agente
> **scansa** il lavoro (*shirk*) perché il principale non può provare la violazione
> del contratto. Lo sforzo risulta **inefficientemente basso**.

## Modello formale (di base)

> [!theorem] Trade-off assicurazione–incentivi
> L'agente ha utilità separabile:
> $$ U = u(w) - e, \qquad u'(w) > 0,\quad u''(w) < 0, $$
> dove $w$ è il salario, $e$ la disutilità dello sforzo (con $e_2 > e_1$ per sforzo
> alto vs. basso). Poiché $u''<0$, l'agente è **avverso al rischio**.
>
> - Per **assicurare** l'agente servirebbe un salario fisso (ottimo se non ci
>   fosse incentivo da fornire).
> - Per **incentivare** lo sforzo non osservabile serve legare il salario all'esito
>   (rischioso).
>
> Il contratto ottimo bilancia **assicurazione** e **incentivi**: in generale **non
> si raggiunge la piena efficienza** del *first best*.

## Rimedi: i contratti ottimali

> [!example] Strumenti di incentivazione
> - Pagamento **legato alla performance**, **bonus**, **tornei** (*tournaments*).
> - **Contratti di incentivo ottimali** (principale–agente).
> - **Meccanismi di controllo esterno** (es. relazione *manager*–azionisti).

Esempi di azzardo morale dalle slide:

- Lo **sforzo del venditore**.
- L'assicurato che installa o no l'**antifurto** sull'auto.
- Lo sforzo per **diagnosticare** una malattia o per fare **ricerca** di qualità.
- **Consulenti finanziari** e investitori.
- Il **manager**, meglio informato del proprietario sulla strategia di business
  ottimale (informazione nascosta *ex post*).

## Caso estremo: i *credence goods* (beni fiduciari)

> [!definition] Credence goods
> Beni/servizi la cui qualità il compratore **non riesce a giudicare nemmeno dopo
> l'acquisto** (medici, meccanici, avvocati, consulenti finanziari). L'esperto
> diagnostica il problema e **raccomanda** un trattamento; il cliente non può
> verificarne la correttezza e deve **fidarsi**.

> [!example] La tentazione dell'esperto — [BB] p. 390
> Detto $v$ il valore del trattamento appropriato, l'utilità lorda del cliente in
> funzione di *ciò di cui ha bisogno* (riga) vs. *ciò che riceve* (colonna):
>
> | Cliente necessita ↓ \ riceve → | $\underline{c}$ (minore) | $\overline{c}$ (maggiore) |
> |---|---|---|
> | $\underline{c}$ (minore) | $v$ | $v$ |
> | $\overline{c}$ (maggiore) | $0$ | $v$ |
>
> Tre forme di comportamento opportunistico: **under-treatment** (cura
> insufficiente), **over-treatment** (cura eccessiva) e **over-charging**
> (sovrafatturazione). (Cfr. Dulleck & Kerschbamer 2006.)

> [!warning] "Don't ask the innkeeper if the wine is good"
> L'osservazione finale delle slide: non si chiede all'oste se il vino è buono —
> perché il suo interesse è in **conflitto** con il tuo. È l'essenza del problema
> dei *credence goods* e, più in generale, dell'[[04_Principale_e_agente|informazione
> asimmetrica con conflitto di interessi]].

## Riferimenti dai libri

> [!quote] Dal libro [BB] — *Information Economics*, cap. 16 "Creating incentives" (p. 369)
> «While hidden information leads to **adverse selection**, hidden action leads to
> **moral hazard**, again a term from insurance literature. [...] We will focus on
> the basic [...] **principal–agent relationship**.»

> [!quote] Dal libro [BB] — cap. 16 (p. 372)
> «The agent dislikes effort; the disutility of a low and a high effort is $e_1$ or
> $e_2 > e_1$. The agent's total utility is [...] $U = u(w) - e$, where $u(w)$ has
> positive but decreasing marginal utility ($u' > 0$, $u'' < 0$).»

> [!quote] Dal libro [KS] — Kerschbamer & Sutter, *The Economics of Credence Goods* (Abstract)
> «[...] the buyer cannot identify the quality of the product that fits her needs
> best, while the seller can do so by performing a diagnosis. [...] the buyer has no
> means to verify the correctness of the recommendation but has to rely on the
> honesty of the seller [...]. Markets for credence goods are typically plagued by
> incentives for fraudulent behavior [...], covering **overprovision** and
> **overcharging**.»

- **[BB]** cap. 16 *Creating incentives* — sez. 16C *Theory: Incentive contracts*
  (p. 371), 16E *Credence goods* (p. 389); cap. 15 *The revelation principle*.
- **[KS]** Kerschbamer & Sutter — survey su esperimenti di laboratorio e di campo
  sui *credence goods*.
- **[M]** Molho — capitolo sull'azzardo morale e i contratti di incentivo.
- Origine teorica: **Holmström**, **Mirrlees** → [[09_Nobel|Nobel 1996 e 2016]].

## 🔗 Connessioni con la Teoria dei Giochi

L'azzardo morale ha la struttura di un **gioco sequenziale con azione nascosta** ([[1. GT/07_Giochi_Dinamici_Sequenziali|forma estesa]]): il Principale offre un contratto, l'Agente accetta, poi sceglie uno sforzo non osservabile. Il [[1. GT/07_Giochi_Dinamici_Sequenziali|SPNE]] è il contratto ottimale che massimizza il profitto del Principale soggetto ai vincoli di compatibilità con gli incentivi.

- Il problema del *shirking* ha la struttura di un [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]]: Principale e Agente "vorrebbero" raggiungere il *first best* (sforzo alto + assicurazione piena), ma l'azione nascosta impedisce di contrattare direttamente sullo sforzo.
- Nei **rapporti di lavoro di lungo periodo**, il meccanismo di reputazione ([[1. GT/09_Giochi_Ripetuti_Indefiniti|giochi ripetuti indefinitamente]]) può sostenere lo sforzo alto senza incentivi espliciti: la minaccia di licenziamento futuro ("[[1. GT/09_Giochi_Ripetuti_Indefiniti|grim trigger]]") rende razionale lo sforzo già nel gioco corrente.
- Per i **beni fiduciari** (*credence goods*), in cui il problema di azzardo morale è particolarmente grave (il cliente non può verificare nemmeno ex post), la reputazione e la ripetizione sono spesso l'unico meccanismo di disciplina — esattamente ciò che il [[1. GT/10_Folk_Theorem|Folk Theorem]] teoricamente giustifica.
