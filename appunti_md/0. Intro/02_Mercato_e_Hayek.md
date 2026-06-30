---
title: "Il mercato e l'ipotesi di Hayek"
tags:
  - economia-informazione
  - mercato
  - prezzi
  - Hayek
  - efficienza
created: 2026-06-20
related:
  - "[[01_Coordinamento_e_incentivi]]"
  - "[[03_Beni_comuni]]"
  - "[[04_Principale_e_agente]]"
  - "[[1. GT/04_Giochi_Coordinamento|Giochi di Coordinamento]]"
  - "[[1. GT/03_Nash_Equilibrium|Nash Equilibrium]]"
---

# Il mercato e l'ipotesi di Hayek

Il **mercato** è la prima delle tre istituzioni di
[[01_Coordinamento_e_incentivi|coordinamento]]: trasmette informazione attraverso
i **prezzi** e motiva attraverso il **benessere individuale**.

## L'ipotesi di Hayek

> [!definition] Hayek Hypothesis
> I **prezzi di equilibrio** e i **guadagni dallo scambio** (*gains from trade*)
> possono essere raggiunti in presenza di informazione **diffusa e
> decentralizzata**, e in **assenza** di comportamento *price-taking* e di una
> direzione centralizzata del mercato.

> [!intuition] Intuizione
> Nessun singolo agente conosce tutta l'informazione rilevante: ciascuno conosce
> solo le proprie preferenze e i prezzi. Eppure il sistema dei prezzi **aggrega**
> queste conoscenze frammentate e le sintetizza in un unico segnale pubblico. Il
> mercato funziona così come un gigantesco **elaboratore di informazione**: i
> prezzi "riassumono" ciò che migliaia di individui sanno separatamente. È
> l'aspetto "informazione" della tabella in [[01_Coordinamento_e_incentivi]].

## L'evidenza sperimentale di Vernon Smith

L'ipotesi è stata testata in laboratorio con mercati sperimentali:

> [!quote] Riferimento dalle slide
> Smith, V. (1982), *Markets As Economizers Of Information: Experimental
> Examination Of The "Hayek Hypothesis"*, **Economic Inquiry** 20(2), pp. 165–179.

L'esperimento mostra che mercati a **doppia asta** raggiungono l'equilibrio
competitivo (prezzi e quantità) anche con pochissimi operatori e con informazione
totalmente privata e decentralizzata — confermando che il mercato "economizza"
informazione.

## Quando l'informazione *aiuta* il mercato: il primo teorema del benessere

Il mercato raggiunge l'efficienza in due dei tre scenari informativi (vedi
[[04_Principale_e_agente]]):

> [!theorem] Primo Teorema del Benessere (scenari 1 e 2)
> **(1) Informazione completa.** Il sistema dei prezzi riduce il fabbisogno
> informativo: a ciascuno basta conoscere le proprie preferenze e i prezzi per
> individuare gli scambi vantaggiosi. L'esito è **Pareto-efficiente**.
>
> **(2) Informazione incompleta ma simmetrica** (es. lo scambio di un'attività
> finanziaria di cui nessuno conosce il valore futuro). Il primo teorema del
> benessere **continua a valere** → ancora efficienza paretiana.

> [!warning] Quando l'informazione *distrugge* il mercato
> L'efficienza si rompe nel **terzo** scenario, quando l'informazione è
> **asimmetrica**: alcuni operatori sanno più di altri. In tal caso *"more
> information is always better"* **non vale più** (vedi [[05_Selezione_avversa]]).

## Riferimenti dai libri

> [!quote] Dal libro [BB] — *Information Economics*, cap. 7 "From information to prices" (titolo di sezione 7C, p. 121)
> Sezione 7C: *"Theory: The market as an information processor"* — il mercato è
> descritto formalmente come meccanismo che trasforma informazioni private
> disperse in un prezzo pubblico.

> [!quote] Dal libro [BB] — cap. 13 (p. 274)
> «Asymmetric information is an area where the simple rule "more information is
> always better" does not hold. More private information often leads to market
> failure due to so-called "adverse selection".»

- **[BB]** Parte II *"How the market aggregates information"* (capp. 7–11): prezzi,
  *prediction markets*, *learning and cascades*.
- **[M]** Molho — discussione del ruolo informativo dei prezzi e dei limiti del
  meccanismo di mercato in presenza di asimmetrie.

## 🔗 Connessioni con la Teoria dei Giochi

L'**ipotesi di Hayek** descrive il mercato come meccanismo di coordinamento che funziona senza direzione centralizzata. La Teoria dei Giochi formalizza le condizioni sotto cui questo coordinamento ha successo o fallisce:

- Quando l'equilibrio di mercato è unico e Pareto-ottimale, corrisponde all'**equilibrio in strategie dominanti** ([[1. GT/01_Strategia_Dominante]]) o al [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] efficiente.
- Quando esistono **equilibri multipli** (come nei [[1. GT/04_Giochi_Coordinamento|giochi di coordinamento]]), il mercato può fallire nel selezionare quello Pareto-ottimale — un caso in cui l'ipotesi di Hayek è messa alla prova.
- L'asimmetria informativa (scenario 3 del [[04_Principale_e_agente|framework P–A]]) dimostra che i prezzi smettono di essere segnali sufficienti: il mercato cessa di essere l'elaboratore di informazione efficiente descritto da Hayek, aprendo la strada alle analisi di [[05_Selezione_avversa|selezione avversa]] e alle soluzioni attraverso [[06_Segnalazione|signalling]] e [[07_Screening|screening]].
