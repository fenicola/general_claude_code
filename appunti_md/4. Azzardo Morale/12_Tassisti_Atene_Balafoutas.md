---
tags: [economia-informazione, azzardo-morale, beni-di-credenza, esperimento-sul-campo, asimmetria-informativa]
aliases: [Balafoutas 2013, Taxi Atene, Taxi Athens]
links: [09_Beni_di_Credenza, 11_Copertura_Assicurativa_Kerschbamer, 10_Riparazioni_Auto_Schneider]
---

# Tassisti ad Atene: frode e asimmetria informativa (Balafoutas et al. 2013)

## Riferimento bibliografico

> Balafoutas, L., Beck, A., Kerschbamer, R. & Sutter, M. (2013). What Drives Taxi Drivers? A Field Experiment on Fraud in a Market for Credence Goods. *The Review of Economic Studies*, 80(3), pp. 876–891.

## Perché i taxi come credence good?

La corsa in taxi in una città sconosciuta è un esempio di [[09_Beni_di_Credenza|credence good]] particolarmente puro. Il passeggero:
- non conosce il percorso ottimale (asimmetria di informazione geografica);
- non conosce la tariffa corretta se ignora la struttura tariffaria locale (asimmetria di informazione sui prezzi);
- non può verificare ex post se il percorso scelto era quello più breve (o se il prezzo era giusto) senza strumenti tecnici.

Il tassista, al contrario, conosce entrambe. L'asimmetria crea spazio per due tipi di frode:
- **Overtreatment**: fare giri più lunghi del necessario.
- **Overcharging**: addebitare un prezzo superiore alla tariffa corrispondente al percorso effettivo.

> [!intuition]
> Chiunque abbia preso un taxi da straniero in una città che non conosce ha vissuto l'esperienza di chiedersi: "Ma è davvero questo il percorso più breve?" La domanda è genuinamente difficile da rispondere — e il tassista lo sa. Questo esperimento trasforma questa intuizione in evidenza scientifica rigorosa.

## Design sperimentale: struttura 3×2

**Tre tipi di passeggero** (identità segnalata verbalmente al tassista):
- **Passeggero locale**: conosce sia la città sia le tariffe.
- **Passeggero non locale nativo**: conosce le tariffe ma non la città.
- **Passeggero straniero**: non conosce né la città né le tariffe.

