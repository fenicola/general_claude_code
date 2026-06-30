---
tags: [economia-informazione, azzardo-morale, beni-di-credenza, assicurazione, second-degree-moral-hazard, esperimento-sul-campo]
aliases: [Kerschbamer 2016, Insurance Coverage, Copertura Assicurativa, Second-degree Moral Hazard]
links: [09_Beni_di_Credenza, 13_Azzardo_Morale_Sanita, 01_Definizione_e_Timing, 12_Tassisti_Atene_Balafoutas]
---

# Copertura Assicurativa e Disonestà nei Mercati di Credence Goods (Kerschbamer, Neururer & Sutter 2016)

## Riferimento bibliografico

> Kerschbamer, R., Neururer, D., & Sutter, M. (2016). Insurance coverage of customers induces dishonesty of sellers in markets for credence goods. *Proceedings of the National Academy of Sciences*, 113(27), 7454–7458.

## Il problema teorico: *second-degree moral hazard*

Questo esperimento affronta una domanda cruciale: perché nei mercati sanitari (e analoghi) la copertura assicurativa è associata a una spesa più elevata? Esistono quattro spiegazioni alternative [KS, p. 15]:

1. **Selezione avversa** (lato domanda): le persone ad alto rischio si assicurano di più → la spesa sale perché chi si assicura ha bisogni maggiori.
2. **Moral hazard di primo grado** (lato domanda): gli assicurati chiedono più prestazioni perché il costo marginale personale è basso.
3. **Agenzia del medico** (lato offerta): il medico fornisce più prestazioni come *agente* del paziente, la cui copay è ridotta dall'assicurazione.
4. **Second-degree moral hazard** (lato offerta): il venditore prescrive di più perché *aspetta meno resistenza* dall'assicurato, che non sopporta direttamente il costo.

> [!definition]
> Il **second-degree moral hazard** (Balafoutas et al. 2015) designa la situazione in cui il venditore-esperto di un credence good sfrutta il fatto che il consumatore è assicurato — e quindi non sopporta direttamente il costo della frode — per gonfiare la prestazione o la fattura. Non è il consumatore che si comporta opportunisticamente, ma il **venditore** che sfrutta il moral hazard della relazione consumatore-assicuratore.

> [KS, p. 16]

Questa è la forma più grave dal punto di vista del benessere: nella spiegazione (1) e (2), la spesa maggiore riflette un beneficio per il paziente (anche se non efficiente); nella spiegazione (4), la spesa aggiuntiva è pura frode — nessun beneficio per il paziente.

> [!intuition]
> Il meccanico sa che se il cliente paga di tasca propria, baderà al centesimo. Se invece il cliente è assicurato (o rimborserà), il meccanico si aspetta che il cliente sia meno attento al prezzo e meno propenso a contestare la fattura. Questo sposta l'incentivo verso la frode.

## Design sperimentale

**Il difetto**: 5 computer ricondizionati e completamente funzionanti vengono danneggiati in modo identico e controllato: un modulo RAM viene tolto, causando un messaggio di errore univoco all'avvio. Il guasto è facilmente diagnosticabile da qualsiasi tecnico del settore e richiede un intervento minimo (sostituire il modulo RAM).

**La scelta del difetto** è cruciale: poiché la diagnosi corretta è univoca e certa, qualsiasi trattamento aggiuntivo è *obiettivamente* non necessario, il che elimina l'ambiguità nella classificazione dell'overtreatment.

**Campione**: 61 negozi di riparazione PC scelti casualmente su tutto il territorio austriaco (su 251 contattati).

**I due trattamenti**, che differiscono solo per una frase:

- **CONTROL**: *"Ho bisogno della fattura per la riparazione."*
- **INSURANCE**: *"Ho bisogno della fattura perché ho un'assicurazione che copre i costi di riparazione."*

In tutto il resto, le condizioni sono identiche: stesso sperimentatore, stessi abiti, stesso modello di PC, stessa gestione del RAM.

