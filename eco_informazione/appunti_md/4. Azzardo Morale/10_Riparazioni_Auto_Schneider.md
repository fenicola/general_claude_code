---
tags: [economia-informazione, azzardo-morale, beni-di-credenza, esperimento-sul-campo, reputazione]
aliases: [Schneider 2012, Auto Repair, Officine Auto]
links: [09_Beni_di_Credenza, 07_Meccanismi_di_Controllo_Esterni, 11_Copertura_Assicurativa_Kerschbamer]
---

# Esperimento sulle Officine Auto (Schneider 2012)

## Riferimento bibliografico

> Schneider, H. (2012). *Agency Problems and Reputation in Expert Services: Evidence from Auto Repair*. The Journal of Industrial Economics, LX: 0022-1821.

## Motivazione

Questo studio è uno dei pochi esperimenti sul campo (*field experiment*) che documenta in modo rigoroso e controllato l'azzardo morale nei [[09_Beni_di_Credenza|mercati di credence goods]]. Il problema di identificazione nei dati osservativi è classico: come distinguere se un meccanico ha consigliato riparazioni superflue perché ha sfruttato l'asimmetria informativa, o perché riteneva genuinamente che fossero necessarie?

La soluzione è il disegno sperimentale: introdurre difetti *noti* all'osservatore ma non al meccanico, così da poter giudicare oggettivamente la risposta.

> [!intuition]
> L'esperimento funziona come un "test nascosto" in grande stile: si porta una macchina con guasti artificiali e noti al ricercatore, ma non al meccanico. Così si può verificare se il meccanico trova i guasti (segnale di competenza e diligenza) e se ne approfitta per consigliare riparazioni eccessive (segnale di opportunismo).

## Design sperimentale

**Il veicolo di prova** era equipaggiato con difetti calibrati:

- **Cavo della batteria allentato**: causa problemi di avviamento intermittenti. La correzione corretta (stringere il cavo) è rapida e quasi gratuita; la risposta opportunistica (sostituire batteria o motorino di avviamento) è costosa → test per l'**overtreatment**.
- **Livello del liquido di raffreddamento basso**: difetto semplice da correggere una volta scoperto, ma richiede ispezione proattiva → test per l'**undertreatment**.
- **Fanale posteriore mancante**: visibile a occhio nudo, richiede ispezione → test per l'**undertreatment**.
- **Cavi delle candele consumati** e altri componenti con segni d'usura ma ancora funzionanti.

La presenza contemporanea di difetti che stimolano risposte opposte (overtreatment sul cavo batteria, undertreatment su liquido e fanale) permette di catturare entrambe le forme di frode nello stesso esperimento.

## Trattamenti: reputazione bassa vs alta

Per testare il ruolo della **reputazione**, l'autore ha creato due trattamenti differenziando le informazioni fornite al meccanico sull'orizzonte temporale del cliente:

- **Low-reputation treatment**: il cliente dichiara di trasferirsi a Chicago entro due settimane → relazione *one-shot*, nessun incentivo reputazionale per il meccanico.
- **High-reputation treatment**: il cliente dichiara di essersi appena trasferito in zona e di dover guidare fino a Montreal tra due settimane → cliente *repeat*, incentivi reputazionali potenzialmente attivi.

In entrambi i casi il cliente chiede un'ispezione approfondita e dichiara di aver acquistato l'auto di recente.

**Campione**: 40 officine indipendenti in quattro città nel Connecticut (USA).

## Risultati principali

### Difetti legittimi: scoperta e riparazione

La tabella dei difetti legittimi mostra che il difetto più facilmente identificato e riparato è il cavo della batteria (scoperto in 27 visite su 40, riparato tutte le volte che scoperto), mentre i difetti che richiedono ispezione proattiva (liquido di raffreddamento, fanale) vengono scoperti molto meno frequentemente.

