---
tags: [economia-informazione, selezione-avversa, malpractice, medicina-difensiva, lieber, politica-sanitaria]
aliases: [Malpractice Medica, Medicina Difensiva, Riforma Malpractice USA]
links: [07_Inefficienza_e_Implicazioni, 09_Modello_Wilson_Equilibri_Multipli, 11_Assicurazione_Vita_Effetto_Distruzione]
---

# La Malpractice Medica come Caso di Selezione Avversa

## Il Contesto: Medicina Difensiva e Costi Sociali

Il mercato delle prestazioni mediche è uno dei casi più importanti in cui la selezione avversa produce effetti distorsivi misurabili su larga scala. Un fenomeno strettamente connesso è la **medicina difensiva**: l'insieme di pratiche cliniche adottate non per motivazioni terapeutiche, ma per ridurre il rischio legale di una causa per malpractice.

> [!definition]
> La **medicina difensiva** (*defensive medicine*) si verifica quando i medici modificano le proprie pratiche cliniche — prescrivendo esami, visite o trattamenti non strettamente necessari — non per il benessere del paziente, ma per ridurre il proprio rischio di essere denunciati per negligenza (*malpractice*). Si distinguono:
> - **Medicina difensiva "positiva"** (*positive defensive medicine*): eccesso di prestazioni (esami, ricoveri, farmaci) non giustificate clinicamente ma utili a "documentare" la cura.
> - **Medicina difensiva "negativa"** (*negative defensive medicine*): rifiuto di trattare pazienti ad alto rischio o di eseguire procedure rischiose per evitare possibili cause legali.

[M, ch. 3 & 4]

---

## La Dimensione del Fenomeno in Italia

Le stime disponibili per il sistema sanitario italiano illustrano l'entità del problema. Il costo della sola medicina difensiva "positiva" ammonta a circa **10 miliardi di euro annui**, pari allo **0,75% del PIL** (dato della Commissione parlamentare d'inchiesta sugli errori sanitari).

Essa incide per circa il **10,5% della spesa sanitaria totale**, con le voci principali:

- Farmaci: 1,9% della spesa
- Visite specialistiche: 1,7%
- Esami di laboratorio: 0,7%
- Esami strumentali: 0,8%
- Ricoveri ospedalieri: 4,6%

Una indagine campionaria sui medici italiani rivela la diffusione del fenomeno:
- Il **77,9%** del campione ha adottato almeno un comportamento difensivo nell'ultimo mese lavorativo (con picchi del **92,3%** nella fascia d'età 32-42 anni).
- Il **68,9%** ha proposto ricoveri ospedalieri per pazienti ritenuti gestibili in regime ambulatoriale.
- Il **61,3%** ha prescritto più esami diagnostici di quanti ritenesse necessari.

> [!example]
> Il meccanismo è chiaro: il medico razionale internalizza il rischio legale nelle proprie decisioni cliniche. Una causa per malpractice è costosa in termini di tempo, stress, reputazione e denaro. L'esame aggiuntivo "non necessario" ha un costo marginale basso per il medico (lo paga il sistema sanitario o il paziente) ma riduce significativamente il rischio legale. Il risultato è un eccesso sistematico di prestazioni.

---

## Il Contributo di Lieber (2014): Selezione Avversa nel Mercato Medico

Lo studio di Lieber (2014) — *"Medical Malpractice Reform, the Supply of Physicians, and Adverse Selection"*, Journal of Law & Economics 57: 501-527 — fornisce un test empirico rigoroso della selezione avversa nel mercato dei medici. Il punto di partenza è l'onda di riforme della responsabilità medica negli USA.

### Il Contesto delle Riforme USA

Tra il 1970 e il 2001, **45 dei 48 stati contigui degli USA** hanno approvato riforme della legislazione sulla malpractice medica. Queste riforme riducono la responsabilità dei medici in due modi principali:
- Limitando la **probabilità** di dover pagare un risarcimento per malpractice.
- Imponendo un **tetto massimo** agli indennizzi (*cap*), in particolare per i danni non economici (*noneconomic damages cap*).

Gli effetti quantitativi sono rilevanti: una riforma è associata a una riduzione del 10-13% nel numero di richieste di risarcimento per medico (Avraham, 2007) e a una riduzione del 20% nel valore monetario dei risarcimenti (Danzon, 1986).

### La Domanda Chiave: Quale Tipo di Medici Si Sposta?