**Due livelli di reddito percepito** (segnalato dall'abbigliamento):
- Reddito basso
- Reddito alto

Il design è quindi **3×2 = 6 celle sperimentali**, con tre sperimentatori che prendono la stessa corsa nello stesso momento — uno per cella di identità — permettendo un confronto diretto a parità di tutte le condizioni esterne (traffico, ora, percorso).

**Misurazione oggettiva**: tutti gli sperimentatori portano GPS-logger che registrano il percorso esatto. Questo permette di calcolare:
- La lunghezza effettiva del percorso vs il percorso più breve.
- Il prezzo giusto applicando la tariffa ufficiale ad Atene.
- La differenza tra prezzo dichiarato e prezzo corretto.

**Campione**: 348 corse in incognito, 4.400 km percorsi, lunghezza media circa 13 km per 22 minuti.

## Risultati: overtreatment

L'*overtreatment index* è il rapporto tra la lunghezza del percorso effettivo e quella del percorso più breve (normalizzata su ogni tripletta di corse). Un indice pari a 1 indica nessun deviazione; maggiore di 1 indica giro più lungo del necessario.

| Ruolo del passeggero | Reddito basso | Reddito alto | Totale |
|---|---|---|---|
| **Locale** | 1.021 | 1.037 | 1.029 |
| **Non locale nativo** | 1.066 | 1.087 | 1.077 |
| **Straniero** | 1.079 | 1.096 | 1.087 |

I passeggeri **non locali e stranieri** percorrono in media circa il **5-8% in più** rispetto ai locali — pochi minuti di percorso ma un pattern statisticamente significativo. Non emerge invece una differenza significativa tra non locali nativi e stranieri: la conoscenza della tariffa (ma non della città) non protegge dall'overtreatment.

Il fatto che l'asimmetria informativa sulla *città* sia sufficiente a generare overtreatment (indipendentemente dalla conoscenza delle tariffe) è consistente con la teoria: il percorso è il luogo dove si esercita l'opportunismo.

## Risultati: overcharging

La frequenza relativa di overcharging mostra un pattern ancora più netto:

| Ruolo del passeggero | Reddito basso | Reddito alto | Totale |
|---|---|---|---|
| **Locale** | 0.034 | 0.034 | 0.034 |
| **Non locale nativo** | 0.034 | 0.121 | 0.078 |
| **Straniero** | 0.259 | 0.190 | 0.224 |

Gli **stranieri** vengono sovrafatturati nel **22% dei casi** contro il **3% dei locali**. Un passeggero straniero ad alto reddito subisce overcharging in quasi 1 caso su 5.

**Quando avviene overcharging**: l'entità media supera il 25% del prezzo corretto — un'overcharge economicamente rilevante.

> [!example]
> Un passeggero straniero su una corsa da 10 euro paga in media circa 12.5 euro (+25%) quando viene sovrafatturato. Questo avviene in circa 1 corsa su 4.

## L'evidenza di comportamento onesto

Il risultato più sorprendente — e metodologicamente prezioso — è che **la grande maggioranza dei tassisti si comporta onestamente**:

- I passeggeri stranieri non vengono sovrafatturati nel **77%** dei casi.
- I passeggeri greci (locali + non locali) evitano la sovrafatturazione nel **94%** dei casi.

Questo dato è sorprendente perché le corse in taxi sono transazioni *one-shot* (nessuna reputazione da costruire), il che teoricamente massimizza l'incentivo a frodare.

L'elevata frequenza di comportamento onesto suggerisce che fattori non monetari — norme sociali, senso di vergogna, preferenze pro-sociali — svolgono un ruolo importante nel limitare la frode, anche in assenza di meccanismi di reputazione.

> [KS, p. 18]

## Confronto con [[11_Copertura_Assicurativa_Kerschbamer|Kerschbamer et al. (2016)]] sul *second-degree moral hazard*

Nel paper originale di Balafoutas et al. (2015) sui taxi (versione estesa), viene anche testato se dichiarare di essere rimborsati dal datore di lavoro (equivalente funzionale dell'assicurazione) aumenta l'overcharging. Il risultato è positivo: i passeggeri che dichiarano di essere rimborsati vengono sovrafatturati con circa il **17%** di probabilità in più.

Questo collegamento conferma che:
1. la separazione tra chi fruisce del servizio e chi ne sopporta il costo amplifica il second-degree moral hazard;
2. il meccanismo è robusto in mercati molto diversi (riparazioni PC vs corse in taxi).

## Implicazioni teoriche

L'esperimento dimostra che:

- L'**asimmetria di informazione geografica** (non conoscere la città) è una fonte di overtreatment.
- L'**asimmetria di informazione tariffaria** (non conoscere le tariffe) è una fonte di overcharging — ma solo se combinata con la percezione che il passeggero sia "straniero" nel senso pieno.
- Il **reddito percepito** aumenta l'overcharging per i non locali nativi con alto reddito (ma non per gli stranieri, già al massimo dello sfruttamento).

> [!summary]
> L'esperimento di Balafoutas et al. (2013) è una prova rigorosa e controllata di frode in un mercato di credence goods. I passeggeri non locali e stranieri subiscono overtreatment (percorsi più lunghi) e quelli stranieri subiscono overcharging molto più frequentemente dei locali. Tuttavia, la maggioranza assoluta dei tassisti si comporta onestamente anche in assenza di incentivi reputazionali, suggerendo un ruolo significativo delle preferenze sociali e delle norme.
