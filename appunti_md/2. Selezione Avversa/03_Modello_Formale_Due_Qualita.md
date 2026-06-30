---
tags: [economia-informazione, selezione-avversa, modello-formale, birchler-butler]
aliases: [Modello Due Qualità, Partial Market Failure, BB Cap 13]
links: [02_Mercato_dei_Limoni_Intuizione, 04_Modello_Akerlof_Formale, 08_Distribuzioni_di_Probabilita_Richiamo]
---

# Il Modello Formale: Due Qualità e Selezione Avversa

## Il Setup

> [!definition]
> Il modello semplificato di Birchler & Bütler (cap. 13) analizza un mercato di beni eterogenei in qualità con informazione asimmetrica. Le assunzioni chiave sono:
> - Due soli livelli di qualità con uguale frequenza (50%-50%)
> - Metà delle auto vale $5.000, l'altra metà $10.000
> - I **venditori** conoscono la qualità effettiva della propria auto
> - I **compratori** non osservano la qualità; conoscono solo la distribuzione
> - I compratori fanno offerte *take-it-or-leave-it* ai venditori

Questo è il caso più semplice per capire la logica della selezione avversa prima di passare al modello continuo di Akerlof ([[04_Modello_Akerlof_Formale]]).

---

## La Strategia Ottimale del Venditore

La miglior risposta (*best response*) del venditore a un prezzo offerto $p$ è semplice:

$$
\text{Vendi se e solo se } p \geq V
$$

