---
title: "Selezione avversa: il mercato dei lemons"
tags:
  - economia-informazione
  - selezione-avversa
  - caratteristiche-nascoste
  - lemons
  - assicurazione
created: 2026-06-20
related:
  - "[[04_Principale_e_agente]]"
  - "[[06_Segnalazione]]"
  - "[[07_Screening]]"
  - "[[09_Nobel]]"
  - "[[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]]"
  - "[[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]]"
---

# Selezione avversa: il mercato dei *lemons*

La **selezione avversa** è la conseguenza tipica delle **caratteristiche
nascoste** (*hidden characteristics*): asimmetria informativa **ex ante**, cioè
**prima** della firma del contratto (a volte detta *ex-ante hidden information*).

## La sequenza temporale (*timing*)

> [!definition] Timing delle caratteristiche nascoste
> $$
> \underbrace{\text{Natura sceglie il tipo}}_{H \,/\, L}
> \;\longrightarrow\;
> \underbrace{\text{Principale offre un contratto}}_{}
> \;\longrightarrow\;
> \underbrace{\text{Agente accetta / rifiuta}}_{}
> $$
> Il tipo dell'agente (alto $H$ / basso $L$) è già determinato e **noto solo
> all'agente** quando il principale formula l'offerta.

## Il meccanismo: perché il mercato si "avvelena"

Nel terzo scenario informativo (vedi [[04_Principale_e_agente]]):

- ci sono asset **buoni** e **cattivi** (o molti tipi);
- solo una parte degli operatori è informata; i **non informati non distinguono**
  buoni da cattivi;
- **non esiste prova credibile/verificabile** (*no hard evidence*) della qualità.

> [!intuition] La spirale verso il basso
> A un dato prezzo, vengono offerti **solo gli asset cattivi**: gli asset sul
> mercato sono una *"selezione avversa"* dall'intero *pool*. I compratori, sapendo
> ciò, non sono disposti a pagare prezzi alti per un cattivo *mix*. Ma a prezzi
> bassi, sempre **meno** qualità vengono offerte. Il processo può portare al
> **congelamento totale dello scambio**, anche se sotto informazione completa le
> parti sarebbero disposte a commerciare.

$$
\text{caratteristiche nascoste} \;\Longrightarrow\; \text{selezione avversa}
$$

## Esempi di selezione avversa

> [!example] Assicurazione sanitaria e *death spiral*
> Sani e malati comprano la stessa polizza, ma i malati la valutano di più.
> - L'assicuratore vuole un *pool* stabile: la maggioranza dei membri
>   relativamente **sana**, i cui premi compensano i costi dei più malati.
> - **Spirale della morte:** i premi salgono → i sani, percependo che non conviene
>   più, **escono** → i premi salgono ancora → escono altri sani → … → il mercato
>   **collassa**.
> - **Contromisura:** rendere **obbligatoria** una copertura minima (es.
>   *Affordable Care Act / Obamacare*, +20–24 milioni di assicurati).

Altri esempi dalle slide:

- **Assicurazione auto:** automobilisti che amano la velocità vs. chi la evita.
- **Lavoratori** molto o poco motivati; venditore con alta o bassa **disutilità
  dello sforzo**.
- **Settore bancario:** progetti ad alto o basso rischio.
- **Legge di Gresham (1551):** *"la moneta cattiva scaccia quella buona"* — quando
  due monete hanno lo stesso valore legale ma diverso contenuto metallico, quella
  "buona" viene tesaurizzata e sparisce dalla circolazione. È una selezione avversa
  ante litteram.

## Dove nasce

> [!note] Contesti tipici
> - **Mercati standard:** il venditore conosce la **qualità** del bene (es. auto
>   usata), che incide sia sulle proprie preferenze sia su quelle del compratore.
> - **Contesti manageriali:** lavoratori di diversa **produttività/abilità**.

## Come rispondere

