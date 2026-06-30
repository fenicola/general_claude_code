---
tags: [economia-informazione, segnalazione, spence, nash-bayesiano, equilibrio]
aliases: [Modello di Spence, Spence 1973, Equilibrio di Segnalazione]
links: [02_Educazione_come_Segnale_Credibile, 04_Esempio_Numerico_Casi_Base, 05_Equilibrio_Separatore]
---

# Il Modello di Spence (1973): Processo ed Equilibrio

## Il Contesto

> [!definition]
> Il **modello di Spence (1973)** è il primo modello formale di segnalazione sul mercato del lavoro. La parte informata (il lavoratore) conosce la propria produttività; la parte non informata (il datore di lavoro) no, ma osserva un *segnale* correlato — il livello di istruzione $y$ — e su quello basa l'offerta salariale. È l'archetipo di tutti i modelli di segnalazione.

Michael Spence ricevette per questo lavoro (insieme ad Akerlof e Stiglitz) il Premio Nobel per l'economia nel 2001.

> [BB, p. 305] Per i loro lavori sull'asimmetria informativa, ricercatori come George Akerlof, A. Michael Spence e Joseph Stiglitz furono insigniti del Premio Nobel per l'economia nel 2001.

---

## Il Processo di Segnalazione (Timing)

Il processo si articola in cinque passi (slide 11):

1. I **candidati** decidono quanto investire in istruzione (il segnale $y$).
2. I **datori di lavoro** non osservano la produttività ma solo il segnale correlato.
3. I datori si formano **credenze soggettive** (*beliefs*) sulla relazione tra la caratteristica osservabile ($y$) e quella non osservabile (la produttività).
4. Offrono **salari** coerenti con quelle credenze.
5. Dopo l'assunzione, il datore **osserva la produttività** effettiva.

Il punto 3 è il cuore concettuale: l'esito dipende dalle credenze, e queste devono risultare *corrette* in equilibrio.

---

## Definizione di Equilibrio di Segnalazione

> [!definition]
> Un **equilibrio di segnalazione** esiste se e solo se valgono *contemporaneamente* due condizioni (slide 12):
>
> **(a) Ottimalità per i candidati.** Nessun candidato ha incentivo a cambiare la propria decisione di segnalazione, dati i costi dell'istruzione e il salario che ottiene. In altre parole, il segnale scelto è quello che massimizza il rendimento netto disponibile per il suo tipo.
>
> **(b) Ottimalità e coerenza per i datori di lavoro:**
> - (i) le offerte salariali sono **competitive** (profitti attesi normali, cioè nulli in concorrenza);
> - (ii) le **credenze sono confermate**: l'interpretazione del segnale risulta corretta a posteriori.

---

## L'Equilibrio è un Nash Bayesiano

> [!intuition]
> Un equilibrio di segnalazione è un **equilibrio di Nash bayesiano**: la scelta di ciascun giocatore è una *miglior risposta* a quella degli altri (slide 13).
> - I **livelli di istruzione** sono scelti per massimizzare il rendimento, dato il salario offerto e i costi di segnalazione.
> - I **salari** sono scelti per massimizzare i profitti del datore, data la produttività segnalata dalla scelta di istruzione.
>
> In equilibrio nessun giocatore vuole cambiare la propria decisione (*revision test*): se nessuno ha incentivo a deviare unilateralmente, le credenze restano confermate e l'equilibrio è auto-sostenuto.

L'aggettivo *bayesiano* segnala che i datori usano la regola di Bayes per aggiornare le credenze sul tipo a partire dal segnale osservato; l'aggettivo *Nash* che, date quelle credenze e i salari risultanti, le strategie dei lavoratori sono ottimali.

Si noti la struttura ricorsiva tipica dei modelli di segnalazione: **le credenze determinano i salari, i salari determinano le scelte di istruzione, e le scelte di istruzione devono confermare le credenze di partenza.** È un punto fisso.

