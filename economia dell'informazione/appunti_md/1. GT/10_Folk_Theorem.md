---
tags: [economia-informazione, game-theory, giochi-ripetuti, folk-theorem, equilibri-multipli]
aliases: [Folk Theorem, Teorema del Folklore, Supergame Equilibria]
links: [06_Dilemma_Prigioniero, 09_Giochi_Ripetuti_Indefiniti, 07_Giochi_Dinamici_Sequenziali, 0. Intro/08_Azzardo_morale, 0. Intro/03_Beni_comuni, 0. Intro/04_Principale_e_agente]
---

# Il Folk Theorem

## Definizione Formale

> [!definition] Folk Theorem
> **Enunciato (versione delle slide)**: "In ogni gioco *n*-personale indefinitamente ripetuto, con un insieme finito di azioni in ogni round, ogni profilo di strategie che porta a un payoff atteso medio superiore al payoff dell'equilibrio di Nash dello stage game rappresenta uno SPNE del supergame."
>
> **Requisiti formali**:
> 1. Il fattore di sconto intertemporale $F$ (o la probabilità di continuazione $P$) deve essere **prossimo a 1**
> 2. La probabilità che il gioco finisca a ogni round deve essere **prossima a 0**
>
> Il teorema è chiamato "del folklore" perché è attribuito tradizionalmente alla comunità dei teorici dei giochi senza un'unica fonte originaria.

> [C, p. 208] "Il Folk theorem implica che i giochi indefinitamente e infinitamente ripetuti hanno equilibri multipli e quindi è quasi impossibile fare una previsione chiara di ciò che accadrà effettivamente."

## Intuizione Economica

> [!intuition]
> Il Folk Theorem è allo stesso tempo un risultato potente e sconcertante. Potente perché mostra che, con sufficiente "futuro" in gioco, qualsiasi esito superiore all'equilibrio non-cooperativo dello stage game può essere sostenuto. Sconcertante perché implica che praticamente qualsiasi cosa può succedere in un gioco ripetuto indefinitamente: la teoria non dice *quale* dei moltissimi equilibri possibili verrà selezionato.
>
> Il Folk Theorem trasforma il problema delle *possibilità* (cosa potrebbe succedere) in un non-problema: quasi tutto potrebbe succedere. Il vero problema diventa quello della *selezione dell'equilibrio* — una questione che la teoria dei giochi classica non riesce a risolvere da sola.

## Modello Formale: Lo Spazio dei Payoff

Consideriamo il PD generalizzato con payoff $c > a > d > b$. Lo spazio dei payoff ammissibili nel supergame può essere visualizzato in un diagramma $(\pi_A, \pi_B)$:

- **(a, a)**: payoff della cooperazione reciproca — Pareto ottimale
- **(d, d)**: payoff dell'equilibrio di Nash dello stage game — "minaccia" di base
- **(c, b)** e **(b, c)**: payoff delle combinazioni asimmetriche

Il **frontiera di Pareto** è il segmento che connette i payoff più alti realizzabili congiuntamente.

Il Folk Theorem dice: **tutti i payoff nell'area tratteggiata** (quella che domina l'equilibrio Nash-dello-stage-game $(d,d)$ in entrambe le dimensioni e si trova sotto la frontiera di Pareto) possono essere sostenuti come SPNE del supergame con $P$ (o $F$) sufficientemente alto.

$$\text{Insieme dei payoff SPNE-sostenibili} \supseteq \{(\pi_A, \pi_B) : \pi_A > d, \; \pi_B > d, \; (\pi_A, \pi_B) \text{ ammissibile}\}$$

> [!example] Visualizzazione del Folk Theorem
> Nell'asse dei payoff $(\pi_A, \pi_B)$ con $b < d < a < c$:
> - Il punto $(d,d)$ è l'equilibrio NE dello stage game
> - Il punto $(a,a)$ è la cooperazione reciproca
> - I punti $(c,b)$ e $(b,c)$ sono le combinazioni asimmetriche
>
> La regione tratteggiata — i payoff che dominano strettamente $(d,d)$ in almeno una dimensione e debolmente nell'altra — è l'insieme di ciò che può essere sostenuto dal Folk Theorem.

## Condizioni Aggiuntive per il Folk Theorem

Oltre ai requisiti formali (alta $P$ o $F$), il Folk Theorem richiede:

1. **Stessa coppia di giocatori**: le interazioni avvengono sempre tra gli stessi soggetti. Se i giocatori cambiano ad ogni round (come in mercati anonimi), la punizione non è possibile.

2. **Osservabilità perfetta delle azioni**: ogni giocatore deve poter osservare perfettamente le scelte degli altri. Con monitoring imperfetto, la sostenibilità della cooperazione è più difficile.

3. **Assenza di errori di esecuzione**: le scelte devono essere implementate senza errori casuali. Con errori, le strategie di punizione come *grim* possono innescarsi per sbaglio portando a spirali di defezione non volute.

> [C, p. 209] Queste condizioni limitano l'applicabilità del Folk Theorem ai mercati reali: i mercati anonimi (supermercati, borsa) non soddisfano la condizione di interazioni ripetute tra le stesse coppie.

## Il Problema della Molteplicità degli Equilibri

Il Folk Theorem porta la molteplicità degli equilibri — già un problema nei giochi one-shot — a proporzioni enormi. In un PD ripetuto indefinitamente ci sono letteralmente **infiniti equilibri**: qualsiasi combinazione di trigger strategies che sostenga payoff superiori a $(d,d)$ è un SPNE valido.