Il problema della selezione avversa apre alle due grandi soluzioni del corso:

- **[[06_Segnalazione|Signalling]]** — la parte **informata** invia un segnale
  costoso e credibile della propria qualità.
- **[[07_Screening]]** — la parte **non informata** offre un **menù di contratti**
  che induce i tipi a auto-selezionarsi.

## Riferimenti dai libri

> [!quote] Dal libro [BB] — *Information Economics*, cap. 13 (p. 274)
> «The path-breaking article on the used car market, "The market for lemons" by
> George Akerlof, was rejected by one journal after another until the Quarterly
> Journal of Economics accepted it in 1970 — seven years after it had been written.
> Today "adverse selection" is a well known concept [...].»

> [!quote] Dal libro [BB] — cap. 13 (p. 278)
> «This looks like a home match for the seller. Yet, this is not the case. [...] As
> it turns out, the seller's information advantage may in fact be a **handicap**:
> buyers are not naïve; and a seller who is known to know cannot sell a poor
> quality car for the value of a high quality car.»

- **[BB]** cap. 13 *"Information and selection"* — sez. 13C *Theory: The market for
  lemons* (p. 277), 13D *insurance destruction effect* (p. 286), 13E *Annuities*
  (p. 293).
- **[M]** Molho — capitolo sulla selezione avversa e il mercato dei *lemons*.
- Origine: **G. Akerlof**, *The Market for "Lemons"*, QJE 1970 → [[09_Nobel|Nobel 2001]].

## 🔗 Connessioni con la Teoria dei Giochi

La selezione avversa può essere letta come un **gioco di segnalazione con informazione incompleta**: il venditore conosce il tipo del bene, il compratore no. Il gioco sequenziale ([[1. GT/07_Giochi_Dinamici_Sequenziali|forma estesa]]) cattura questa struttura:

- Al primo nodo, la Natura sceglie il tipo (alto/basso)
- L'Agente (venditore) decide se e come partecipare al mercato
- Il Principale (compratore) offre un prezzo basato sulle sue credenze

Senza segnali credibili (→ [[06_Segnalazione]]) o screening (→ [[07_Screening]]), l'equilibrio può essere il **mercato vuoto**: un esito che ha la struttura di un [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]] tra compratori e venditori di qualità — dove entrambi vorrebbero commerciare ma l'equilibrio è la non-transazione. Il [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] di questo mercato è Pareto-inferiore all'ottimo di first-best.

---

## 📂 Approfondimenti nella cartella 2

Questa nota offre una panoramica. I modelli formali completi sono nella cartella `2. Selezione Avversa`:

- [[2. Selezione Avversa/01_Informazione_Asimmetrica_e_Caratteristiche_Nascoste|01 — Informazione asimmetrica e caratteristiche nascoste]] — il timing formale dell'asimmetria ex-ante
- [[2. Selezione Avversa/02_Mercato_dei_Limoni_Intuizione|02 — Mercato dei Limoni: intuizione]] — l'esempio Akerlof, la Legge di Gresham
- [[2. Selezione Avversa/03_Modello_Formale_Due_Qualita|03 — Modello formale a due qualità]] — il caso BB con grafico domanda/offerta
- [[2. Selezione Avversa/04_Modello_Akerlof_Formale|04 — Modello Akerlof formale]] — funzioni di utilità, $\mu = p/2$, collasso del mercato
- [[2. Selezione Avversa/07_Inefficienza_e_Implicazioni|07 — Inefficienza e rimedi]] — cheap talk, segnalazione, screening, reputazione
- [[2. Selezione Avversa/09_Modello_Wilson_Equilibri_Multipli|09 — Wilson: equilibri multipli]] — quando il mercato non collassa del tutto
- [[2. Selezione Avversa/11_Assicurazione_Vita_Effetto_Distruzione|11 — Effetto Hirshleifer]] — più informazione può distruggere il mercato assicurativo