Questo documenta:
- **Overtreatment** diffuso: il cavo allentato è spesso "risolto" con la sostituzione della batteria o dello starter.
- **Undertreatment** sistematico: il meccanico non si preoccupa di cercare guasti ulteriori, specialmente quelli semplici ma non evidenti a prima vista.

### Riparazioni inutili raccomandate

In 19 casi su 40 visite totali viene raccomandata almeno una riparazione non necessaria. Le raccomandazioni più comuni includono: sostituzione del motorino d'avviamento (7 casi), sostituzione della batteria (3 casi), sostituzione del radiatore, del termostato, della pompa dell'acqua.

### Effetto reputazione sui prezzi

Il costo medio della diagnosi:
- Visite **one-time** (low-reputation): **\$59,75**
- Visite **repeat-business** (high-reputation): **\$37,70**
- Differenza: **\$22,05** (statisticamente significativa, $p = 0.05$)

La reputazione abbassa il costo della diagnosi, ma **non elimina** l'overtreatment.

## Interpretazione economica: verifiability e liability

I risultati illuminano le due condizioni teoriche di Dulleck e Kerschbamer (2006) applicate al caso reale:

**Perché l'overtreatment è comune ma l'overcharging è raro?**

> La risposta è la **condizione di verificabilità parziale**: il cliente *può* vedere quali pezzi sono stati smontati e sostituiti dopo la riparazione. Questo rende l'overcharging rischioso (il cliente potrebbe verificare). Di contro, non può sapere se quelle riparazioni fossero *davvero necessarie*, il che lascia aperta la porta all'overtreatment.

Formalmente: con verifiability parziale, il venditore non può addebitare servizi non eseguiti, ma può eseguire (e addebitare) servizi non necessari.

**Perché l'undertreatment persiste?**

> Il meccanico non viene penalizzato per non aver scoperto difetti che il cliente non conosceva. È il **fallimento della condizione di liability**: il cliente non apprende della negligenza, o non ha gli strumenti legali per sanzionarla.

> [KS, p. 4–5]

## L'effetto limitato della reputazione

Il risultato più sorprendente è che la reputazione **non riduce significativamente** l'overtreatment. Schneider lo spiega con la natura dei beni di credenza: anche dopo la riparazione, l'automobilista non riesce a valutare se le riparazioni raccomandate fossero realmente necessarie. Senza questa valutazione ex post, il meccanismo reputazionale non scatta — il cliente non impara.

> La reputazione funziona solo là dove il cliente può valutare la qualità del servizio ricevuto. Nei credence goods, questa valutazione è strutturalmente impossibile, il che rende la reputazione un rimedio debole. [KS, p. 14]

La reputazione incide invece sul **prezzo della diagnosi** (dove la comparazione è possibile), confermando che il meccanismo funziona nelle dimensioni in cui c'è verificabilità ex post.

## Rimedi proposti

Schneider identifica tre soluzioni di policy:

1. **Pubblicazione pubblica dei risultati di valutazioni di terze parti** sulla qualità del servizio (es. ispezioni a sorpresa da associazioni di consumatori).
2. **Separazione tra diagnosi e riparazione**: officine specializzate nella sola diagnosi eliminano l'incentivo a raccomandare riparazioni eccessive, perché la diagnosi è il loro unico prodotto.
3. **Piattaforme di esperienze degli utenti** (Yelp, RepairPal): anche se il singolo cliente non riesce a valutare la qualità, i pattern aggregati rivelati dalle esperienze di molti clienti possono emergere e diventare informativi.

> [!summary]
> L'esperimento di Schneider documenta empiricamente le tre forme di inefficienza nei credence goods: l'overtreatment è comune, l'undertreatment è sistematico, l'overcharging è raro (perché la verifiability parziale scoraggia la fatturazione di servizi non eseguiti). La reputazione riduce i prezzi della diagnosi ma non elimina l'opportunismo nei trattamenti. Il rimedio istituzionale più promettente è la verifiability strutturata tramite terze parti.
