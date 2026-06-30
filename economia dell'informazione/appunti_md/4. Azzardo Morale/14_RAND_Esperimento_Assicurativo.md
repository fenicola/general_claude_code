---
tags: [economia-informazione, azzardo-morale, sanità, assicurazione, RCT, esperimento-randomizzato]
aliases: [RAND HIE, RAND Health Insurance Experiment, Esperimento Assicurativo RAND]
links: [13_Azzardo_Morale_Sanita, 08_Karlan_Zinman_Test_Empirico, 01_Definizione_e_Timing]
---

# Il RAND Health Insurance Experiment (1974–1982)

## Riferimento

> Brook, R.H. et al. (2006). *The Health Insurance Experiment: A Classic RAND Study Speaks to the Current Health Care Reform Debate*. RAND Corporation.
> Newhouse, J.P. and the Insurance Experiment Group (1993). *Free For All? Lessons from the RAND Health Insurance Experiment*. Harvard University Press.

## Il problema empirico fondamentale

La domanda cardine della [[13_Azzardo_Morale_Sanita|sezione sulla sanità]] è: **l'assicurazione sanitaria aumenta il consumo di cure mediche?** La risposta sembra ovvia, ma provarla rigorosamente è tutt'altro che banale.

Il problema è quello classico della **selezione** nell'econometria dell'istruzione e della salute: le persone con e senza assicurazione differiscono sistematicamente nelle caratteristiche che determinano anche il consumo di cure.

