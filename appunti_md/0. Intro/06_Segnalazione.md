---
title: "Segnalazione (signalling): segnali costosi e credibili"
tags:
  - economia-informazione
  - signalling
  - segnalazione
  - handicap-principle
  - istruzione
  - IPO
created: 2026-06-20
related:
  - "[[05_Selezione_avversa]]"
  - "[[07_Screening]]"
  - "[[04_Principale_e_agente]]"
  - "[[09_Nobel]]"
  - "[[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali (SPNE)]]"
  - "[[1. GT/05_Chicken_Game|Chicken Game (impegno credibile)]]"
---

# Segnalazione (*signalling*)

Il **signalling** è una risposta alla [[05_Selezione_avversa|selezione avversa]]:
è la parte **informata** (l'agente) che, di propria iniziativa, **rivela** la sua
qualità inviando un **segnale costoso e credibile**.

## La sequenza temporale (*timing*)

> [!definition] Timing del signalling
> $$
> \text{Natura sceglie il tipo}\,(H/L)
> \;\to\;
> \boxed{\text{Agente invia un segnale}}
> \;\to\;
> \text{Principale offre un contratto}
> \;\to\;
> \text{Agente accetta / rifiuta}
> $$
> Come nella selezione avversa, l'informazione è nascosta **ex ante**; la novità è
> che la parte informata **può segnalare credibilmente** la propria informazione
> (es. la qualità) prima del contratto.

## La condizione di credibilità

> [!theorem] Un segnale funziona solo se è costoso (in modo differenziale)
> Un segnale separa i tipi **solo se** i tipi a **bassa** qualità **non possono
> imitarlo in modo profittevole**. Formalmente serve una **single-crossing /
> condizione di costo decrescente nel tipo**: il segnale deve costare **meno** ai
> tipi alti che ai tipi bassi.
>
> Esempio: un titolo di studio difficile, ma **più facile da ottenere per i
> lavoratori di alta abilità**, è un segnale credibile — anche se **non aumenta**
> la produttività.

> [!intuition] Perché conviene a entrambi
> - I lavoratori di **alta abilità** sono disposti a sostenere il costo del segnale
>   per distinguersi → ottengono un salario più alto.
> - Un segnale **onesto e credibile** è conveniente sia per l'agente sia per il
>   principale: **riduce** l'inefficienza da selezione avversa (anche se non la
>   elimina del tutto).

## Il principio del *handicap* (segnalazione onesta)

> [!example] Teoria della segnalazione onesta — *Handicap Principle*
> In biologia (Zahavi), un segnale è credibile proprio perché **costoso/rischioso**:
> la coda del pavone o il *"land diving"* di Vanuatu (tuffo dalla torre con liane)
> sono "handicap" che solo gli individui realmente in forma possono permettersi.
> Stessa logica del segnale economico: la credibilità nasce dal costo.

## Esempi economici di segnali

- **Istruzione** come segnale dell'abilità del lavoratore (Spence).
- **Garanzie** (*warranties*) sui prodotti.
- **Etichette e *rating*** (labels & ratings).
- **L'arrossire** (*blush*) — segnale involontario e quindi credibile.
- **Il dono** (*gift-giving*).

> [!example] Il dono come segnale — Waldfogel (1993)
> Waldfogel, *"The Deadweight Loss of Christmas"* (AER 1993): nei regali chi compra
> ≠ chi consuma → rischio di *mismatch* → **perdita secca** stimata tra 1/10 e 1/3
> del valore. Ma il dono ha anche un **valore segnaletico**: non è solo un
> trasferimento di utilità, è un **messaggio** che segnala (1) conoscenza del
> destinatario, (2) impegno e tempo, (3) *commitment* alla relazione, (4) fiducia e
> intimità, (5) status e riconoscimento.

> [!example] Signalling e IPO (*initial public offering*)
> Gli investitori hanno informazione limitata sul vero valore dell'impresa →
> rischio di *mispricing*. Le imprese con buone prospettive **segnalano** la
> qualità:
> - il proprietario **mantiene il controllo** (non vende tutto);
> - le azioni sono offerte a **prezzo scontato** (*underpricing*).
>
> Gli investitori inferiscono razionalmente che **solo i migliori** possono
> recuperare il costo del segnale con le emissioni successive. (Vedi [BB] cap. 12,
> *the underpricing of IPOs*, p. 266.)

## Riferimenti dai libri

> [!quote] Dal libro [BB] — *Information Economics*, cap. 14, problema sul signalling (p. 338)
> Esempio di segnalazione formalizzato: l'utilità di Bob è
> $$ U = a - \tfrac{1}{\theta}\, b, $$
> dove $a\in[0,1]$ è l'apprezzamento (non osservabile) di Alice, $b$ le ore spese
> nel "segnale" (babysitting) e $\theta$ il tipo di Bob ($\theta_0$ uncool …
> $\theta_1$ cool). Il costo del segnale **decresce nel tipo** $\theta$: i tipi
> alti segnalano a costo minore → segnale credibile (figura 14.14).

> [!quote] Dal libro [C] — *A Guide to Game Theory*, cap. 7 "Mystery players"
> §7.3 *Entry deterrence with signalling* (p. 173), §7.5 *The beer and quiche
> signalling game* (p. 178): i giochi di segnalazione con informazione incompleta
> e gli equilibri *separating* / *pooling*.

- **[BB]** cap. 14, sez. signaling (fig. 14.14, p. 338); cap. 12 *underpricing of
  IPOs* (p. 266).
- **[C]** cap. 7, giochi di segnalazione (*beer and quiche*).
- **[M]** Molho — capitolo sul *signalling* (modello di Spence sull'istruzione).
- Origine: **M. Spence**, *Job Market Signaling* (1973) → [[09_Nobel|Nobel 2001]].

## 🔗 Connessioni con la Teoria dei Giochi

Il *signalling* è per eccellenza un **gioco sequenziale con informazione asimmetrica** ([[1. GT/07_Giochi_Dinamici_Sequenziali|forma estesa]]): la parte informata muove per prima (invia il segnale), quella non informata aggiorna le proprie credenze e risponde (offre il contratto). Gli equilibri rilevanti sono:

- **Equilibrio separante** (*separating equilibrium*): i due tipi scelgono segnali diversi → il Principale li identifica perfettamente. È uno [[1. GT/07_Giochi_Dinamici_Sequenziali|SPNE]] in cui il segnale è credibile.
- **Equilibrio pooling**: entrambi i tipi scelgono lo stesso segnale → nessuna informazione viene rivelata.

La condizione di credibilità del segnale (costo differenziale per tipo) richiama il concetto di [[1. GT/05_Chicken_Game|impegno credibile]] nel Chicken Game: il segnale funziona esattamente perché è costoso, come una minaccia credibile in un gioco di deterrenza. Il *beer and quiche game* di Cho & Kreps (1987) è analizzato da Carmichael in [[1. GT/07_Giochi_Dinamici_Sequenziali|cap. 7]] e mostra come l'equilibrio separante sopravviva al *Intuitive Criterion*.
