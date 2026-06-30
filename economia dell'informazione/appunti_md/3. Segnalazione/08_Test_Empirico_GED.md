---
tags: [economia-informazione, segnalazione, empirico, capitale-umano, GED, diff-in-diff]
aliases: [Test Empirico Segnalazione, GED, Tyler Murnane Willett, Capitale Umano vs Segnalazione]
links: [02_Educazione_come_Segnale_Credibile, 05_Equilibrio_Separatore, 06_Proprieta_Equilibrio_Separatore]
---

# Test Empirico: Capitale Umano vs Segnalazione (lo studio GED)

## Il Problema dell'Identificazione

> [!definition]
> Il **modello di segnalazione** (l'istruzione *rivela* la produttività) e il **modello del capitale umano** (l'istruzione *crea* produttività) fanno le **stesse previsioni di superficie**. Distinguerli empiricamente richiede un disegno di ricerca capace di separare i due effetti.

Implicazioni condivise dai due modelli (slide 51):

1. Chi ha più anni di scuola è più produttivo → **SÌ** in entrambi (per il capitale umano perché la scuola crea produttività; per la segnalazione perché solo i produttivi raggiungono l'istruzione alta).
2. Chi ha più scuola riceve salari più alti → **SÌ** in entrambi.
3. Le persone vanno a scuola da giovani, prima di entrare nel mercato → **SÌ** in entrambi.

Poiché le previsioni coincidono, osservare la correlazione "istruzione–salario" **non distingue** i due modelli.

---

## Quali Test Funzionano e Quali No

Si passano in rassegna possibili strategie (slide 52–53):

| Test | Distingue i modelli? | Perché |
|---|---|---|
| Misurare se i più istruiti sono più produttivi | **NO** | Vero in entrambi |
| Misurare la produttività prima/dopo l'istruzione | concettualmente OK | molto difficile da realizzare |
| Verificare se i più capaci vanno a scuola | **NO** | Vero in entrambi (certo nella segnalazione) |
| Assegnare *casualmente* il college a persone di pari abilità e confrontare i salari | **NO** | Entrambi prevedono salari più alti |
| **Assegnare *casualmente* un diploma a persone di pari abilità** e vedere se i diplomati guadagnano di più | **SÌ** | È un test *puro* di segnalazione |

> [!intuition]
> La chiave è separare il **diploma** (il segnale) dall'**istruzione** (che crea capitale umano). Se si assegna il *pezzo di carta* a persone con identica abilità e formazione, il modello del capitale umano predice salari uguali (stessa abilità ⇒ stessa produttività), mentre il modello di segnalazione predice salari più alti per chi ha il diploma (il segnale fa la differenza). È l'unico test che li discrimina.

---

## Lo Studio: Tyler, Murnane & Willett (2000)

> [!definition]
> **Tyler, Murnane & Willett (2000)** studiano se il **GED** (*General Educational Development certificate* — il diploma di scuola superiore ottenuto tramite esame, alternativo al percorso scolastico tradizionale) aumenti i salari futuri di chi lo consegue. La domanda è rilevante per le politiche educative.

Contesto (slide 54):
- Nel 1996, il $9{,}8\%$ dei 18–24enni aveva completato la *High School* tramite GED, contro il $76{,}5\%$ con diploma tradizionale.
- Tra 1990 e 1996 i tassi di diploma tradizionale erano crollati per i neri non ispanici; l'aumento del GED aveva compensato il calo. Era quindi importante capire se i titolari di GED stessero almeno un po' meglio dei *dropout* senza titolo.

I dati grezzi (slide 55, Tabella II) mostrano che i **titolari di GED guadagnano meno dei diplomati tradizionali ma più dei dropout** senza titolo.

---

## Il Problema della Self-Selection

> [!intuition]
> Il confronto grezzo dei salari **non identifica l'effetto causale del segnale** a causa della **self-selection** (slide 56). I titolari di GED, rispetto agli altri dropout, hanno:
> - più anni di scuola prima dell'abbandono,
> - livelli misurati di abilità cognitive più alti,
> - genitori con più istruzione.
>
> Avrebbero quindi guadagnato di più *comunque*, GED o no. Una semplice differenza di salari tra dropout / titolari di GED / diplomati **non dice nulla** sull'effetto-segnale causale del GED.

---

## La Strategia: un Quasi-Esperimento sulle Soglie

> [!definition]
> Lo stratagemma (slide 57): **le soglie di superamento del GED variano per Stato USA**. Chi ottiene un punteggio di $40$–$44$ riceve il GED in Texas (soglia bassa) ma *non* lo riceve in New York, Florida, Oregon, Connecticut (soglia alta).
>
> A parità di abilità ($40$–$44$), il segnale GED viene quindi **assegnato quasi casualmente** in base allo Stato di residenza. È il test "puro" cercato sopra: stesso livello di abilità, diploma assegnato o meno per ragioni esogene (la legislazione statale).

Cosa prevede ciascun modello (slide 60):
- **Segnalazione:** a parità di punteggio $40$–$44$, chi *riceve* il GED guadagna di più di chi *non lo riceve*.
- **Capitale umano:** poiché l'abilità è comparabile tra i due gruppi, i salari saranno **comparabili** (il pezzo di carta non aggiunge produttività).

---

## Le Condizioni di Equilibrio Stimate

Lo studio interpreta il mercato come un [[05_Equilibrio_Separatore|equilibrio separatore]] (alcuni dropout prendono il GED, altri no). In equilibrio devono valere, per gli individui (slide 59):

$$
w_{GED} - w_{NO\text{-}GED} \ge C_{GED} \;\Rightarrow\; \text{ottieni il GED}
$$
$$
w_{GED} - w_{NO\text{-}GED} < C_{GED} \;\Rightarrow\; \text{non lo ottieni}
$$

dove $C_{GED}$ sono i costi diretti e indiretti del conseguimento. E per i datori:

$$
w_{GED} = E(\text{produttività} \mid C_{GED} \le w_{GED} - w_{NO\text{-}GED})
$$
$$
w_{NO\text{-}GED} = E(\text{produttività} \mid C_{GED} > w_{GED} - w_{NO\text{-}GED})
$$

Perché il GED funzioni da segnale serve il **single-crossing** ([[02_Educazione_come_Segnale_Credibile]]): il costo dev'essere più basso per i lavoratori più produttivi — plausibile, "non si supera il GED senza un minimo di studio" (slide 58).

---

## Il Disegno Difference-in-Differences

> [!definition]
> TMW usano una **difference-in-differences** (slide 61–62). Si incrociano *punteggio* (basso 40–44 vs alto, sopra la soglia ovunque) e *Stato* (soglia bassa vs alta):
>
> | | Soglia bassa | Soglia alta |
> |---|---|---|
> | **Punteggio basso** (trattamento) | GED | NO GED |
> | **Punteggio alto** (controllo) | GED | GED |
>
> Il gruppo di **trattamento** (punteggio 40–44) ottiene il GED solo negli Stati a soglia bassa; il gruppo di **controllo** (punteggio alto) lo ottiene ovunque.

Con i salari $\$_{punteggio,\,Stato}$ nelle quattro celle:

$$
(1)\quad \$_{L,L} - \$_{L,H} \;=\; \text{differenza GED/non-GED a parità di (basso) punteggio}
$$
$$
(2)\quad \$_{H,L} - \$_{H,H} \;=\; \text{differenza tra Stati a parità di (alto) punteggio (tutti hanno il GED)}
$$
$$
\boxed{(1) - (2) \;=\; \text{stima difference-in-differences}}
$$

> [!intuition]
> La sottrazione $(1)-(2)$ **nettifica le differenze tra Stati** non legate al GED (mercati del lavoro locali, costo della vita, ecc.). Il gruppo di controllo (punteggio alto), che ha il GED in entrambi i tipi di Stato, isola e rimuove l'effetto-Stato; ciò che resta in $(1)$ dopo aver tolto $(2)$ è l'effetto causale del *solo segnale* GED. È lo stesso principio di identificazione del quasi-esperimento sulla [[2. Selezione Avversa/10_Malpractice_Medica_Selezione_Avversa|malpractice medica]].

---

## I Risultati

> [!definition]
> Lo studio trova **ampi effetti di segnalazione per i bianchi**, stimati in un **guadagno salariale del ~20% dopo 5 anni** (slide 63).

Questo **dimostra che i titolari di GED sono in media più produttivi** dei dropout simili senza GED: perché esista un equilibrio (separatore) di segnalazione, dev'essere vero che i titolari di GED siano in media più produttivi (slide 63–64). Lo studio mostra inoltre che il GED è letto come **segnale positivo** dai datori, il che può essere vero solo se:

1. i titolari di GED sono in media più produttivi dei non titolari;
2. il GED è più "costoso" da ottenere per i meno produttivi (single-crossing — maturità, intelletto, ecc.);
3. i datori non riescono a osservare direttamente la produttività e usano lo status GED come segnale.

> [!example]
> Il risultato è elegante perché ribalta l'intuizione ingenua: il GED "vale" *non* perché insegni qualcosa di nuovo (capitale umano), ma perché **separa** chi è disposto/capace di ottenerlo da chi non lo è. Lo stesso pezzo di carta, assegnato per caso a persone di pari abilità, fa guadagnare il 20% in più: è la prova diretta del valore-segnale.

---

## Take-home message

> [!summary]
> Segnalazione e capitale umano fanno le stesse previsioni di superficie (più scuola ⇒ più salario), quindi la correlazione istruzione–salario non li distingue. L'unico test pulito è **assegnare casualmente il diploma a parità di abilità**: il capitale umano predice salari uguali, la segnalazione salari più alti per i diplomati. Tyler, Murnane & Willett (2000) realizzano questo test sfruttando le **diverse soglie di superamento del GED tra Stati USA**: a parità di punteggio (40–44), il GED è assegnato in modo quasi casuale. Con una **difference-in-differences** (incrociando punteggio e severità della soglia) nettificano gli effetti-Stato e isolano l'effetto-segnale. Risultato: **~20% di guadagno salariale dopo 5 anni per i bianchi**, prova diretta che il GED funziona da segnale e che i suoi titolari sono in media più produttivi (condizione necessaria per un equilibrio separatore).

> [!summary] Nota su un tema delicato
> Lo studio tocca differenze di esiti tra gruppi razziali, un tema sensibile: i risultati riportati riguardano stime statistiche su campioni storici (1990–91, *High School and Beyond*) e vanno letti nel loro contesto metodologico, non come affermazioni causali sui gruppi.

---

## Vedi anche

- [[02_Educazione_come_Segnale_Credibile]] — Il single-crossing del GED (condizione 2)
- [[05_Equilibrio_Separatore]] — Le condizioni di equilibrio separatore qui stimate
- [[06_Proprieta_Equilibrio_Separatore]] — Perché il segnale può essere informativo anche se improduttivo

---

## Connessioni con il Vault

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/10_Malpractice_Medica_Selezione_Avversa|Malpractice Medica]] — **stessa strategia di identificazione**: un quasi-esperimento basato su differenze legislative tra Stati USA, analizzato con difference-in-differences. Il confronto tra i due studi è un'ottima palestra metodologica

**Da `1. GT`:**
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — il mercato GED è interpretato come gioco di segnalazione il cui equilibrio (separatore) impone le condizioni stimate empiricamente
