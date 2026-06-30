---
tags: [economia-informazione, azzardo-morale, beni-di-credenza, asimmetria-informativa]
aliases: [Credence Goods, Expert Services, Beni Fiducia]
links: [01_Definizione_e_Timing, 05_Inefficienza_e_Costi_di_Agenzia, 10_Riparazioni_Auto_Schneider, 11_Copertura_Assicurativa_Kerschbamer, 12_Tassisti_Atene_Balafoutas]
---

# Beni di Credenza (*Credence Goods*)

## Cos'è un bene di credenza?

> [!definition]
> Un **bene di credenza** (*credence good*) è un bene o servizio per il quale il consumatore non è in grado di verificare autonomamente né la qualità ricevuta né la quantità adeguata ai propri bisogni — né prima né dopo la transazione. La valutazione richiede l'intervento di un **esperto** (*expert*), che però ha anche l'interesse e la capacità di influenzare la fornitura a proprio vantaggio.

La struttura informativa è dunque doppiamente asimmetrica:

- Il **venditore-esperto** conosce il bisogno reale del consumatore (dopo diagnosi) e il tipo di trattamento somministrato.
- Il **consumatore** osserva solo l'utilità finale (o i sintomi residui) e non può distinguere se l'eventuale fallimento del servizio sia dovuto al trattamento errato, al trattamento insufficiente, o alla difficoltà intrinseca del caso.

> [KS, p. 2]

## Distinguere i beni: search, experience, credence

La letteratura economica distingue tre categorie di beni secondo la possibilità di valutarne la qualità:

- **Search goods**: la qualità è valutabile *prima* dell'acquisto (es. un vestito, un'automobile in showroom).
- **Experience goods**: la qualità emerge *dopo* il consumo (es. un ristorante, un film).
- **Credence goods**: la qualità non è valutabile neppure *dopo* il consumo — o almeno non senza un costo proibitivo.

L'esempio canonico di Darby e Karni (1973) è la visita medica: il paziente sa se si sente meglio, ma non sa se era necessaria proprio quella terapia, o una meno costosa.

> [!intuition]
> Immagina di portare l'auto dal meccanico per un problema di avviamento. Dopo la riparazione, l'auto funziona. Hai appena capito se la riparazione era davvero necessaria, o se bastava stringere un morsetto allentato? Probabilmente no. Questa impossibilità di valutazione ex post è il cuore dei beni di credenza.

## Struttura del problema

Il rapporto tra consumatore ed esperto condivide la struttura del [[01_Definizione_e_Timing|problema Principale-Agente]]:

- Il **consumatore** (Principale) delega la diagnosi e il trattamento.
- Il **venditore-esperto** (Agente) ha informazione privata sul tipo di problema e può scegliere il trattamento.

Tuttavia, a differenza del classico AM, qui l'asimmetria è sia *ex ante* (tipo di problema nascosto) sia *ex post* (azione nascosta: cosa è stato fatto davvero?). Questo rende i beni di credenza un caso particolarmente critico.

> [KS, p. 3]

## Le tre forme di inefficienza

In un mercato di credence goods privo di salvaguardie istituzionali, l'esperto può frodare il consumatore in tre modi:

> [!example]
> **Il meccanico come caso paradigmatico** [KS, p. 2]:
>
> **1. Overtreatment (sovra-trattamento)**: Il meccanico sostituisce componenti non necessarie. I costi aggiuntivi per il consumatore superano i benefici. La batteria viene sostituita quando sarebbe bastato stringere il cavo.
>
> **2. Undertreatment (sotto-trattamento)**: Il meccanico esegue una riparazione insufficiente. Il cliente paga ma il problema persiste. Il meccanico non segnala che il livello del liquido di raffreddamento era basso o che mancava un fanale.
>
> **3. Overcharging (sovrafatturazione)**: Il trattamento è corretto, ma la fattura eccede quanto effettivamente eseguito. Si addebita la sostituzione dello starter quando si è solo stretto il morsetto.

