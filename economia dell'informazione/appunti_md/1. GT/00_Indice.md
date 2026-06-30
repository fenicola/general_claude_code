---
tags: [economia-informazione, game-theory, indice]
aliases: [Indice Game Theory, Mappa GT]
links: [0. Intro/01_Coordinamento_e_incentivi, 0. Intro/03_Beni_comuni, 0. Intro/04_Principale_e_agente]
---

# 🗺️ Teoria dei Giochi — Mappa Concettuale

> Lezioni 4 e 5 — Prof. Vittorio Pelligra  
> Riferimento principale: [C] Carmichael, *A Guide to Game Theory*, capp. 1–3

---

## Filo Logico dell'Argomento

La teoria dei giochi studia le **situazioni di interdipendenza strategica**: contesti in cui il risultato delle mie azioni dipende dalle azioni altrui. Il percorso concettuale si articola in tre fasi.

**Fase 1 — Costruire il gioco** (slide 4): Prima di risolvere un gioco, occorre descriverlo. Ogni gioco è definito da giocatori, strategie, informazione, mosse e payoff. La rappresentazione può essere *in forma strategica* (matrice) o *in forma estesa* (albero). La distinzione fondamentale riguarda il *timing*: i giochi simultanei (statici) contrappongono quelli dinamici (sequenziali e ripetuti).

**Fase 2 — Risolvere il gioco** (slide 4-5): La soluzione richiede congetture razionali sulle altrui scelte. Si procede per forza crescente del concetto d'equilibrio:
1. [[01_Strategia_Dominante]] → criterio più forte: un'azione che è sempre la migliore risposta
2. [[02_Iterated_Dominance]] → eliminazione iterativa delle strategie dominate
3. [[03_Nash_Equilibrium]] → criterio più generale: mutua miglior risposta

Ogni equilibrio di strategia dominante è un Nash, ma non viceversa.

**Fase 3 — Giochi con struttura speciale** (slide 5): Tre grandi famiglie di giochi mostrano come la struttura delle preferenze generi esiti radicalmente diversi:
- [[04_Giochi_Coordinamento]] (Stag Hunt, puntualità): *equilbri Pareto-ordinabili*
- [[05_Chicken_Game]] (guerra di attrito): *equilibri Pareto-non-ordinabili*
- [[06_Dilemma_Prigioniero]]: *il classico conflitto cooperazione/defezione*

**Fase 4 — Tempo e ripetizione** (slide 5): Quando il gioco si ripete, la strategia cambia natura: occorre pianificare per tutto l'orizzonte temporale.
- [[07_Giochi_Dinamici_Sequenziali]]: backward induction e SPNE
- [[08_Giochi_Ripetuti_Finiti]]: il paradosso dell'induzione a ritroso
- [[09_Giochi_Ripetuti_Indefiniti]]: trigger strategies e condizioni di cooperazione
- [[10_Folk_Theorem]]: molteplicità degli equilibri nella ripetizione infinita/indefinita

---

## Schema dei Concetti e dei Loro Legami

```
DESCRIZIONE DEL GIOCO
│
├── Forma Strategica (matrice payoff)
│     └── giochi simultanei/statici
└── Forma Estesa (albero di gioco)
      └── giochi dinamici/sequenziali

CONCETTI DI EQUILIBRIO (dal più forte al più debole)
│
├── Equilibrio in Strategie Dominanti
│     └── ⊂ Equilibrio per Dominanza Iterata
│              └── ⊂ Nash Equilibrium
│
└── (Nei giochi dinamici)
      └── Nash ⊃ Subgame Perfect Nash Equilibrium (SPNE)

CLASSI DI GIOCHI NOTEVOLI
│
├── Giochi di Coordinamento
│     ├── Stag Hunt (equilibri Pareto-ordinabili)
│     └── Battle of the Sexes (equilibri Pareto-non-ordinabili)
│
├── Chicken Game (guerra di attrito)
│
└── Dilemma del Prigioniero
      └── Soluzione nei giochi ripetuti:
            ├── Ripetizione finita → paradosso backward induction
            ├── Ripetizione indefinita → trigger strategies
            └── Folk Theorem
```

