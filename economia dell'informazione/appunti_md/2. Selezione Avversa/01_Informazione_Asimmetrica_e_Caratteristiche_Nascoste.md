---
tags: [economia-informazione, selezione-avversa, informazione-asimmetrica]
aliases: [Hidden Information, Caratteristiche Nascoste, Ex-ante Asymmetry]
links: [02_Mercato_dei_Limoni_Intuizione, 04_Modello_Akerlof_Formale]
---

# Informazione Asimmetrica e Caratteristiche Nascoste

## Definizione

> [!definition]
> L'**informazione asimmetrica** (o *hidden information*) descrive una situazione in cui le parti di una transazione non dispongono dello stesso insieme di informazioni rilevanti. In particolare, si parla di **caratteristiche nascoste** (*hidden characteristics*) quando una delle parti conosce, prima della stipula del contratto, una proprietà del bene o del servizio che l'altra parte non può osservare. Questa forma di asimmetria è detta **ex-ante** perché precede la firma del contratto.

La dimensione temporale è cruciale. Formalmente, il timing del problema è il seguente:

$$
t=0 \quad \longrightarrow \quad t=1 \quad \longrightarrow \quad t=2
$$

- **$t=0$**: Il venditore apprende la qualità del bene (caratteristica nascosta)
- **$t=1$**: Il compratore formula un'offerta di prezzo; il venditore accetta o rifiuta
- **$t=2$**: Il compratore apprende la qualità effettiva del bene (troppo tardi!)

L'asimmetria informativa esiste **al momento della contrattazione** ($t=1$): il venditore sa già tutto, il compratore agisce solo sulla base di probabilità.

> [BB, p. 278] La struttura informativa — incluse le probabilità a priori delle diverse qualità — è *common knowledge* tra acquirente e venditore. Ciò che non è common knowledge è la qualità specifica del singolo bene.

---

## Intuizione economica

> [!intuition]
> Il problema non è che nessuno sa nulla: è che *il venditore sa più del compratore*. Questa asimmetria rompe il meccanismo ordinario del mercato. In un mercato normale, il prezzo riflette la qualità e la qualità giustifica il prezzo. Quando il venditore conosce la qualità e il compratore no, il prezzo perde il suo ruolo di segnale affidabile. Anzi, diventa fonte di inferenza negativa: «se lo vende a quel prezzo, forse vale meno».

Un'altra distinzione fondamentale è tra due tipi di asimmetria:

- **Asimmetria informativa** (*hidden information/characteristics*): l'asimmetria esiste **prima** del contratto. È il caso della selezione avversa. Il venditore *è nato* con un'informazione superiore.
- **Azione nascosta** (*hidden action/moral hazard*): l'asimmetria sorge **dopo** il contratto. Una parte può compiere azioni non osservabili dall'altra. È il tema dell'azzardo morale (trattato altrove).

> [BB, p. 273] In questo capitolo ci concentriamo sul tipo di asimmetria informativa che esiste già prima che le proposte vengano formulate e accettate — il caso della *selezione avversa*. Un caso correlato sorge quando una parte acquisisce informazioni rilevanti *dopo* la stipula del contratto (Capitolo 15). Un caso ancora diverso riguarda le azioni, non i fatti: questo è il *moral hazard* (Capitolo 16).

---

## Esempio: L'Assicurazione Matrimoniale

> [!example]
> **Svizzera, 1990.** Una compagnia assicurativa lancia un prodotto innovativo: i genitori possono assicurare i figli sotto i 10 anni contro il rischio di un matrimonio prima dei 25 anni (copertura massima CHF 100.000). Il prezzo viene calcolato sulla base delle statistiche matrimoniali svizzere medie: il 17% degli uomini e il 29% delle donne si sposano entro i 25 anni.
>
> Risultato: la polizza diventa popolarissima presso comunità etniche e religiose dove i matrimoni precoci sono la norma. Il tasso di matrimoni precoci tra gli assicurati raggiunge il **99%**. Il prezzo medio nascondeva la varianza tra i gruppi. Coloro che *sapevano* di avere un'alta probabilità di sposarsi presto erano esattamente coloro che si assicuravano.
>
> Conclude l'agente: «There was a technical loss on each and every policy sold.»

Questo esempio illustra perfettamente il meccanismo: chi compra l'assicurazione *sa qualcosa* che la compagnia non sa. La compagnia ragiona sulla media della popolazione; i clienti ragionano sulla propria situazione specifica. Ne risulta che la "media" che la compagnia assicura non corrisponde alla media effettiva dei propri clienti.

> [BB, p. 274] C'è un vecchio detto nel settore assicurativo: «Il profumo del premio non dovrebbe mai mascherare l'odore del rischio». Quando un affare sembra troppo attraente, qualcosa potrebbe non andare.

---

## L'Higher-Order Knowledge