Formalmente, per ciascun consumatore esiste una **necessità oggettiva** $q^* \in \{q_L, q_H\}$ (bisogno basso o alto), e il venditore sceglie:
- la qualità effettivamente fornita $q \in \{q_L, q_H\}$
- il prezzo addebitato $p \in \{p_L, p_H\}$

Le inefficienze emergono quando $q \neq q^*$ oppure $p \neq p_q$ (prezzo non corrispondente alla qualità fornita).

## Condizioni per l'efficienza: Liability e Verifiability

Dulleck e Kerschbamer (2006) mostrano che ciascuna delle due seguenti condizioni istituzionali è sufficiente per l'efficienza:

**Condizione di Responsabilità (*Liability*)**: il venditore è giuridicamente obbligato a fornire una qualità che soddisfi il bisogno del consumatore. Previene l'undertreatment, ma non l'overtreatment né l'overcharging.

**Condizione di Verificabilità (*Verifiability*)**: il consumatore può osservare e verificare il tipo e la qualità del servizio ricevuto *dopo* la transazione (es. "mostrami i pezzi sostituiti"). Previene l'overcharging, ma non necessariamente l'overtreatment né l'undertreatment.

> [KS, p. 4]

In assenza di entrambe le condizioni, la teoria standard prevede il collasso del mercato. Ma — come mostrano i risultati sperimentali di Dulleck, Kerschbamer e Sutter (2011) — le *preferenze sociali* degli esperti (altruismo, avversione all'ineguaglianza) tengono il mercato più vitale di quanto la teoria predica.

## Esempi empirici del corso

Le slide della Lezione 14 presentano quattro esperimenti sul campo che documentano le inefficienze nei mercati di credence goods:

- [[10_Riparazioni_Auto_Schneider|Schneider (2012)]] — officine auto in Connecticut: prevalenza di overtreatment, assenza di overcharging (la verifiability è parzialmente presente).
- [[11_Copertura_Assicurativa_Kerschbamer|Kerschbamer, Neururer & Sutter (2016)]] — riparazioni PC in Austria: la copertura assicurativa induce disonestà del venditore (*second-degree moral hazard*).
- [[12_Tassisti_Atene_Balafoutas|Balafoutas, Beck, Kerschbamer & Sutter (2013)]] — taxisti ad Atene: i passeggeri stranieri subiscono overtreatment e overcharging in misura maggiore.
- [[13_Azzardo_Morale_Sanita|AS e AM nell'assistenza sanitaria]] — il caso dei mercati sanitari come archetipo di credence goods con rilevanza di policy.

## Rimedi possibili

Oltre alla liability e alla verifiability, la letteratura identifica rimedi alternativi:

- **Reputazione**: in contesti ripetuti, la minaccia di perdita di clientela futura scoraggia la frode. Tuttavia, la reputazione è efficace *solo* in assenza di salvaguardie istituzionali — in presenza di liability o verifiability, il suo effetto marginale scompare. [KS, p. 14]
- **Competizione**: più concorrenti riducono l'overcharging (meno rendite da estrarre), ma la pressione finanziaria da competizione intensa può *aumentare* la frode. [KS, p. 13]
- **Informazione pubblica**: la divulgazione delle esperienze dei consumatori (es. piattaforme di recensioni) può creare un surrogato di verifiability aggregata.
- **Standard professionali e certificazioni**: obblighi deontologici che internalizzano preferenze pro-sociali.

> [!summary]
> I beni di credenza sono caratterizzati da un'asimmetria informativa persistente che genera tre tipi di inefficienza: overtreatment, undertreatment e overcharging. La teoria individua nella *liability* e nella *verifiability* le condizioni istituzionali sufficienti per l'efficienza, ma l'evidenza empirica mostra che le preferenze sociali degli esperti, la reputazione e la competizione svolgono un ruolo rilevante anche in loro assenza. I mercati sanitari rappresentano il caso più importante e politicamente sensibile di credence goods.