$$\text{osservazione}: \text{assicurati consumano più cure}$$
$$\downarrow$$
$$\text{ma è per l'assicurazione, o per la malattia che li ha spinti ad assicurarsi?}$$

Ricorda la [[08_Karlan_Zinman_Test_Empirico|logica di Karlan & Zinman]]: come separare selezione avversa (chi si assicura è già più malato) da moral hazard (l'assicurazione induce più consumo)?

> [!intuition]
> Il problema è identico a chiedersi se il fatto che le persone in ospedale siano malate dimostri che gli ospedali causano malattia. La soluzione è la stessa: un esperimento randomizzato.

## Il disegno del RAND HIE

Il RAND Health Insurance Experiment è **uno degli RCT più ambiziosi mai condotti nelle scienze sociali**: avviato nel 1974, durato fino al 1982, con una spesa complessiva di circa 300 milioni di dollari (in dollari 2011), coinvolge circa **2.000 famiglie (5.800 persone)** in 6 sedi diverse negli Stati Uniti.

**Meccanismo**: le famiglie vengono assegnate casualmente a piani assicurativi con diversi livelli di **compartecipazione al costo** (*consumer cost-sharing*), e monitorate per 3-5 anni.

### I piani assicurativi sperimentali

Il parametro chiave è il tasso di **coinsurance** — la percentuale di costo medico sopportata dal paziente:

| Piano | Coinsurance | Massimale out-of-pocket |
|---|---|---|
| **Free care** | 0% | nessuno |
| Piano 1 | 25% | \$1.000 (2011 $) |
| Piano 2 | 50% | \$1.000 (2011 $) |
| Piano 3 | 95% (quasi privo) | \$1.000 (2011 $) |
| Piano misto | 25% (eccetto dentale/mentale al 50%) | — |
| Piano individuale | 95% outpatient, 0% inpatient | — |

Il piano "free care" è il benchmark di **piena copertura**: nessun costo per l'assistito. Il piano al 95% è equivalente a nessuna copertura per la maggior parte delle spese ordinarie (il massimale protegge dalle catastrofi).

I piani diversi creano dunque variazione *esogena* (assegnata casualmente) nel **prezzo percepito** della cura sanitaria — esattamente quello che serve per misurare la risposta della domanda.

## La logica della domanda: il prezzo implicito delle cure

Formalmente, per un individuo nel piano con coinsurance $c$, il prezzo percepito di una visita medica con costo $p$ è:

$$p^* = c \cdot p$$

Nel piano free care: $p^* = 0$. Nel piano al 95%: $p^* \approx p$.

Se la domanda di cure mediche dipende dal prezzo percepito (come quasi tutti i beni normali), ci aspettiamo:

$$Q_{free} > Q_{25\%} > Q_{50\%} > Q_{95\%}$$

Se invece Gladwell ha ragione e la domanda è dettata dai "bisogni" e non dai prezzi, allora $Q_{free} \approx Q_{95\%}$.

## Risultati: il moral hazard esiste

I risultati del RAND HIE sono chiari e definitivi:

**Visite mediche (per capita)**: con copertura totale (0% coinsurance) circa 4,5 visite annue; con il piano al 95% circa 2,7 visite. Il costo condiviso **riduce il numero di visite del 40%**.

**Ricoveri ospedalieri (per capita)**: con 0% coinsurance circa 0,12 ricoveri annui; con il 95% circa 0,10 ricoveri. Riduzione circa del 17%.

**Spesa sanitaria media annua** (aggiustata per l'inflazione, in dollari 2005):
- Piano free (0%): ~\$1.450
- Piano 25%: ~\$1.200
- Piano 50%: ~\$1.100
- Piano 95%: ~\$1.000

La riduzione dal piano gratuito al piano quasi-privo è di circa il **30%** della spesa totale.

Tutti questi risultati mostrano una chiara risposta della domanda al prezzo: **il moral hazard ex post esiste**, ed è economicamente rilevante.

> [!example]
> In termini intuitivi: una famiglia con piena copertura spende il 45% in più di cure mediche rispetto a una famiglia con copertura minima. La differenza non è perché la prima famiglia sia più malata (l'assegnazione è casuale), ma perché il costo percepito è zero.

## Ma la salute peggiora? Il compromesso cruciale

La domanda normativa è: questa riduzione nel consumo di cure è **efficiente** o **pericolosa**?

Il RAND HIE rivela una risposta sfumata:

**In media, la riduzione del consumo non peggiora la salute**: la coinsurance non ha effetti avversi significativi sulla salute media dei partecipanti.

**Tuttavia, per i sottogruppi più vulnerabili, la piena copertura fa la differenza**:

- La cura gratuita porta a **miglioramenti nell'ipertensione** (più soggetti hanno pressione sotto controllo).
- Miglioramenti nella **salute dentale** e nella **vista**.
- Miglioramenti in **sintomi gravi selezionati**.

Questi miglioramenti si concentrano negli **individui più malati e più poveri** — esattamente chi ha maggiori difficoltà ad affrontare i costi out-of-pocket.

### L'interpretazione economica

Questo risultato suggerisce che il moral hazard non è uniforme: la maggior parte delle cure "aggiuntive" consumate in regime di copertura totale hanno un **basso valore marginale** (non migliorano la salute misurabile). Tuttavia, per una minoranza di pazienti poveri e con condizioni croniche, le cure aggiuntive sono **critiche**.

La riduzione della coinsurance riduce il consumo in modo relativamente proporzionale tra cure efficaci e inefficaci — è una riduzione "democratica" ma non "intelligente".

> [!intuition]
> Il cost-sharing è uno strumento grossolano: riduce il consumo di cure inutili (visita per un raffreddore), ma riduce anche il consumo di cure necessarie (controllo pressione per un iperteso povero). Per il paziente medio sano, la riduzione è benign; per il paziente povero con cronicità, può essere pericolosa.

## Limiti del RAND HIE e generalizzazioni

Il RAND HIE non misura l'effetto dell'**assenza completa di assicurazione** (tutti i piani, anche quello al 95%, prevedevano una protezione catastrofica). Non risponde quindi alla domanda su chi non ha nessuna copertura.

Lo studio era rappresentativo delle famiglie con adulti sotto i 62 anni — i gruppi ad alto rischio (anziani) e in condizioni di povertà estrema erano esclusi.

Nonostante questi limiti, il RAND HIE rimane il **gold standard** per la stima del moral hazard nell'assicurazione sanitaria, e i suoi risultati sono stati confermati da numerosi studi successivi che sfruttano variazioni quasi-sperimentali naturali (es. l'introduzione di Medicare).

## Connessioni con la teoria

Il RAND HIE risponde alla domanda posta da [[13_Azzardo_Morale_Sanita|Pauly (1968)]] sull'azzardo morale ex post. I risultati confermano che la curva di domanda di cure sanitarie ha pendenza negativa — il consumo risponde ai prezzi — ma con un'elasticità della domanda che varia significativamente per tipo di cura e tipo di paziente.

Il disegno del RAND HIE è strutturalmente analogo all'esperimento di [[08_Karlan_Zinman_Test_Empirico|Karlan & Zinman (2009)]] sul credito: in entrambi i casi, la randomizzazione del contratto (assicurativo nel RAND, creditizio in K&Z) permette di separare effetti causali da effetti di selezione.

> [!summary]
> Il RAND HIE (1974–1982) è la prova sperimentale definitiva che il moral hazard ex post nell'assicurazione sanitaria esiste: la piena copertura aumenta il consumo di cure del 30–45% rispetto alla quasi-assenza di copertura. Tuttavia, la riduzione del consumo indotta dalla coinsurance è in media innocua per la salute, con importanti eccezioni per i pazienti più poveri e malati. Il compromesso tra contenimento dei costi (coinsurance) ed equità (accesso per i fragili) rimane il dilemma centrale del design assicurativo sanitario.