dove $V$ è il valore reale dell'auto, noto al venditore. Non c'è incertezza dal lato del venditore. Se il prezzo copre il suo costo opportunità (il valore che attribuisce all'auto), vende; altrimenti no.

> [BB, p. 279] La miglior risposta di un venditore a un prezzo $p$ offerto da un compratore è: accetta se il prezzo $p$ è almeno uguale al valore dell'auto $V$ (cioè se $p \geq V$), altrimenti rifiuta.

---

## La Funzione di Valore Atteso del Compratore

Il compratore non può osservare $V$. Tuttavia, sa che il venditore accetta solo se $p \geq V$. Quindi, se il compratore offre il prezzo $p$, sa che la qualità dell'auto che riceverà soddisfa $V \leq p$.

Il valore atteso dell'auto che il compratore riceverà, data un'offerta $p$, è:

$$
E[V \,|\, p] = E[V \,|\, V \leq p]
$$

Questo è il **valore atteso condizionato** — la media dei valori delle auto che il venditore sarebbe disposto a cedere a quel prezzo.

Nel caso discreto con due qualità ($V = 5.000$ o $V = 10.000$, con uguale probabilità):

- Se $p < 5.000$: nessuna auto viene offerta → $E[V|p] = 0$
- Se $5.000 \leq p < 10.000$: solo l'auto da $5.000$ viene offerta → $E[V|p] = 5.000$
- Se $p \geq 10.000$: entrambe le auto vengono offerte → $E[V|p] = 7.500$

Questa funzione è una **funzione a gradini**: sale bruscamente in corrispondenza dei valori di qualità.

> [BB, p. 279-280] La funzione di valore atteso può essere vista come una curva di "offerta". Descrive il valore atteso — cioè la qualità media — offerta in funzione del prezzo (a differenza di una curva di offerta standard che descrive la *quantità* in funzione del prezzo).

---

## La Curva di Domanda del Compratore

Il compratore accetterà l'acquisto solo se il valore atteso dell'auto è almeno pari al prezzo pagato:

$$
E[V|p] \geq p
$$

Questa è la condizione di **partecipazione del compratore**. Graficamente, corrisponde alla retta a 45° nel piano $(p, E[V])$, che rappresenta il valore atteso minimo richiesto per indurre il compratore ad acquistare.

---

## L'Equilibrio di Mercato

Combinando le due curve:

- **"Offerta"** (funzione di valore atteso): $E[V|V \leq p]$ — descrive la qualità media offerta in funzione di $p$
- **"Domanda"** (condizione di partecipazione): $E[V] = p$ — il compratore compra solo se il valore atteso eguaglia il prezzo

L'equilibrio si trova dove le due curve si intersecano:

$$
p^* = E[V|V \leq p^*] = 5.000
$$

**Interpretazione**: l'unico equilibrio è a $p^* = 5.000$. A questo prezzo, solo le auto da $5.000$ vengono offerte. Se il compratore provasse ad alzare il prezzo a $10.000$ per attrarre anche le auto di alta qualità, il valore atteso sarebbe $7.500 < 10.000$ → il compratore farebbe una perdita. Se invece offre meno di $5.000$, nessun venditore accetta.

Esito: **solo il 50% delle auto viene scambiato** (quelle di bassa qualità). Le auto da $10.000$ rimangono invendute nonostante ci siano potenziali guadagni dallo scambio.

> [BB, p. 280] Il mercato è in equilibrio a $p = E[V] = 5.000$. Solo le auto di bassa qualità vengono vendute. Un compratore che annunciasse un prezzo tale da portare al mercato le auto di alta qualità farebbe una perdita. Esattamente il 50% del parco auto verrà venduto. L'altra metà, migliore, non viene venduta.

---

## Estensione: Qualità Continue (Distribuzione Uniforme)

Se le qualità sono distribuite in modo continuo e uniforme tra $\$5.000$ e $\$10.000$ (cioè $V \sim U[5.000, 10.000]$), l'esito è ancora più drastico:

- Per $p < 5.000$: nessuna auto offerta
- Per $5.000 \leq p \leq 10.000$: la qualità media delle auto offerte è $E[V|V \leq p] = \frac{5.000 + p}{2}$
- Questa è sempre inferiore a $p$ per ogni $p > 5.000$ → il compratore non acquista
- L'unico equilibrio è $p = 5.000$, dove quasi nessuna auto viene venduta

Il mercato **collassa quasi completamente**: rimane solo il bene di qualità minima.

> [BB, p. 281] Il completo fallimento del mercato in questo contesto non è di per sé un problema: le auto hanno lo stesso valore comune per venditori e compratori. Dal punto di vista del benessere sociale è irrilevante chi possiede l'auto. Il fallimento del mercato *di per sé* non è inefficiente. Un esito di mercato è inefficiente solo quando un'auto non viene venduta, sebbene valga di più per un potenziale compratore che per il proprietario attuale.

---

## Estensione: Guadagni Dallo Scambio (Caso con $a > 1$)

> [!definition]
> Supponiamo ora che le auto abbiano **valore diverso per compratore e venditore**: $V = a \cdot V_S$ con $a > 1$. Il compratore valuta l'auto $a$ volte più del venditore. Questo rappresenta i *guadagni dallo scambio* (*gains from trade*): esiste un surplus potenziale dallo scambio.

La funzione di valore atteso del compratore diventa:

$$
E[V|p] = E[a V_S \,|\, V_S \leq p] = a \cdot E[V_S \,|\, V_S \leq p]
$$

Con $a = 1,2$ (compratori valorizzano le auto il 20% in più):

- Questa funzione è traslata **verso l'alto** rispetto al caso $a=1$
- Esiste ora un range di prezzi per cui $E[V|p] > p$ → il compratore accetta
- L'equilibrio è a $p^* = 7.500$ con qualità media venduta $E[V_S] = 6.250$

Tuttavia, l'esito rimane **inefficiente**: metà delle auto (quelle di qualità superiore) rimangono invendute, anche se i compratori le valorizzerebbero più degli attuali proprietari.

> [BB, p. 282] Sebbene il mercato non collassi completamente (come nell'esempio precedente), l'esito è inefficiente. La metà migliore delle auto rimane invenduta, sebbene i compratori la valorizzerebbero più degli attuali proprietari. Questo fenomeno si chiama *selezione avversa*.

---

## Guadagni Dallo Scambio: Chi Guadagna e Chi Perde?

Con $a = 1,2$ e qualità distribuita uniformemente tra $5.000$ e $10.000$:

- Valore aggregato delle auto per i venditori: $7.500$ (il valore medio)
- Guadagni potenziali totali dallo scambio: $20\% \times 7.500 = 1.500$
- Con informazione completa, tutti i guadagni andrebbero ai compratori (che fanno offerte)
- Con asimmetria informativa: solo $7.500 - 7.500 \times 50\% = 3.750$ viene scambiato → perdita di benessere

I venditori di beni di bassa qualità creano una **esternalità negativa** sui venditori di beni di alta qualità: la loro presenza abbassa la qualità media percepita, rendendo impossibile per i venditori di alta qualità ottenere un prezzo adeguato.

> [BB, p. 283] I venditori di beni di bassa qualità acquisiscono quote relativamente alte dei guadagni realizzati dallo scambio; la loro presenza crea un'esternalità negativa per tutti i venditori di beni di alta qualità (che non riescono a vendere) e per i venditori di qualità mediana (che ottengono meno di quanto avrebbero ottenuto con qualità osservabile).

---

## Take-home message

> [!summary]
> Il modello a due qualità di Birchler & Bütler (BB cap. 13) illustra con la massima chiarezza il meccanismo della selezione avversa: il compratore, non potendo osservare la qualità, forma aspettative sulla qualità media delle auto che il venditore è disposto a cedere a quel prezzo. Questa aspettativa è sistematicamente inferiore al prezzo che sarebbe necessario per attrarre le auto di alta qualità. L'equilibrio si stabilisce solo sul bene peggiore. Quando si aggiungono guadagni dallo scambio ($a > 1$), il mercato non collassa del tutto, ma rimane inefficiente: le auto di alta qualità non vengono scambiate pur esistendo un surplus potenziale.

---

## Vedi anche

- [[01_Informazione_Asimmetrica_e_Caratteristiche_Nascoste]] — La struttura temporale dell'asimmetria
- [[02_Mercato_dei_Limoni_Intuizione]] — L'intuizione qualitativa
- [[04_Modello_Akerlof_Formale]] — Il modello completo con funzioni di utilità esplicite
- [[05_Equilibrio_di_Mercato_Adverse_Selection]] — L'equilibrio di zero scambi nel dettaglio
- [[08_Distribuzioni_di_Probabilita_Richiamo]] — Ripasso sulla distribuzione uniforme

---

## Connessioni con il Vault

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — l'equilibrio grafico di questo modello (intersezione domanda/offerta) *è* un Nash Equilibrium: nessun agente vuole deviare unilateralmente date le aspettative degli altri
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — la struttura del modello BB (compratore forma aspettative, poi decide) si formalizza naturalmente come gioco in forma estesa; il NE del gioco è l'equilibrio di mercato qui analizzato
- [[1. GT/01_Strategia_Dominante|Strategia Dominante]] — vendere un'auto di bassa qualità è strategia (debolmente) dominante per il venditore di fronte a un compratore che non distingue i tipi