La riduzione dei costi attesi di malpractice attrae medici in uno stato che ha riformato. Ma la domanda cruciale dal punto di vista della selezione avversa è: **i medici che arrivano sono migliori o peggiori della media?**

Se i medici che si spostano verso stati con norme più favorevoli sono *più propensi a commettere errori* rispetto alla media, allora la riforma produce **selezione avversa**: lo stato riformato migliora la propria situazione (attira medici), ma al costo di peggiorare la qualità media dei propri medici.

> [!intuition]
> Il collegamento con la selezione avversa classica è diretto. Il "mercato" in questione è quello dei medici che scelgono in quale stato praticare. La "qualità" nascosta è la propensione a commettere errori (non osservabile ex ante). Le riforme cambiano i "prezzi" (riducono il costo atteso di una causa) e quindi cambiano la composizione dei medici che trovano conveniente praticare in quello stato. Se i medici ad alto rischio malpractice rispondo di più a queste riforme, si ha selezione avversa.

[M, ch. 4]

---

## La Strategia di Identificazione: Differenze-in-Differenze Geografiche

Stimare causalmente l'effetto delle riforme è metodologicamente difficile. Il problema principale è che le riforme modificano simultaneamente tre fattori:
1. **Incentivi a commettere errori** (*moral hazard*): riduzione di responsabilità → riduzione di cautela.
2. **Sorting geografico** (*selezione avversa*): i medici ad alto rischio si spostano verso stati favorevoli.
3. **Incentivi dei pazienti a denunciare**: meno facile vincere → meno denunce.

Misurare direttamente l'effetto 2 (selezione avversa) richiede controllare per 1 e 3.

### La Soluzione: Riforme degli Stati Confinanti

Lieber utilizza una strategia brillante: considera l'effetto delle riforme approvate dagli **stati confinanti** sul tasso di malpractice dello stato di riferimento.

> [!example]
> **Esempio: Illinois, Indiana, California.** Quando l'Indiana approva una riforma, i medici dell'Illinois sono *geograficamente vicini* e possono trasferire la propria pratica in Indiana con costi relativamente bassi (alcuni possono addirittura non cambiare residenza, solo studio). I medici della California, invece, sono lontani e subiscono costi di spostamento molto più alti. Dunque, si osserva che il tasso di malpractice dell'Illinois varia quando l'Indiana approva una riforma — ma questo non può essere attribuito né a cambiamenti negli incentivi dei medici rimasti in Illinois, né a cambiamenti nel comportamento dei pazienti dell'Illinois (che non sono toccati dalla legge dell'Indiana). L'unica causa possibile è il **cambiamento nella composizione** dei medici in Illinois (alcuni se ne sono andati in Indiana).

Formalmente, il modello stimato è:

$$\ln\left(\frac{\text{malpractice}_{it}}{\text{doctors}_{it}}\right) = X_{it}\beta_2 + C_{it}\Gamma_2 + \lambda_t + \lambda_s + \rho_{st} + \varepsilon_{it}$$

dove $C_{it}$ rappresenta lo status riformistico degli stati confinanti, $\lambda_t$ e $\lambda_s$ sono effetti fissi di tempo e stato, e $\rho_{st}$ cattura tendenze stato-specifiche nel tempo.

---

## I Risultati

### Risultato 1: Le Riforme Riducono l'Offerta di Medici

Quando uno stato confinante approva un **tetto ai danni non economici** (*noneconomic damages cap*), l'offerta di medici nei contee confinanti si riduce del **4%**. Questa è la risposta di selezione: alcuni medici si spostano verso lo stato riformato.

### Risultato 2: Selezione Avversa — Si Spostano i Medici "Cattivi"

I medici che lasciano uno stato quando il confinante riforma sono **più inclini a commettere malpractice rispetto alla media** dei medici rimasti. Questo si dimostra osservando che il tasso di malpractice nello stato di origine *diminuisce* dopo la riforma del confinante — segno che i medici ad alto rischio malpractice erano i più sensibili all'incentivo della riforma e se ne sono andati.

L'interpretazione è che le riforme attraggono selettivamente i medici che si trovano sotto maggiore pressione legale (quelli con più richieste di risarcimento), ovvero i medici mediamente più rischiosi.

### Risultato 3: Effetti sulla Mortalità

