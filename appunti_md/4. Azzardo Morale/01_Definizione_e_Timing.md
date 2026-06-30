---
tags: [economia-informazione, azzardo-morale, hidden-action, timing, principale-agente]
aliases: [Azzardo Morale Definizione, Hidden Action, Azione Nascosta]
links: [02_Setup_Modello_PA]
---

# Azzardo Morale: Definizione, Timing ed Esempi

## Cos'è l'Azzardo Morale

> [!definition]
> L'**azzardo morale** (*moral hazard*) è una forma di asimmetria informativa **ex-post**: l'informazione diventa asimmetrica *dopo* che il contratto è stato firmato e accettato. La parte non informata (il Principale) non può osservare l'azione compiuta dalla parte informata (l'Agente) dopo la firma del contratto. Questa azione non osservabile è detta **azione nascosta** (*hidden action*).

La distinzione temporale rispetto alla [[2. Selezione Avversa/01_Informazione_Asimmetrica_e_Caratteristiche_Nascoste|selezione avversa]] è cruciale:

| | Selezione Avversa | Azzardo Morale |
|---|---|---|
| Asimmetria | Ex-ante (prima del contratto) | Ex-post (dopo il contratto) |
| Cosa è nascosto | **Tipo** (caratteristica) | **Azione** (comportamento) |
| Problema | Selezione sbagliata | Incentivo sbagliato |
| Soluzione tipica | Screening / Segnalazione | Contratto contingente |

> [!intuition]
> Nella selezione avversa il Principale non sa *chi* sta di fronte; nell'azzardo morale il Principale non sa *cosa fa* la persona che ha assunto. Il primo è un problema di selezione, il secondo di comportamento post-contrattuale.

> [BB, ch. 16] L'informazione è asimmetrica *dopo* l'accettazione del contratto. L'Agente compirà un'azione non verificabile dopo la firma.

---

## Il Caso Delle Ferrovie: Un Esempio Storico

Le slide di apertura mostrano due ferrovie in modo non casuale: la linea svizzera Chur–St. Moritz (quello che fu costruito) e la ferrovia sarda (quello che *avrebbe dovuto* essere costruito).

> [!example]
> Un concessionario privato riceve dal governo un contratto per costruire una ferrovia in base alle **miglia richieste** (ad esempio, da Mandas a Tortolì in Sardegna). Una volta firmato il contratto, il costruttore ha la tentazione di costruire **meno miglia** di quelle pattuite, riducendo i costi e intascando la differenza. Il governo non può osservare in tempo reale l'effort del costruttore, né distinguere facilmente tra un cantiere lento per difficoltà tecniche e uno lento per negligenza deliberata. Risultato: meno miglia costruite del contrattato.
>
> Lo stesso schema vale con la ferrovia svizzera: il contratto era per una linea più lunga, ma l'impresa ha interesse a costruire meno. L'azione nascosta è la *qualità e quantità dell'effort* produttivo.

Questo esempio cattura l'essenza dell'azzardo morale: c'è una **discrepanza tra ciò che è contrattato e ciò che viene effettivamente eseguito**, resa possibile dall'impossibilità di osservare e verificare il comportamento dell'Agente.

---

## Il Timing del Gioco

Il modello di azzardo morale si struttura in **quattro periodi** (slide 6):

$$t = 0 \quad \xrightarrow{\quad} \quad t = 1 \quad \xrightarrow{\quad} \quad t = 2 \quad \xrightarrow{\quad} \quad t = 3$$

| Periodo | Chi agisce | Cosa accade |
|---|---|---|
| $t=0$ | Principale | Offre un contratto (proposta take-it-or-leave-it) |
| $t=1$ | Agente | Accetta o rifiuta il contratto |
| $t=2$ | Agente | **Sceglie il livello di sforzo** (work / shirk) — *azione non osservabile* |
| $t=3$ | Natura | Si realizza l'esito del progetto ($X_H$ o $X_L$) |

> [!intuition]
> La chiave del timing è che l'asimmetria nasce **tra $t=1$ e $t=2$**: dopo che l'Agente ha già accettato, compie un'azione che il Principale non può vedere. Il contratto viene scritto a $t=0$, ma lo sforzo viene scelto a $t=2$ — il Principale non può contrattare direttamente su ciò che accade a $t=2$.