Questo significa che la teoria dei giochi, da sola, non può prevedere l'esito di un gioco ripetuto indefinitamente. Sono necessari meccanismi aggiuntivi di selezione:
- **Focali di Schelling**: equilibri che hanno una salienza naturale
- **Equità**: preferenze per outcomes "giusti"
- **Evoluzione e apprendimento**: quali equilibri emergono da processi di adattamento dinamico?

> [C, p. 208–209] "Il Folk Theorem implica che i giochi indefinitamente e infinitamente ripetuti hanno equilibri multipli e quindi è quasi impossibile fare una previsione chiara. Il problema degli equilibri multipli... sembra essere cresciuto a proporzioni da incubo. Ciononostante, l'analisi in questa sezione ha mostrato che nei PD ripetuti infinitamente e indefinitamente dovremmo aspettarci cooperazione almeno alcune volte."

## Il Folk Theorem e l'Economia dell'Informazione

Il Folk Theorem è particolarmente rilevante per l'economia dell'informazione perché:

1. **Reputazione e qualità**: un venditore di [[0. Intro/08_Azzardo_morale|beni di qualità non verificabile (*credence goods*)]] può sostenere prezzi alti grazie alla reputazione — ma questo è possibile solo se il gioco è ripetuto e il venditore non è anonimo.

2. **Mercati con asimmetria informativa**: il Folk Theorem spiega come le relazioni di lungo periodo tra agenti con informazioni asimmetriche (banca-impresa, assicurato-assicuratore, creditore-debitore → [[0. Intro/04_Principale_e_agente|Principale–Agente]]) possano sostenere esiti cooperativi senza enforcement formale.

3. **Collusione implicita in oligopolio**: le imprese oligopolistiche possono colludere tacitamente senza comunicazione esplicita — il Folk Theorem mostra che questa collusione può essere un SPNE. Questo è il fondamento economico di molta politica antitrust.

> [BB, p. 222–224] Birchler & Bütler discutono come nei mercati finanziari le relazioni di lungo periodo tra banca e impresa sostituiscano i contratti formali attraverso esattamente questo meccanismo. La banca "minaccia" di non rifinanziare chi non adempie, il che rende l'adempimento razionale anche senza coercizione legale diretta.

## Relazione con i Concetti Precedenti

```
Stage Game (one-shot)
     │
     ├── Ripetizione FINITA → SPNE unico: Nash dello stage game ovunque
     │                        (paradosso backward induction)
     │
     └── Ripetizione INDEFINITA/INFINITA
           │
           ├── Con P o F piccolo → SPNE unico: Nash dello stage game
           │
           └── Con P o F sufficientemente grande
                     │
                     └── FOLK THEOREM: tutti i payoff nell'insieme ammissibile
                                       che dominano il NE dello stage game
                                       sono SPNE del supergame
                                       (infiniti equilibri possibili)
```

> [!summary] Take-home message
> Il Folk Theorem è il risultato più sorprendente dei giochi ripetuti: quasi tutto ciò che migliora l'equilibrio non-cooperativo dello stage game può essere sostenuto come SPNE, purché il futuro conti abbastanza. Questo spiega perché le relazioni ripetute favoriscono la cooperazione — ma anche perché è così difficile prevedere quale accordo (implicito o esplicito) si realizzerà. Il prezzo della flessibilità è l'indeterminazione: da possibilità teorica a molteplicità dei casi reali, la teoria dei giochi ripetuta indica che *può* succedere ma non *cosa* succederà. Per rispondere a questa domanda occorrono strumenti aggiuntivi: selezione dell'equilibrio, istituzioni, norme sociali.

## 🔗 Connessioni con l'Economia dell'Informazione

Il **Folk Theorem** è il risultato di teoria dei giochi con le implicazioni più vaste per l'economia dell'informazione:

- **[[0. Intro/08_Azzardo_morale|Credence goods e reputazione]]**: il Folk Theorem garantisce che un esperto onesto può sopravvivere nel mercato se le interazioni sono ripetute tra gli stessi soggetti e l'orizzonte è sufficientemente lungo. Questo spiega perché medici, avvocati e meccanici di quartiere (dove c'è ripetizione) si comportano meglio di quelli in mercati anonimi (turisti, passanti).
- **[[0. Intro/03_Beni_comuni|Governance dei commons]]**: il Folk Theorem giustifica formalmente perché le comunità stabili con interazioni ripetute riescono a gestire beni comuni senza privatizzazione né regolazione statale — proprio la tesi di Ostrom (Nobel 2009).
- **Mercati finanziari**: nelle relazioni bancarie di lungo periodo, il Folk Theorem spiega come si sostituiscano contratti formali incompleti con impegni impliciti — rilevante per il framework [[0. Intro/04_Principale_e_agente|Principale–Agente]] con contratti incompleti (Hart, Nobel 2016).
- **Limiti**: il Folk Theorem si applica solo a relazioni con gli stessi soggetti e osservabilità perfetta. Nei mercati anonimi e con monitoring imperfetto (es. assicurazioni), i meccanismi di [[0. Intro/06_Segnalazione|segnalazione]] e [[0. Intro/07_Screening|screening]] diventano necessari proprio perché il Folk Theorem non basta.