## Come si misurano overcharging e overtreatment

Dopo la riparazione, i computer vengono portati all'ufficio IT dell'università per un'ispezione completa di quanto è stato fatto:

- **Overtreatment** (dimensione ricambi): qualsiasi intervento non collegato alla sostituzione del RAM rotto. Esempio: sostituire l'alimentatore quando il problema è solo il RAM.
- **Overcharging** (dimensione tempo di lavoro): si misura confrontando i tempi dichiarati in fattura tra CONTROL e INSURANCE. Dato che il difetto è identico e la riparazione standard richiede 10-15 minuti, tempi di lavoro significativamente superiori sono attribuibili all'overcharging.

## Risultati

58 dei 61 negozi riescono a riparare il computer con successo.

**Prezzo medio di riparazione**:

$$\bar{p}_{CONTROL} = \text{€}70.17 \qquad \bar{p}_{INSURANCE} = \text{€}128.68$$

Differenza: circa **+83%** nel gruppo assicurazione — uno dei risultati più forti in letteratura sul second-degree moral hazard.

**Decomposizione della differenza** (su 27 osservazioni comparabili):

| Fonte | Effetto stimato | Quota della differenza |
|---|---|---|
| Overcharging (tempo di lavoro) | ~€41 (28 min in più) | ~70% |
| Overtreatment (ricambi non necessari) | ~€18 | ~30% |

- Tempo medio dichiarato: **0,55 ore** in CONTROL vs **1,02 ore** in INSURANCE.
- L'overtreatment si verifica **solo** nel gruppo INSURANCE — nel gruppo CONTROL non vi è alcun caso documentato.

> [!example]
> Se un negozio impiegasse davvero più tempo per controllare altri componenti, dovrebbe trovare ulteriori guasti. Ma i computer sono stati ricondizionati e verificati come perfettamente funzionanti. Le ore di lavoro aggiuntive non corrispondono ad alcuna attività aggiuntiva reale.

## Interpretazione: identificazione causale

Il disegno sperimentale permette di **escludere** le spiegazioni (1), (2) e (3):

- **Non è selezione avversa**: i computer sono identici; non c'è "tipo" più rischioso.
- **Non è moral hazard di primo grado**: non è il consumatore che chiede più prestazioni — il consumatore si comporta in modo identico nei due gruppi.
- **Non è agenzia** nel senso classico: il tecnico non è un agente del consumatore che massimizza il benessere di quest'ultimo — altrimenti perché addebitare ore di lavoro mai effettuate?

Rimane la spiegazione (4): il venditore percepisce che l'assicurato è meno attento al prezzo e meno propenso a contestare, e sfrutta questa percezione per gonfiare la fattura.

> [KS, p. 17]

## Connessione con la teoria

Questo esperimento si collega ai risultati di [[12_Tassisti_Atene_Balafoutas|Balafoutas et al. (2013)]] sui taxi, dove il rimborso spese dal datore di lavoro produce un effetto analogo (il passeggero che dichiara di essere rimborsato viene overcharged con maggiore frequenza).

In entrambi i casi, il meccanismo causale è identico: la **separazione tra chi decide il consumo e chi ne sopporta il costo** crea lo spazio per il second-degree moral hazard.

Il collegamento con il [[13_Azzardo_Morale_Sanita|mercato sanitario]] è diretto: l'assicurazione sanitaria crea esattamente questa struttura tripartita (paziente — assicuratore — medico/struttura), con i noti problemi di spesa eccessiva.

> [!summary]
> L'esperimento di Kerschbamer et al. (2016) isola causalmente il second-degree moral hazard: la sola informazione che il cliente è assicurato aumenta il prezzo di riparazione dell'83%. La differenza è composta per il 70% da overcharging (ore di lavoro mai svolte) e per il 30% da overtreatment (interventi non necessari). Questo risultato ha implicazioni dirette per la comprensione dell'aumento della spesa sanitaria nei sistemi con assicurazione.