Le dimensioni dell'effetto selezione sono notevoli. Se tutti gli stati confinanti di uno stato adottassero riforme sui danni non economici, si stima una riduzione di **311 morti l'anno** nello stato di riferimento (per confronto: lo stato medio aveva 335 omicidi, 313 morti per il morbo di Parkinson e 290 morti per complicanze da HIV nell'anno 2000).

> [!summary]
> Le riforme della malpractice non sono neutre dal punto di vista della qualità dei medici. Riducono la responsabilità di tutti, ma attraggono selettivamente i medici più rischiosi. Questo è un caso emblematico di **selezione avversa nel mercato del lavoro**: la riduzione del "prezzo" (costo atteso delle cause) modifica la composizione di chi partecipa al mercato in un modo socialmente costoso.

---

## Extensions: Moral Hazard vs. Selezione Avversa

Lo studio di Lieber si concentra sulla selezione, ma la letteratura ha anche esaminato gli effetti di *moral hazard* delle riforme:

**Argomento dell'overprovision:** Kessler e McClellan (2002) sostengono che i medici sovra-prescrivono per paura delle cause. Ridurre la responsabilità riduce l'eccesso di cure senza aumentare la mortalità.

**Argomento del peggioramento della qualità:** Al contrario, Currie e MacLeod (2008) trovano che riduzioni di responsabilità sono associate a *aumenti* degli esiti avversi prevenibili. Iizuka (2013) trova che le riforme aumentano il numero di complicanze mediche prevenibili.

Il quadro teorico suggerisce che i due effetti sono in tensione: riduzioni di responsabilità possono sia (a) eliminare la medicina difensiva costosa inutile, sia (b) ridurre la cura appropriata. L'effetto netto dipende da quale meccanismo domina nel contesto specifico.

---

## Il Caso Italiano: Legge Gelli-Bianco (n. 24/2017)

In Italia, la risposta legislativa al problema della malpractice è la **Legge Gelli-Bianco (n. 24/2017)**, che introduce:

- **Esclusione di responsabilità penale** per omicidio colposo o lesioni personali colpose se: (a) l'evento è dovuto a imperizia (ma non a negligenza o imprudenza), *e* (b) sono state rispettate le raccomandazioni delle linee guida cliniche o delle buone pratiche clinico-assistenziali.
- **Responsabilità della struttura sanitaria** (pubblica o privata) — non solo del singolo medico.
- **Onere della prova** a carico del paziente danneggiato.
- **Assicurazione obbligatoria** per le strutture sanitarie.

> [!intuition]
> La riforma italiana persegue una logica simile a quella analizzata da Lieber: ridurre il rischio legale per attrarre e trattenere medici, riducendo la medicina difensiva. Ma alla luce dei risultati di Lieber, sorge la domanda: se anche in Italia i medici più rischiosi sono i più sensibili a queste riforme, l'effetto di selezione negativa potrebbe parzialmente compensare i benefici. La valutazione empirica della Gelli-Bianco rimane un campo di ricerca aperto.

---

## Vedi Anche

- [[07_Inefficienza_e_Implicazioni]] — I meccanismi generali di selezione avversa
- [[09_Modello_Wilson_Equilibri_Multipli]] — L'estensione di Wilson del modello base
- [[11_Assicurazione_Vita_Effetto_Distruzione]] — Selezione avversa nel mercato assicurativo

---

## Connessioni con il Vault

**Da `0. Intro`:**
- [[0. Intro/05_Selezione_avversa|Selezione avversa — Introduzione]] — questa nota è un'applicazione empirica del meccanismo illustrato nell'introduzione: il mercato del lavoro medico è un caso di selezione avversa dove il "tipo" è la propensione al rischio del medico
- [[0. Intro/04_Principale_e_agente|Principale e Agente]] — il rapporto paziente-medico è un classico framework P–A: il paziente (Principale) non osserva le caratteristiche del medico (Agente) né la sua effettiva cura nella pratica clinica

**Da `1. GT`:**
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — la struttura del "natural experiment" di Lieber è un gioco sequenziale: prima viene la riforma nello Stato B, poi il medico dello Stato A decide se migrare o restare; Lieber identifica la selezione avversa osservando chi migra *condizionatamente* alla riforma
- [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]] — la reputazione professionale del medico funge da meccanismo disciplinante analogo alla cooperazione in giochi ripetuti; la riforma riduce il costo della "defezione" (negligenza), modificando il calcolo del payoff intertemporale