> [C, p. 165] Nei giochi dinamici con informazione asimmetrica si introducono la regola di Bayes e l'idea di un equilibrio bayesiano, e si esplora il ruolo della segnalazione.

---

## I Possibili Esiti

> [!definition]
> A seconda delle credenze sostenibili in equilibrio, il modello ammette **esiti qualitativamente diversi** (slide 10):
> - I segnali **non vengono trasmessi** (nessuno segnala).
> - I segnali sono trasmessi e **differenziano** i tipi → [[05_Equilibrio_Separatore|equilibrio separatore]].
> - I segnali sono trasmessi ma **non riescono a differenziare** i tipi → [[07_Equilibrio_Aggregante_Pooling|equilibrio aggregante (pooling)]].
> - **Nessun equilibrio** esiste.

Questa molteplicità di esiti è la firma dei modelli di segnalazione: a differenza dell'equilibrio (quasi) unico della [[2. Selezione Avversa/05_Equilibrio_di_Mercato_Adverse_Selection|selezione avversa]], qui credenze diverse e auto-confermanti generano mondi diversi.

---

## Il Setup Numerico della Lezione

Il modello viene reso concreto con un esempio a due tipi (sviluppato in [[04_Esempio_Numerico_Casi_Base]]):

- Due tipi di candidati: **L** con produttività $1$ e quota $q$; **H** con produttività $2$ e quota $1-q$.
- La **produttività è fissa**: l'istruzione *non* la modifica (ipotesi che isola il puro effetto-segnale).
- Il **salario di riserva è molto basso** (i lavoratori accettano comunque di lavorare).
- Costi di segnalazione: $c_L(y)=y$, $c_H(y)=y/2$ (single-crossing, vedi [[02_Educazione_come_Segnale_Credibile]]).

> [BB, p. 338] Per esempio, uno studente si aspetta che il salario aumenti con il livello di istruzione. Tali aspettative costituiscono lo sfondo contrattuale dell'attività di segnalazione.

---

## Take-home message

> [!summary]
> Il modello di Spence (1973) formalizza la segnalazione sul mercato del lavoro: il lavoratore sceglie un livello di istruzione $y$, il datore osserva $y$, forma credenze sulla produttività e offre un salario. Un **equilibrio di segnalazione** è un **Nash bayesiano**: (a) nessun lavoratore vuole cambiare il proprio segnale dati salario e costi; (b) i datori fanno offerte competitive (profitto atteso nullo) e le loro credenze risultano confermate. La struttura è un punto fisso fra credenze, salari e scelte di istruzione. A seconda delle credenze auto-confermanti, l'esito può essere separatore (tipi distinti), aggregante (tipi indistinti) o di non-esistenza: è la molteplicità tipica della segnalazione.

---

## Vedi anche

- [[02_Educazione_come_Segnale_Credibile]] — Perché il segnale è credibile (single-crossing), ingrediente della condizione (a)
- [[04_Esempio_Numerico_Casi_Base]] — Il setup numerico e i regimi informativi a confronto
- [[05_Equilibrio_Separatore]] — L'esito che differenzia i tipi
- [[07_Equilibrio_Aggregante_Pooling]] — L'esito che non differenzia i tipi

---

## Connessioni con il Vault

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — l'equilibrio di segnalazione *è* un Nash (bayesiano): nessuno devia unilateralmente date le strategie altrui. Il *revision test* della slide 13 è la definizione operativa di Nash
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — il timing (segnale → salario) è un gioco in forma estesa con informazione incompleta; l'equilibrio rilevante è perfetto nei sottogiochi e bayesiano
- [[1. GT/04_Giochi_Coordinamento|Giochi di Coordinamento]] — la molteplicità di equilibri auto-confermanti ha la stessa natura del problema di coordinamento sulle aspettative

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/05_Equilibrio_di_Mercato_Adverse_Selection|Equilibrio di Mercato]] — contrasto utile: lì l'equilibrio è (quasi) unico e Pareto-inferiore; qui la segnalazione introduce molteplicità e possibilità di separazione
