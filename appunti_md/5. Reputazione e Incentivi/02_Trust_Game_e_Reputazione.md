---
tags: [economia-informazione, reputazione, teoria-dei-giochi, trust-game]
aliases: [Trust Game, Gioco della Fiducia, Trust Game e Reputazione]
links: [01_Mercati_Reputazionali, 03_Bolton_Katok_Ockenfels]
---

# Trust Game e Reputazione

## Il gioco della fiducia

Lo scambio in un mercato con asimmetria informativa può essere descritto come un **gioco sequenziale** detto *trust game* (gioco della fiducia), con due giocatori: un **compratore** (*buyer*) e un **venditore** (*seller*).

> [!definition] Struttura del trust game
> 1. Il **compratore** decide se *comprare* (mandare i soldi) oppure *non comprare*.
> 2. Se non compra → si resta nello **status quo**: entrambi ottengono **(35, 35)**.
> 3. Se compra → il **venditore** decide se *mandare* il bene oppure *non mandarlo*.
>    - *Send* → si realizzano i guadagni dallo scambio: **(50, 50)**.
>    - *Don't send* → il venditore tiene soldi e bene: **(0, 70)**, il compratore è derubato.

I payoff catturano l'idea che lo scambio crea valore (50+50 > 35+35), ma che il venditore, *se potesse agire impunemente*, preferirebbe non spedire (70 > 50).

## L'equilibrio one-shot: il non-scambio

Si risolve per **backward induction** (→ [[1. GT/07_Giochi_Dinamici_Sequenziali|SPNE]]):

- Nell'ultimo nodo il venditore sceglie tra *send* (50) e *don't send* (70): sceglie **don't send**.
- Anticipandolo, il compratore sceglie tra *buy* (che gli darebbe 0) e *don't buy* (35): sceglie **don't buy**.

> [!warning] Equilibrio Pareto-inefficiente
> L'equilibrio di Nash perfetto nei sottogiochi del gioco *one-shot* è
> **(don't buy, don't send)**: il mercato **collassa**, non avviene alcuno
> scambio, pur esistendo guadagni dallo scambio. È la stessa logica del
> [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]] e del non-scambio nel
> [[2. Selezione Avversa/02_Mercato_dei_Limoni_Intuizione|mercato dei limoni]].

La minaccia della causa legale non basta a disciplinare il venditore: per un bene di basso valore, il costo degli avvocati renderebbe la causa irrazionale. Serve un altro meccanismo.

## Come la reputazione cambia il gioco

Se il gioco è ripetuto **e** il comportamento passato del venditore è osservabile da tutti i futuri compratori, si crea di fatto un unico **super-game**: ogni compratore, pur incontrando il venditore una sola volta, eredita la storia delle interazioni precedenti.

> [!intuition]
> Con un sistema reputazionale, il venditore che oggi "non manda" perde la
> fiducia di *tutti* i compratori futuri. Se la probabilità di nuovi scambi è
> sufficientemente alta, il valore dei guadagni futuri dalla cooperazione supera
> il guadagno immediato dell'inganno: il [[1. GT/10_Folk_Theorem|Folk Theorem]]
> garantisce che *send* possa diventare parte di un equilibrio.

**Previsioni teoriche estreme:**
- Gioco *one-shot* senza reputazione → **0% di scambi** (equilibrio di non-scambio).
- Gioco con reputazione → **100% degli scambi** vantaggiosi dovrebbe realizzarsi.

> [!note]
> Nessuna delle due previsioni è esatta: la realtà sta nel mezzo. Lo dimostra
> l'esperimento di laboratorio di [[03_Bolton_Katok_Ockenfels|Bolton, Katok &
> Ockenfels]], che misura quanto effettivamente la reputazione migliora
> l'efficienza.

## 🔗 Connessioni

- Cornice generale: [[01_Mercati_Reputazionali]]
- Verifica sperimentale: [[03_Bolton_Katok_Ockenfels]]
- Strumenti formali: [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali (SPNE, backward induction)]], [[1. GT/10_Folk_Theorem|Folk Theorem]], [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]]
- Analogia strutturale: [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]], [[4. Azzardo Morale/09_Beni_di_Credenza|Beni di Credenza]]