Un aspetto sottile ma essenziale: non basta sapere cosa sa il venditore. Bisogna sapere cosa sa il venditore **di quello che sa il compratore**, e viceversa. Questo è il cosiddetto *higher-order knowledge*.

> [!intuition]
> Alice e Bob sanno che Fred conosce il valore della propria auto meglio di chiunque altro. Fred sa che Alice e Bob sanno questo. Alice e Bob sanno che Fred sa che loro sanno... Questa catena di conoscenze reciproche è *common knowledge*. Un compratore naïve ignorerebbe l'informazione di Fred. Un compratore razionale — come Alice e Bob — la usa per aggiornare le proprie aspettative *negativamente*: se Fred vende, è più probabile che l'auto non valga molto.

Questo meccanismo di inferenza razionale è ciò che trasforma l'asimmetria informativa in un problema di mercato: non è l'ignoranza del compratore a causare il fallimento, ma la sua *razionalità* nell'inferire la qualità dal comportamento del venditore.

> [BB, p. 278] L'acquirente sa che il venditore sa la qualità dell'auto (e il venditore sa che l'acquirente lo sa, ecc.). Questa informazione di ordine superiore su chi sa cosa è importante quanto l'informazione fondamentale sulla qualità dell'auto. Il vantaggio informativo del venditore può in realtà diventare un handicap: i compratori non sono naïve; e un venditore che *è noto sapere* non può vendere un'auto di bassa qualità al prezzo di una di alta qualità.

---

## Applicazioni nel mondo reale

Le caratteristiche nascoste compaiono in molti mercati:

- **Mercato delle auto usate**: il venditore conosce la storia del veicolo
- **Mercato assicurativo**: l'assicurato conosce il proprio rischio (salute, guida)
- **Mercato del lavoro**: il lavoratore conosce le proprie abilità reali
- **Credito bancario**: il debitore conosce la rischiosità del proprio progetto
- **Beni di esperienza e fiducia**: il venditore conosce la qualità che il compratore non può verificare nemmeno dopo l'acquisto (→ [[07_Inefficienza_e_Implicazioni]])

> [BB, p. 275] I ristoranti, i venditori di auto, i produttori di computer, i medici, gli avvocati e i consulenti finanziari hanno tutti un vantaggio informativo sui propri clienti. In altri ambiti sono i compratori ad essere meglio informati: i mercati assicurativi sono l'esempio classico.

---

## Take-home message

> [!summary]
> L'informazione asimmetrica *ex-ante* — dove il venditore conosce una caratteristica del bene non osservabile dal compratore — è la causa strutturale della selezione avversa. Il problema non è l'incompletezza dell'informazione (nessuno sa nulla), ma la sua asimmetria (qualcuno sa, qualcun altro no). I compratori razionali usano il comportamento del venditore come segnale, il che innesca una dinamica di selezione negativa: vengono scambiati solo i beni di qualità peggiore. Il timing conta: solo l'asimmetria *prima* del contratto produce selezione avversa; dopo il contratto si parla di moral hazard.

---

## Vedi anche

- [[02_Mercato_dei_Limoni_Intuizione]] — Cosa succede quando l'asimmetria colpisce un mercato
- [[03_Modello_Formale_Due_Qualita]] — Il modello grafico formale
- [[04_Modello_Akerlof_Formale]] — Il modello completo di Akerlof (Molho cap. 2)
- [[07_Inefficienza_e_Implicazioni]] — I rimedi all'asimmetria informativa

---

## Connessioni con il Vault

> [!note] Dove si inserisce nel corso
> Questa nota approfondisce il cuore teorico dell'[[0. Intro/05_Selezione_avversa|introduzione alla selezione avversa]] (cartella `0. Intro`). Mentre quella nota offre una panoramica del problema, qui si sviluppa il meccanismo formale passo per passo.

**Da `0. Intro`:**
- [[0. Intro/04_Principale_e_agente|Principale e Agente]] — il framework P–A è la struttura generale di cui l'informazione asimmetrica ex-ante è un caso speciale (il tipo dell'Agente è ignoto al Principale prima del contratto)
- [[0. Intro/05_Selezione_avversa|Selezione avversa — Introduzione]] — la panoramica concettuale che questa nota espande formalmente
- [[0. Intro/06_Segnalazione|Segnalazione]] — la risposta della parte *informata* al problema di asimmetria qui descritto
- [[0. Intro/07_Screening|Screening]] — la risposta della parte *non informata* (il Principale) allo stesso problema

**Da `1. GT`:**
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali (SPNE)]] — il timing dell'asimmetria ($t=0 \to t=1 \to t=2$) corrisponde esattamente alla struttura di un gioco in forma estesa con nodi informativi non singoletti
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — il NE di questo gioco informativo è l'equilibrio di zero-scambio, Pareto-inferiore all'ottimo