---

## Mappa delle Note

| File | Concetto | Argomento slide |
|------|----------|-----------------|
| [[01_Strategia_Dominante]] | Strategia strettamente/debolmente dominante; equilibrio | Lec 4, slide 10-12 |
| [[02_Iterated_Dominance]] | Eliminazione iterativa; iterated-dominance equilibrium | Lec 4, slide 13-20 |
| [[03_Nash_Equilibrium]] | Nash Eq.; revision test; relazione con altri equilibri | Lec 4, slide 21-26 |
| [[04_Giochi_Coordinamento]] | Stag Hunt; equilibri Pareto-ordinabili; fiducia sociale | Lec 5, slide 2-6 |
| [[05_Chicken_Game]] | Chicken; guerra di attrito; equilibri non-ordinabili | Lec 5, slide 7-8 |
| [[06_Dilemma_Prigioniero]] | PD; cooperazione; soluzioni istituzionali | Lec 5, slide 9-11 |
| [[07_Giochi_Dinamici_Sequenziali]] | Forma estesa; SPNE; backward induction | Lec 5, slide 12-21 |
| [[08_Giochi_Ripetuti_Finiti]] | Ripetizione finita; paradosso | Lec 5, slide 24 |
| [[09_Giochi_Ripetuti_Indefiniti]] | Trigger strategies; grim; TFT; condizione P | Lec 5, slide 25-33 |
| [[10_Folk_Theorem]] | Folk Theorem; molteplicità equilibri; stage game | Lec 5, slide 34-37 |

---

> [!summary] Messaggio chiave
> La Teoria dei Giochi fornisce il linguaggio per analizzare l'interdipendenza strategica. Il Nash Equilibrium è il concetto centrale, ma la sua generalità è anche la sua debolezza: molti giochi ne hanno più di uno, e nei giochi dinamici occorre raffinarlo in SPNE. Il Dilemma del Prigioniero e i giochi ripetuti mostrano come il *tempo* e la *reputazione* possano trasformare l'equilibrio non-cooperativo in cooperazione sostenuta.

---

## 🔗 Connessioni con l'Economia dell'Informazione

La Teoria dei Giochi è il **linguaggio formale** dell'Economia dell'Informazione. I concetti sviluppati in questa sezione trovano applicazione diretta nei temi della cartella [[0. Intro/00_Indice|Introduzione]]:

| Concetto GT | Applicazione in Economia dell'Informazione |
|-------------|-------------------------------------------|
| [[01_Strategia_Dominante]] | La defezione nel [[0. Intro/06_Dilemma_Prigioniero\|PD]] / il dilemma del pescatore [[0. Intro/03_Beni_comuni\|beni comuni]] |
| [[03_Nash_Equilibrium]] | Equilibri di mercato con asimmetria informativa [[0. Intro/04_Principale_e_agente\|P–A]] |
| [[04_Giochi_Coordinamento]] | Il mercato come elaboratore di info [[0. Intro/02_Mercato_e_Hayek\|Hayek]]; fallimenti di coordinamento |
| [[06_Dilemma_Prigioniero]] | Beni comuni [[0. Intro/03_Beni_comuni\|commons]]; collusione vs. concorrenza; azzardo morale [[0. Intro/08_Azzardo_morale\|moral hazard]] |
| [[07_Giochi_Dinamici_Sequenziali]] | Segnalazione [[0. Intro/06_Segnalazione\|signalling]], screening [[0. Intro/07_Screening\|screening]], contratti [[0. Intro/08_Azzardo_morale\|ottimali]] |
| [[09_Giochi_Ripetuti_Indefiniti]] | Reputazione, qualità credibile, *credence goods* [[0. Intro/08_Azzardo_morale\|azzardo morale]] |
| [[10_Folk_Theorem]] | Molteplicità degli equilibri contrattuali; collusione tacita; governance dei beni comuni [[0. Intro/03_Beni_comuni\|commons]] |
