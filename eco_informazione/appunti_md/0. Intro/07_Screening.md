---
title: "Screening: menù di contratti e discriminazione di prezzo"
tags:
  - economia-informazione
  - screening
  - menu-di-contratti
  - discriminazione-di-prezzo
  - auto-selezione
created: 2026-06-20
related:
  - "[[05_Selezione_avversa]]"
  - "[[06_Segnalazione]]"
  - "[[04_Principale_e_agente]]"
  - "[[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali (SPNE)]]"
  - "[[1. GT/03_Nash_Equilibrium|Nash Equilibrium]]"
---

# Screening: menù di contratti

Lo **screening** è la risposta "duale" al [[06_Segnalazione|signalling]] di fronte
alla [[05_Selezione_avversa|selezione avversa]]: qui è la parte **non informata**
(il **principale**) a muovere per primo, offrendo un **menù di contratti** che
induce i diversi tipi di agente ad **auto-selezionarsi** scegliendo *bundle*
diversi.

> [!definition] Screening
> Asimmetria informativa **ex ante** (come nella selezione avversa). Il principale
> *screena* i tipi di agente progettando un menù tale che ogni tipo,
> massimizzando la propria utilità, sceglie **spontaneamente** il contratto
> pensato per lui (es. diversi schemi di compensazione, qualità, quantità).

## La sequenza temporale (*timing*)

> [!definition] Timing dello screening
> $$
> \text{Natura sceglie il tipo}\,(H/L)
> \;\to\;
> \boxed{\text{Principale offre un MENÙ di contratti}}
> \;\to\;
> \text{Agente accetta / rifiuta}
> \;\to\;
> \text{Agente invia un segnale verificabile}
> $$

> [!intuition] Signalling vs. Screening
> | | Chi muove per primo | Strumento |
> |---|---|---|
> | **[[06_Segnalazione\|Signalling]]** | la parte **informata** (agente) | un **segnale** costoso |
> | **Screening** | la parte **non informata** (principale) | un **menù** di contratti |
>
> Entrambi mirano a far emergere l'informazione privata; cambiano il primo mover e
> lo strumento.

## Esempi di screening

- **Assunzioni:** i candidati conoscono la propria abilità, il datore no →
  pacchetti che variano salario, bonus, *research grants*…
- **Finanza:** il debitore conosce il rischio del progetto, il creditore no →
  pacchetti con diversi tassi e requisiti di **collaterale**.
- **Assicurazione:** l'assicurato conosce il proprio rischio, l'assicuratore no →
  pacchetti con diversi **premi** e **franchigie** (*deductibles*); questionari su
  età, stato civile, abitudine al fumo…
- **Pricing:** il compratore conosce la propria valutazione, il venditore no →
  diverse **qualità a diversi prezzi**, o **sconti quantità**.

## La discriminazione di prezzo

Il *pricing* è la forma più diffusa di screening: il venditore non osserva la
disponibilità a pagare e progetta un menù che la rivela.

> [!example] Domande dalle slide
> - Perché compagnie aeree e *autonoleggi* fanno pagare di più a chi **non** passa
>   almeno un sabato notte fuori? (separano *business* da *leisure*).
> - Carta termica per fax / cartucce d'inchiostro; prezzi differenziati via siti web.
> - **Spotify price index:** differenziali di prezzo per Paese.

> [!definition] I tre gradi di discriminazione di prezzo
> - **1° grado (perfetta):** il venditore fa pagare per ogni unità il **massimo
>   prezzo** che il consumatore è disposto a pagare → cattura **tutto** il surplus
>   del consumatore.
> - **2° grado:** prezzo diverso per **quantità** diverse consumate (sconti
>   quantità, tariffe *peak / off-peak*). Il consumatore **si auto-seleziona**.
> - **3° grado:** prezzo diverso per **gruppi** di consumatori diversi (es. tariffe
>   studenti/anziani, prezzi per Paese).

> [!intuition] Lettura grafica
> Nel diagramma domanda–offerta, la discriminazione di prezzo permette al venditore
> di "scendere lungo la curva di domanda" $D$ e appropriarsi delle aree di surplus
> (regioni $A$, $B$, … nelle slide) che sotto prezzo unico $p^\*$ resterebbero al
> consumatore.

## Riferimenti dai libri

> [!quote] Dal libro [BB] — *Information Economics*, cap. 14, "Application: Price–quality discrimination" (p. 322)
> «The insurer can try **separating contracts**, offering a menu with $c_L$ and
> $c_H$. [...] it is the high-risk type who is tempted to buy the contract designed
> for low-risk individuals. [...] The contract for low-risk individuals $c_L$ [...]
> must contain a different repellent for high-risk individuals. This repellent is
> the **incomplete insurance** that comes with $c_L$.»

> [!quote] Dal libro [BB] — cap. 14, "The economic lie detector" (p. 307)
> «[...] how an uninformed party [...] can extract hidden information from an
> informed party. The magic word in this context is **contracting**. The uninformed
> party offers [...] a contract which the informed party must either accept or
> reject. By accepting or rejecting, the informed party **discloses** their hidden
> information.»

- **[BB]** cap. 14 *Optimal contracts* — sez. 14C *Theory: Optimal contracts*
  (p. 312), 14D *Price–quality discrimination* (p. 322). Il modello di
  Rothschild–Stiglitz dei contratti assicurativi separanti.
- **[M]** Molho — capitolo sullo *screening* e i menù di contratti.
- Origine teorica: **J. Stiglitz** (Rothschild–Stiglitz 1976) → [[09_Nobel|Nobel 2001]].

## 🔗 Connessioni con la Teoria dei Giochi

Lo screening è un **gioco sequenziale** ([[1. GT/07_Giochi_Dinamici_Sequenziali|forma estesa]]) in cui il Principale (non informato) muove per primo — speculare al [[06_Segnalazione|signalling]], dove muove l'Agente informato. Il Principale offre un menù di contratti; l'Agente sceglie l'opzione che massimizza la sua utilità, **rivelando** il proprio tipo.

Il [[1. GT/07_Giochi_Dinamici_Sequenziali|SPNE]] del gioco di screening è il menù di contratti ottimale, che soddisfa le vincoli di:
- **Compatibilità con gli incentivi** (*IC*): ogni tipo preferisce il contratto pensato per lui
- **Partecipazione** (*IR*): ogni tipo preferisce accettare che rifiutare

Questo è esattamente la condizione di [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] applicata a ciascun sottogioco del meccanismo: nessun tipo vuole deviare verso il contratto dell'altro tipo, e nessun tipo vuole rifiutare il proprio. La discriminazione di prezzo di 2° e 3° grado sono applicazioni dirette in cui i consumatori "si auto-selezionano" in un menù progettato strategicamente.