Confronta con il timing della selezione avversa, dove l'asimmetria è già presente a $t=0$ (il tipo del venditore è noto a lui ma non al compratore prima ancora che si parli di contratto).

---

## La Delegazione e il Problema Fondamentale

Kenneth Arrow ha catturato il problema alla radice (slide 7):

> "Per definizione, l'Agente è stato selezionato per la sua conoscenza specializzata e il Principale non può mai sperare di controllare completamente le prestazioni dell'Agente."

Questo è il **paradosso della delegazione**: si delega a qualcuno proprio perché è più competente, ma quella competenza superiore rende impossibile la verifica completa delle sue azioni.

> [!intuition]
> La delegazione richiede fiducia, ma la fiducia non basta: serve un **sistema di incentivi** che allinei gli interessi dell'Agente con quelli del Principale. Il problema dell'azzardo morale è esattamente il problema di progettare questo sistema in modo ottimale.

---

## Esempi di Relazioni Principale–Agente con Azione Nascosta

Le relazioni P–A con azzardo morale sono ovunque nell'economia (slide 8):

| Principale | Agente | Azione Nascosta |
|---|---|---|
| Datore di lavoro | Dipendente | Livello di sforzo / impegno |
| Paziente | Medico | Appropriatezza della cura |
| Medico | Paziente | Compliance terapeutica |
| Azionista | Manager | Strategia aziendale (risk-taking) |
| Assicuratore | Assicurato | Grado di cautela / prevenzione |
| Banca | Debitore | Effort per ripagare il prestito |
| Investitore | Banca | Livello di rischio assunto |
| Studente | Docente | Qualità della didattica |
| Docente | Studente | Impegno nello studio |
| P.A. | Appaltatore | Qualità / quantità realizzata |
| Elettori | Politici | Onestà, fedeltà al mandato |

Questi esempi mostrano la pervasività del problema: ogni volta che una parte **delega** un compito a un'altra parte con **interessi non perfettamente allineati** e azioni **non verificabili**, si crea un problema di azzardo morale.

> [BB, ch. 16] Il modello di base ha un Principale di fronte a un Agente. Il Principale offre all'Agente un contratto in base al quale l'Agente esegue il compito delegato dal Principale.

---

## Perché è Necessario un Contratto di Incentivo

Il contratto standard — un salario fisso indipendente dall'esito — non funziona quando lo sforzo è nascosto: l'Agente preferirà sempre "shirk" (non lavorare) poiché riceve lo stesso compenso indipendentemente dall'effort. Per indurre uno sforzo più elevato, il contratto deve:

1. **Essere abbastanza attraente** da far accettare l'Agente (vincolo di partecipazione, PC)
2. **Promettere un rendimento atteso sufficiente** a compensare il costo dello sforzo (vincolo di incentivo, IC)

Se l'Agente è avverso al rischio, soddisfare entrambe queste condizioni con sforzo *non osservabile* avrà un costo: il costo di agenzia. Questo è il tema centrale sviluppato nei modelli formali che seguono.

---

## Take-home Message

> [!summary]
> L'azzardo morale nasce quando l'asimmetria informativa è **ex-post**: l'Agente compie un'**azione nascosta** dopo la firma del contratto ($t=2$) che il Principale non può osservare. Il Principale può contrattare solo sull'esito ($t=3$), non sullo sforzo ($t=2$). La risposta è il **contratto di incentivo**: un contratto che rende il compenso dell'Agente dipendente dall'esito in modo tale da allineare gli interessi. Il problema fondamentale — delegare richiede fiducia ma la fiducia è costosa — percorre tutto il modello.

---

## Vedi Anche

- [[02_Setup_Modello_PA]] — Il setup formale del modello: utilità, effort, esiti, albero del gioco
- [[0. Intro/08_Azzardo_morale|Azzardo Morale (Intro)]] — Panoramica introduttiva del concetto
- [[0. Intro/04_Principale_e_agente|Principale e Agente]] — Il framework generale P–A
- [[2. Selezione Avversa/01_Informazione_Asimmetrica_e_Caratteristiche_Nascoste|Info Asimmetrica]] — Confronto con l'asimmetria ex-ante
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — Il timing $t=0 \to t=3$ è un gioco in forma estesa
