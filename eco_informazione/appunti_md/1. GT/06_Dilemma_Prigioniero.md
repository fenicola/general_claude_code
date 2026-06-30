---
tags: [economia-informazione, game-theory, dilemma-prigioniero, cooperazione]
aliases: [Dilemma del Prigioniero, Prisoner's Dilemma, PD]
links: [01_Strategia_Dominante, 03_Nash_Equilibrium, 08_Giochi_Ripetuti_Finiti, 09_Giochi_Ripetuti_Indefiniti, 0. Intro/03_Beni_comuni, 0. Intro/01_Coordinamento_e_incentivi, 0. Intro/08_Azzardo_morale]
---

# Dilemma del Prigioniero

## Definizione Formale

> [!definition] Dilemma del Prigioniero
> Il **Dilemma del Prigioniero** (PD) è un gioco a due giocatori con struttura di payoff:
> $$c > a > d > b$$
> dove:
> - $a$ = payoff da cooperazione reciproca (Cooperate, Cooperate)
> - $b$ = payoff da cooperazione unilaterale quando l'altro defeziona (Cooperate, Defect)
> - $c$ = payoff da defezione unilaterale quando l'altro coopera (Defect, Cooperate)
> - $d$ = payoff da defezione reciproca (Defect, Defect)
>
> *Defect* è una strategia **strettamente dominante** per entrambi i giocatori. Il NE unico è {*Defect*, *Defect*} con payoff $(d, d)$, che è **Pareto-inferiore** a {*Cooperate*, *Cooperate*} con payoff $(a, a)$.

## Intuizione Economica

> [!intuition]
> Il PD è "il classico gioco della teoria dei giochi" per eccellenza. Il paradosso che lo rende famoso è questo: ciascun individuo, agendo in modo *perfettamente razionale* e *nel proprio interesse*, produce un esito collettivo che è *peggiore* per tutti rispetto a quello che otterrebbero cooperando.
>
> Non si tratta di irrazionalità né di cattiveria: è la struttura dei payoff stessa a incentivare la defezione. Qualunque cosa faccia l'altro, io sto meglio defezionando. Eppure, se entrambi ragionano così, entrambi finiscono peggio che se avessero cooperato.
>
> Il PD è il modello paradigmatico di tutti i fallimenti della cooperazione sociale: dalla corsa agli armamenti alle guerre commerciali, dall'inquinamento ai [[0. Intro/03_Beni_comuni|beni comuni]], dalla pubblicità comparativa all'evasione fiscale.

## Modello Formale

> [!example] Matrix 3.1 — Prisoners' Dilemma (Carmichael)
> Due giocatori scelgono simultaneamente tra *Cooperate* (C) e *Defect* (D).
>
> |  | Giocatore 2: *Cooperate* | Giocatore 2: *Defect* |
> |---|---|---|
> | **Giocatore 1: *Cooperate*** | 10, 10 | 0, 11 |
> | **Giocatore 1: *Defect*** | 11, 0 | 1, 1 |
>
> **Verifica delle strategie dominanti:**
> - Se Gioc. 2 coopera: Gioc. 1 ottiene 11 (D) vs 10 (C) → *Defect* è migliore
> - Se Gioc. 2 defeziona: Gioc. 1 ottiene 1 (D) vs 0 (C) → *Defect* è migliore
>
> *Defect* è strategia strettamente dominante per Giocatore 1. Per simmetria, lo è anche per Giocatore 2.
>
> **Nash Equilibrium unico**: {*Defect*, *Defect*} con payoff (1, 1) — Pareto-inferiore a {*Cooperate*, *Cooperate*} con payoff (10, 10).

## Il Paradosso della Razionalità

La versione generalizzata del PD (Carmichael, Matrix 8.2) usa payoff letterali con $c > a > d > b$:

|  | Cooperate | Defect |
|---|---|---|
| **Cooperate** | $a, a$ | $b, c$ |
| **Defect** | $c, b$ | $d, d$ |

La condizione strutturale $c > a > d > b$ assicura che:
- *Defect* è sempre preferibile a *Cooperate* (domina strettamente)
- La cooperazione reciproca $(a, a)$ è preferibile alla defezione reciproca $(d, d)$ per entrambi

> [C, p. 59–75] Il PD è la tensione fondamentale tra interesse individuale e interesse collettivo. La razionalità individuale porta all'irrazionalità collettiva. Questo problema è al cuore di molte questioni economiche e di politica pubblica.

> [BB, p. 222] Il PD nella ripetizione: in un PD one-shot tra agenti razionali, la defezione è sempre la scelta dominante. Ma nei mercati reali, le interazioni si ripetono nel tempo, e ciò apre la porta alla cooperazione attraverso meccanismi di reputazione e punizione.

## Soluzioni al Dilemma del Prigioniero (One-Shot)

Il PD in un gioco singolo sembra non avere soluzione cooperativa compatibile con la razionalità. Le principali proposte sono:

**1. Accordi coercitivi (Leviatano)**
Un'autorità esterna (lo Stato, un contratto vincolante) può rendere la defezione illegale o costosa, modificando i payoff in modo che la cooperazione diventi dominante. È la risposta hobbesiana: senza un sovrano, ci sarebbe solo "la guerra di tutti contro tutti."

**2. Reti informali di punizione (gossip)**
In comunità piccole e ripetute, la reputazione di "defezioniatore" si diffonde e chi defeziona è punito dall'esclusione dalle future interazioni. Il gossip funziona come meccanismo di enforcement decentralizzato.

**3. Ripetizione e reputazione**
Se il gioco si ripete, la prospettiva di interazioni future cambia i calcoli. → Vedi [[08_Giochi_Ripetuti_Finiti]] e [[09_Giochi_Ripetuti_Indefiniti]]

**4. Incertezza sulla durata (ripetizione indefinita)**
Se i giocatori non sanno quando finirà il gioco, le strategie di punizione come *grim trigger* o *tit-for-tat* possono sostenere la cooperazione. → [[09_Giochi_Ripetuti_Indefiniti]]

**5. Preferenze non-egoistiche**
Se i giocatori si preoccupano anche del benessere altrui (altruismo, equità, identità di gruppo), i payoff effettivi cambiano e la cooperazione può emergere anche in one-shot. Questo è il "passaggio dall'Homo Economicus all'Homo Sapiens" citato nelle slide.

## Applicazioni Reali

- **Oligopolio e cartelli**: due imprese farebbero profitti più alti colludendo sui prezzi, ma ciascuna ha incentivo a imbrogliare abbassando il prezzo segretamente.
- **Corsa agli armamenti**: entrambi i paesi farebbero meglio disarmando, ma ciascuno ha incentivo ad armarsi per sicurezza.
- **Inquinamento**: ridurre le emissioni è costoso; ciascun paese preferisce che riducano gli altri.
- **Lavoro di gruppo**: in un gruppo, ogni membro preferirebbe che lavorassero gli altri.
- **Beni pubblici e free-rider**: il bene pubblico beneficia tutti, ma nessuno vuole pagarlo.

> [C, p. 62–64] Il PD modella situazioni in cui l'accordo a cooperare "avrebbe chiaramente senso" se i giocatori cercassero di massimizzare i payoff congiunti, ma la logica dell'interesse individuale rende tale accordo difficile da sostenere senza enforcement.

> [!summary] Take-home message
> Il Dilemma del Prigioniero è il punto di partenza per comprendere i fallimenti della cooperazione. Il suo messaggio fondamentale: la razionalità individuale può portare all'irrazionalità collettiva. Questo non è solo un paradosso teorico ma il modello di una vasta gamma di problemi economici reali. La chiave per risolvere il PD non è rendere gli agenti meno razionali, ma cambiare la struttura del gioco attraverso istituzioni, ripetizione o preferenze sociali. Il tema della ripetizione è sviluppato in [[08_Giochi_Ripetuti_Finiti]] e [[09_Giochi_Ripetuti_Indefiniti]].

## 🔗 Connessioni con l'Economia dell'Informazione

Il **Dilemma del Prigioniero** è il modello sottostante di moltissimi problemi dell'economia dell'informazione:

- [[0. Intro/03_Beni_comuni|Beni comuni e tragedia dei commons]]: il dilemma del pescatore ha esattamente la struttura del PD — defezione = pescare sopra il limite; cooperazione = pescare sotto.
- [[0. Intro/08_Azzardo_morale|Azzardo morale]]: il lavoratore che non esercita sforzo gioca una strategia dominante (defezione) in un PD contro il Principale. Il contratto ottimale deve modificare i payoff affinché lo sforzo diventi razionale.
- [[0. Intro/01_Coordinamento_e_incentivi|Coordinamento e incentivi]]: le istituzioni (Stato, Impresa) esistono precisamente per trasformare PD in giochi dove la cooperazione è sostenibile — attraverso sanzioni (modificano i payoff), contratti (cambiano la struttura del gioco), o ripetizione (→ [[09_Giochi_Ripetuti_Indefiniti]]).
- La collusione tacita tra oligopolisti è un PD risolto dalla ripetizione: il [[10_Folk_Theorem|Folk Theorem]] mostra che la cooperazione implicita è sostenibile se il futuro conta abbastanza — ed è per questo che il diritto antitrust esiste.
