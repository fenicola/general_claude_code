---
tags: [economia-informazione, reputazione, esperimento-di-laboratorio, trust-game]
aliases: [Bolton Katok Ockenfels, Esperimento Reputazione, Strangers vs Partners]
links: [02_Trust_Game_e_Reputazione, 01_Mercati_Reputazionali, 04_Hygiene_Grade_Cards_Jin_Leslie]
---

# Esperimento sui Meccanismi Reputazionali (Bolton, Katok & Ockenfels)

## Riferimento bibliografico

> Bolton, G., Katok, E. & Ockenfels, A. (2004). *How Effective Are Electronic Reputation Mechanisms? An Experimental Investigation*. Management Science, 50(11), 1587–1602.

## Motivazione

Le previsioni teoriche sul [[02_Trust_Game_e_Reputazione|trust game]] sono estreme (0% di scambi senza reputazione, 100% con reputazione). L'esperimento porta soggetti reali in laboratorio a giocare ripetutamente il trust game **con incentivi monetari reali** (possono guadagnare o perdere soldi veri), confrontando tre ambienti di mercato.

## I tre trattamenti

> [!definition] Gli ambienti di mercato a confronto
> 1. **Mercato senza reputazione** (*strangers*): a ogni round buyer e seller sono
>    abbinati casualmente, senza alcuna informazione sul passato → sequenza di
>    giochi *one-shot*.
> 2. **Mercato con reputazione** (*strangers + feedback*): coppie sempre diverse,
>    ma è disponibile l'informazione su come il seller si è comportato nei round
>    precedenti con *altri* buyer → informazione di **seconda mano**.
> 3. **Mercato relazionale** (*partners*): le interazioni avvengono sempre tra gli
>    **stessi** soggetti, un numero finito di volte → informazione di **prima mano**.

## Risultati

### 1) Senza reputazione: convergenza al non-scambio

Anche senza incentivi reputazionali esiste una **fiducia di default**: circa il **27%** dei buyer si fida (manda i soldi) e circa il **37%** dei seller è affidabile (manda il bene). Quindi l'equilibrio di puro non-scambio **non** è verificato letteralmente.

> [!warning] Il problema non è (solo) la motivazione, ma il matching
> Perché avvenga uno scambio, un buyer fiducioso (27%) deve incontrare un seller
> affidabile (37%): $0{,}27 \times 0{,}37 \approx 10\%$. Senza informazione, i due
> tipi non riescono a "trovarsi". L'efficienza, round dopo round, **converge a
> zero**: chi si fida della persona sbagliata viene tradito e smette di fidarsi.

### 2) Con reputazione (strangers): efficienza ≈ 50%

Introducendo il sistema di feedback sul comportamento passato del seller, l'efficienza si **mantiene sostenuta** per quasi tutti i round: molti buyer si fidano e circa metà dei seller risponde in modo affidabile. Crolla solo negli **ultimi round**, quando — venendo meno l'incentivo futuro — scatta l'opportunismo (effetto di backward induction tipico dei [[1. GT/08_Giochi_Ripetuti_Finiti|giochi ripetuti finiti]]).

> [!warning] Anche la reputazione lascia inefficienza
> Contrariamente alla previsione del [[1. GT/10_Folk_Theorem|Folk Theorem]] (piena
> efficienza), il meccanismo reputazionale produce solo **~50%** degli scambi.
> Quando c'è asimmetria informativa, **c'è sempre una perdita di efficienza**.

### 3) Relazionale (partners): efficienza più alta

Quando i soggetti interagiscono sempre tra loro (anche un numero finito di volte), l'efficienza è **nettamente maggiore** che nel mercato reputazionale con feedback.

> [!intuition] Prima mano ≠ seconda mano
> Il risultato più sorprendente: **non tutta l'informazione è uguale**.
> L'informazione di *prima mano* (averlo sperimentato direttamente) vale più di
> quella di *seconda mano* (averlo letto in una recensione), **anche quando dice
> esattamente la stessa cosa**. La disponibilità a fidarsi cresce con
> l'esperienza diretta — un fenomeno "anomalo" rispetto alla teoria standard.

## 🔗 Connessioni

- Modello sottostante: [[02_Trust_Game_e_Reputazione]]
- Quadro generale: [[01_Mercati_Reputazionali]]
- Controparte "sul campo": [[04_Hygiene_Grade_Cards_Jin_Leslie]]
- Effetto ultimi round = backward induction: [[1. GT/08_Giochi_Ripetuti_Finiti|Giochi Ripetuti Finiti]]
- Inefficienza residua: stessa lezione dei [[4. Azzardo Morale/09_Beni_di_Credenza|beni di credenza]] (la reputazione riduce ma non elimina l'opportunismo)
