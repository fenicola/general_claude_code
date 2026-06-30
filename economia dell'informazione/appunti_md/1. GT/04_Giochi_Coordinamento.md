---
tags: [economia-informazione, game-theory, coordinamento, equilibri-multipli]
aliases: [Coordination Games, Giochi di Coordinamento, Stag Hunt, Caccia al Cervo]
links: [03_Nash_Equilibrium, 05_Chicken_Game, 06_Dilemma_Prigioniero, 0. Intro/01_Coordinamento_e_incentivi, 0. Intro/02_Mercato_e_Hayek, 0. Intro/03_Beni_comuni]
---

# Giochi di Coordinamento

## Definizione Formale

> [!definition] Gioco di Coordinamento
> Un **gioco di coordinamento** è un gioco in cui i giocatori hanno un incentivo a coordinare le proprie strategie per ottenere esiti mutuamente vantaggiosi o evitare esiti mutuamente dannosi. Questi giochi si caratterizzano per la presenza di **equilibri di Nash multipli**, e il problema strategico centrale è *quale* equilibrio i giocatori selezioneranno.
>
> In molti giochi di coordinamento gli equilibri sono **Pareto-ordinabili**: uno domina l'altro nel senso che almeno un giocatore sta meglio senza che nessun giocatore stia peggio. Si parla in questo caso di *coordinamento con assurance* (Carmichael) o di *stag hunt*.

## Intuizione Economica

> [!intuition]
> Perché alcune società sono puntualissime (Germania, Giappone) e altre hanno una cultura del tempo elastica (Italia, Brasile)? Entrambe le norme sociali possono essere equilibri stabili: se tutti si aspettano che gli altri arrivino in ritardo, è razionale arrivare in ritardo anche tu (altrimenti aspetti da solo). Se tutti si aspettano puntualità, è razionale essere puntuali.
>
> Questo è l'intuizione dei giochi di coordinamento: la storia, la cultura e le aspettative condivise — non solo le preferenze individuali — determinano quale equilibrio viene selezionato. Siamo "intrappolati" in un equilibrio non perché sia il migliore in assoluto, ma perché nessuno ha incentivo a deviare *unilateralmente*.

## Il Gioco della Puntualità

> [!example] Coordinamento sulla puntualità
> Due soggetti si incontrano. Ciascuno può arrivare *in orario* (On time) o *in ritardo* (Late). I payoff riflettono il fatto che è peggio essere gli unici puntuali (aspetti), ma che la puntualità condivisa è preferita al ritardo condiviso.
>
> |  | Giocatore 2: *On time* | Giocatore 2: *Late* |
> |---|---|---|
> | **Giocatore 1: *On time*** | 10, 10 | −5, 10 |
> | **Giocatore 1: *Late*** | 10, −5 | 5, 5 |
>
> **Due Nash Equilibria:**
> - {*On time*, *On time*}: payoff (10, 10) — entrambi puntuali
> - {*Late*, *Late*}: payoff (5, 5) — entrambi in ritardo
>
> Il primo NE **domina Pareto** il secondo: entrambi preferiscono la puntualità condivisa. Ma se ci si aspetta che l'altro arrivi in ritardo, arrivare in ritardo è la miglior risposta! Ecco il problema della selezione dell'equilibrio.

## Lo Stag Hunt (Caccia al Cervo)

Il caso più famoso di gioco di coordinamento con equilibri Pareto-ordinabili è il **Gioco della Caccia al Cervo**, ispirato a Jean-Jacques Rousseau.

> [!example] Matrix 2.25 — Stag Hunt (Carmichael)
> Due cacciatori scelgono simultaneamente se cacciare un cervo (*stag*) — impresa che richiede la collaborazione di entrambi — o una lepre (*hare*) da soli.
>
> |  | Giocatore 2: *stag* | Giocatore 2: *hare* |
> |---|---|---|
> | **Giocatore 1: *stag*** | 5, 5 | 0, 1 |
> | **Giocatore 1: *hare*** | 1, 0 | 1, 1 |
>
> **Due Nash Equilibria:**
> - {*stag*, *stag*}: payoff (5, 5) — cooperazione efficiente
> - {*hare*, *hare*}: payoff (1, 1) — sicurezza individuale
>
> Il NE {*stag*, *stag*} **domina Pareto** {*hare*, *hare*}: entrambi preferirebbero cacciare il cervo insieme. Ma cacciare il cervo è *rischioso*: se l'altro caccia la lepre, il mio payoff è 0. Cacciare la lepre garantisce almeno 1.
>
> Il dilemma non è tra interesse personale e collettivo (come nel [[06_Dilemma_Prigioniero]]), ma tra **efficienza** e **sicurezza**.

> [C, p. 43–45] L'equilibrio {*stag*, *stag*} è Pareto superiore perché entrambi possono guadagnare passando da {*hare*, *hare*} a {*stag*, *stag*}. Il motivo per cui le società possono restare bloccate nell'equilibrio inferiore è la mancanza di **fiducia reciproca**: non è che nessuno voglia cooperare, è che nessuno sa se l'altro si fiderà abbastanza da cooperare.

## Il Ruolo della Fiducia: Applicazione all'Italia

Le slide mostrano una connessione profonda tra lo Stag Hunt e le differenze regionali italiane in termini di PIL pro-capite e punteggi PISA. Il Nord Italia tende a coordinate sull'equilibrio "alto" (maggiore cooperazione sociale, maggiore capitale sociale), il Sud sull'equilibrio "basso".

Dati da un trust game sperimentale mostrano che:
- Le aspettative di fiducia sono più alte verso soggetti della *stessa regione* in alcune aree
- Le aspettative di fiducia verso soggetti di *aree macro diverse* sono molto più basse nel Sud

Questo suggerisce che la selezione dell'equilibrio nello Stag Hunt sia mediata dalle **istituzioni sociali informali** (fiducia, norme, capitale sociale), non solo dalle preferenze individuali.

> [BB, p. 222] Birchler & Bütler collegano i giochi di coordinamento alla questione del come le aspettative si formano e si coordinano nei mercati. In assenza di un meccanismo di coordinamento esogeno, le economie possono restare intrappolate in equilibri inefficienti.

## Giochi di Coordinamento Senza Assurance: Battle of the Sexes

Non tutti i giochi di coordinamento con equilibri multipli hanno un equilibrio Pareto-dominante. Nel **Battle of the Sexes** (o giochi simili come *Friends or Enemies 3*), i due giocatori preferiscono equilibri *diversi*: John preferisce {pub, pub}, Janet preferisce {party, party}. Qui il problema non è la fiducia ma il **conflitto di preferenze sull'equilibrio da raggiungere**.

> [C, p. 46–47] Nel Battle of the Sexes e nel Chicken Game, la molteplicità degli equilibri è accompagnata da preferenze asimmetriche tra i giocatori sugli equilibri stessi. Questo rende la previsione dell'esito particolarmente difficile.

## Confronto Schematico

| Gioco | NE multipli | Pareto-ordinabili? | Problema centrale |
|-------|-------------|-------------------|-------------------|
| Stag Hunt | Sì (2) | Sì | Fiducia / sicurezza vs efficienza |
| Puntualità | Sì (2) | Sì | Aspettative condivise / norme sociali |
| Battle of the Sexes | Sì (2) | No | Conflitto su quale NE raggiungere |
| [[05_Chicken_Game\|Chicken Game]] | Sì (2) | No | Guerra di attrito / dissuasione |

> [!summary] Take-home message
> I giochi di coordinamento mostrano che la razionalità individuale non basta per selezionare l'equilibrio efficiente: servono aspettative condivise, istituzioni, fiducia o meccanismi focali (punti di Schelling). Lo Stag Hunt in particolare modella con precisione la tensione tra efficienza collettiva e sicurezza individuale — una tensione che spiega molte differenze economiche tra regioni e paesi. La presenza di [[03_Nash_Equilibrium|equilibri di Nash multipli]] è la regola, non l'eccezione, nei giochi reali.

## 🔗 Connessioni con l'Economia dell'Informazione

I **giochi di coordinamento** hanno un ruolo fondamentale nel capire le istituzioni e i mercati:

- **[[0. Intro/01_Coordinamento_e_incentivi|Il problema del coordinamento]]**: le tre istituzioni (Mercato, Stato, Impresa) sono esattamente meccanismi per selezionare un equilibrio nei giochi di coordinamento. Il Mercato funziona bene quando c'è un equilibrio naturalmente focale; Stato e Impresa intervengono quando l'equilibrio Pareto-superiore non emerge spontaneamente.
- **[[0. Intro/02_Mercato_e_Hayek|Ipotesi di Hayek]]**: i mercati raggiungono l'equilibrio efficiente quando i prezzi coordinano le aspettative verso il NE Pareto-ottimale. Quando esistono equilibri multipli (come nello Stag Hunt), il semplice sistema dei prezzi non basta — servono istituzioni complementari.
- **Norme sociali e capitale sociale**: le differenze regionali italiane in fiducia e cooperazione riflettono diverse storie di selezione dell'equilibrio nei giochi di coordinamento — con conseguenze misurabili su [[0. Intro/03_Beni_comuni|governance dei commons]] e efficienza economica.
